---
title: 대상자 활성화
description: Adobe Real-Time CDP Collaboration에서 대상을 활성화하는 방법을 알아봅니다.
audience: admin, publisher
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/kr/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: fd82fcbf-ab39-48e0-9438-0a9046693431
source-git-commit: afe8560a12017c6b993f93cde8636288aa6e4991
workflow-type: tm+mt
source-wordcount: '1003'
ht-degree: 2%

---

# 대상자 활성화

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>**[!UICONTROL 활성화]** 작업 영역은 연결 프로세스 **에서**&#x200B;대상 활성화[&#x200B; 사용 사례를 사용하도록 설정한 경우 &#x200B;](../connect/establishing-connections.md#connection-settings)에만 사용할 수 있습니다. 사용 사례에 대한 자세한 내용은 [프로젝트 관리](./manage-projects.md#project-use-cases) 안내서를 참조하세요.

대상자 활성화를 사용하면 캠페인에서 사용할 대상자를 활성화할 수 있습니다. 연결에 구성된 대상 활성화 설정 [에 따라 공동 작업자가 활성화할 수 있습니다](/help/guide/connect/establishing-connections.md#configure-connection-settings). [캠페인에 가장 적합한 대상을 검색](./discover.md)한 후 대상을 활성화하여 사용할 수 있도록 만드십시오. 대상을 활성화하면 공동 작업자가 미리 구성한 대상(예: Adobe Experience Platform)으로 보내져 캠페인에서 사용할 수 있게 됩니다. 대상 설정에 대한 자세한 내용은 [대상 개요](../destinations/overview.md) 안내서를 참조하십시오.

## 새 대상 활성화 {#activate-new-audiences}

대상자 활성화를 시작하려면 프로젝트 작업 영역에서 **[!UICONTROL 활성화]** 탭으로 이동합니다.

>[!IMPORTANT]
>
>**대상자를 활성화하기 전에** 공동 작업자 **대상 구성**. 대상자를 활성화하면 자동으로 공동 작업자가 구성한 대상으로 전송됩니다. 설정된 대상이 없으면 대상을 활성화할 수 없습니다.
>
>![Collaborator에 구성된 대상이 없는 경우 작업 영역 활성화.](/help/assets/collaborate/activate/no-destination-configured.png)

추가 아이콘(![추가 아이콘)을 선택합니다.](/help/assets/icons/plus.png)) 또는 활성화를 위해 전송된 이전 대상이 없는 경우 **[!UICONTROL 대상 활성화]** 옵션을 사용할 수 있습니다.

![추가된 대상이 없는 프로젝트의 작업 영역을 활성화하십시오.](/help/assets/collaborate/activate/activate-new-audiences.png)

대상자 활성화 워크플로우가 열리고, 공동 작업자에게 보낼 대상자를 선택할 수 있습니다. 드롭다운을 사용하여 대상자를 선택하거나 특정 대상자를 검색합니다. 선택하기 전에 대상자에 대한 자세한 정보를 보려면 **[!UICONTROL 대상자 찾아보기]**&#x200B;를 선택하십시오.

![드롭다운 및 대상자 찾아보기 옵션이 강조 표시된 대상자 활성화 워크플로우입니다.](/help/assets/collaborate/activate/audience-activation.png)

**[!UICONTROL 대상자 찾아보기]**&#x200B;에서 각 대상자에 대해 **[!UICONTROL ID 개수]**, **[!UICONTROL 중복 ID]** 및 **[!UICONTROL 중복 %]**&#x200B;을(를) 볼 수 있습니다.

![사용 가능한 대상을 표시하는 대상 찾아보기 대화 상자입니다.](/help/assets/collaborate/activate/browse-audiences.png)

>[!IMPORTANT]
>
>여러 일치 키가 사용되는 대상을 활성화할 때 하나(또는 그 이상) 일치 키에 겹침이 없거나 대상 수가 없거나 임계값 미만이면 전체 활성화가 실패합니다. 활성화하기 전에 대상이 충분히 겹치고 모든 일치 키에서 최소 1000 ID 임계값을 충족하는지 확인하십시오.

캠페인에서 활성화할 대상을 선택한 다음 **[!UICONTROL 저장]**&#x200B;을 선택합니다. 이제 대상이 표시되고, 선택한 대상의 **[!UICONTROL ID 개수]**, **[!UICONTROL 중복 ID]** 및 **[!UICONTROL 중복 %]**&#x200B;을(를) 볼 수 있습니다.

![선택한 대상이 표시된 대상자 활성화 워크플로우입니다.](/help/assets/collaborate/activate/audience-selected.png)

### 일치 키 편집 {#edit-match-keys}

그런 다음 선택한 대상 내에서 **[!UICONTROL 일치 키 편집]**&#x200B;을 선택하여 대상의 일치 키를 편집할 수 있습니다. 이러한 옵션은 공동 작업자 간의 연결이 처음 설정되었을 때 일치하는 키 선택에서 상속됩니다. 특정 캠페인에 적용되지 않는 경우 선택한 일치 키를 제거할 수 있지만 새 일치 키를 추가할 수는 없습니다.

![일치 키 편집 옵션이 강조 표시된 대상자 활성화 워크플로우입니다.](/help/assets/collaborate/activate/edit-match-keys.png)

사용하지 않을 일치 키를 해제할 수 있는 **[!UICONTROL 일치 키 편집]** 대화 상자가 열립니다. 변경 내용을 저장하려면 **[!UICONTROL 저장]**&#x200B;을 선택하세요.

>[!NOTE]
>
>일치 키를 하나 이상 선택해야 합니다. 현재 릴리스에서는 사용 가능한 일치 키만 **[!UICONTROL 해시된 이메일]**&#x200B;이므로 이 일치 키를 제거할 수 없습니다.

![Audience 활성화 워크플로의 일치 키 편집 대화 상자입니다.](/help/assets/collaborate/activate/edit-match-keys-selection.png)

### 대상 새로 고침 빈도 설정 {#set-audience-refresh-frequency}

마지막으로 새로 고침할 대상에 대해 원하는 빈도 및 날짜 범위를 설정합니다. 현재 릴리스에서 지원되는 빈도 옵션은 **[!UICONTROL 한 번]**&#x200B;뿐입니다. **[!UICONTROL Once]** 빈도는 대상이 한 번 활성화되고 새로 고쳐지지 않음을 의미합니다. **[!UICONTROL 날짜]** 옵션이 현재 날짜로 자동 채워집니다.

![빈도 섹션이 강조 표시된 대상자 활성화 워크플로우입니다.](/help/assets/collaborate/activate/audience-frequency.png)

선택 항목이 만족스러우면 **[!UICONTROL 활성화]**&#x200B;를 선택하여 워크플로우를 완료합니다.

## 대시보드 활성화 {#activate-dashboard}

**[!UICONTROL 활성화]** 탭에서 공동 작업자에게 보낸 모든 대상과 공동 작업자가 대상으로 활성화한 모든 대상을 볼 수 있습니다.

![보낸 대상 및 활성화된 대상 섹션을 표시하는 활성화 대시보드입니다.](/help/assets/collaborate/activate/activate-dashboard.png)

## 보낸 대상자 보기 {#view-sent-audiences}

**[!UICONTROL Sent audiences to]** collaborator 섹션에 보낸 모든 대상이 나열됩니다. 현재, 대상자는 사용자가 보낸 후 공동 작업자의 구성된 대상으로 자동으로 전송됩니다. 공동 작업자의 보기에서 이러한 대상은 **[!UICONTROL 활성화된 대상]** 섹션에 표시됩니다.

전송된 각 대상자 내에서 다음 지표를 볼 수 있습니다.

| 지표 | 설명 |
|---------|----------|
| **[!UICONTROL 이름]** | 대상자의 이름입니다. |
| **[!UICONTROL 상태]** | 보낸 대상의 상태입니다. |
| **[!UICONTROL ID 개수]** | 대상자의 ID 수입니다. |
| **[!UICONTROL 중복 ID]** | 이 대상자와 공동 작업자 인벤토리에서 프로필의 총 인구 간에 겹치는 ID 수입니다. |
| **[!UICONTROL 생성일]** | 대상이 처음 전송된 날짜입니다. |
| **[!UICONTROL 마지막으로 보냄]** | 대상자를 마지막으로 공동 작업자에게 보낸 날짜입니다. |
| **[!UICONTROL 키 일치]** | 대상에 사용되는 일치 키를 나타냅니다. |

## 활성화된 대상자 보기 {#view-activated-audiences}

**[!UICONTROL 활성화된 대상]** 섹션에서 대상에 대해 활성화된 모든 대상을 볼 수 있습니다.

활성화된 각 대상자 내에서 다음 지표를 볼 수 있습니다.

| 지표 | 설명 |
|---------|----------|
| **[!UICONTROL 이름]** | 대상자의 이름입니다. |
| **[!UICONTROL 상태]** | 활성화된 대상자의 상태입니다. |
| **[!UICONTROL ID 개수]** | 공동 작업자가 대상자를 보낼 때 겹치는 ID를 기반으로 활성화된 ID의 수입니다. |
| **[!UICONTROL 생성일]** | 대상이 활성화된 날짜입니다. |
| **[!UICONTROL 마지막으로 새로 고침]** | 활성화 중에 선택한 새로 고침 일정에 따라 대상을 마지막으로 새로 고친 날짜입니다. |
| **[!UICONTROL 대상]** | 대상자가 활성화된 대상입니다. |
| **[!UICONTROL 키 일치]** | 대상에 사용되는 일치 키를 나타냅니다. |

## 보낸 대상자 삭제 {#delete-sent-audiences}

더 이상 활성화하지 않을 보낸 대상자를 삭제할 수 있습니다. 보낸 대상을 삭제하면 **[!UICONTROL 보낸 대상]** 섹션에서 제거되며 더 이상 공동 작업자의 대상으로 활성화되지 않습니다.

보낸 대상자를 삭제하려면 **[!UICONTROL 삭제]** 아이콘(![삭제 아이콘)을 선택하십시오.](/help/assets/icons/delete.png)): **[!UICONTROL 대상자를]** 섹션으로 보냈습니다.

![Sent audiences to 섹션의 Delete 옵션입니다.](/help/assets/collaborate/activate/delete-sent-audiences.png)

삭제를 확인하는 확인 대화 상자가 열립니다. **[!UICONTROL 삭제]**&#x200B;를 선택하여 확인합니다.

![삭제 확인 대화 상자](/help/assets/collaborate/activate/delete-sent-audiences-confirmation.png)

## 다음 단계 {#next-steps}

대상을 활성화하고 캠페인을 실행한 후 Adobe 지원 및 엔지니어링 팀과 협력하여 측정 데이터를 업로드하고 해당 [측정 보고서](/help/guide/collaborate/measure.md)를 보십시오.
