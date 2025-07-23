---
title: 중복 검색 및 대상 비교
description: 와 공동 작업자의 대상 간에 겹치는 부분을 살펴봅니다. 캠페인에 사용할 최상의 대상을 찾는 방법을 알아봅니다.
audience: admin, publisher, advertiser
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/kr/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 38c42ad3-9d01-4d09-b80e-37fb51cbf42b
source-git-commit: eed99cfafd5ffad5a468741f7258c162454769b7
workflow-type: tm+mt
source-wordcount: '1167'
ht-degree: 15%

---

# 중복 검색 및 대상 비교

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>**[!UICONTROL Discover]** 작업 영역은 연결 프로세스 동안 **대상 검색** 사용 사례가 [활성화되었을 경우에만 사용할 수 있습니다](../connect/establishing-connections.md#connection-settings). 사용 사례에 대한 자세한 내용은 [프로젝트 관리](./manage-projects.md#project-use-cases) 안내서를 참조하세요.

[프로젝트를 만들고](/help/guide/collaborate/manage-projects.md) 나면 대상을 공동 작업자와 비교할 수 있습니다. 이렇게 하면 캠페인에 대한 관련 대상을 식별하고 활성화를 위해 게시자에게 전송할 대상을 결정하는 데 도움이 됩니다.

>[!IMPORTANT]
>
>업데이트되지 않았거나 새로 고침되지 않은 [데이터 스케치](/help/guide/glossary.md#sketches)는 7일 후에 삭제됩니다. 이런 경우 이 페이지의 여러 겹치기 보고서에 표시된 수치가 0으로 변경되고 만료된 이러한 대상자는 대상 공유를 사용할 수 없게 됩니다. [활성 새로 고침 일정](/help/guide/setup/onboard-audiences.md#schedule)을 사용하는 대상에 대해 데이터 스케치가 자동으로 새로 고쳐집니다.

대상을 검색하고 비교하는 데 사용되는 일치 키가 연결 프로세스[에서 ](/help/guide/connect/establishing-connections.md#connection-settings)설정됩니다. 일치 키는 대상자 간의 겹침을 계산하는 데 사용되며 켜거나 끌 수 있습니다. 일치 키를 편집하려면 **[!UICONTROL 일치 키 편집]** 옵션을 선택하십시오.

![대상 인사이트를 보여주는 Dicover 탭 작업 영역입니다.](/help/assets/collaborate/discover/discover-overview.png)

사용하지 않을 일치 키를 해제할 수 있는 **[!UICONTROL 일치 키 편집]** 대화 상자가 열립니다. 변경 내용을 저장하려면 **[!UICONTROL 저장]**&#x200B;을 선택하세요.

![검색 작업 영역의 일치 키 편집 대화 상자](/help/assets/collaborate/discover/edit-match-keys.png)

## 전제 조건 {#prerequisites}

프로젝트 내에서 **[!UICONTROL 검색]** 탭을 사용하려면 다음 작업을 수행해야 합니다.

* 계정에 대한 [소스 대상](/help/guide/setup/onboard-audiences.md)
* [대상 검색](/help/guide/connect/establishing-connections.md) 사용 사례가 활성화된 공동 작업자가 있는 **연결됨**
* [사용자와 공동 작업자 간에 프로젝트를 만들었습니다](/help/guide/collaborate/manage-projects.md)

이러한 사전 요구 사항이 충족되면 공동 작업자의 대상자를 통해 중복을 조사하고 비교할 수 있습니다.

## 대상자 비교 {#compare-audiences}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_compare_audiences"
>title="대상자 비교"
>abstract="본인과 공동 작업자의 대상자 간에 중복되는 대상자를 찾습니다. 드롭다운 선택기에서 설정을 조정하여 본인의 대상자 중 하나 이상과 공동 작업자의 대상자 중 하나 이상 간에 중복되는 대상자를 확인할 수 있습니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_your_identity_count"
>title="ID의 중요성"
>abstract="프로젝트에 대해 귀하와 공동 작업자가 합의한 일치 키를 기반으로 하는 선택한 대상자 내의 고유 ID 수입니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_collaborator_identity_count"
>title="공동 작업자 ID 수"
>abstract="프로젝트에 대해 귀하와 공동 작업자가 합의한 일치 키를 기반으로 하는 공동 작업자의 대상자 내 고유 ID 수입니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlapping_identities_count"
>title="ID 중복 수"
>abstract="프로젝트에 대해 귀하와 공동 작업자가 합의한 일치 키를 기반으로 하는 귀하와 공동 작업자의 대상자 모두에 존재하는 고유 ID 수입니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlapping_identities_percentage"
>title="중복되는 ID 비율"
>abstract="본인과 공동 작업자가 선택한 대상자 간에 중복되는 ID의 비율입니다."

대상 비교 섹션을 사용하여 와 공동 작업자 대상 간의 겹침에 대한 다양한 정보를 얻을 수 있습니다. 대상 선택을 변경하려면 **[!UICONTROL 대상 비교]** 섹션 맨 위에 있는 드롭다운 선택기를 사용하십시오. 한 명 또는 모든 대상과 한 명 또는 모든 공동 작업자 대상을 선택하여 서로 비교할 수 있습니다.

![대상 비교 섹션에서 대상 선택기가 강조 표시된 검색 작업 영역입니다.](/help/assets/collaborate/discover/compare-audiences-selector.png)

대상 비교 섹션에서 사용자와 공동 작업자가 프로젝트에 대해 동의한 일치 키를 기반으로 하는 다음 지표를 볼 수 있습니다.

| 지표 | 설명 |
|---------|----------|
| **[!UICONTROL ID 개수]**(본인) | 선택한 대상자 내의 고유 ID 수입니다. |
| **[!UICONTROL ID 개수]**(공동 작업자) | 공동 작업자 대상 내의 고유 ID 수입니다. |
| **[!UICONTROL 중복 ID]** | 와 공동 작업자의 대상 모두에 있는 고유 ID 수입니다. |
| **[!UICONTROL 겹치기 %]** | 본인과 공동 작업자가 선택한 대상자 간에 중복되는 프로필의 비율입니다. |
| **[!UICONTROL 일치 키별 ID 분류]** | 각 공동 작업자에 대해 선택된 대상을 기반으로 프로젝트에서 선택한 각 일치 키에 대한 ID 분류. |

{style="table-layout:auto"}

>[!NOTE]
>
>겹치기 비율 수치가 모든 대상에 항상 제공되지는 않을 수 있습니다. 겹치기 비율 표시기의 표시 여부는 공동 작업자가 [메타데이터 표시 섹션](/help/guide/setup/onboard-audiences.md#metadata-visibility)에서 대상에 대해 선택한 설정에 따라 다릅니다.

## 관련 대상자 {#relevant-audiences}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_relevant_audiences"
>title="관련 대상자"
>abstract="오버랩 비율에 따라 이러한 대상은 캠페인에 적합할 수 있습니다. <br><br> <b>ID 개수</b>는 공동 작업자의 대상 크기입니다. <br><br> <b>ID가 겹침</b>은(는) 권장 대상자와 모든 대상자 간의 겹침을 나타냅니다. <br><br> <b>겹치기 %</b>은(는) 겹치는 ID의 수를 대상 <i>모두</i>의 크기로 나눈 값을 나타냅니다."

**[!UICONTROL 검색]** 탭의 **[!UICONTROL 관련 대상]** 섹션은 공동 작업자의 대상과 모든 대상자 간의 겹침 비율을 기반으로 상위 5명의 대상자에 대해 선별된 목록을 제공합니다. 이 기능을 사용하면 겹치는 정도가 가장 높은 대상을 신속하게 식별할 수 있으므로 캠페인을 보다 효과적으로 타기팅할 수 있습니다. 섹션의 오른쪽 상단에 있는 페이지 선택기를 사용하여 관련 대상 간에 전환합니다.

![관련 대상 섹션이 강조 표시된 검색 작업 영역입니다.](/help/assets/collaborate/discover/relevant-audiences.png)

>[!NOTE]
>
>공동 작업자 대상의 가시성은 공동 작업자가 [메타데이터 가시성 섹션](/help/guide/setup/onboard-audiences.md#metadata-visibility)에서 대상에 대해 선택한 설정에 따라 다릅니다. 공동 작업자가 모든 대상을 비공개로 설정한 경우 이 섹션에는 대상이 표시되지 않습니다.

**[!UICONTROL 관련 대상]** 섹션에는 각 권장 대상에 대한 다음 정보가 표시됩니다.

| 지표 | 설명 |
|---------|----------|
| **[!UICONTROL ID 개수]** | 대상 내의 이름 고유 ID. |
| **[!UICONTROL 중복 ID]** | 권장 대상과 모든 대상자 간에 겹치는 고유 ID의 수입니다. |
| **[!UICONTROL 겹치기 %]** | 권장 대상과 모든 대상자 간의 ID가 겹치는 비율입니다. |
| **[!UICONTROL 대상 범주]** | 공동 작업자가 대상자에게 할당한 카테고리입니다. |
| **[!UICONTROL 키 일치]** | 공동 작업자가 대상에 대해 선택한 일치 키입니다. |

{style="table-layout:auto"}

## 중복 항목 탐색 {#discover-overlaps}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlaps_collaborator_audiences"
>title="개별 대상자와의 중복 항목 확인"
>abstract="본인과 공동 작업자의 대상자 간에 중복되는 대상자에 대한 인사이트를 얻을 수 있습니다."

중복을 발견하여 대상이 공동 작업자의 대상과 어떻게 비교되는지에 대한 통찰력을 얻으십시오. 기본적으로 이 섹션에서는 모든 대상을 각 공동 작업자의 대상과 비교합니다. 섹션 하단에 있는 페이지 매김 컨트롤을 사용하여 사용 가능한 대상을 탐색합니다.

![검색 겹침 섹션이 강조 표시된 검색 작업 영역입니다.](/help/assets/collaborate/discover/discover-overlaps.png)

>[!NOTE]
>
>공동 작업자 대상의 가시성은 공동 작업자가 [메타데이터 가시성 섹션](/help/guide/setup/onboard-audiences.md#metadata-visibility)에서 대상에 대해 선택한 설정에 따라 다릅니다. 공동 작업자가 모든 대상을 비공개로 설정한 경우 이 섹션에는 대상이 표시되지 않습니다.

대상자 선택을 변경하려면 **[!UICONTROL 대상자 변경]**&#x200B;을 선택하세요.

![대상자 변경 옵션이 강조 표시된 검색 작업 영역입니다.](/help/assets/collaborate/discover/change-audience.png)

공동 작업자의 대상과 비교할 특정 대상을 선택할 수 있는 **[!UICONTROL 대상 변경]** 대화 상자가 열립니다. 원하는 대상을 선택하거나 선택 내용을 지워 모든 대상을 선택한 다음 **[!UICONTROL 저장]**&#x200B;을 선택합니다.

![검색 작업 영역의 대상자 변경 대화 상자입니다.](/help/assets/collaborate/discover/change-audience-selection.png)

원하는 대상을 선택하면 **[!UICONTROL 중복 검색]** 섹션에 각 대상에 대한 다음 정보가 표시됩니다.

| 지표 | 설명 |
|---------|----------|
| **[!UICONTROL ID 개수]** | 대상 내 고유 ID 수입니다. |
| **[!UICONTROL 중복 ID]** | 권장 대상과 모든 대상자 간에 겹치는 고유 ID의 수입니다. |
| **[!UICONTROL 겹치기 %]** | 권장 대상과 모든 대상자 간의 ID가 겹치는 비율입니다. |
| **[!UICONTROL 대상 범주]** | 공동 작업자가 대상자에게 할당한 카테고리입니다. |
| **[!UICONTROL 키 일치]** | 공동 작업자가 대상에 대해 선택한 일치 키입니다. |

{style="table-layout:auto"}

## 다음 단계

원하는 대상을 탐색하고 찾은 후에는 캠페인에 사용해야 하는 대상을 [활성화](/help/guide/collaborate/activate.md)할 차례입니다.
