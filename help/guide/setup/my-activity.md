---
title: 크레딧 사용 활동 추적
description: 조직의 Credit Wallet을 보고 Real-Time CDP Collaboration에서 신용 소비 활동을 추적하는 방법에 대해 알아봅니다.
audience: admin, publisher, advertiser
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/kr/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: b24d63e7-60f4-4cdb-ab1b-77c284543486
TQID: https://experienceleague.adobe.com/hDvkKFUCBYvsX8wntcYFrL6qZTxOo5CZOWAbxNwk7mw
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 681f4af47a58a2ce66b25b09d793d0b5b127df39
workflow-type: tm+mt
source-wordcount: 726
ht-degree: 4%

---

# 크레딧 사용 활동 추적 {#track-credit-consumption-activity}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_my_activity"
>title="자세히 보기"
>abstract=""

{{limited-availability-release-note}}

>[!BEGINSHADEBOX]

**90일 초과 사용 금지 기간**: 적격 지역의 고객은 해당 지역의 사용 가능한 날로부터 시작되는 90일 초과 사용 금지 기간을 이용할 수 있습니다. 이 기간 동안 고객은 크레딧 이용 한도를 초과한 과다 수수료를 부담하지 않습니다.

>[!ENDSHADEBOX]

신용 지갑 및 신용 사용 활동에 액세스하려면 기본 탐색에서 **[!UICONTROL 설정]**(으)로 이동한 다음 **[!UICONTROL 내 활동]** 탭을 선택하십시오.

![크레딧, 사용된 크레딧, 사용 가능한 크레딧, 크레딧 사용 활동 테이블을 표시하는 내 활동 탭입니다.](/help/assets/setup/my-activity-credits/activity-dashboard.png)

>[!TIP]
>
>**[!UICONTROL 내 활동]** 보기에는 Real-Time CDP Collaboration 인터페이스의 다른 영역에서 사용자 작업이 포함되지 않습니다. [감사 로그](/help/guide/setup/audit-logs.md) 기능을 사용하여 해당 정보를 가져옵니다.

## 내 활동 보기 이해 {#understand-dashboard}

**[!UICONTROL 내 활동]** 보기를 사용하여 크레딧 사용을 모니터링하고 크레딧을 사용하는 활동을 검토하세요. 뷰에는 신용 전자 지갑 및 활동 테이블이 포함됩니다.

신용 지갑에는 공급된 크레딧, 소비된 크레딧 및 사용 가능한 크레딧이 표시됩니다.

| 지표 | 설명 |
|---------|-------------|
| **[!UICONTROL 크레딧 프로비전됨]** | 계정에 대해 프로비저닝된 크레딧의 수입니다. |
| **[!UICONTROL 사용한 크레딧]** | 최근 일별 새로 고침 기준으로 계정에서 사용한 크레딧 수입니다. |
| **[!UICONTROL 사용 가능한 점수]** | 공급된 크레딧에서 소비된 크레딧을 뺀 값에서 계산되는 계정에 사용할 수 있는 크레딧 수입니다. |

{style="table-layout:auto"}

활동 테이블에는 일자, 활동 유형, 처리된 입력 및 사용된 대변별로 일일 신용 소비 레코드가 나열됩니다.

>[!NOTE]
>
>**[!UICONTROL Audience Management]** 활동이 다른 공동 작업자와 연결되어 있지 않으므로 이러한 활동 유형의 **[!UICONTROL 연결 ID]** 및 **[!UICONTROL 연결 이름]** 열에 **[!UICONTROL -]** 값이 표시됩니다.

| 열 | 설명 |
|------------|--------------|
| **[!UICONTROL 날짜]** | 활동이 발생한 날짜로서 YYYY/MM/DD 형식으로 표시됩니다. |
| **[!UICONTROL 연결 ID]** | 신용 소비 활동과 연관된 각 연결에 대한 고유 식별자로, 영숫자 문자열로 표시됩니다. |
| **[!UICONTROL 연결 이름]** | 연결 및 신용 소비 활동과 연관된 공동 작업자의 이름입니다. |
| **[!UICONTROL 활동]** | 수행된 활동 유형(예: **[!UICONTROL 활성화 - 대상 액세스(한 번)]**, **[!UICONTROL 활성화 - 대상 액세스(반복)]**, **[!UICONTROL 활성화 - 대상 이그레스(한 번)]**, **[!UICONTROL 활성화 - 대상 이그레스(반복)]** 또는 **[!UICONTROL 대상 관리]**). |
| **[!UICONTROL 처리된 입력]** | 활동에 대해 처리된 총 입력(예: ID 또는 행) 수입니다. |
| **[!UICONTROL 사용된 총 크레딧]** | 활동에서 소비한 총 크레딧. |
| **[!UICONTROL 내 크레딧 공유]** | 활동에 사용된 크레딧 중 계정의 부분입니다. |

{style="table-layout:auto"}

## 활동 유형 {#types-of-activities}

**[!UICONTROL Activity]** 열에는 크레딧을 사용하는 다양한 작업 유형이 표시됩니다.

* **[!UICONTROL 대상 관리]**: 대상을 Collaboration으로 가져올 때 크레딧이 사용됩니다. 크레딧은 모든 대상에 대해 Collaboration 내에서 인덱싱된 ID 수와 해당 인덱싱의 빈도(예: 매일, 3일마다 또는 매주)의 함수로 사용됩니다. 자세한 내용은 [대상자 소싱 및 관리](/help/guide/setup/onboard-audiences.md) 안내서를 참조하십시오.
* **[!UICONTROL 활성화 - 대상 액세스(한 번)]**: 활성화 워크플로우를 통해 대상 액세스를 한 번 처리하면 크레딧이 사용됩니다. 자세한 내용은 [대상자 활성화](/help/guide/collaborate/activate.md) 안내서를 참조하십시오.
* **[!UICONTROL 활성화 - 대상 액세스(반복)]**: 활성화 워크플로를 통해 대상 액세스가 반복 일정에서 처리될 때 크레딧이 사용됩니다. 자세한 내용은 [대상자 활성화](/help/guide/collaborate/activate.md) 안내서를 참조하십시오.
* **[!UICONTROL 활성화 - 대상 이그레스(한 번)]**: 대상에 대한 대상 이그레스가 활성화 워크플로우를 통해 한 번 처리되면 크레딧이 사용됩니다. 이 활동은 대상자를 받는 공동 작업자에게 청구됩니다. 자세한 내용은 [대상자 활성화](/help/guide/collaborate/activate.md) 안내서를 참조하십시오.
* **[!UICONTROL 활성화 - 대상 이그레스(반복)]**: 대상에 대한 대상 이그레스가 활성화 워크플로를 통해 반복 일정에서 처리될 때 크레딧이 사용됩니다. 이 활동은 대상자를 받는 공동 작업자에게 청구됩니다. 자세한 내용은 [대상자 활성화](/help/guide/collaborate/activate.md) 안내서를 참조하십시오.
* **[!UICONTROL 측정]**: Collaboration에서 캠페인 성과 보고서와 통찰력을 생성할 때 크레딧이 사용됩니다. 크레딧은 모든 캠페인에서 캠페인 보고서의 행 수 및 보고 빈도(예: 매일, 3일마다 또는 매주)를 기반으로 소비됩니다.

## 신용 소비 관리 {#manage-credit-consumption}

신용 소비를 효과적으로 관리하려면

1. 각 활동과 관련된 신용 소비를 **이해**&#x200B;합니다. 활동당 사용되는 크레딧 표에 대해서는 [Collaboration 제품 설명](https://helpx.adobe.com/kr/legal/product-descriptions/real-time-customer-data-platform-collaboration.html){target=_blank}을 확인하세요.
2. **정기적으로 사용 모니터링**: 사용 가능한 크레딧과 활동 테이블을 검토하여 대상 관리, 대상 액세스, 대상 이그레스 및 측정 활동 전반의 사용 패턴을 이해합니다.
3. **연결별 추적**: 연결 이름을 사용하여 크레딧을 가장 많이 사용하는 연결을 식별하십시오.
