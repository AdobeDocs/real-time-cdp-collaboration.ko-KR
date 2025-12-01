---
title: 대상 소싱을 위한 AWS 권한 구성
description: AWS의 대상 소싱용  [!DNL Amazon S3] 버킷에 대한 읽기 전용 보안 액세스 권한을 Adobe에 부여하도록 Real-Time CDP Collaboration Identity and Access Management(IAM) 권한을 구성하는 방법에 대해 알아봅니다.
source-git-commit: 73f11b7341cf94540dc01f8803291f6dc3cd5038
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 1%

---

# 대상 소싱을 위한 AWS 권한 구성

이 안내서를 사용하여 AWS S3 버킷에 대한 읽기 전용 보안 액세스 권한을 Adobe에 부여하는 IAM(Amazon Identity and Access Management) 정책 및 역할을 구성합니다. 이 액세스 권한을 사용하면 Real-Time CDP Collaboration이 S3 버킷에서 대상을 소싱할 수 있습니다.

## 전제 조건 {#prerequisites}

계속하기 전에 다음 요구 사항을 충족하고 필요한 정보에 액세스할 수 있는지 확인하십시오.

### 필수 AWS 권한

이 설정을 완료하려면 계정에 AWS 관리자 액세스 권한이 있어야 합니다. 관리자 액세스를 통해 Adobe의 S3 버킷에 대한 액세스 권한을 부여하는 데 필요한 IAM 정책 및 역할을 만들고 관리할 수 있습니다. 관리자 권한이 없는 경우 계속 진행하기 전에 AWS 관리자에게 문의하십시오.

### 필수 정보

아래 단계를 진행할 때 다음 정보를 기록해 두십시오. 이러한 세부 정보는 [[!DNL Amazon S3] 대상 소싱 UI 안내서](./configure-aws-s3-audience-sourcing.md)에서 사용됩니다.

* 대상 파일이 저장되는 S3 버킷 이름입니다.
* 대상 파일이 있는 폴더 경로(접두사)입니다.
* 새로 만든 IAM 역할에 대한 Amazon 리소스 이름(ARN)(예: `arn:aws:s3:::my-company-data/audience-files/`)

>[!TIP]
>
>ARN(Amazon 리소스 이름)은 S3 버킷 및 IAM 역할과 같은 AWS 리소스를 고유하게 식별합니다. 버킷 및 선택적 폴더 경로를 지정하려면 다음 형식을 사용하십시오.
>
>```
>arn:aws:s3:::<bucket-name>/<optional-folder-path>
>```

## IAM 정책 만들기 {#create-policy}

설정을 시작하려면 먼저 S3 버킷에 **읽기 전용 액세스 권한**&#x200B;을 부여하는 IAM 정책을 만드십시오. 이 정책을 사용하면 Adobe에서 대상 소싱에 필요한 파일을 읽을 수 있지만, 쓰기 또는 삭제 권한은 부여하지 않습니다.

[AWS 관리 콘솔](https://aws.amazon.com/console/)을 열고 **[!DNL IAM]** > **[!DNL Policies]** > **[!DNL Create policy]**(으)로 이동합니다.

AWS 정책 만들기 작업 영역에서 **JSON** 탭을 선택하고 다음 예제 정책을 붙여 넣습니다.

>[!NOTE]
>
>`<Your AWS ARN for bucket folder path>` 및 `<Your AWS ARN for bucket>`을(를) 특정 S3 ARN으로 바꿉니다. 버킷 폴더 경로를 지정할 때 ARN 끝에 `/*`을(를) 포함합니다(예: `arn:aws:s3:::my-company-data/audience-files/*`). 이렇게 하면 Adobe이 지정된 폴더 경로 내의 모든 파일 및 하위 폴더에 액세스할 수 있습니다.

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "Statement1",
      "Effect": "Allow",
      "Action": [
        "s3:GetObject",
        "s3:ListBucket",
        "s3:GetBucketLocation"
      ],
      "Resource": "<Your AWS ARN for bucket folder path>"
    },
    {
      "Sid": "Statement2",
      "Effect": "Allow",
      "Action": [
        "s3:ListBucket"
      ],
      "Resource": "<Your AWS ARN for bucket>"
    }
  ]
}
```

정책 설정을 검토하고 **[!DNL Create policy]**&#x200B;을(를) 선택하십시오. 이후 단계에서 사용할 정책 이름을 기록하십시오.

>[!TIP]
>
>버킷 이름과 폴더 경로를 찾으려면 **Amazon S3 관리 콘솔**&#x200B;을 여십시오. **버킷** 페이지에서 버킷 이름을 선택하여 엽니다. **개체** 보기에는 파일 및 폴더가 나열되며, 페이지 위쪽에 있는 경로에 현재 폴더 경로가 표시됩니다.

## IAM 역할 만들기 {#create-role}

그런 다음 IAM 역할을 만들고 Real-Time CDP Collaboration AWS IAM 역할을 **신뢰할 수 있는 엔터티**(으)로 설정합니다. 이를 통해 Adobe 서비스는 역할을 맡아 S3 대상 데이터를 안전하게 읽을 수 있습니다.

Amazon S3 관리 콘솔의 **[!DNL IAM]** 탭에서 **[!DNL Roles]** > **[!DNL Create role]**(으)로 이동합니다.

[!DNL Step 1] 워크플로의 [!DNL Create role] 아래 **[!DNL Trusted entity type]** 섹션에서 **[!DNL Custom trust policy]**&#x200B;을(를) 선택합니다. 그런 다음 **[!DNL Custom trust policy]** 편집기에서 다음 예제를 붙여 넣고 `<Adobe IAM Role ARN>`을(를) 해당 지역의 값으로 바꿉니다.

* 해당 지역에 적합한 Adobe IAM 역할 ARN:

| 지역 | Adobe IAM 역할 ARN |
|---------|-------------------|
| 북미 | `arn:aws:iam::590183896800:role/rtcdp-collab-prod-va6-role` |
| 오스트레일리아 | `arn:aws:iam::590183896800:role/rtcdp-collab-prod-aus3-role` |
| EMEA | `arn:aws:iam::590183896800:role/rtcdp-collab-prod-deu1-role` |

트러스트 정책의 예:

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "Statement1",
      "Effect": "Allow",
      "Principal": {
        "AWS": "<Adobe IAM Role ARN>"
      },
      "Action": "sts:AssumeRole"
    }
  ]
}
```

정책을 검토하고 계속하려면 **다음**&#x200B;을(를) 선택하십시오.

[!DNL Step 2] 워크플로의 **[!DNL Add permissions]** [!DNL Create role] 섹션에서 [이전](#create-policy)에 만든 IAM 정책을 검색하고 연결합니다. **[!DNL Next]**&#x200B;을(를) 계속하려면 정책 다음에 [!DNL Step 3]을(를) 선택하십시오.

[!DNL Step 3] **[!DNL Name review, and create - Role details]** 섹션에서 역할 이름(예: `s3-iam-role`) 및 선택적 설명을 제공합니다.

이 페이지에는 신뢰할 수 있는 엔티티 정책, 권한 정책 요약 및 내부 조직 및 추적을 위해 추가한 태그가 표시됩니다.

마지막으로 **역할 만들기**&#x200B;를 선택하여 설정을 확인합니다.

>[!IMPORTANT]
>
>역할을 만든 후 Amazon 리소스 이름(ARN)을 기록해야 합니다. **대상 소싱에 대한 AWS S3 구성** 워크플로우의 [S3 연결 인증](./configure-aws-s3-audience-sourcing.md) 단계에서 IAM 역할 ARN을 제공해야 합니다.

## 다음 단계 {#next-steps}

이 설정은 Adobe에게 S3 버킷에 대한 읽기 전용 액세스 권한을 부여하고 Adobe의 IAM 역할과 신뢰할 수 있는 연결을 설정합니다.

다음으로 [대상 소싱에 대한 AWS S3 구성](./configure-aws-s3-audience-sourcing.md)으로 진행하여 S3 버킷을 Collaboration에 연결합니다.

소싱 대상에 대한 자세한 내용은 [Source 및 대상 관리](./onboard-audiences.md)를 참조하세요.
