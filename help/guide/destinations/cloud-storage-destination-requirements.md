---
title: 대상 연결 요구 사항
description: Real-Time CDP Collaboration에서 지원되는 대상을 구성하는 데 필요한 연결 정보를 검토하십시오.
audience: admin, publisher
source-git-commit: c84582bb81289ce761c664af7db177535ff00a00
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 1%

---

# 대상 연결 요구 사항

Real-Time CDP Collaboration에서 대상을 구성하기 전에 대상 공급자가 요구하는 자격 증명과 연결 정보를 얻습니다.

이 페이지에는 Collaboration에서 사용할 수 있는 인증 방법이 요약되어 있습니다. 자격 증명을 만들거나, 권한을 할당하거나, 네트워크 액세스를 구성하거나, 대상 시스템을 준비하는 방법에 대한 지침은 연결된 Adobe Experience Platform 대상 설명서를 참조하십시오.

>[!NOTE]
>
>연결된 Adobe Experience Platform 설명서는 표준 대상 워크플로우에 대해 설명합니다. Real-Time CDP Collaboration에서 대상을 구성할 때 일부 단계, 필드 또는 옵션이 적용되지 않을 수 있습니다.

## 요구 사항 개요 {#requirements-at-a-glance}

| 대상 | 인증 또는 연결 방법 | 시작하기 전에 준비 | 자세한 요구 사항 |
|---|---|---|---|
| [!DNL Amazon S3] | 액세스 키 및 비밀 키 또는 가설 역할 | AWS 액세스 키 쌍 또는 IAM 역할 ARN, 버킷 및 폴더 정보 | [[!DNL Amazon S3] 대상 설명서](https://experienceleague.adobe.com/ko/docs/experience-platform/destinations/catalog/cloud-storage/amazon-s3) |
| SFTP | 암호 또는 SSH 키 | 서버 도메인, 포트, 사용자 이름, 인증 자격 증명 및 폴더 경로 | [SFTP 대상 설명서](https://experienceleague.adobe.com/ko/docs/experience-platform/destinations/catalog/cloud-storage/sftp) |
| [!DNL Azure Blob Storage] | 연결 문자열 | Azure 저장소 연결 문자열, 컨테이너 및 폴더 정보 | [[!DNL Azure Blob Storage] 대상 설명서](https://experienceleague.adobe.com/ko/docs/experience-platform/destinations/catalog/cloud-storage/azure-blob) |
| [!DNL Google Cloud Storage] | 액세스 키 ID 및 비밀 액세스 키 | [!DNL Google Cloud Storage] 상호 운용성 자격 증명, 버킷 및 폴더 정보 | [[!DNL Google Cloud Storage] 대상 설명서](https://experienceleague.adobe.com/ko/docs/experience-platform/destinations/catalog/cloud-storage/google-cloud-storage) |
| [!DNL Snowflake Batch] | [!DNL Snowflake] 데이터 공유 | [!DNL Snowflake] 계정 ID, 지역, 비공개 링크 상태 및 비공개 목록에 대한 액세스 권한 | [[!DNL Snowflake Batch] 대상 설명서](https://experienceleague.adobe.com/ko/docs/experience-platform/destinations/catalog/warehouse/snowflake-batch) |
| [!DNL Data Landing Zone] | 별도의 인증 필요 없음 | 대상 폴더 경로 및 파일 출력 환경 설정 | [[!DNL Data Landing Zone] 대상 설명서](https://experienceleague.adobe.com/ko/docs/experience-platform/destinations/catalog/cloud-storage/data-landing-zone) |

## 커넥터 노트 {#connector-notes}

대상을 구성하기 전에 다음 커넥터별 인증 방법 및 워크플로 차이점을 검토하십시오.

### [!DNL Amazon S3] {#amazon-s3}

Collaboration은 **[!UICONTROL 액세스 키]** 및 **[!UICONTROL 역할 가정]** 인증을 지원합니다. 액세스 키 인증에는 액세스 키와 비밀 액세스 키가 필요합니다. 가정된 역할 인증에는 Adobe에서 가정할 수 있는 AWS IAM 역할의 ARN이 필요합니다.

자격 증명, 역할 및 권한 설정에 대해서는 [대상 인증 [!DNL Amazon S3] 을 참조하십시오.](https://experienceleague.adobe.com/ko/docs/experience-platform/destinations/catalog/cloud-storage/amazon-s3#authenticate)

### SFTP {#sftp}

Collaboration은 **[!UICONTROL 암호를 사용하는 SFTP]** 및 **[!UICONTROL SSH 키를 사용하는 SFTP]** 인증을 지원합니다. 두 방법 모두 서버 도메인, 포트 및 사용자 이름이 필요합니다. 포트의 기본값은 `22`입니다.

SSH 키 형식, 서버, 네트워크 및 허용 목록에 추가하다 요구 사항에 대해서는 [SFTP 인증 정보](https://experienceleague.adobe.com/ko/docs/experience-platform/destinations/catalog/cloud-storage/sftp#authentication-information)를 참조하십시오.

### [!DNL Azure Blob Storage] {#azure-blob-storage}

Collaboration은 저장소 계정 연결 문자열을 사용하여 [!DNL Azure Blob Storage]에 대해 인증합니다.

연결 문자열을 가져오고 저장소 권한을 할당하는 방법에 대한 지침은 [대상에 대한 인증 [!DNL Azure Blob Storage] 대상](https://experienceleague.adobe.com/ko/docs/experience-platform/destinations/catalog/cloud-storage/azure-blob#authenticate)을 참조하십시오.

### [!DNL Google Cloud Storage] {#google-cloud-storage}

Collaboration에는 [!DNL Google Cloud Storage] 상호 운용성 설정을 통해 생성된 [!DNL Google Cloud Storage] 액세스 키 ID 및 비밀 액세스 키가 필요합니다.

자격 증명 생성 및 버킷 권한 요구 사항에 대해서는 [대상에 대한 인증 [!DNL Google Cloud Storage] 대상](https://experienceleague.adobe.com/ko/docs/experience-platform/destinations/catalog/cloud-storage/google-cloud-storage#authenticate)을 참조하십시오.

### [!DNL Snowflake Batch] {#snowflake-batch}

[!DNL Snowflake Batch]은(는) 파일을 고객 관리 저장소로 내보내는 대신 [!DNL Snowflake] 데이터 공유를 사용합니다. Collaboration에는 별도의 인증 단계가 없습니다. 대상을 만드는 동안 Snowflake 계정 ID, 지역, 개인 링크 상태 및 계정 소유권 확인을 입력합니다.

계정 준비 및 비공개 목록 요구 사항에 대해서는 [[!DNL Snowflake Batch] 대상 설명서](https://experienceleague.adobe.com/ko/docs/experience-platform/destinations/catalog/warehouse/snowflake-batch)를 참조하십시오.

### [!DNL Data Landing Zone] {#data-landing-zone}

[!DNL Data Landing Zone]은(는) Adobe에서 프로비저닝되었으며 Collaboration에서 별도의 인증 단계가 필요하지 않습니다. 대상을 만드는 동안 대상 폴더 경로 및 파일 출력 설정을 지정합니다.

AWS에서 제공한 [!DNL Data Landing Zone]에 액세스하는 방법에 대한 자세한 내용은 [AWS에서 제공한 데이터 랜딩 영역 인증](https://experienceleague.adobe.com/ko/docs/experience-platform/destinations/catalog/cloud-storage/data-landing-zone#authenticate-dlz-aws)을 참조하십시오.

## 다음 단계 {#next-steps}

필요한 연결 정보를 얻은 후 [대상을 구성하고 관리합니다](./manage-destinations.md).
