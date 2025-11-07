---
title: 대상 소싱에 대해  [!DNL Amazon S3] 구성
description: 대상 데이터를 Real-Time CDP Collaboration에 수집하기 위해  [!DNL Amazon S3] 저장소를 셀프서비스 데이터 소스로 구성 및 연결하는 방법에 대해 알아봅니다.
source-git-commit: 05fd7ec466ba2b20264490bbbfadc9bb6d361bc8
workflow-type: tm+mt
source-wordcount: '1515'
ht-degree: 0%

---

# 대상 소싱에 대해 [!DNL Amazon S3] 구성

활성화 및 중복 분석을 위해 Adobe Real-Time CDP Collaboration UI에서 [!DNL Amazon S3] 저장소를 구성하고 소스 대상 데이터에 연결하는 방법을 알아봅니다.

>[!IMPORTANT]
>
>이 안내서를 따르려면 먼저 AWS 계정 내에서 Adobe의 IAM 역할을 승인하는 단계를 완료해야 합니다.\
>단계별 설정 지침은 **[대상 소싱에 대한 AWS 권한 구성](./configure-aws-permissions-audience-sourcing.md)** 안내서를 참조하십시오.

## 개요 {#overview}

이 워크플로우를 사용하여 [!DNL Amazon S3]에서 직접 자사 대상자를 소스 및 관리합니다. 구성 후 Collaboration은 자동으로 S3 버킷에서 대상을 소싱하여 통찰력 및 활성화에 사용할 수 있도록 합니다.

S3를 통해 가져온 대상자는 Adobe Experience Platform에서 가져온 대상과 동일한 거버넌스 및 데이터 처리 규칙을 따릅니다.

## 전제 조건 {#prerequisites}

S3 데이터 연결을 구성하기 전에 다음을 확인하십시오.

* **[!DNL Amazon S3]대상 소싱 사양(v1.1)**&#x200B;을 준수하는 대상 파일을 포함하는 활성 **[버킷](../../assets/quick-start/RTCDP_Collaboration_Audience_Sourcing_Spec_v1.1.pdf)**&#x200B;에 액세스할 수 있습니다.
* AWS에서 **가정된 역할** 메서드(액세스/비밀 키 아님)를 사용하여 버킷에 액세스할 수 있는 Adobe 권한을 부여하는 **IAM 역할**&#x200B;을(를) 만들었습니다. 자세한 지침은 **[대상 소싱에 대한 AWS 권한 구성](./configure-aws-permissions-audience-sourcing.md)**&#x200B;을 참조하십시오. IAM 역할에는 다음 권한이 포함되어야 합니다.

   * `ListBucket`
   * `GetBucketLocation`
   * `GetObject`

* 다음 값이 준비되었습니다.

   * **IAM 역할 Amazon 리소스 이름(ARN)**
   * **S3 버킷 이름**
   * **폴더 경로**(대상 파일이 포함된 디렉터리 접두사)

>[!NOTE]
>
>대상 파일은 승인된 S3 버킷의 **루트 폴더 경로**&#x200B;에 있어야 합니다. 하위 폴더 구조는 지원되지 않습니다.

## [!DNL Amazon S3] 연결 구성 {#configure-aws-s3-connection}

**[!UICONTROL 설정]** 작업 영역의 **[!UICONTROL 내 대상]** 탭에서 추가 아이콘(![추가 아이콘)을 선택합니다.](/help/assets/icons/plus.png))을(를) 선택한 다음 **[!UICONTROL 대상]**&#x200B;을 선택합니다.

첫 번째 대상자인 경우 **[!UICONTROL 추가]** 옵션도 선택할 수 있습니다.

![설정 작업 영역의 [내 대상] 탭에 추가 아이콘과 대상 추가 옵션이 표시됩니다.](../../assets/setup/add-manage-audiences/add-audiences.png)

대상자 추가 워크플로우가 나타납니다. **[!UICONTROL 새 데이터 연결 추가]**&#x200B;를 선택한 후 **[!UICONTROL 다음]**&#x200B;을 선택합니다.

![새 데이터 연결 추가 옵션이 강조 표시된 대상자 추가 작업 영역입니다.](../../assets/setup/add-manage-audiences/add-data-connection.png){zoomable="yes"}

### [!DNL Amazon S3]을(를) 데이터 연결로 선택 {#select-aws-s3}

**[!UICONTROL Amazon S3]**&#x200B;을(를) 데이터 연결로 선택한 후 **[!UICONTROL 다음]**&#x200B;을(를) 선택하십시오.

![선택 가능한 옵션으로 사용할 수 있는 [!DNL Amazon S3]의 데이터 연결 선택 화면입니다.](../../assets/setup/aws-audience-sourcing/select-s3-data-connection.png)

### 대상 파일 요구 사항 검토 {#review-audience-requirements}

대상자 파일을 구조화하는 방법을 설명하는 대화 상자가 나타납니다. **[[!UICONTROL 대상 소싱 사양]](../../assets/quick-start/RTCDP_Collaboration_Audience_Sourcing_Spec_v1.1.pdf)**&#x200B;에 연결된 링크를 사용하여 Collaboration에서 대상 데이터를 올바르게 읽을 수 있도록 [!DNL Amazon S3]의 대상 데이터를 포맷하고 구성하는 방법을 알아보십시오.

>[!IMPORTANT]
>
>Adobe에서 처리를 위해 [!DNL Amazon S3] 저장소에서 데이터를 검색할 수 있도록 [!DNL Amazon S3] 사용자로 Adobe을 승인해야 합니다.

대상 파일은 대상 소싱 사양을 준수해야 합니다. 일치 키는 필요한 형식에 따라 자동으로 매핑됩니다.

주요 고려 사항은 다음과 같습니다.

* 파일은 CSV 형식이어야 합니다. 쉼표를 구분 기호로 사용하고 여러 값에 대해 파이프(`|`)를 사용합니다.
* 여러 파일을 업로드하는 경우 모든 파일에 동일한 열이 포함되어 있는지 확인하십시오.
* 각 대상 레코드에는 `AUDIENCE_ID`이(가) 있어야 하며 `HASHED_EMAIL_SHA_256`, `HASHED_PHONE_SHA_256`, `HASHED_IPV4_SHA_256`, `CRM_ID`, `LOYALTY_ID` 또는 `ADFIXUS_ID`과(와) 같은 일치 키가 하나 이상 있어야 합니다.
* 데이터 새로 고침은 Collaboration에서 소싱 설정 중 선택한 항목을 기준으로 1~6일마다 발생합니다.

![대상 소싱 사양에 대한 링크가 있는 [소싱을 위한 데이터 준비] 대화 상자입니다.](../../assets/setup/aws-audience-sourcing/prepare-data-sourcing-dialog.png)

### S3 연결 인증 {#authenticate-s3-connection}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_sources_s3_folderpath"
>title="폴더 경로 형식"
>abstract="대상 파일이 저장된 [!DNL Amazon S3] 버킷 내의 폴더 경로(접두사)를 입력하십시오.<br><ul><li>슬래시(/)로 경로를 시작하지 마십시오.</li><li>경로 끝에 슬래시를 포함합니다.</li><ul><br>올바른 예: `base/path/`<br>잘못된 예: `/base/path`"

그런 다음 S3 버킷을 Collaboration에 연결하기 위해 [!DNL Amazon S3] 자격 증명을 제공합니다.

**[대상 소싱에 대한 AWS 권한 구성](./configure-aws-permissions-audience-sourcing.md)**에 설명된 단계에 따라 사용자에게 Adobe 액세스 권한을 부여합니다.
저장소 [!DNL Amazon S3]개. 완료되면 다음 UI 필드에 값을 입력합니다.

* IAM 역할
* S3 버킷 이름
* 폴더 경로

![IAM 역할, S3 버킷 이름 및 폴더 경로 필드가 있는 [!DNL Amazon S3] 연결 양식입니다.](../../assets/setup/aws-audience-sourcing/s3-authentication-credentials-form.png)

### 동의 승인 확인 {#confirm-consent}

그런 다음 계속하기 전에 동의 옵트아웃이 제거되었음을 확인해야 합니다. 확인 상자를 선택한 다음 **[!UICONTROL 확인]**&#x200B;을 선택하여 확인합니다.

![계속하기 전에 확인이 필요한 동의 옵트아웃 승인 대화 상자.](../../assets/setup/aws-audience-sourcing/consent-optout-acknowledgment.png)

### 인증 결과 확인 {#validate-authentication}

접속 후 시스템이 자격 증명을 확인하고 다음 메시지 중 하나를 표시합니다.

| 상태 | 메시지 | 설명 |
|---| ---|---|
| **성공** | **[!UICONTROL 인증 성공]** | [!DNL Amazon S3]에 대한 연결이 정상적으로 설정되었습니다. |
| **실패** | **[!UICONTROL 인증 실패]** | 자격 증명을 검토하고 다시 시도하십시오. |
| **액세스 거부됨** | **[!UICONTROL 액세스 거부됨]** | 자격 증명에는 이 [!DNL Amazon S3] 버킷에 액세스하는 데 필요한 권한이 없습니다. 액세스 설정을 확인하거나 관리자에게 문의하십시오. |
| **잘못된 파일 형식** | **[!UICONTROL 잘못된 파일 형식]** | 대상 데이터가 예상 구조와 일치하지 않습니다. 파일이 대상 소싱 사양을 준수하는지 확인하십시오. |
| **대상 파일이 없습니다** | **[!UICONTROL 대상 파일이 없습니다]** | 대상 파일이 지정된 폴더 경로에 있으며 경로에 액세스할 수 있는지 확인하십시오. |
| **내부 오류** | **[!UICONTROL 내부 오류가 발생했습니다]** | 다시 시도하십시오. 문제가 지속되면 고객 지원 센터에 문의하십시오. |


### 연결 세부 정보 제공 {#provide-connection-details}

S3 데이터 연결에 대한 설명 이름과 설명(선택 사항)을 입력합니다. 다음 UI 필드에 값을 입력합니다.

* **[!UICONTROL 데이터 연결 이름]**(필수)
* **[!UICONTROL 데이터 연결 설명]**(선택 사항)

![연결 이름 및 설명 필드가 있는 데이터 연결 세부 정보 양식입니다.](../../assets/setup/aws-audience-sourcing/s3-connection-name-description.png)

### 자동 매핑된 ID 필드 검토 {#auto-mapped-fields}

**[!UICONTROL 매핑]** 화면은 읽기 전용입니다. 변형을 추가, 삭제 또는 적용할 수 없습니다. Collaboration은 대상 소싱 사양을 기반으로 대상 파일의 소스 ID 필드를 대상 필드에 자동으로 매핑합니다.

매핑된 필드를 시각적으로 확인하고 계속하려면 **[!UICONTROL 다음]**&#x200B;을(를) 선택하십시오.

![자동 매핑된 원본 및 대상 ID 필드를 표시하는 필드 매핑 화면입니다.](../../assets/setup/aws-audience-sourcing/s3-field-mapping-auto-mapped.png)

### 일정 새로 고침 빈도 및 날짜 범위 {#schedule-refresh}

**[!UICONTROL 일정]** 보기가 나타납니다. 드롭다운 메뉴를 사용하여 1일에서 6일 사이의 새로 고침 빈도를 선택한 다음 활성 날짜 범위를 설정합니다. 달력 아이콘을 사용하여 시작 날짜와 종료 날짜를 지정합니다.

>[!IMPORTANT]
>
>Collaboration 크레딧을 효과적으로 관리하려면 기본 S3 데이터의 업데이트 빈도와 일치하거나 이 빈도를 초과하도록 새로 고침 빈도를 설정하십시오. 지원되는 최소 새로 고침 간격은 6일에 한 번입니다.

![새로 고침 빈도 옵션 및 날짜 범위 구성이 포함된 예약 설정 화면입니다.](../../assets/setup/aws-audience-sourcing/s3-schedule-refresh-frequency.png)

### 연결 검토 및 완료 {#review-and-complete}

마지막으로 요약 화면에서 구성 설정을 검토합니다. 이 보기에는 다음 섹션의 요약이 포함되어 있습니다.

* **[!UICONTROL 데이터 연결]**: IAM 역할, S3 버킷 이름 및 구성한 폴더 경로를 표시합니다.
* **[!UICONTROL 세부 정보]**: 나중에 식별하는 데 도움이 되도록 데이터 연결의 이름 및 선택적 설명을 표시합니다.
* **[!UICONTROL 매핑]**: 업로드한 대상 파일의 원본 필드(예: `HASHED_EMAIL`)가 Collaboration에서 사용되는 대상 필드(예: 해시된 이메일)에 매핑되는 방법을 나열합니다.
* **[!UICONTROL 일정]**: 연결이 소싱에 대한 대상 데이터 및 활성 날짜 범위를 새로 고치는 빈도를 요약합니다.

섹션을 편집해야 하는 경우 연필 아이콘을 선택합니다. **[!UICONTROL 완료]**&#x200B;를 선택하여 모든 섹션을 확인합니다.

![데이터 연결, 세부 정보, 매핑 및 일정 섹션이 표시되는 검토 요약 화면입니다.](../../assets/setup/aws-audience-sourcing/s3-connection-review-summary.png)

데이터 연결이 성공적으로 만들어졌으며 대상 소싱이 진행 중임을 나타내는 대화 상자 확인이 나타납니다.

## 소스 대상자 검토 {#review-sourced-audiences}

구성을 완료한 후 Collaboration은 S3 버킷에서 대상자 소싱을 시작합니다. [!DNL Amazon S3] 버킷을 통해 가져온 대상은 **[!UICONTROL 내 대상]** 탭에 나타나며 Experience Platform에서 가져온 대상과 동일한 기능 및 정보를 갖습니다.

대상자 소싱이 진행 중인 경우 화면 상단에 배너가 나타납니다. 개별 대상은 소싱이 완료된 후에만 표시됩니다.

![대상자 [!DNL Amazon S3]명에 대한 소싱이 진행 중임을 보여 주는 대상자 탭.](../../assets/setup/aws-audience-sourcing/s3-audiences-sourcing-in-progress.png)

S3 대상이 제공되면 사용 가능한 대상 목록이 표 또는 카드 보기에서 제공됩니다.

>[!TIP]
>
>대상 소싱 시간은 S3 데이터 크기와 구성한 새로 고침 빈도에 따라 다릅니다. 데이터 세트가 커지거나 새로 고침 빈도가 낮은 일정이 **[!UICONTROL 내 대상]** 작업 영역에 표시되는 데 시간이 더 오래 걸릴 수 있습니다.

![소스 대상의 테이블 목록을 표시하는 대상 탭입니다.](../../assets/setup/aws-audience-sourcing/s3-audiences-list-view.png)

표 보기 또는 표 보기에서 행 항목을 선택하거나 **[!UICONTROL 대상자 보기]**&#x200B;를 선택하여 특정 대상자에 대한 개요를 봅니다. 대상자의 상태, 소스 및 데이터 연결 이름과 함께 다음에 대한 세부 패널이 표시됩니다.

**[!UICONTROL ID]**: 데이터를 사용할 수 있게 되면 총 ID 수 및 분류를 표시합니다.
**[!UICONTROL 범주]**: 대상을 구성하거나 필터링하는 데 사용되는 모든 태그를 나열합니다.
**[!UICONTROL 연결 액세스]**: 대상이 개인, 공개 또는 특정 공동 작업자와 공유되는지 여부를 나타냅니다.
**[!UICONTROL 메타데이터 가시성]**: 공동 작업자가 볼 수 있는 대상 정보(ID 수, 겹침 비율, 색인 등)를 정의합니다.

공동 작업 프로젝트에서 대상을 사용하기 전에 이 보기를 사용하여 대상 구성 및 가시성 설정을 확인하십시오.

자세한 내용은 [대상자 보기 대시보드 설명서](https://experienceleague.adobe.com/en/docs/real-time-cdp-collaboration/using/setup/onboard-audiences#view-audiences-dashboard)를 참조하세요.

## S3 데이터 연결 보기 {#view-s3-connection}

새로 추가한 [!DNL Amazon S3] 연결은 **[!UICONTROL 내 데이터 연결]** 탭에서 즉시 사용할 수 있습니다. 대상 원본은 [!UICONTROL Amazon S3]&#x200B;(으)로 표시됩니다.

S3 데이터 연결에는 다른 대상 데이터 연결과 동일한 기능 및 세부 사항이 포함되어 있습니다. 단, 이 보기에서 직접 대상을 추가하거나 편집할 수 없습니다.

>[!NOTE]
>
>[!DNL Amazon S3] 데이터 연결을 편집할 수 없습니다. 일단 연결이 생성되면 새로 고침 빈도와 같은 설정은 수정할 수 없습니다. 구성을 업데이트하려면 기존 연결을 삭제하고 새 연결을 만들어야 합니다.

![소싱 상태 정보가 있는 [!DNL Amazon S3] 데이터 연결을 표시하는 내 데이터 연결 탭입니다.](../../assets/setup/aws-audience-sourcing/s3-data-connections-tab.png)

## 다음 단계 {#next-steps}

이제 [!DNL Amazon S3] 저장소를 Collaboration에서 데이터 소스로 구성하고 연결했습니다. 이 워크플로우를 완료함으로써 활성화 및 중복 분석을 위해 자사 대상 데이터의 보안 소싱을 활성화했습니다.

소싱이 완료되면, 대상자가 **[!UICONTROL 내 대상자]** 작업 영역에 표시되어 공동 작업 및 활성화할 수 있습니다. 자세한 관리 옵션은 [소스 및 대상자 관리 설명서](./onboard-audiences.md)를 참조하세요.
