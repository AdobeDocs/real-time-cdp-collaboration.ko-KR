---
title: 성능 측정
description: 다양한 채널에서 캠페인의 성과를 측정합니다. 다양한 보고서를 사용하고 해석하는 방법을 알아봅니다.
audience: admin, publisher, advertiser
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: c92b263e-1f96-49f1-841a-ef2e97a4cb9a
source-git-commit: e06ee94afdd1edbf86430cbe348dc448419b8f4e
workflow-type: tm+mt
source-wordcount: '2612'
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

이 테이블을 검토하여 원하는 작업을 수행할 때 캠페인의 효과를 평가하십시오.

![누적 전환입니다.](/help/assets/collaborate/measure/cumulative-conversions.png)

### 일별 전환 {#conversions-by-day}

이 차트는 속성 보고서를 만들 때 설정되는 각 이벤트에 대한 변환을 일별로 분류합니다. 이 보기를 사용하여 일별 패턴을 파악하고, 높은 전환 또는 낮은 전환 활동 기간을 식별하고, 캠페인 타임라인에서 다양한 전환 이벤트가 수행되는 방식을 비교할 수 있습니다.

일별 ![전환](/help/assets/collaborate/measure/conversions-by-day.gif)

## 측정 보고서 생성 {#create-measurement-report}

Collaboration에서 두 가지 주요 측정 보고서 유형을 만들 수 있습니다.

* **캠페인 요약**: 도달, 노출 횟수, 평균 빈도, 채널별 게재와 같은 높은 수준의 지표를 제공하여 전반적인 캠페인 성능에 대한 간략한 개요를 제공합니다.
* **속성**: 캠페인 노출이 전환 또는 구매와 같은 다운스트림 작업을 유도하여 캠페인 효과를 파악하는 데 도움이 되는 방법을 측정합니다.

캠페인 요약 보고서를 직접 실행할 수 있지만 속성 보고서에서는 두 보고서 유형을 모두 함께 선택해야 합니다.

### 캠페인 요약 보고서 만들기 {#create-campaign-summary-report}

게시자와 광고주 모두 **캠페인 요약** 보고서를 생성하여 캠페인 성과를 평가할 수 있습니다. 이 보고서를 사용하여 [도달](#cumulative-reach-curve), [빈도](#frequency-distribution), [노출 횟수](#impressions-by-placement)와 같은 주요 지표에 대한 통찰력을 얻고 캠페인이 전달된 방식과 전반적인 영향을 파악합니다.

**캠페인 요약** 보고서를 생성하려면 **[!UICONTROL Collaborator]** 작업 영역에서 프로젝트 작업 영역으로 이동합니다. **[!UICONTROL 측정]** 탭에서 추가 아이콘(![추가 아이콘.](/help/assets/icons/plus.png))을 선택합니다. **[!UICONTROL 측정값]**&#x200B;을(를) 선택합니다.

첫 번째 보고서인 경우 **[!UICONTROL 보고서 실행]** 옵션도 선택할 수 있습니다.

![보고서 실행 옵션과 측정값 옵션을 강조 표시하는 측정값 탭입니다.](/help/assets/collaborate/measure/run-measure-report.png)

**[!UICONTROL 측정 보고서 만들기]** 화면에 **[!UICONTROL 청구 세부 정보]**, **[!UICONTROL 캠페인 세부 정보]** 및 **[!UICONTROL 보고서 세부 정보]** 섹션에 그룹화된 정보 및 입력 필드가 표시됩니다.

#### 과금 세부 정보 {#billing-details}

이 섹션에서는 측정 보고서를 생성할 때 크레딧을 사용하는 방법을 설명합니다. [연결 설정](../connect/establishing-connections.md#credit-split) 중에 신용 책임이 설정됩니다. 보고서를 실행하기 전에 공동 작업자와 신용 분할 설정 및 보고 역할을 검토하고 확인해야 합니다.

#### 캠페인 세부 정보 {#campaign-details}

**[!UICONTROL 캠페인 세부 정보]** 섹션에서 보고서에 연결할 적절한 **광고주 ID**&#x200B;을(를) 선택하십시오. 이러한 광고주 이름 또는 ID는 [연결 설정](../connect/establishing-connections.md#advertiser-names) 중에 추가되었습니다. 이름이 하나만 구성된 경우 기본적으로 표시됩니다. 이름이 설정되지 않은 경우 **[!UICONTROL 광고주 ID(이름)]** 필드가 비활성화되고 광고주 계정 이름으로 미리 채워집니다.

![광고주 ID(이름) 옵션을 표시하는 측정 보고서 만들기 화면이 비활성화되었습니다.](/help/assets/collaborate/measure/advertiser-id.png)

그런 다음 **[!UICONTROL 캠페인 ID]** 드롭다운 메뉴에서 원하는 캠페인을 선택합니다. 이 메뉴에는 게시자가 프로젝트에 대해 입력한 모든 캠페인 ID가 나열됩니다. 필요한 캠페인을 사용할 수 없는 경우 보고서를 생성하기 전에 [UI에 추가](./manage-projects.md#manage-campaign-id)하십시오.

![캠페인 ID 드롭다운 메뉴를 표시하는 측정 보고서 만들기 화면이 확장되었습니다.](/help/assets/collaborate/measure/campaign-id.png)

그런 다음 보고서에서 다룰 기간을 지정합니다. **[!UICONTROL 보고서 날짜 범위]**&#x200B;를 선택한 다음 달력을 사용하여 시작 날짜와 종료 날짜를 선택하십시오.

![보고서 날짜 범위 달력을 보여 주는 측정 보고서 만들기 화면입니다.](/help/assets/collaborate/measure/report-date-range.png)

#### 보고서 세부 정보 {#report-details}

**보고서 실행 날짜**

**[!UICONTROL 보고서 세부 정보]** 섹션에서 보고서를 실행할 날짜를 선택합니다. **[!UICONTROL 보고서 실행 날짜]**&#x200B;를 선택하고 달력에서 원하는 날짜를 선택하십시오.

* 오늘 날짜 또는 과거 날짜를 선택하면 **캠페인 요약** 보고서가 즉시 실행됩니다.
* 미래 날짜를 선택하면 **캠페인 요약** 보고서가 해당 날짜에 실행되도록 예약됩니다.

![보고서 실행 날짜 일정을 표시하는 측정 보고서 만들기 화면입니다.](/help/assets/collaborate/measure/report-run-date.png)

**보고서 유형**

* 광고주라면 사용 가능한 옵션에서 **[!UICONTROL 캠페인 요약]** 보고서 유형을 선택할 수 있습니다. 광고주만 속성 보고서를 생성할 수 있습니다.
* 게시자인 경우 **[!UICONTROL 캠페인 요약]** 보고서 유형이 미리 선택되었으므로 변경할 수 없습니다. 현재 게시자는 속성 보고서를 실행할 수 없습니다.

![캠페인 요약 옵션을 미리 선택된 변경할 수 없는 보고서 유형으로 표시하는 측정 보고서 만들기 화면입니다.](/help/assets/collaborate/measure/cs-report-type.png)

마지막으로 설정을 검토하고 **[!UICONTROL 만들기]**&#x200B;를 선택하세요. 캠페인 요약 보고서는 실행 날짜가 오늘 또는 이전이거나 선택한 미래 날짜인 경우 즉시 생성됩니다. 실행 날짜 이전에 예약된 보고서를 편집할 수 있습니다. 단계별 지침은 [측정 보고서 편집] 섹션을 참조하십시오.

사용 가능한 상태가 되면 프로젝트 작업 영역의 **[!UICONTROL 측정]** 탭에서 언제든지 보고서를 볼 수 있습니다.

![정보 및 [만들기] 옵션이 강조 표시된 측정 보고서 만들기 화면입니다.](/help/assets/collaborate/measure/cs-review.png)

### 속성 보고서 만들기 {#create-attribution-report}

광고주로서 **속성** 보고서를 생성하여 캠페인 노출이 가입 또는 구매와 같은 주요 결과에 어떻게 기여하는지 평가할 수 있습니다. 이러한 보고서를 사용하여 캠페인과의 사용자 상호 작용을 이해하고, 가장 큰 영향을 미치는 접점을 식별하고, 보다 효과적인 마케팅 전략을 알려줍니다.

>[!IMPORTANT]
>
> 속성 보고서를 생성하기 전에 측정 데이터를 [Collaboration에 소스](../setup/onboard-measurement-data.md#add-measurement-data)해야 합니다.
>![측정 데이터에 대한 요구 사항과 사용하지 않는 측정 옵션이 있는 측정 탭입니다.](/help/assets/collaborate/measure/require-measurement-data.png)

**속성** 보고서를 생성하려면 **[!UICONTROL Collaborator]** 작업 영역에서 프로젝트 작업 영역으로 이동합니다. **[!UICONTROL 측정]** 탭에서 추가 아이콘(![추가 아이콘.](/help/assets/icons/plus.png))을 선택합니다. **[!UICONTROL 측정값]**&#x200B;을(를) 선택합니다.

첫 번째 보고서인 경우 **[!UICONTROL 보고서 실행]** 옵션도 선택할 수 있습니다.

![보고서 실행 옵션과 측정값 옵션을 강조 표시하는 측정값 탭입니다.](/help/assets/collaborate/measure/run-measure-report-attribution.png)

**[!UICONTROL 측정 보고서 만들기]** 화면에 **[!UICONTROL 청구 세부 정보]**, **[!UICONTROL 캠페인 세부 정보]** 및 **[!UICONTROL 보고서 세부 정보]** 섹션에 그룹화된 정보 및 입력 필드가 표시됩니다.

[캠페인 요약 보고서 만들기](#create-campaign-summary-report) 섹션의 단계를 읽고 수행하여 다음 설정을 구성하십시오.

* [청구 세부 정보](#billing-details)
* [캠페인 세부 정보](#campaign-details)

#### 속성 보고서에 대한 보고서 세부 사항 {#report-details-attribution}

**보고서 실행 날짜**

>[!IMPORTANT]
>
> 속성 보고서의 경우 보고서 실행 날짜는 미래 날짜여야 하며, 보고서 날짜 범위의 종료 날짜와 정의된 전환 확인 기간의 전체 기간 최소 1일 이후에 발생해야 합니다.
> **보고서 실행 날짜 ≥ 보고서 종료 날짜 + 전환 확인 기간 + 1**
> 
> 예를 들어 보고서 날짜 범위가 6월 15일에 끝나고 전환 확인 기간이 14일인 경우 보고서 실행 날짜는 6월 30일 이후가 됩니다.

**[!UICONTROL 보고서 세부 정보]** 섹션에서 보고서를 실행할 날짜를 선택합니다. **[!UICONTROL 보고서 실행 날짜]**&#x200B;를 선택하고 달력에서 원하는 날짜를 선택하십시오.

**보고서 유형**

광고주는 **[!UICONTROL 캠페인 요약]** 외에 **[!UICONTROL 속성]**&#x200B;을 보고서 유형으로 선택할 수 있습니다. 속성 보고서를 선택하면 결과에 표준 캠페인 요약 지표와 세부 속성 분석이 모두 포함되어 캠페인 성과를 종합적으로 볼 수 있습니다.

![선택한 캠페인 요약 및 속성 보고서 유형을 모두 강조 표시하는 측정 보고서 만들기 화면입니다.](/help/assets/collaborate/measure/attribution-report-type.png)

**[!UICONTROL 속성]**&#x200B;을 보고서 유형으로 선택하면 **[!UICONTROL 속성]** 구성 섹션이 추가 필수 설정과 함께 표시됩니다.

* **전환 확인 기간(일)**: 각 전환 전에 보고서에서 캠페인 노출 횟수를 고려하는 기간을 정의합니다. 이 기간 내의 노출만 기여도 크레딧에 적용됩니다.
* **전환 이벤트**: 측정할 전환 작업(예: 구매 또는 등록)을 지정합니다. 이러한 이벤트는 [측정 데이터를 Collaboration에 소스](../setup/onboard-measurement-data.md#add-conversion-event)할 때 미리 설정해야 합니다.

먼저 **[!UICONTROL 전환 확인 기간(일 수]**) 필드에 값을 입력하거나 증가/감소 옵션으로 조정하십시오.

![전환 확인 기간(일) 값을 강조 표시하는 측정 보고서 만들기 화면입니다.](/help/assets/collaborate/measure/lookback-window-in-days.png)

사용 가능한 목록에서 최대 **3**&#x200B;개의 전환 이벤트를 선택합니다. 특정 이벤트에 대한 자세한 내용을 보려면 **[!UICONTROL i]** 아이콘을 선택하여 세부 정보를 확인하십시오.

![선택한 전환 이벤트와 구매 이벤트의 정보를 강조 표시하는 측정 보고서 만들기 화면입니다.](/help/assets/collaborate/measure/attribution-conversion-events.png)

마지막으로 설정을 검토하고 **[!UICONTROL 만들기]**&#x200B;를 선택하여 보고서를 예약하십시오. 속성 보고서는 지정된 실행 날짜에 생성됩니다. 실행 날짜 이전에 예약된 보고서를 편집할 수 있습니다. 단계별 지침은 [측정 보고서 편집] 섹션을 참조하십시오.

사용 가능한 상태가 되면 프로젝트 작업 영역의 **[!UICONTROL 측정]** 탭에서 언제든지 보고서를 볼 수 있습니다.

![정보 및 [만들기] 옵션이 강조 표시된 측정 보고서 만들기 화면입니다.](/help/assets/collaborate/measure/attribution-review.png)

## 측정 보고서 편집 {#edit-measurement-report}

>[!IMPORTANT]
>
>나중에 실행되도록 예약된 경우에만 측정 보고서의 설정을 편집할 수 있습니다. 이미 실행된 보고서의 경우 설정을 변경할 수 없습니다.

측정 보고서 설정을 업데이트하여 보고서가 특정 기간 내에 캠페인에 대한 올바른 분석을 제공하고 원하는 날짜에 실행되도록 합니다.

시작하려면 업데이트할 측정 보고서의 작업 공간으로 이동합니다. 삭제 아이콘 옆에 있는 편집 아이콘(![편집 아이콘](/help/assets/icons/edit.png))을 선택합니다.

![편집 아이콘이 강조 표시된 측정 보고서 작업 영역입니다.](/help/assets/collaborate/measure/edit-report.png)

>[!TIP]
>
>**[!UICONTROL 측정값]** 탭에서 편집할 보고서 섹션으로 이동합니다. 설정을 업데이트하려면 **[!UICONTROL 전체 보고서 보기]** 옆에 있는 편집 아이콘(![편집 아이콘](/help/assets/icons/edit.png))을 선택하십시오.
>![보고서 섹션 내의 편집 아이콘을 강조 표시하는 측정값 탭입니다.](/help/assets/collaborate/measure/measure-tab-edit-report.png)

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
