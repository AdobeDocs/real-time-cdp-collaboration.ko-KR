---
title: Amazon Marketing Cloud
description: Real-Time CDP Collaboration에서 Amazon Marketing Cloud과의 공동 작업에 대해 알아봅니다.
audience: publisher, advertiser
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 1a1b8fec-384b-465f-832d-0772c518fdf1
source-git-commit: f0e260d9bf15a0230940c967e6d73e7431625358
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 4%

---

# Amazon Marketing Cloud

{{limited-availability-release-note}}

[!DNL Amazon Marketing Cloud]&#x200B;([!DNL AMC])과(와) 연결을 형성한 후 광고주는 [프로젝트를 만들고](../manage-projects.md#create-project) [!DNL AMC]과(와) 공동 작업하여 고급 분석 기능을 활용할 수 있습니다. 프로젝트를 만든 후 **[!UICONTROL 검색]** 섹션을 사용하여 대상 인사이트를 비교하고 캠페인에 대한 관련 대상을 검색할 수 있습니다.

>[!IMPORTANT]
>
>[!DNL AMC]에서 지원되는 사용 사례는 **대상 검색** 및 **측정**&#x200B;뿐입니다. 현재 프로젝트 내에서 **[!UICONTROL 을(를) 통해]**&#x200B;검색[!DNL AMC] 섹션만 사용할 수 있습니다.

## 검색 {#discover}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_compare_audiences"
>title="대상자 비교"
>abstract="대상을 Amazon 광고가 제공하는 모든 소비자와 비교합니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_relevant_audiences"
>title="관련 대상자"
>abstract="Amazon DSP 노출 횟수만을 고려하여 대상자가 겹치는 정도가 가장 높은 세그먼트를 타겟팅합니다(이러한 세그먼트는 DSP에서만 타겟팅할 수 있음)."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_resolved_ids"
>title="해결된 ID"
>abstract="대상 데이터를 사용하여 Amazon의 ID 확인을 확인할 수 있는 ID 수입니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_overlapping_ad_exposed_ids"
>title="중복 광고 노출 ID"
>abstract="업로드된 대상자 중 Amazon Ads를 통해 광고에도 노출된 &#39;해결된 ID&#39; 수를 나타냅니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_overlap_percentage"
>title="중복 %"
>abstract="Amazon 광고를 통해 광고에 노출된 &#39;해결된 ID&#39;의 비율입니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_amazon_breakdown"
>title="Amazon 광고 제품별 분류"
>abstract="Amazon Ads 후원 제품 및/또는 Amazon Ads DSP에 의해 도달된 &#39;겹치는 광고 노출 ID&#39; 분류입니다."

**[!UICONTROL 검색]** 섹션에서 AMC 대상자와 Amazon 광고가 제공하는 모든 소비자를 비교할 수 있습니다. DSP 노출 횟수만을 고려하여, 대상자와 가장 겹치는 Amazon 타겟팅 세그먼트를 볼 수도 있습니다(이러한 세그먼트는 DSP에서만 타겟팅할 수 있음).

>[!IMPORTANT]
>
>대상 데이터는 [!DNL Amazon Ads] 계정에 업로드된 대상에서 처리됩니다. [보내기]에서 Experience Platform의 대상 기능을 사용하여 대상자를 [!DNL Amazon Ads] 계정으로 보내는 방법에 대해 알아보려면 [Amazon 광고 연결](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/advertising/amazon-ads) 안내서를 참조하십시오.

![Amazon Marketing Cloud을 사용하는 프로젝트의 검색 섹션.](/help/assets/collaborate/advertising-platforms/amc-discover.png){zoomable="yes"}

### 대상자 비교 {#compare-audiences}

**[!UICONTROL 대상 비교]** 섹션에서는 [!DNL AMC] 대상이 Amazon 광고에서 도달한 소비자와 겹치는 방식에 대한 통찰력을 제공합니다. **[!UICONTROL 대상 비교]** 섹션 내에서 다음 지표를 볼 수 있습니다.

| 지표 | 설명 |
|--------------------------------|---------------------------------------------------------------------------------------------------|
| [!UICONTROL 확인된 ID] | 대상 데이터를 사용하여 ID [!DNL Amazon’s Identity Resolution]의 수를 확인할 수 있습니다. |
| [!UICONTROL 겹치는 광고 노출 ID] | 업로드된 대상자 중 [!UICONTROL 을(를) 통해 광고에 노출된 &#x200B;]확인된 ID[!DNL Amazon Ads]의 수입니다. |
| [!UICONTROL 겹치기 %] | [!UICONTROL 을(를) 통해 광고에 노출된 &#x200B;]확인된 ID[!DNL Amazon Ads]의 비율입니다. |
| [!UICONTROL Amazon 광고 제품별 분류] | [!UICONTROL 스폰서 제품] 및/또는 [!UICONTROL DSP]에 의해 [!UICONTROL 겹치는 광고 노출 ID]의 분류가 도달했습니다. 각각은 총 광고 노출 ID 수에서 개별 백분율로 표시됩니다. ID는 [!UICONTROL 스폰서 제품]과(와) [!UICONTROL DSP] 모두에 속할 수 있으므로 백분율이 100%로 합산되지 않을 수 있습니다. |


### 관련 대상자 {#relevant-audiences}

**[!UICONTROL 관련 대상]** 섹션에서는 DSP 노출 횟수만 고려하여 대상이 가장 많이 겹치는 [!DNL Amazon]개의 타깃팅 세그먼트 또는 대상에 대한 통찰력을 제공합니다(이러한 세그먼트는 DSP에서만 타깃팅할 수 있음). 모든 관련 대상을 전환하고 각 섹션 내에서 다음 지표를 볼 수 있습니다.

| 지표 | 설명 |
|--------------------------------|---------------------------------------------------------------------------------------------------|
| [!UICONTROL 확인된 ID] | 대상 데이터를 사용하여 ID [!DNL Amazon’s Identity Resolution]의 수를 확인할 수 있습니다. |
| [!UICONTROL 겹치는 광고 노출 ID] | 업로드한 대상자에서 [!UICONTROL 을(를) 통해 광고에 노출된 &#x200B;]확인된 ID[!DNL Amazon Ads]의 수를 나타냅니다. DSP 노출 횟수만 고려합니다. |
| [!UICONTROL 겹치기 %] | [!UICONTROL 을(를) 통해 광고에 노출된 &#x200B;]확인된 ID[!DNL Amazon Ads]의 비율입니다. |
| [!UICONTROL 범주] | 대상자가 속한 범주 또는 범주입니다. 대상은 여러 범주에 속할 수 있습니다. |

### [!DNL Amazon Marketing Cloud]과(와) 겹침 검색 {#discover-overlaps}

**[!UICONTROL Amazon Marketing Cloud과 겹침]** 섹션에서는 대상이 [!DNL Amazon] 타깃팅 세그먼트 또는 대상과 겹치는 방법에 대한 통찰력을 제공합니다. 다음 지표를 볼 수 있습니다.

| 지표 | 설명 |
|--------------------------------|---------------------------------------------------------------------------------------------------|
| [!UICONTROL 확인된 ID] | 대상 데이터를 사용하여 ID [!DNL Amazon’s Identity Resolution]의 수를 확인할 수 있습니다. |
| [!UICONTROL 겹치는 광고 노출 ID] | 업로드한 대상자에서 [!UICONTROL 을(를) 통해 광고에 노출된 &#x200B;]확인된 ID[!DNL Amazon Ads]의 수를 나타냅니다. DSP 노출 횟수만 고려합니다. |
| [!UICONTROL 겹치기 %] | [!UICONTROL 을(를) 통해 광고에 노출된 &#x200B;]확인된 ID[!DNL Amazon Ads]의 비율입니다. |
