---
title: 성능 측정
description: 다양한 채널에서 캠페인의 성과를 측정합니다. 다양한 보고서를 사용하고 해석하는 방법을 알아봅니다.
audience: admin, publisher, advertiser
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: c92b263e-1f96-49f1-841a-ef2e97a4cb9a
TQID: https://experienceleague.adobe.com/pr-qF4sd-NHd55kxh1dCstHRnVCUEhIvtv-47-ljiu4
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
feature_v2:
  - id: ba929a52-9339-4154-9487-317dc875a3c7
topic_v2:
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 3ce7e66b31332836fd6cc6137c94622436505cc9
workflow-type: tm+mt
source-wordcount: 2612
ht-degree: 5%

---

# 성능 측정

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>**[!UICONTROL Measure]** 작업 영역은 연결 프로세스 [&#128279;](../connect/establishing-connections.md#connection-settings) 동안 **Measurement** 사용 사례를 사용하도록 설정한 경우에만 사용할 수 있습니다. 사용 사례에 대한 자세한 내용은 [프로젝트 관리](./manage-projects.md#project-use-cases) 안내서를 참조하세요.

Adobe Real-Time CDP Collaboration의 사용 가능한 보고서에 대해 알아보고 다양한 채널에서 마케팅 캠페인의 성과를 측정하고 분석하는 방법을 이해합니다.

## 전제 조건 {#prerequisites}

Collaboration에서 측정 보고서에 액세스하려면 먼저 다음을 수행해야 합니다.

* **Measurement** 사용 사례가 활성화된 공동 작업자와 [연결](/help/guide/connect/establishing-connections.md)
* 공동 작업자와 하나 이상의 프로젝트에 대해 공동 작업을 수행합니다. [프로젝트를 만드는](/help/guide/collaborate/manage-projects.md#create-project) 방법을 알아봅니다.
* 캠페인을 실행하고 [캠페인에 대해 캠페인 ID가 제공되었는지 확인](../collaborate/manage-projects.md#manage-campaign-id):
   * 게시자인 경우 광고주의 캠페인에 연결된 캠페인 ID를 입력합니다.
   * 광고주인 경우 공동 작업자(게시자)에게 캠페인 ID를 제공하도록 요청하십시오. [측정값 작업 영역에서 보고서를 생성](#create-measurement-report)하는 데 필요합니다.
* [&#128279;](#create-attribution-report)속성 보고서를 만들려면[측정 데이터를 Collaboration에 업로드](/help/guide/setup/onboard-measurement-data.md)하십시오.

## 보고서 보기 {#view-reports}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_measurement_create_report_campaignID"
>title="캠페인 ID"
>abstract="캠페인 ID에 대한 관련 정보를 UI에 추가하기 위한 플레이스홀더입니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_measurement_create_report"
>title="캠페인 ID"
>abstract="캠페인 ID에 대한 관련 정보를 UI에 추가하기 위한 플레이스홀더입니다."

측정 탭에서 사용할 수 있는 보고서를 보려면 다음과 같이 하십시오.

1. **[!UICONTROL 공동 작업]** > **[!UICONTROL 내 프로젝트]**(으)로 이동합니다.
2. 원하는 프로젝트에 대해 **[!UICONTROL 보기]**&#x200B;를 선택하세요.
3. 프로젝트에서 **[!UICONTROL 측정값]** 탭을 선택합니다.

**[!UICONTROL 전체 보고서 보기]**&#x200B;를 선택하여 아래에서 자세히 설명하는 사용 가능한 다양한 보고서에 액세스합니다.

![프로젝트의 측정 탭에 액세스하는 방법](/help/assets/collaborate/measure/measurement.gif)

### 요약 보기

측정 탭의 페이지 상단 보기에는 참조할 수 있는 몇 가지 높은 수준의 숫자가 포함된 캠페인 요약이 표시됩니다.

**[!UICONTROL 노출 횟수]**: 크리에이티브가 표시된 총 횟수입니다.
**[!UICONTROL 고유 도달 범위]**: 크리에이티브를 본 개별 ID의 수입니다.
**[!UICONTROL 총 평균 빈도]**: 고유 ID로 나눈 노출 횟수에 도달했습니다. 이 수치는 모든 ID가 얼마나 자주 크리에이티브에 표시되었는지를 나타냅니다.

![캠페인 요약 보기](/help/assets/collaborate/measure/campaign-summary.png)

### 시간 경과에 따른 지표 {#metrics-over-time}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_measure_metricsovertime"
>title="시간 경과에 따른 지표"
>abstract="시간 경과에 따른 지표 보기를 사용하면 캠페인 기간 동안 광고에 대해 표시된 총 노출 수를 파악할 수 있습니다. 보고서에 표시할 차원을 최대 두 개까지 선택할 수 있습니다."

시간 경과에 따른 지표 보기를 사용하면 캠페인 기간 동안 광고에 대해 표시된 총 노출 수를 파악할 수 있습니다. 보고서에 표시하고 분석할 지표를 최대 2개까지 선택할 수 있습니다.

![시간 경과에 따른 지표 보기.](/help/assets/collaborate/measure/metrics-over-time.png)

### 빈도 분포 {#frequency-distribution}

빈도 분포 보기를 사용하여 각 고유 사용자에게 표시된 노출 횟수를 분류할 수 있습니다. 이 보기는 향후 캠페인에서 대상자 억제를 시작할 시점을 결정하는 데 도움이 될 수 있습니다. 예를 들어 이미 크리에이티브를 세 번 본 프로필을 표시하지 않을 수 있습니다.

![빈도 분포 보기.](/help/assets/collaborate/measure/frequency-distribution.gif)

### 차원별 지표 {#metric-by-dimension}

배치 매체의 컨텍스트에서 노출 횟수, 볼 수 있는 노출 횟수, 고유한 도달 범위, 비용 등과 같은 다양한 지표를 분석합니다. 캠페인에 가장 적합한 결과를 도출하는 미디어(예: 모바일 스트리밍, CTV 프로그래밍 방식 또는 기타)를 분석합니다.

차원별 ![지표.](/help/assets/collaborate/measure/metric-by-dimension.png)

### 누적 도달 곡선 {#cumulative-reach-curve}

캠페인이 진행되고 노출 횟수가 증가하면서 연락이 닿을 수 있었던 사용자 수도 늘어났는지 파악한다. 캠페인의 일반적인 패턴은 특정 시점 이후 크리에이티브가 동일한 사람에게 반복적으로 표시되는 고원에 도달한다는 것입니다. 이 보기는 새 사용자에게 더 이상 연락되지 않는 시점에 따라 향후 캠페인 기간을 조정하는 데 도움이 될 수 있습니다.

![누적 도달 곡선.](/help/assets/collaborate/measure/cumulative-reach-curve.png)

### 배치별 노출 횟수 {#impressions-by-placement}

어떤 매체가 창의적인 인상을 가져오는지 이해합니다. 이를 통해 향후 캠페인에 광고 지출을 어디에 투자할지 결정하는 데 도움이 될 수 있습니다.

배치별 ![노출 횟수.](/help/assets/collaborate/measure/impressions-by-placement.png)

### 누적 전환 {#cumulative-conversions}

이 보기는 측정하도록 선택한 전환 이벤트에 대한 세부 분류를 테이블 형식으로 제공합니다. 이 표에는 다음이 포함됩니다.

* **전환 이벤트**: 추적 중인 각 전환 이벤트의 이름.
* **전환 수**: 각 이벤트에 대해 발생한 총 전환 수입니다.
* **예상 매출**: 각 전환 이벤트에 속하는 예상 값입니다.

Review this table to evaluate the effectiveness of your campaign in driving the desired actions.

![Cumulative conversions.](/help/assets/collaborate/measure/cumulative-conversions.png)

### 일별 전환 {#conversions-by-day}

This chart provides a day-by-day breakdown of conversions for each event set up when you create an Attribution report. Use this view to uncover daily patterns, identify periods of high or low conversion activity, and compare how different conversion events perform across your campaign timeline.

![Conversions by day.](/help/assets/collaborate/measure/conversions-by-day.gif)

## 측정 보고서 생성 {#create-measurement-report}

In Collaboration, you can create two main types of measurement reports:

* **Campaign Summary**: Provides high-level metrics such as reach, impressions, average frequency, and delivery by channel, giving a quick overview of overall campaign performance.
* **Attribution**: Measures how campaign exposures drive downstream actions like conversions or purchases, helping you understand campaign effectiveness.

You can run Campaign Summary report on its own, while Attribution report requires both report types to be selected together.

### Create campaign summary report {#create-campaign-summary-report}

Both publishers and advertisers can generate **Campaign Summary** reports to evaluate campaign performance. Use these reports to gain insights into key metrics such as [reach](#cumulative-reach-curve), [frequency](#frequency-distribution), and [impressions](#impressions-by-placement), and understand how your campaign was delivered and its overall impact.

To generate a **Campaign Summary** report, navigate to the project workspace from the **[!UICONTROL Collaborator]** workspace. From the **[!UICONTROL Measure]** tab, select the add icon (![Add icon.](/help/assets/icons/plus.png)) and then select **[!UICONTROL Measure]**.

If this is your first report, you may also select the **[!UICONTROL Run report]** option.

![The Measure tab highlighting the Run report option and the Measure option.](/help/assets/collaborate/measure/run-measure-report.png)

The **[!UICONTROL Create measurement report]** screen appears with information and input fields grouped under **[!UICONTROL Billing details]**, **[!UICONTROL Campaign details]**, and **[!UICONTROL Report details]** sections.

#### 과금 세부 정보 {#billing-details}

This section explains how credits are used when generating measurement reports. Credit responsibility is established during [connection setup](../connect/establishing-connections.md#credit-split). Before running any reports, make sure to review and confirm the credit split settings and reporting roles with your collaborator.

#### 캠페인 세부 정보 {#campaign-details}

In the **[!UICONTROL Campaign details]** section, select the appropriate **Advertiser ID** to associate with your report. These advertiser names or IDs were added during [connection setup](../connect/establishing-connections.md#advertiser-names). If only one name was configured, it appears by default. If no name was set up, the **[!UICONTROL Advertiser ID (Name)]** field is disabled and prefilled with the advertiser account name.

![The Create measurement report screen showing the Advertiser ID (Name) option disabled.](/help/assets/collaborate/measure/advertiser-id.png)

Then, select the desired campaign from the **[!UICONTROL Campaign ID]** dropdown menu. This menu lists all campaign IDs entered by the publisher for your project. If the campaign you need isn&#39;t available, [add it in the UI](./manage-projects.md#manage-campaign-id) before generating the report.

![The Create measurement report screen showing the Campaign ID dropdown menu expanded.](/help/assets/collaborate/measure/campaign-id.png)

Next, specify the period you want the report to cover. Select **[!UICONTROL Report date range]**, then use the calendar to choose the start and end dates.

![The Create measurement report screen showing the Report date range calendar.](/help/assets/collaborate/measure/report-date-range.png)

#### 보고서 세부 정보 {#report-details}

**Report run date**

In the **[!UICONTROL Report details]** section, choose the date on which the report should run. Select **[!UICONTROL Report run date]** and choose your preferred date from the calendar.

* If you choose today&#39;s date or a date in the past, the **Campaign Summary** report runs right away.
* If you choose a future date, the **Campaign Summary** report is scheduled to run on that day.

![The Create measurement report screen showing the Report run date calendar.](/help/assets/collaborate/measure/report-run-date.png)

**Report type**

* If you&#39;re an advertiser, you can select the **[!UICONTROL Campaign summary]** report type from the available options. Only advertisers can generate attribution reports.
* If you&#39;re a publisher, the **[!UICONTROL Campaign summary]** report type is preselected and cannot be changed. At this time, publishers cannot run attribution reports.

![The Create measurement report screen showing the Campaign summary option as a preselected and unchangable report type.](/help/assets/collaborate/measure/cs-report-type.png)

Finally, review your settings and select **[!UICONTROL Create]**. Your campaign summary report generates immediately if the run date is today or earlier, or on the chosen future date. You can edit the scheduled report before its run date. For step-by-step instructions, refer to the [Edit measurement report] section.

Once available, you can view your report at any time in the **[!UICONTROL Measure]** tab within your project workspace.

![The Create measurement report screen showing the information and the Create option highlighted.](/help/assets/collaborate/measure/cs-review.png)

### Create attribution report {#create-attribution-report}

As an advertiser, you can generate **Attribution** reports to assess how your campaign exposures contribute to key outcomes such as sign-ups or purchases. Use these reports to understand user interactions with your campaign, identify which touchpoints drive the most impact, and inform more effective marketing strategies.

>[!IMPORTANT]
>
> You must [source your measurement data](../setup/onboard-measurement-data.md#add-measurement-data) into Collaboration before generating Attribution reports.
>![The Measure tab with the requirements for Measurement data and the disabled Measure option.](/help/assets/collaborate/measure/require-measurement-data.png)

To generate an **Attribution** report, navigate to the project workspace from the **[!UICONTROL Collaborator]** workspace. From the **[!UICONTROL Measure]** tab, select the add icon (![Add icon.](/help/assets/icons/plus.png)) and then select **[!UICONTROL Measure]**.

If this is your first report, you may also select the **[!UICONTROL Run report]** option.

![The Measure tab highlighting the Run report option and the Measure option.](/help/assets/collaborate/measure/run-measure-report-attribution.png)

The **[!UICONTROL Create measurement report]** screen appears with information and input fields grouped under **[!UICONTROL Billing details]**, **[!UICONTROL Campaign details]**, and **[!UICONTROL Report details]** sections.

Read and follow steps in the [Create campaign summary report](#create-campaign-summary-report) section to configure the following settings:

* [Billing details](#billing-details)
* [캠페인 세부 정보](#campaign-details)

#### Report details for Attribution reports {#report-details-attribution}

**Report run date**

>[!IMPORTANT]
>
> For attribution reports, the report run date must be a future date, and must occur at least one day after the end date of your report date range plus the full duration of the defined lookback window.
> **Report run date ≥ report end date + lookback window + 1**
> 
> For example, if your report date range ends on June 15 and the lookback window is 14 days, the report run date is June 30 or later.

In the **[!UICONTROL Report details]** section, choose the date on which the report should run. Select **[!UICONTROL Report run date]** and choose your preferred date from the calendar.

**Report type**

As an advertiser, you can select **[!UICONTROL Attribution]** as a report type in addition to **[!UICONTROL Campaign summary]**. When you choose the Attribution report, your results include both standard Campaign Summary metrics and detailed Attribution analysis, providing a comprehensive view of campaign performance.

![The Create measurement report screen highlighting both the Campaign summary and Attribution report types selected.](/help/assets/collaborate/measure/attribution-report-type.png)

When you select **[!UICONTROL Attribution]** as the report type, an **[!UICONTROL Attribution]** configuration section appears with additional required settings:

* **Lookback window in days**: Defines how far back the report considers campaign impressions before each conversion. Only impressions within this period are eligible for attribution credit.
* **Conversion events**: Specifies which conversion actions you want to measure, for example, purchases or sign-ups. These events must be set up in advance when you [source your measurement data](../setup/onboard-measurement-data.md#add-conversion-event) into Collaboration.

First, enter a value for the **[!UICONTROL Lookback window in days]** field, or adjust it with the increment/decrement options.

![The Create measurement report screen highlighting the value for Lookback window in days.](/help/assets/collaborate/measure/lookback-window-in-days.png)

Next, choose up to **3** conversion events from the available list. For more information about a particular event, select the **[!UICONTROL i]** icon to view its details.

![The Create measurement report screen highlighting the selected conversion events and the information of the Purchase event.](/help/assets/collaborate/measure/attribution-conversion-events.png)

Finally, review your settings and select **[!UICONTROL Create]** to schedule the report. Your attribution report will be generated on the specified run date. You can edit the scheduled report before its run date. For step-by-step instructions, refer to the [Edit measurement report] section.

Once available, you can view your report at any time in the **[!UICONTROL Measure]** tab within your project workspace.

![The Create measurement report screen showing the information and the Create option highlighted.](/help/assets/collaborate/measure/attribution-review.png)

## 측정 보고서 편집 {#edit-measurement-report}

>[!IMPORTANT]
>
>You can edit the settings of a measurement report only if it is scheduled to run in the future. For reports that have already been executed, settings cannot be changed.

Update a measurement report settings to ensure the report provides the correct analysis of your campaign within a specific period and runs on a desired date.

To begin, navigate to the workspace of the measurement report you want to update. Select the edit icon (![Edit icon](/help/assets/icons/edit.png)) next to the delete icon.

![The measurement report workspace with the Edit icon highlighted.](/help/assets/collaborate/measure/edit-report.png)

>[!TIP]
>
>In the **[!UICONTROL Measure]** tab, navigate to the report section you wish to edit. Select the edit icon (![Edit icon](/help/assets/icons/edit.png)) next to **[!UICONTROL View full report]** to update its settings.
>![The Measure tab highlighting the Edit icon within a report section.](/help/assets/collaborate/measure/measure-tab-edit-report.png)

다음 섹션에 보고서의 현재 설정이 있는 **[!UICONTROL 측정 보고서 편집]** 대화 상자가 나타납니다.

* [**청구 세부 정보**](#billing-details): 측정 보고서를 실행할 때 크레딧에 대한 정보를 표시합니다. 구성이 필요하지 않습니다.
* [**캠페인 세부 정보**](#campaign-details): 광고주, 캠페인 ID, 보고 기간 및 사용자에게 친숙한 보고서 이름에 대한 설정을 표시합니다.
* [**보고서 세부 정보**](#report-details): 보고서 유형, 보고서 실행 날짜 및 특성 보고서에 대한 구성 옵션에 대한 설정을 표시합니다.

![청구 세부 정보, 캠페인 세부 정보 및 보고서 세부 정보 섹션의 현재 설정을 표시하는 측정 보고서 편집 대화 상자입니다.](/help/assets/collaborate/measure/edit-measurement-report-dialog.png)

### 캠페인 세부 정보 편집 {#edit-campaign-details}

**[!UICONTROL 측정 보고서 편집]** 대화 상자에서 **[!UICONTROL 광고주 ID(이름)]** 및 **[!UICONTROL 캠페인 ID]** 드롭다운 메뉴를 사용하여 보고서의 광고주와 캠페인 ID를 편집합니다.

![캠페인 ID 드롭다운 메뉴를 강조 표시하는 측정 보고서 편집 대화 상자가 열립니다.](/help/assets/collaborate/measure/edit-campaign-id.png)

그런 다음 **[!UICONTROL 보고서 날짜 범위]**&#x200B;를 선택하고 달력을 사용하여 보고서의 시작 날짜와 종료 날짜를 변경합니다.

![보고서 날짜 범위 달력을 강조 표시하는 측정 보고서 편집 대화 상자가 열려 있습니다.](/help/assets/collaborate/measure/edit-report-date-range.png)

최근 변경 내용을 캡처하려면 업데이트된 친숙한 보고서 이름을 입력하십시오. 이렇게 하면 나중에 이 보고서를 인식하고 찾는 데 도움이 됩니다.

![업데이트된 친숙한 보고서 이름을 강조 표시하는 측정 보고서 편집 대화 상자입니다.](/help/assets/collaborate/measure/edit-friendly-report-name.png)

### 보고서 세부 정보 편집 {#edit-report-details}

다른 날짜에 대해 보고서를 예약하려면 **[!UICONTROL 보고서 세부 정보]** 섹션으로 이동하십시오. 현재 실행 날짜 옵션을 선택한 다음 달력을 사용하여 원하는 날짜를 선택합니다.

![보고서 실행 날짜 달력을 강조 표시하는 측정 보고서 편집 대화 상자입니다.](/help/assets/collaborate/measure/edit-report-run-date.png)

광고주는 **[!UICONTROL 캠페인 요약]** 외에 **[!UICONTROL 속성]** 보고서 유형을 선택하거나 제거할 수 있습니다. **[!UICONTROL 속성]**&#x200B;을 선택하는 경우 속성 보고서에는 표준 캠페인 요약 지표와 심층적인 속성 통찰력이 모두 포함됩니다. **캠페인 요약** 및 **속성** 보고서 유형에 대한 자세한 내용은 [측정 보고서 만들기](#create-measurement-report) 섹션을 참조하십시오.

>[!IMPORTANT]
>
>**게시자**&#x200B;인 경우 기본 보고서 유형은 **[!UICONTROL 캠페인 요약]**&#x200B;이며 지금은 변경할 수 없습니다.

* 보고서 유형으로 **[!UICONTROL 속성]**&#x200B;을(를) 선택하는 경우 **[!UICONTROL 속성]** 섹션의 필수 필드를 입력해야 합니다. 설정 지침은 [속성 보고서 세부 정보](#report-details-attribution) 섹션을 참조하십시오.
* 이전에 보고서를 만들 때 속성 설정을 구성한 경우 전환 확인 기간(일 단위)을 편집하고 보고할 전환 이벤트를 선택하도록 선택할 수 있습니다.

**[!UICONTROL 전환 확인 기간을 일 단위로 업데이트하려면]** 숫자 값을 입력하거나 증가/감소 옵션으로 조정하십시오. 그런 다음 보고할 전환 이벤트를 선택합니다. 사용 가능한 목록에서 최대 **3**&#x200B;개의 전환을 선택할 수 있습니다.

![업데이트된 전환 이벤트를 강조 표시하는 측정 보고서 편집 대화 상자입니다.](/help/assets/collaborate/measure/edit-conversion-events.png)

완료되면 업데이트를 검토하고 **[!UICONTROL 편집]**&#x200B;을 선택하여 변경 내용을 적용합니다.

![[편집] 옵션이 강조 표시된 측정 보고서 편집 대화 상자입니다.](/help/assets/collaborate/measure/edit-report-confirm.png)

확인 대화 상자에서 보고서가 저장되었음을 확인합니다.

## 측정 보고서 삭제 {#delete-measurement-report}

Collaboration에서 측정 보고서를 삭제하면 시스템에서 측정 보고서가 영구적으로 제거됩니다. 이 작업은 실행 취소할 수 없습니다. 이렇게 하려면 **[!UICONTROL 측정값]** 탭에서 삭제할 보고서를 선택하십시오.

측정 보고서 작업 영역에서 삭제 아이콘(![삭제 아이콘](/help/assets/common/delete.svg))을 선택합니다.

![삭제 아이콘이 강조 표시된 측정 보고서 작업 영역입니다.](/help/assets/collaborate/measure/delete-report.png)

**[!UICONTROL 보고서 삭제]** 대화 상자가 나타나고 삭제를 확인하는 메시지가 표시됩니다. **[!UICONTROL 삭제]**&#x200B;를 선택합니다.

![삭제 옵션이 강조 표시된 보고서 삭제 대화 상자입니다.](/help/assets/collaborate/measure/delete-report-confirm.png)

보고서가 성공적으로 삭제되었음을 확인하는 대화 상자가 표시됩니다.
