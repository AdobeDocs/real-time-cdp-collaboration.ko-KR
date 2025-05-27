---
title: 신용 소비 활동 추적
description: Real-Time CDP Collaboration에서 조직의 신용 사용 활동을 추적하는 방법에 대해 알아봅니다.
audience: admin, publisher, advertiser
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: b24d63e7-60f4-4cdb-ab1b-77c284543486
source-git-commit: 7e9e6ae51d9741891e916c0dfd5ec0047a995c21
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# 신용 소비 활동 추적

{{limited-availability-release-note}}

**[!UICONTROL 내 활동]** 탭을 사용하여 모든 공동 작업 활동에서 조직의 예상 크레딧 소비를 모니터링하고 추적합니다. 이 기능은 다양한 연결 및 활동에서 크레딧이 사용되는 방법에 대한 자세한 통찰력을 제공하여 리소스를 효과적으로 관리하는 데 도움이 됩니다.

>[!IMPORTANT]
>
>신용 소비 테이블은 모니터링하기 위해 일별로 반올림되고 집계됩니다. **[!UICONTROL 내 활동]** 대시보드의 수치는 *예상* 신용 소비를 나타냅니다. 청구에 사용된 *실제* 신용 소모는 내부 시스템에서 추적되며 요청 시 사용할 수 있습니다. 해당 정보를 얻으려면 Adobe 담당자에게 문의하십시오.

예상 신용 사용 활동에 액세스하려면 기본 탐색에서 **[!UICONTROL 설정]**(으)로 이동한 다음 **[!UICONTROL 내 활동]** 탭을 선택하십시오.

![크레딧 사용 세부 정보를 표시하는 내 활동 대시보드](/help/assets/setup/my-activity-credits/activity-dashboard.png)

>[!TIP]
>
>**[!UICONTROL 내 활동]** 보기에는 Real-Time Collaboration CDP 사용자 인터페이스의 다른 부분에 있는 사용자 작업에 대한 정보가 포함되어 있지 않습니다. [감사 로그](/help/guide/setup/audit-logs.md) 기능을 사용하여 해당 정보를 가져옵니다.

## 활동 대시보드 이해 {#understand-dashboard}

활동 대시보드에는 조직 내에서 크레딧을 사용하는 모든 작업의 전체 목록이 표시됩니다. 각 행은 개별 활동을 나타내며 신용 사용에 대한 주요 정보를 제공합니다.

>[!NOTE]
>
>**[!UICONTROL Audience Management]** 활동이 다른 공동 작업자와 연결되어 있지 않으므로 이러한 활동 유형의 **[!UICONTROL 연결 ID]** 및 **[!UICONTROL 연결 이름]** 열은 **[!UICONTROL N/A]** 값을 나타냅니다.

| 열 | 설명 |
|------------|--------------|
| **[!UICONTROL 날짜]** | 활동이 발생한 날짜로서 YYYY/MM/DD 형식으로 표시됩니다. |
| **[!UICONTROL 연결 ID]** | 신용 소비 활동과 연관된 각 연결에 대한 고유 식별자로, 영숫자 문자열로 표시됩니다. |
| **[!UICONTROL 연결 이름]** | 연결 및 신용 소비 활동과 연관된 공동 작업자의 이름입니다. |
| **[!UICONTROL 활동]** | **활성화 - 공유**, **활성화 - 이그레스** 또는 **대상자 관리**&#x200B;와 같이 수행되는 활동 유형입니다. |
| **[!UICONTROL 처리된 입력]** | 활동에 대해 처리된 총 입력(예: ID 또는 행) 수입니다. |
| **[!UICONTROL 사용된 총 크레딧]** | 활동에서 소비한 총 크레딧 수입니다. |
| **[!UICONTROL 내 크레딧 공유]** | 활동에 사용된 크레딧의 조직 부분입니다. |

{style="table-layout:auto"}

## 활동 유형 {#types-of-activities}

**[!UICONTROL Activity]** 열에는 크레딧을 사용하는 다양한 작업 유형이 표시됩니다.

* **[!UICONTROL 대상 관리]**: 대상을 Real-Time CDP Collaboration으로 가져올 때 크레딧이 사용됩니다. 크레딧은 모든 대상에 대해 Real-Time CDP Collaboration 내에서 인덱싱된 ID 수(백만 단위)와 해당 인덱싱의 빈도(매일, 3일마다 또는 매주)의 함수로 사용됩니다. 자세한 내용은 [대상자 가져오기 및 관리](/help/guide/setup/onboard-audiences.md) 안내서를 참조하십시오.
* **[!UICONTROL 활성화 - 일치]** - 크레딧은 일치하고 활성화를 위해 준비된 ID 수의 함수로 사용됩니다. 자세한 내용은 [대상자 활성화](/help/guide/collaborate/activate.md) 안내서를 참조하십시오.
* **[!UICONTROL 활성화 - 이그레스]** - 대상으로 전송된 ID 수에 따라 크레딧이 사용됩니다. 이는 항상 대상자를 받는 공동 작업자에게 청구됩니다. 자세한 내용은 [대상자 활성화](/help/guide/collaborate/activate.md) 안내서를 참조하십시오.
* **[!UICONTROL 대상 측정]** - Real-Time CDP Collaboration에서 활동을 실행하여 캠페인 성과 보고서와 통찰력을 생성합니다. 크레딧은 모든 캠페인의 캠페인 보고서 행 수 및 보고 빈도를 기반으로 사용됩니다(매일, 3일마다 또는 매주).

## 신용 소비 관리 {#manage-credit-consumption}

신용 소비를 효과적으로 관리하려면

1. 각 활동과 관련된 신용 소비를 **이해**&#x200B;합니다. 활동당 사용된 공동 작업 크레딧 표에 대해서는 [Real-Time CDP Collaboration 제품 설명](https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html){target=_blank}을 확인하십시오.
2. **정기적으로 모니터링**: 사용 패턴을 이해하려면 활동 대시보드를 자주 확인하십시오.
3. **연결별 추적**: 연결 이름을 사용하여 크레딧을 가장 많이 사용하는 파트너 관계를 식별합니다.

<!--

## Pagination and navigation

The activity list is paginated to improve performance and readability. Use the navigation controls at the bottom of the table to move between pages and adjust how many records you can view at once.

-->
