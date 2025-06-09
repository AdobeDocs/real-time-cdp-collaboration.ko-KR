---
title: 대상자 활성화
description: Adobe Real-Time CDP Collaboration에서 대상을 활성화하는 방법을 알아봅니다.
audience: admin, publisher
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: fd82fcbf-ab39-48e0-9438-0a9046693431
source-git-commit: f19aff1b7d10a446dd209721e7a6fdf537c9d63e
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 1%

---

# 대상자 활성화

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>**[!UICONTROL 활성화]** 작업 영역은 연결 프로세스 ](../connect/establishing-connections.md#connection-settings)에서 **대상 활성화** 사용 사례를 사용하도록 설정한 경우 [에만 사용할 수 있습니다. 사용 사례에 대한 자세한 내용은 [프로젝트 관리](./manage-projects.md#project-use-cases) 안내서를 참조하세요.

대상자 활성화를 사용하면 캠페인에서 대상자를 활성화할 수 있습니다. 활동 프로세스는 광고주와 게시자 간의 협업입니다. [캠페인에 가장 적합한 대상을 발견](./discover.md)한 후 대상자는 타겟팅된 대상을 활성화할 수 있습니다. 활성화된 대상은 캠페인에 사용할 수 있도록 게시자의 사전 구성된 대상(예: Adobe Experience Platform)으로 전송됩니다. 지정 설정에 대한 자세한 내용은 [대상 개요](../destinations/overview.md) 안내서를 참조하세요.

>[!IMPORTANT]
>
>현재 광고주가 대상을 활성화하면 해당 조직에 대해 구성된 게시자가 대상으로 자동으로 활성화됩니다. 게시자 **must**&#x200B;이(가) 대상을 구성하고 *before* 광고주가 대상을 활성화합니다. 구성된 대상이 없으면 대상자가 게시자에게 전송되지만 캠페인에서 활성화할 수 없습니다.

## 새 대상 활성화

대상자 활성화를 시작하려면 프로젝트 작업 영역에서 **[!UICONTROL 활성화]** 탭으로 이동합니다.

추가 아이콘(![추가 아이콘)을 선택합니다.](/help/assets/icons/plus.png)) 또는 활성화를 위해 전송된 이전 대상이 없는 경우 **[!UICONTROL 대상 활성화]** 옵션을 사용할 수 있습니다.

![추가된 대상이 없는 프로젝트의 작업 영역을 활성화하십시오.](/help/assets/collaborate/activate/activate-new-audiences.png)

대상자 활성화 워크플로우가 열리고, 공동 작업자에게 보낼 대상자를 선택할 수 있습니다. 드롭다운을 사용하여 대상자를 선택하거나 특정 대상자를 검색합니다. 선택하기 전에 대상자에 대한 자세한 정보를 보려면 **[!UICONTROL 대상자 찾아보기]**&#x200B;를 선택하십시오.

![드롭다운 및 대상자 찾아보기 옵션이 강조 표시된 대상자 활성화 워크플로우입니다.](/help/assets/collaborate/activate/audience-activation.png)

**[!UICONTROL 대상자 찾아보기]**&#x200B;에서 각 대상자에 대해 **[!UICONTROL ID 개수]**, **[!UICONTROL 중복 ID]** 및 **[!UICONTROL 중복 %]**&#x200B;을(를) 볼 수 있습니다.

![사용 가능한 대상을 표시하는 대상 찾아보기 대화 상자입니다.](/help/assets/collaborate/activate/browse-audiences.png)

캠페인에서 활성화할 대상을 선택한 다음 **[!UICONTROL 저장]**&#x200B;을 선택합니다. 이제 대상이 표시되고, 선택한 대상의 **[!UICONTROL ID 개수]**, **[!UICONTROL 중복 ID]** 및 **[!UICONTROL 중복 %]**&#x200B;을(를) 볼 수 있습니다.

![선택한 대상이 표시된 대상자 활성화 워크플로우입니다.](/help/assets/collaborate/activate/audience-selected.png)

### 일치 키 편집

그런 다음 선택한 대상 내에서 **[!UICONTROL 일치 키 편집]**&#x200B;을 선택하여 대상의 일치 키를 편집할 수 있습니다. 이러한 옵션은 공동 작업자 간의 연결이 처음 설정되었을 때 일치하는 키 선택에서 상속됩니다. 특정 캠페인에 적용되지 않는 경우 선택한 일치 키를 제거할 수 있지만 새 일치 키를 추가할 수는 없습니다.

![일치 키 편집 옵션이 강조 표시된 대상자 활성화 워크플로우입니다.](/help/assets/collaborate/activate/edit-match-keys.png)

사용하지 않을 일치 키를 해제할 수 있는 **[!UICONTROL 일치 키 편집]** 대화 상자가 열립니다. 변경 내용을 저장하려면 **[!UICONTROL 저장]**&#x200B;을 선택하세요.

>[!NOTE]
>
>일치 키를 하나 이상 선택해야 합니다. 현재 릴리스에서는 사용 가능한 일치 키만 **[!UICONTROL 해시된 이메일]**&#x200B;이므로 이 일치 키를 제거할 수 없습니다.

![Audience 활성화 워크플로의 일치 키 편집 대화 상자입니다.](/help/assets/collaborate/activate/edit-match-keys-selection.png)

### 대상 새로 고침 빈도 및 간격 설정

마지막으로 새로 고침할 대상에 대해 원하는 빈도 및 날짜 범위를 설정합니다. 현재 릴리스에서 지원되는 빈도 옵션은 **[!UICONTROL 한 번]**&#x200B;뿐입니다. **[!UICONTROL Once]** 빈도는 대상이 한 번 활성화되고 새로 고쳐지지 않음을 의미합니다. **[!UICONTROL 날짜]** 옵션이 현재 날짜로 자동 채워집니다.

![빈도 섹션이 강조 표시된 대상자 활성화 워크플로우입니다.](/help/assets/collaborate/activate/audience-frequency.png)

선택 항목이 만족스러우면 **[!UICONTROL 활성화]**&#x200B;를 선택하여 워크플로우를 완료합니다. 이제 대상이 활성화되었으며 **[!UICONTROL 활성화]** 탭에서 볼 수 있습니다. 공동 작업자가 **[!UICONTROL 활성화]** 탭에서 캠페인에서 사용할 수도 있습니다.

대상자의 이름 편집 아이콘(![연필 아이콘)을 편집할 수 있습니다.](/help/assets/icons/edit.png)) 또는 **[!UICONTROL 비활성화]**&#x200B;를 선택하여 대상자를 비활성화합니다.

![활성화된 대상이 표시되고 편집 및 비활성화 옵션이 강조 표시된 활성화 탭입니다.](/help/assets/collaborate/activate/edit-activate-audience.png)

## 활성화된 대상자 보기

**[!UICONTROL 활성화]** 탭에서 게시자와 광고주 모두 현재 활성화된 대상자를 볼 수 있습니다. 현재 대상자는 광고주가 활성화한 후 게시자가 구성한 대상으로 자동으로 전송됩니다.

![활성화 탭에 대한 개요로서 활성화된 대상을 표시합니다.](/help/assets/collaborate/activate/activate-overview.png)

활성화된 각 대상자 내에서 다음 지표를 볼 수 있습니다.

| 지표 | 설명 |
|---------|----------|
| **[!UICONTROL 활성화된 ID]** | 대상자 내에서 활성화된 ID의 수를 나타냅니다. |
| **[!UICONTROL 중복 ID]** | 이 대상자와 공동 작업자 인벤토리에서 프로필의 총 인구 간에 겹치는 ID 수를 나타냅니다. |
| **[!UICONTROL 키 분류 일치]** | 대상에 사용된 각 ID의 ID 수를 표시합니다. 예를 들어 총 50만 명의 사용자 ID는 해시된 이메일 ID를 키로 사용하는 사용자 40만 명과 모바일 ID를 키로 사용하는 사용자 10만 명으로 구성될 수 있습니다. 여기에 설명된 예에서 동일한 사람은 이메일 및 모바일 ID와 함께 대상에 두 번 표시될 수 있습니다. |

## 다음 단계 {#next-steps}

데이터를 활성화하고 캠페인을 실행한 후 Adobe 지원 및 엔지니어링 팀과 협력하여 측정 데이터를 업로드하고 해당 [측정 보고서](/help/guide/collaborate/measure.md)를 보십시오.
