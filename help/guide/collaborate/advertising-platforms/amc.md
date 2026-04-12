---
title: Amazon Marketing Cloud
description: Learn about collaborating with Amazon Marketing Cloud in Real-Time CDP Collaboration.
audience: publisher, advertiser
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/kr/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 1a1b8fec-384b-465f-832d-0772c518fdf1
source-git-commit: f0e260d9bf15a0230940c967e6d73e7431625358
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 21%

---

# Amazon Marketing Cloud

{{limited-availability-release-note}}

After forming a connection with [!DNL Amazon Marketing Cloud] ([!DNL AMC]), advertisers can [create a project](../manage-projects.md#create-project) to collaborate with [!DNL AMC] to leverage its advanced analytics capabilities. After creating a project, you can use the **[!UICONTROL Discover]** section to compare audience insights and discover relevant audiences for your campaigns.

>[!IMPORTANT]
>
>The only use cases supported with [!DNL AMC] are **Audience discovery** and **Measurement**. Currently, only the **[!UICONTROL Discover]** section is available within your project with [!DNL AMC].

## 검색 {#discover}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_compare_audiences"
>title="대상자 비교"
>abstract="Amazon Ads로 도달한 모든 소비자와 대상자를 비교합니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_relevant_audiences"
>title="관련 대상자"
>abstract="DSP 노출 횟수만을 고려하여 대상자가 가장 많이 중복된 Amazon 타기팅 세그먼트(이 세그먼트는 DSP에서만 타기팅할 수 있음)입니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_resolved_ids"
>title="해결된 ID"
>abstract="대상자 데이터를 사용하여 Amazon의 ID 확인을 해결할 수 있는 ID 수입니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_overlapping_ad_exposed_ids"
>title="중복 광고 노출 ID"
>abstract="이는 업로드된 대상자 중 Amazon Ads를 통해 광고에 노출된 “해결된 ID”의 수를 나타냅니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_overlap_percentage"
>title="중복 %"
>abstract="Amazon Ads를 통해 광고에 노출된 “해결된 ID”의 비율입니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_amazon_breakdown"
>title="Amazon 광고 제품별 분류"
>abstract="Amazon Ads 스폰서 제품 및/또는 Amazon Ads DSP에서 도달한 “중복 광고 노출 ID” 분류입니다."

In the **[!UICONTROL Discover]** section, you can compare your AMC audience to all consumers reached by your Amazon Ads. You can also view Amazon targeting segments that your audience has the highest overlaps with, considering only DSP impressions (these segments can only be targeted in the DSP).

>[!IMPORTANT]
>
>Audience data is processed from the audiences uploaded to your [!DNL Amazon Ads] account. To learn how send use Experience Platform&#39;s Destinations feature to send yours audiences to your [!DNL Amazon Ads] account, read the [Amazon Ads connection](https://experienceleague.adobe.com/ko/docs/experience-platform/destinations/catalog/advertising/amazon-ads) guide.

![The Discover section in a project with Amazon Marketing Cloud.](/help/assets/collaborate/advertising-platforms/amc-discover.png){zoomable="yes"}

### 대상자 비교 {#compare-audiences}

The **[!UICONTROL Compare audiences]** section provides insights into how your [!DNL AMC] audience overlaps with consumers reached by your Amazon Ads. Within the **[!UICONTROL Compare audiences]** section, you can view the following metrics:

| 지표 | 설명 |
|--------------------------------|---------------------------------------------------------------------------------------------------|
| [!UICONTROL Resolved IDs] | The number of IDs [!DNL Amazon’s Identity Resolution] was able to resolve using your audience data. |
| [!UICONTROL Overlapping ad exposed IDs] | The number of [!UICONTROL Resolved IDs] from the uploaded audience that have also been exposed to an ad via [!DNL Amazon Ads]. |
| [!UICONTROL Overlap %] | The proportion of [!UICONTROL Resolved IDs] that have been exposed to an ad via [!DNL Amazon Ads]. |
| [!UICONTROL Breakdown by Amazon ad product] | Breakdown of [!UICONTROL Overlapping ad exposed IDs] reached by either [!UICONTROL Sponsored Product] and/or [!UICONTROL DSP]. Each is represented as an individual percentage from total number of ad exposed IDs. Since an ID can belong to both [!UICONTROL Sponsored Products] and [!UICONTROL DSP], the percentages may not sum to 100%. |


### 관련 대상자 {#relevant-audiences}

**[!UICONTROL 관련 대상]** 섹션에서는 DSP 노출 횟수만 고려하여 대상이 가장 많이 겹치는 [!DNL Amazon]개의 타깃팅 세그먼트 또는 대상에 대한 통찰력을 제공합니다(이러한 세그먼트는 DSP에서만 타깃팅할 수 있음). 모든 관련 대상을 전환하고 각 섹션 내에서 다음 지표를 볼 수 있습니다.

| 지표 | 설명 |
|--------------------------------|---------------------------------------------------------------------------------------------------|
| [!UICONTROL 확인된 ID] | 대상 데이터를 사용하여 ID [!DNL Amazon’s Identity Resolution]의 수를 확인할 수 있습니다. |
| [!UICONTROL 겹치는 광고 노출 ID] | 업로드한 대상자에서 [!DNL Amazon Ads]을(를) 통해 광고에 노출된 [!UICONTROL 확인된 ID]의 수를 나타냅니다. DSP 노출 횟수만 고려합니다. |
| [!UICONTROL 겹치기 %] | [!DNL Amazon Ads]을(를) 통해 광고에 노출된 [!UICONTROL 확인된 ID]의 비율입니다. |
| [!UICONTROL 범주] | 대상자가 속한 범주 또는 범주입니다. 대상은 여러 범주에 속할 수 있습니다. |

### [!DNL Amazon Marketing Cloud]과(와) 겹침 검색 {#discover-overlaps}

**[!UICONTROL Amazon Marketing Cloud과 겹침]** 섹션에서는 대상이 [!DNL Amazon] 타깃팅 세그먼트 또는 대상과 겹치는 방법에 대한 통찰력을 제공합니다. 다음 지표를 볼 수 있습니다.

| 지표 | 설명 |
|--------------------------------|---------------------------------------------------------------------------------------------------|
| [!UICONTROL 확인된 ID] | 대상 데이터를 사용하여 ID [!DNL Amazon’s Identity Resolution]의 수를 확인할 수 있습니다. |
| [!UICONTROL 겹치는 광고 노출 ID] | 업로드한 대상자에서 [!DNL Amazon Ads]을(를) 통해 광고에 노출된 [!UICONTROL 확인된 ID]의 수를 나타냅니다. DSP 노출 횟수만 고려합니다. |
| [!UICONTROL 겹치기 %] | [!DNL Amazon Ads]을(를) 통해 광고에 노출된 [!UICONTROL 확인된 ID]의 비율입니다. |
