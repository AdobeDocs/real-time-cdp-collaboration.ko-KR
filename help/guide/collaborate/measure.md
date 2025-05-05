---
title: 성능 측정
description: 다양한 채널에서 캠페인의 성과를 측정합니다. 다양한 보고서를 사용하고 해석하는 방법을 알아봅니다.
audience: admin, publisher, advertiser
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: c92b263e-1f96-49f1-841a-ef2e97a4cb9a
source-git-commit: acaaaa1e1fab981d874210639c16e76e48fc3394
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 13%

---

# 성능 측정

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>**[!UICONTROL Measure]** 작업 영역은 연결 프로세스 [&#128279;](../connect/establishing-connections.md#connection-settings) 동안 **Campaign 측정** 사용 사례를 사용하도록 설정한 경우에만 사용할 수 있습니다.  사용 사례에 대한 자세한 내용은 [프로젝트 관리](./manage-projects.md#project-use-cases) 안내서를 참조하세요.

Real-Time CDP Collaboration의 사용 가능한 보고서에 대해 알아보고 다양한 채널에서 마케팅 캠페인의 성과를 측정하고 분석하는 방법을 이해합니다.

## 전제 조건

Real-Time CDP Collaboration에서 측정 보고서에 액세스하려면 먼저 다음을 수행해야 합니다.

* **캠페인 측정** 사용 사례가 활성화된 원하는 광고주 또는 게시자와 [연결됨](/help/guide/connect/establishing-connections.md) 및 [프로젝트](/help/guide/collaborate/manage-projects.md)에 대한 공동 작업을 시작했습니다.
* 캠페인을 실행하고 [업로드된 측정 데이터](/help/guide/setup/onboard-measurement-data.md)를 Real-Time CDP Collaboration으로 보내십시오.

## 보고서 보기

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

## 다음 단계

![광고주를 검색, 활성화, 측정합니다.](/help/assets/end-to-end-workflow/discover-activate-measure.png)

위의 이미지에서 순환성 측면에서 다음 캠페인을 계획할 때 보고서를 보고 얻은 통찰력을 사용하십시오. 광고주는 필요한 경우 뒤로 돌아가서 다른 게시자를 찾고 를 실행하여 다음 캠페인에 대해 다른 대상자를 검색합니다.
