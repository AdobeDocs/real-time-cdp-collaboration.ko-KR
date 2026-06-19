---
title: 소스 개요
description: Adobe Real-Time CDP Collaboration의 소스 커넥터에 대해 알아보기
audience: admin, publisher, advertiser
source-git-commit: b30d1b01e929e586404faac34650c7fd479d071b
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 10%

---

# 소스 개요

Adobe Real-Time CDP Collaboration에서 소스(또는 데이터 연결)는 대상 데이터의 출처입니다. Adobe 응용 프로그램, 클라우드 기반 저장소 또는 로컬 시스템의 파일과 같은 다양한 소스 유형에 연결하여 Collaboration 프로젝트의 [대상을 소스 및 관리](./onboard-audiences.md)할 수 있습니다. 대상자 소싱 워크플로우 동안 조직의 필요에 따라 선호하는 출처를 선택하고 설정할 수 있습니다.

## 소스 연결 {#connect-a-source}

출처를 연결하려면 출처를 입력해야 합니다. 먼저 **[!UICONTROL 설정]** 작업 영역에서 **[!UICONTROL 내 대상]** 탭으로 이동합니다.

추가 아이콘(![추가 아이콘](/help/assets/icons/plus.png))을 선택합니다. **[!UICONTROL 대상]**&#x200B;을(를) 선택하여 소싱 워크플로우를 시작합니다.

![대상자 추가 옵션과 대상자 옵션이 강조 표시된 내 대상자 작업 영역입니다.](/help/assets/setup/add-manage-audiences/add-audiences.png)

워크플로우 중에 소스를 선택하여 새 데이터 연결을 추가하라는 메시지가 표시됩니다. 선택하는 소스는 대상 데이터를 Collaboration으로 가져오는 방법을 결정합니다. 지원되는 모든 소스의 목록은 [사용 가능한 소스](#available-sources) 표를 참조하십시오.

![새 데이터 연결 추가 옵션이 강조 표시된 대상자 추가 작업 영역입니다.](/help/assets/setup/add-manage-audiences/add-data-connection.png)

소스를 선택하면 워크플로가 인증, 필드 매핑, 예약, 대상자 선택 등 연결별 설정 단계를 안내합니다.

### 사용 가능한 소스 {#available-sources}

Collaboration에서 사용할 수 있는 소스는 다음과 같습니다. 해당 출처에 대한 단계별 소싱 가이드를 보려면 아래 테이블에서 출처명을 선택합니다. 현재 사용할 수 없는 소스에 관심이 있는 경우 Adobe 담당자에게 문의하십시오.

| 소스 | 설명 | 가용성 |
| --- | --- | --- |
| [Adobe Experience Platform](./onboard-audiences.md) | 연결된 Experience Platform 인스턴스에서 대상을 가져오고 기존 고객 세그먼트를 다시 사용합니다. | 사용 가능 |
| [Amazon S3](./configure-aws-s3-audience-sourcing.md) | S3 버킷을 클라우드 인프라에서 대규모 자사 데이터 세트를 소싱하도록 연결합니다. | 사용 가능 |
| [[!DNL Snowflake]](./configure-snowflake-audience-sourcing.md) | 대규모 대상 데이터 집합을 가져오려면 [!DNL Snowflake Secure Data Share]을(를) 연결하세요. | 사용 가능 |
| [[!DNL Google Cloud Storage]](./configure-gcs-audience-sourcing.md) | GCS 버킷을 연결하여 [!DNL Google Cloud] 환경에 저장된 대상 데이터를 가져옵니다. | 사용 가능 |
| [CSV 파일 업로드](./upload-csv-audience-sourcing.md) | 로컬 시스템에서 바로 형식이 지정된 CSV 파일을 업로드하십시오. | 사용 가능 |
| Adobe Audience Manager | 기존 Audience Manager 세그먼트를 Collaboration 프로젝트로 가져옵니다. | *준비 중* |
| [[!DNL Azure Blob Storage]](./configure-azure-storage-audience-sourcing.md) | [!DNL Azure Blob Storage] 컨테이너를 [!DNL Microsoft Azure] 환경의 소스 자사 데이터 세트에 연결합니다. | 사용 가능 |
| [[!DNL Azure Data Lake Storage]](./configure-azure-storage-audience-sourcing.md) | [!DNL Azure Data Lake Storage Gen 2] 계정을 연결하여 [!DNL Azure] 데이터 레이크에 저장된 대상 데이터를 가져옵니다. | 사용 가능 |

{style="table-layout:auto"}

## 다음 단계

소스를 연결하고 대상자를 가져온 다음에는 세부 정보를 보거나 구성을 업데이트하거나 기존 소스를 삭제할 수 있습니다. 자세한 내용은 [데이터 연결 관리](./manage-data-connection.md) 안내서를 참조하십시오.
