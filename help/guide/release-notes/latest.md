---
title: 최신 Real-Time CDP Collaboration 릴리스 노트
description: Real-Time CDP Collaboration의 최신 릴리스를 따르십시오.
audience: admin, publisher, advertiser
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 8513c648-1cc1-4544-b86d-2ee3193ab60f
TQID: https://experienceleague.adobe.com/re4oFblCLiZpspWIS7D4EEYNh36EDhULEOd2-ccXH28
product_v2: id: fdddec33-c9cb-4459-b8b6-2664395a6f10
feature_v2: id: ba929a52-9339-4154-9487-317dc875a3c7
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: c1579802-ddd4-4214-8a91-97b2066abe11id: c2be0313-b3ae-45e0-b454-d20bf54b23f2id: e1e0219c-f879-479f-8427-888ed2a6e9c2id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
source-git-commit: e6156a39107edb0e15e2115db0762f6a86801ed6
workflow-type: tm+mt
source-wordcount: 1968
ht-degree: 4%

---

# 최신 Real-Time CDP Collaboration 릴리스 노트

{{limited-availability-release-note}}

**마지막 업데이트**: 2026년 7월.

이러한 릴리스 노트는 Adobe Real-Time CDP Collaboration에 릴리스된 기능을 다룹니다. Collaboration 릴리스는 연속 게재 모델에서 작동하므로 대략적인 월별 릴리스 케이던스를 사용할 수 있습니다. 이러한 릴리스 노트는 자주 업데이트되므로 정기적으로 확인하십시오.

## 2026년 7월 {#july-2026}

이제 Real-Time CDP Collaboration에서 추가적인 셀프서비스 대상 소싱 옵션을 지원합니다.

**새로운 기능 또는 업데이트된 기능**

| 기능 | 설명 |
| ------- | ----------- |
| [!DNL Databricks Delta Share] 및 Adobe Audience Manager의 셀프서비스 대상 소싱 | 이제 [!DNL Databricks Delta Share]에서 직접 자사 대상을 소싱하거나 적격한 Adobe Audience Manager 세그먼트를 Collaboration으로 가져올 수 있습니다. 설치 지침은 다음 안내서를 참조하십시오. <ul><li>대상 소싱에 대해 [구성 [!DNL Databricks Delta Share] 구성](../setup/configure-databricks-audience-sourcing.md)</li><li>[대상 소싱에 대한 Adobe Audience Manager 구성](../setup/configure-aam-audience-sourcing.md)</li></ul> |

{style="table-layout:auto"}

## 2026년 4월 {#april-2026}

이제 Real-Time CDP Collaboration에서 새로운 기능을 사용할 수 있습니다. 여기에는 파트너 초대를 위한 Collaboration [!DNL Starter], 대상 소싱 범위를 [!DNL Snowflake] 및 [!DNL Google Cloud Storage]에서 확대하고, 일치 키로 [!DNL Demdex ID (ECID)]에 대한 지원과, 에이전시와 데이터 파트너의 두 가지 새로운 공동 작업자 역할이 포함됩니다.

**새로운 기능 또는 업데이트된 기능**

| 기능 | 설명 |
| ------- | ----------- |
| Real-Time CDP Collaboration [!DNL Starter] | 이제 Collaboration 라이선스가 없는 파트너를 Collaboration [!DNL Starter]을(를) 통해 귀하와 공동 작업하도록 초대할 수 있습니다. 초대된 파트너는 공유 연결 내에서 대상을 소싱하고, 중복을 발견하고, 대상을 활성화할 수 있습니다. 시작하려면 [Collaboration [!DNL Starter] 개요](../overview/starter-overview.md)를 참조하세요. |
| [!DNL Snowflake] 및 [!DNL Google Cloud Storage]의 셀프서비스 대상 소싱 | 이제 [!DNL Snowflake Secure Data Share] 또는 [!DNL Google Cloud Storage] 버킷에서 직접 자사 대상자를 Collaboration에 소싱할 수 있습니다. 설치 지침은 다음 안내서를 참조하십시오. <ul><li>대상 소싱에 대해 [구성 [!DNL Snowflake] 구성](../setup/configure-snowflake-audience-sourcing.md) </li><li> 대상 소싱에 대해 [구성 [!DNL Google Cloud Storage] 구성](../setup/configure-gcs-audience-sourcing.md) </li></ul> |
| [!DNL Demdex ID] 일치 키 | [!DNL Demdex ID]&#x200B;(ECID)은(는) 이제 여러 플랫폼에서 익명 쿠키 기반 ID를 일치시키기 위한 일치 키로 지원됩니다. 인증된 사용자 데이터에 의존하지 않고 대상 겹침 정확도를 향상시킵니다. 자세한 내용은 [지원되는 일치 키](../setup/onboard-account.md#supported-match-keys)를 참조하십시오. |
| 새 공동 작업자 역할 | 이제 Collaboration에서 **Agency** 및 **Data partner**&#x200B;를 비롯한 두 개의 추가 공동 작업자 역할을 지원합니다. 이러한 역할은 다양한 조직이 플랫폼 내에서 참여하고 함께 작업할 수 있는 방법을 확장합니다. 자세히 알아보기: <ul><li>[공동 작업자 계정 역할](../overview/roles.md)</li><li>[Collaboration 패턴](../overview/collaboration-patterns.md)</li><li>[전체 워크플로](../overview/end-to-end-workflow.md)</li></ul> |

{style="table-layout:auto"}

## 2026년 3월 {#march-2026}

이제 Real-Time CDP Collaboration에서 캠페인 측정 보고서를 생성하고 측정 데이터를 관리할 수 있습니다.

**새로운 기능 또는 업데이트된 기능**

| 기능 | 설명 |
| ------- | ----------- |
| 측정 일반 가용성 | 이제 Collaboration에서 측정 보고를 일반적으로 사용할 수 있습니다. 이제 마케팅 캠페인과 연결된 캠페인 ID를 게시자로, 소스 전환 데이터를 광고주로 입력하고, 두 가지 유형의 보고서를 생성할 수 있습니다. 전체 캠페인 결과의 경우 **캠페인 요약**, 캠페인 효과 통찰력의 경우 **속성**. 시작하려면 다음 안내서를 참조하십시오. <ul><li>[캠페인 ID 입력](../collaborate/manage-projects.md#manage-campaign-id)</li><li>[Source 전환 데이터](../setup/onboard-measurement-data.md)</li><li>[측정 보고서 만들기 및 보기](../collaborate/measure.md)</li></ul> |
| 측정 수명 주기 관리 | Collaboration은 또한 측정 관리를 지원합니다.<ul><li> 이제 광고주는 정확한 최신 캠페인 분석을 위해 측정 데이터 연결 및 관련 전환 이벤트를 모두 편집하거나 삭제할 수 있습니다. 자세한 내용은 [측정 데이터 연결 관리](../setup/manage-measurement-data-connection.md) 및 [전환 이벤트 관리](../setup/onboard-measurement-data.md#edit-measurement-data)를 참조하십시오.</li><li>공동 작업 프로젝트의 **[!UICONTROL 측정]** 탭에서 예약된 측정 보고서를 직접 편집하거나 삭제할 수도 있습니다. 모든 사용자가 사용할 수 있습니다. 자세한 내용은 [측정 보고서 관리 가이드](../collaborate/measure.md)를 참조하세요.</li></ul> |

{style="table-layout:auto"}

## 2026년 2월 {#february-2026}

Real-Time CDP Collaboration은 이제 인터페이스에서 직접 기존 연결 및 데이터 연결 설정을 편집할 수 있습니다.

**새 기능 또는 업데이트된 기능**

| 기능 | 설명 |
| ------- | ----------- |
| 연결 설정 편집 | 이제 연결 소유자는 연결이 설정된 후 사용 사례, 일치 키, 활성화 권한 및 크레딧 분할을 업데이트할 수 있습니다. 단계별 지침은 [연결 편집](../connect/manage-connections.md#edit-connection)을 참조하십시오. |
| 데이터 연결 편집 | Collaboration 내에서 직접 기존 데이터 연결에 대한 일치 키 및 예약 구성을 업데이트합니다. 단계별 지침은 [데이터 연결 편집](../setup/manage-data-connection.md#edit-data-connection)을 참조하십시오. |

## 2026년 1월 {#january-2026}

이제 Real-Time CDP Collaboration은 향상된 대상 일치 및 측정을 위한 새 모바일 일치 키(IDFA 및 GAID)는 물론, 대상 소싱을 위한 새 방법으로 CSV 파일 업로드를 지원합니다.

**새로운 기능 또는 업데이트된 기능**

| 기능 | 설명 |
| ------- | ----------- |
| 대상자 소싱에 대한 CSV 업로드 | CSV 파일을 소스 대상자에 업로드하여 UI에서 바로 Collaboration으로 사용할 수 있습니다. 단기 공동 작업 프로젝트를 위한 자사 데이터에 온보딩하는 데 이상적입니다. 자세한 내용은 [대상 소싱 안내서의 CSV 파일 업로드](../setup/upload-csv-audience-sourcing.md)를 참조하십시오. |
| 모바일 일치 키 지원 | Collaboration은 이제 대상 일치 및 측정을 위해 IDFA 및 GAID를 포함한 모바일 일치 키를 지원합니다. 이러한 일치 키는 계정 설정 중에 선택한 다음 새 연결에 대한 연결 설정을 구성할 때와 다운스트림 공동 작업 워크플로에서 사용할 수 있습니다. 자세한 내용은 [키 일치 설정 가이드](../setup/onboard-account.md#set-up-match-keys)를 참조하세요. |

{style="table-layout:auto"}

## 2025년 12월 {#december-2025}

이제 **유럽, 중동 및 아프리카(EMEA)**&#x200B;의 고객이 Real-Time CDP Collaboration을 사용할 수 있습니다. 이러한 지역의 Real-Time CDP Prime 및 Ultimate 고객이 자동으로 사용할 수 있습니다.

## 2025년 8월 {#august-2025}

이제 **캐나다**&#x200B;의 고객이 Real-Time CDP Collaboration을 사용할 수 있습니다. 이러한 지역의 Real-Time CDP Prime 및 Ultimate 고객이 자동으로 사용할 수 있습니다.

* Collaboration은 이제 다음 [일치 키](../setup/onboard-account.md#supported-match-keys)를 지원합니다.
  * 해시된 이메일
  * 해시된 전화번호
  * CRM ID
  * 충성도 ID
  * 해시된 IPv4
  * AdFixus ID
* 이제 Collaboration 전체에서 여러 일치 키를 사용할 수 있으므로 대상 크기를 확장하고 일치율을 향상시킬 수 있습니다. 대상을 소싱하고, 연결을 설정하고, 대상을 활성화할 때 여러 일치 키를 사용할 수 있습니다. 여러 일치 키 사용에 대한 자세한 내용은 [일치 키 설정](../setup/onboard-account.md) 및 [소싱 대상](../setup/onboard-audiences.md#map-fields) 안내서를 참조하십시오.

>[!IMPORTANT]
>
>여러 일치 키가 사용되는 대상을 활성화할 때, 하나(또는 그 이상) 일치 키에 겹침이 없거나, 대상자 규모가 없거나, 임계값 미만이면 전체 활성화가 실패합니다. 활성화하기 전에 대상이 충분히 겹치고 모든 일치 키에서 최소 1000 ID 임계값을 충족하는지 확인하십시오.

* 이제 Adobe Experience Platform 대상이 여러 일치 키로 대상 활성화를 지원합니다. 또한 이제 활성화 중에 전송되는 일치 키를 지정하기 위해 대상의 매핑을 구성할 때 연결된 키를 사용할 수 있습니다. 자세한 내용은 [Experience Platform 대상](../destinations/experience-platform.md#linked-keys) 안내서를 참조하십시오.
* 이제 공동 작업자가 여러 대상을 한 번에 편집할 수 있습니다. 이제 일괄 편집 도구를 사용하여 여러 대상에 대한 대상 메타데이터, 연결 액세스, 이름, 설명 및 범주를 편집할 수 있습니다. 대상자 편집에 대한 자세한 내용은 [대상자 관리](../setup/onboard-audiences.md#edit-audiences) 안내서를 참조하십시오.

## 2025년 7월 {#july-2025}

Real-Time CDP Collaboration은 이제 브랜드 간 공동 작업을 지원합니다. 이제 공동 작업자는 광고주인지 게시자인지에 관계없이 연결을 형성할 수 있습니다. 이를 통해 보다 유연한 공동 작업 기회를 얻을 수 있으며 브랜드가 서로의 데이터와 통찰력을 활용할 수 있습니다. 브랜드 간 공동 작업과 광고주 간 공동 작업의 차이점에 대해 자세히 알아보려면 [공동 작업 패턴](../overview/collaboration-patterns.md) 안내서를 읽어 보십시오.

* 공동 작업자는 이제 [개인 연결 초대](../connect/establishing-connections.md#private-connection-invites)를 사용하여 서로 연결할 수 있습니다. 계정의 고유 연결 코드를 공동 작업자와 공유하면 공동 작업자가 이를 사용하여 사용자와 직접 연결할 수 있습니다. 이는 브랜드 간 공동 작업의 핵심 기능으로, 공동 작업자는 **[!UICONTROL 공동 작업자 검색]** 디렉터리를 탐색하는 광고주를 넘어 연결을 설정할 수 있습니다.
* 이제 [셀프 서비스 대상](../setup/manage-destinations.md)을 광고주와 게시자 모두에서 사용할 수 있습니다.
* 이제 [계정 역할](../overview/roles.md)에 관계없이 연결된 두 공동 작업자에 대해 대상 활성화를 사용할 수 있습니다. 대상 활성화 설정은 [연결을 설정하는 동안](../connect/establishing-connections.md#configure-connection-settings)구성되어 대상을 활성화할 수 있는 공동 작업자를 지정할 수 있습니다. 대상자 활성화에 대한 자세한 내용은 [대상자 활성화](../collaborate/activate.md) 안내서를 참조하십시오.
* 브랜드 간 공동 작업을 지원하도록 **[!UICONTROL 활성화]** 사용 사례를 다시 구성했습니다. 이제 프로젝트 내의 **[!UICONTROL 활성화]** 탭에 공동 작업자에게 전송된 대상과 공동 작업자가 대상으로 활성화한 대상이 표시됩니다. 자세한 내용은 [대상자 활성화](../collaborate/activate.md) 안내서를 참조하십시오. <br> ![대상자 및 대상자 활성화 섹션이 있는 대시보드 활성화.](/help/assets/release-notes/2025/activate-dashboard.png){zoomable="yes"}
* 이제 프로젝트의 **[!UICONTROL 검색]** 탭에서 대상 인덱스 점수를 사용할 수 있습니다. 대상 색인 점수는 대상이 공동 작업자의 대상과 얼마나 잘 일치하는지 측정하는 것입니다. 이 점수는 기본 대상자 규모 및 중복을 기반으로 계산됩니다. 대상 색인 점수에 대한 자세한 내용은 [대상 색인 점수](../collaborate/discover.md#audience-index-score) 안내서를 참조하십시오.

## 2025년 5월 {#may-2025}

* 이제 **호주** 및 **뉴질랜드**&#x200B;의 고객이 Real-Time CDP Collaboration을 사용할 수 있습니다. 이러한 지역의 Real-Time CDP Prime 및 Ultimate 고객이 자동으로 사용할 수 있습니다.
* 이제 Real-Time CDP Collaboration에서 **[!UICONTROL 설정]** 섹션의 **[!UICONTROL 내 대상]** 탭을 통해 [셀프 서비스 대상](../setup/manage-destinations.md)을 제공합니다. 대상을 사용하면 광고 네트워크 또는 데이터 관리 플랫폼과 같은 서드파티 플랫폼에서 대상을 활성화하여 다양한 채널에서 고객에게 도달할 수 있습니다. 현재 Adobe Experience Platform 대상만 지원됩니다. 다른 대상을 구성하는 데 관심이 있는 경우 Adobe 담당자에게 문의하십시오. 대상에 대한 자세한 내용은 [대상 개요](../destinations/overview.md) 안내서를 참조하십시오.
  * 대상에는 [Collaboration 대상 포털](https://experienceleague.adobe.com/en/docs/experience-platform/segmentation/ui/audience-portal.md#manage-audiences)에서 Adobe Experience Platform 대상을 볼 수 있는 지원도 추가됩니다.
* 이제 Collaboration에서 기존 데이터 연결의 대상 새로 고침 빈도를 편집할 수 있습니다. 현재 대상자를 매일 또는 2~6일마다 새로 고치도록 선택할 수 있습니다. 대상 새로 고침 빈도를 편집하는 방법에 대한 자세한 내용은 [데이터 연결 관리](../setup/manage-data-connection.md#scheduling) 안내서를 참조하십시오.
* 이제 연결 내에서 선택한 각 사용 사례에 대해 공동 작업자 간의 크레딧 분할이 설정됩니다. 각 사용 사례에 대해 서로 다른 크레딧 소비 규칙을 설정하여 크레딧이 사용되는 방식을 보다 효과적으로 제어할 수 있습니다. 크레딧 분할 기능에 대해 자세히 알아보려면 [연결 설정](../connect/establishing-connections.md#connection-settings) 안내서를 읽어 보십시오. 크레딧 사용 방법에 대한 자세한 내용은 [크레딧 활동 유형](../setup/my-activity.md#types-of-activities) 안내서를 참조하십시오. <br> ![크레딧 분할 기능을 표시하는 연결 설정 화면입니다.](/help/assets/release-notes/2025/credit-split.png){zoomable="yes"}
* 이제 게시자는 광고주로부터 연결 설정을 수락하기 전에 광고주 이름과 ID를 설정할 수 있습니다. 게시자는 광고주의 이름 및 ID와 다를 수 있는 내부 시스템에 맞는 이름 및 ID를 설정할 수 있습니다. 광고주 이름 및 ID 추가에 대한 자세한 내용은 [연결 설정](../connect/establishing-connections.md#connection-settings.md) 안내서를 참조하십시오. <br> ![게시자 설정 광고주 이름 및 ID를 표시하는 연결 설정 화면입니다.](/help/assets/release-notes/2025/add-advertiser-names-modal.png){zoomable="yes"}

## 2025년 4월 {#april-2025}

* 새 **[!UICONTROL 입력 처리됨]** 열이 신용 소비 활동 테이블에 추가되었습니다. 이 열에는 각 활동에 대해 처리된 총 입력 수(예: ID 또는 행)가 표시됩니다. [자세히 보기](/help/guide/setup/my-activity.md#inputs-processed). <br> ![내 활동 보기에서 처리된 입력 열이 강조 표시되었습니다.](/help/assets/release-notes/2025/inputs-processed-column.png){zoomable="yes"}
* 새 연락처 이메일 옵션이 계정 만들기에 추가되었습니다. 이렇게 하면 파트너 공동 작업자가 연결 프로세스 중에 필요에 따라 연락할 수 있습니다. [자세히 보기](../setup/onboard-account.md).

## 2025년 3월 {#march-2025}

* 이제 [대상을 Collaboration에 소싱](/help/guide/setup/onboard-audiences.md)할 때 [대상 관리 크레딧 활동](/help/guide/setup/my-activity.md#types-of-activities)을 더 잘 관리하기 위해 **1일에서 6일마다**&#x200B;의 대상 새로 고침 빈도를 설정할 수 있습니다. 자세한 내용은 [대상자 관리](https://experienceleague.adobe.com/en/docs/experience-platform/segmentation/ui/audience-portal.md#manage-audiences) 안내서를 참조하십시오. <br> ![대상자 멤버십을 업데이트하기 위한 다른 빈도 간격을 보여 주는 예약 화면입니다.](/help/assets/setup/add-manage-audiences/audience-scheduling-frequency.png "대상자 멤버십을 업데이트하기 위한 다른 빈도 간격을 보여 주는 예약 화면"){width="250" align="center" zoomable="yes"}
* 이제 공동 작업자와 연결을 설정할 때 사전 정의된 **사용 사례**&#x200B;에서 선택할 수 있습니다. 선택한 사용 사례에 따라 사용 가능한 프로젝트 섹션과 제품 기능이 결정됩니다. 자세한 내용은 [프로젝트 관리](/help/guide/collaborate/manage-projects.md#project-use-cases) 안내서를 참조하십시오.
  * *Measurement*&#x200B;에서 **Measure** 프로젝트 섹션을 사용하도록 설정합니다.
  * *대상 검색*&#x200B;에서 **검색** 프로젝트 섹션을 사용하도록 설정합니다.
  * *대상 활성화*&#x200B;를 통해 **활성화** 프로젝트 섹션 <br>을(를) 사용할 수 있습니다.
* 이제 더 이상 함께 작업하지 않으려는 공동 작업자와의 연결을 삭제할 수 있습니다. 연결을 삭제하는 방법에 대해 알아보려면 [연결 삭제](/help/guide/connect/establishing-connections.md#delete-connections) 안내서를 참조하십시오.

## 2025년 2월 {#february-2025}

광고주와 게시자가 서드파티 쿠키 없이 고부가가치 대상을 검색, 활성화 및 측정할 수 있도록 특별히 제작된 Adobe Real-Time CDP Collaboration은 현재 미국에서 일반적으로 사용할 수 있습니다.

### 시작하기

1. **액세스 설정**: 시스템 관리자는 사용자에 대한 액세스 권한을 구성합니다. 액세스 권한 구성에 대한 자세한 내용은 [사용자 액세스 관리](/help/guide/permissions/manage-user-access.md#RTCDP-collaboration-access) 안내서를 참조하십시오.
2. **데이터 원본 연결**: Collaboration에서 사용할 Source 대상입니다. 대상자 소싱을 시작하려면 [소스 및 대상자 관리](/help/guide/setup/onboard-audiences.md) 안내서를 읽어 보세요.
3. **연결 설정**: 신뢰할 수 있는 광고주 또는 게시자와 공동 작업을 시작합니다. 연결 형성에 대한 자세한 내용은 [연결 설정](/help/guide/connect/establishing-connections.md) 안내서를 참조하십시오.
4. **검색 및 활성화**: 캠페인에서 활성화할 중요한 대상을 식별하는 프로젝트를 만듭니다. 프로젝트 만들기에 대한 자세한 내용은 [프로젝트 관리](/help/guide/collaborate/manage-projects.md) 안내서를 참조하십시오.

### 가용성

* Adobe Real-Time CDP Collaboration은 현재 미국 고객만 사용할 수 있습니다.
* Adobe Real-Time CDP Prime 및 Ultimate 고객에게 자동으로 제공됩니다

자세한 내용은 다음을 참조하십시오.

* [Collaboration 개요](/help/guide/home.md)
* [전체 워크플로](/help/guide/overview/end-to-end-workflow.md)
* [권한 개요](/help/guide/permissions/overview.md)
