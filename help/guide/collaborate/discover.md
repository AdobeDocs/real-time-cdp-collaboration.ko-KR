---
title: 중복 검색 및 대상 비교
description: 와 공동 작업자의 대상 간에 겹치는 부분을 살펴봅니다. 캠페인에 사용할 최상의 대상을 찾는 방법을 알아봅니다.
audience: admin, publisher, advertiser
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 38c42ad3-9d01-4d09-b80e-37fb51cbf42b
source-git-commit: dd1386f9371cb40285315d11e07b139d3115e147
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 24%

---

# 중복 검색 및 대상 비교

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>**[!UICONTROL Discover]** 작업 영역은 연결 프로세스 동안 **대상 검색** 사용 사례가 [활성화되었을 경우에만 사용할 수 있습니다](../connect/establishing-connections.md#connection-settings). 사용 사례에 대한 자세한 내용은 [프로젝트 관리](./manage-projects.md#project-use-cases) 안내서를 참조하세요.

이제 광고주와 게시자 간의 공동 작업 공간에서 [프로젝트를 만들고](/help/guide/collaborate/manage-projects.md) 나면 대상을 공동 작업자의 대상과 비교할 수 있습니다. 이렇게 하면 대상 간의 중복을 검색하고 일치 키 또는 ID별로 분류된 통찰력을 얻을 수 있습니다. 이렇게 하면 광고주가 활성화를 위해 게시자와 공유할 대상을 결정하는 데 도움이 됩니다.

>[!IMPORTANT]
>
>업데이트되지 않았거나 새로 고침되지 않은 [데이터 스케치](/help/guide/glossary.md#sketches)는 7일 후에 삭제됩니다. 이런 경우 이 페이지의 여러 겹치기 보고서에 표시된 수치가 0으로 변경되고 만료된 이러한 대상자는 대상 공유를 사용할 수 없게 됩니다. [활성 새로 고침 일정](/help/guide/setup/onboard-audiences.md#schedule)을 사용하는 대상에 대해 데이터 스케치가 자동으로 새로 고쳐집니다.

![중복 검색](/help/assets/collaborate/discover-overlaps/discover-overlaps.png)

대상을 검색하고 비교하는 데 사용되는 일치 키는 [게시자와 연결](/help/guide/connect/establishing-connections.md#connection-settings)할 때 설정됩니다. 캠페인 실행 준비 시 표시된 오버랩 비율을 변경하려면 일치 키를 제거할 수 있지만, 이 시점에서 새 일치 키를 추가할 수는 없습니다. 이렇게 하려면 공동 작업자 간의 [연결 설정](/help/guide/connect/establishing-connections.md#connection-settings)(으)로 이동하십시오.

![일치 키 편집 화면](/help/assets/collaborate/discover-overlaps/edit-match-keys.png)

## 전제 조건 {#prerequisites}

**[!UICONTROL 공동 작업]** 워크플로의 **[!UICONTROL 검색]** 탭에서 기능을 완전히 활용하려면 이미 다음을 수행했습니다.

* [가져온 대상자](/help/guide/setup/onboard-audiences.md)
* **대상 검색** 사용 사례가 활성화된 원하는 광고주 또는 게시자와 [연결됨](/help/guide/connect/establishing-connections.md)
* [사용자와 공동 작업자 간에 프로젝트를 만들었습니다](/help/guide/collaborate/manage-projects.md)

위에 언급된 전제 조건이 충족되면 공동 작업자의 대상자와 대상 간의 겹침 탐색 및 비교를 시작할 수 있습니다.

## 대상 비교 {#compare-audiences}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_compare_audiences"
>title="대상 비교"
>abstract="본인과 공동 작업자의 대상자 간에 중복되는 대상자를 찾습니다. 드롭다운 선택기에서 설정을 조정하여 본인의 대상자 중 하나 이상과 공동 작업자의 대상자 중 하나 이상 간에 중복되는 대상자를 확인할 수 있습니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_your_identity_count"
>title="ID의 중요성"
>abstract="선택한 대상자에 속하며 선택한 ID가 있는 프로필의 수"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_collaborator_identity_count"
>title="공동 작업자 ID 수"
>abstract="공동 작업자가 선택한 대상자에 속하며 선택한 ID가 있는 프로필의 수"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlapping_identities_count"
>title="ID 중복 수"
>abstract="본인과 공동 작업자의 대상자 모두에 존재하며 선택된 해당 ID가 있는 프로필의 수"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlapping_identities_percentage"
>title="중복되는 ID 비율"
>abstract="본인과 공동 작업자가 선택한 대상자 간에 중복되는 프로필의 비율입니다."

대상 비교 카드를 사용하여 와 공동 작업자의 대상 간 겹침에 대한 다양한 정보를 얻을 수 있습니다. 다음 대상 조합 중 하나를 비교하도록 선택할 수 있습니다.

* 대상 중 하나와 공동 작업자의 대상 중 하나
* 모든 공동 작업자의 대상에 대해 대상 중 하나
* 공동 작업자의 대상 중 하나에 대한 모든 대상
* 모든 대상 대 모든 공동 작업자 대상

표시되는 정보는 다음과 같습니다.

| 지표 | 설명 |
|---------|----------|
| **[!UICONTROL ID 개수]**(본인) | 선택한 대상자에 속하는 선택한 ID를 가진 프로필의 수입니다. |
| **[!UICONTROL ID 개수]**(공동 작업자) | 공동 작업자가 선택한 대상에 속하는 선택된 ID를 가진 프로필의 수입니다. |
| **[!UICONTROL 중복 ID]** | 및 공동 작업자 대상에 모두 있는 선택된 ID를 가진 프로필의 수입니다. |
| **[!UICONTROL 겹치기 비율]** | 본인과 공동 작업자가 선택한 대상자 간에 중복되는 프로필의 비율입니다. |
| **[!UICONTROL 일치 키별 ID 분류]** | 귀하와 공동 작업자가 프로젝트에 대해 합의한 일치 키를 기반으로 개별 일치 키별 중복 계산에서 ID의 구성을 봅니다. |

{style="table-layout:auto"}

>[!TIP]
>
>겹치기 비율 수치가 모든 대상에 항상 제공되지는 않을 수 있습니다. 겹치기 비율 표시기의 표시 여부는 공동 작업자가 [메타데이터 표시 섹션](/help/guide/setup/onboard-audiences.md#metadata-visibility)에서 대상에 대해 선택한 설정에 따라 다릅니다.

## 관련 대상자 {#relevant-audiences}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_relevant_audiences"
>title="관련 대상자"
>abstract="중복 비율을 기준으로 할 때, 이러한 게시자 대상자는 캠페인에 적합할 수 있습니다. <br><br><b>ID 수</b>는 게시자 대상자의 크기입니다. <br><br> <b>중복 ID</b>는 권장 게시자 대상자 및 모든 광고주 대상자 간의 중복을 나타냅니다. <br><br> <b>중복 비율</b>은 중복되는 ID의 수를 <i>모든</i> 광고주 대상자 크기로 나눈 값을 나타냅니다."

**[!UICONTROL Discover]** 모듈의 **[!UICONTROL 관련 대상]** 보기는 겹침 비율에 따라 상위 5개 대상의 선별된 목록을 제공합니다. 이 기능을 사용하면 현재 데이터와 가장 많이 겹치는 대상을 신속하게 식별할 수 있으므로 캠페인을 보다 효과적으로 타기팅할 수 있습니다.

* **[!UICONTROL ID 개수]**&#x200B;는 게시자의 대상 크기입니다.
* **[!UICONTROL ID가 겹침]**&#x200B;은(는) 권장 게시자 대상과 모든 광고주 대상자 간의 겹침을 나타냅니다.
* **[!UICONTROL 겹치기 %]**&#x200B;은(는) 겹치는 ID 수를 *모두* 광고주 대상 크기로 나눈 값을 나타냅니다.

![관련 대상 보기](/help/assets/collaborate/discover-overlaps/relevant-audiences-highlighted.png)

## 중복 항목 탐색 {#discover-overlaps}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlaps_collaborator_audiences"
>title="개별 대상자와의 중복 항목 확인"
>abstract="이 대상자의 모집단과 해당 모집단 및 공동 작업자의 ID 간 중복 항목에 대한 인사이트를 제공합니다."

![다른 대상 보기와 겹침 발견](/help/assets/collaborate/discover-overlaps/discover-overlaps-cards-view.png)

공동 작업자의 대상에 대한 광범위한 정보를 확인하고 이러한 대상을 모든 대상의 전체 모집단 수 또는 특정 대상의 모집단과 비교하는 중복 정보를 봅니다.

>[!TIP]
>
>스크린샷에 표시된 숫자 중 일부를 모든 대상자가 항상 사용할 수 있는 것은 아닙니다. 가시성은 공동 작업자가 [메타데이터 가시성 섹션](/help/guide/setup/onboard-audiences.md#metadata-visibility)의 대상에 대해 선택한 설정에 따라 다릅니다.

## 다음 단계

원하는 대상을 탐색하고 찾은 후에는 게시자와 캠페인에 사용해야 하는 대상을 [공유](/help/guide/collaborate/share.md)할 차례입니다.
