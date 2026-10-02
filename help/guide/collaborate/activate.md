---
title: 대상자 활성화
description: Adobe Real-Time CDP Collaboration의 대상에 대상을 보내고, 받은 대상을 자동 또는 수동으로 활성화하는 방법을 알아봅니다.
audience: admin, publisher, advertiser
exl-id: fd82fcbf-ab39-48e0-9438-0a9046693431
TQID: https://experienceleague.adobe.com/bfPHtcW8Mf6RhIlg5fKcJmPSEKDyAODjbNRJ5D3SMkQ
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
    internal-label: Real-Time Customer Data Platform
feature_v2:
  - id: ba929a52-9339-4154-9487-317dc875a3c7
    internal-label: Use cases
topic_v2:
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
    internal-label: Measurement
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: df0c7fe0d09203a02a192931135abaa1715e593f
workflow-type: tm+mt
source-wordcount: '2043'
ht-degree: 1%
---
# 대상자 활성화

프로젝트 내의 **[!UICONTROL 활성화]** 탭을 사용하여 Collaborator에 대상을 보내고, Collaborator로부터 받은 대상을 검토하고, 구성된 대상에 전달하기 위해 받은 대상을 활성화합니다. 대상자가 수신될 때 자동으로 활성화를 만들거나 수신 공동 작업자가 수동으로 만들 수 있습니다. 최상위 **[!UICONTROL 활성화]** 작업 영역에서 대상을 구성하고 관리하려면 [대상 개요](../destinations/overview.md)를 참조하십시오.

>[!IMPORTANT]
>
>**[!UICONTROL 활성화]** 탭은 **대상자 활성화** 사용 사례가 연결 프로세스 [동안 활성화됨](../connect/establishing-connections.md#connection-settings)인 경우에만 사용할 수 있습니다. 사용 사례에 대한 자세한 내용은 [프로젝트 관리](./manage-projects.md#project-use-cases)를 참조하십시오.

[검색 탭](./discover.md)을 사용하여 캠페인과 가장 일치하는 대상을 식별한 다음 공동 작업자에게 보냅니다.

수신자가 연결 설정에서 자동 활성화 대상을 구성하는 경우 발신자는 대상자를 보낼 때 활성화 일정을 선택합니다. 대상은 보낸 사람의 읽기 전용입니다. 대상자가 수신되면 발신자의 활성화 일정에 따라 대상자가 수신자의 구성된 대상에 자동으로 활성화됩니다. 연결 설정 지침은 [자동 활성화 대상 구성](../connect/manage-connections.md#configure-auto-activation-destination)을 참조하십시오.

수신자가 자동 활성화 대상을 구성하지 않은 경우 보내기 및 활성화는 별도의 작업으로 유지됩니다. 보내기를 통해 수신자는 대상에 액세스할 수 있으며 수신자는 대상을 수동으로 활성화할 때 대상 및 일정을 선택합니다. 프로젝트 내에서 활성화하기 위해 사전 구성된 대상만 선택할 수 있습니다. 대상 구성 지침은 [대상 관리](../destinations/manage-destinations.md)를 참조하십시오.

사용 가능한 섹션 및 작업은 조직에서 프로젝트의 대상을 보내고 있는지 아니면 받고 있는지에 따라 다릅니다. **[!UICONTROL 활성화]** 탭에는 다음 섹션이 포함되어 있습니다.

| 섹션 | 설명 |
|---|---|
| **[!UICONTROL 대상자를 [공동 작업자]]**&#x200B;에게 보냈습니다. | 공동 작업자에게 보낸 대상입니다. |
| **[!UICONTROL 받은 대상]** | 공동 작업자가 보내어 활성화할 수 있는 대상입니다. |
| **[!UICONTROL 활성화된 대상자]** | 자동 또는 수동으로 생성된 활성화가 있는 대상을 받았습니다. |

![프로젝트 수준의 활성화 탭으로, 맨 위에 요약 카운트가 있고 확장된 [보낸 대상], [받은 대상] 및 [활성화된 대상] 섹션이 있습니다. 각 섹션에는 상태 카운트 및 대상자 세부 정보 테이블이 표시됩니다.](/help/assets/collaborate/activate/activate-dashboard.png){zoomable="yes"}

## 사전 요구 사항 {#prerequisites}

대상자를 보내거나 활성화하기 전에 다음을 확인하십시오.

- 대상자는 소스에 추가되고 전송할 수 있습니다. 자세한 내용은 [Source 및 대상자 관리](../setup/onboard-audiences.md)를 참조하십시오.
- 대상은 전송 및 활성화에 필요한 최소 1,000개의 ID 중복 임계값을 충족합니다.
- 다중 일치 키 대상을 사용할 때 필요한 일치 키로 대상을 구성합니다.
- 받은 대상을 활성화해야 하는 경우 하나 이상의 대상이 구성됩니다. 자세한 내용은 [대상 개요](../destinations/overview.md)를 참조하세요.
- 자동 활성화의 경우 수신자가 활성 대상을 소유하고 이 대상을 연결의 [자동 활성화 대상](../connect/manage-connections.md#configure-auto-activation-destination)(으)로 선택했습니다.

## 대상자 보내기 {#send-audiences}

공동 작업자에게 이에 대한 액세스 권한을 부여할 대상을 보냅니다. 대상자를 전송하면 **[!UICONTROL 대상자를 [공동 작업자]]** 섹션으로 전송함 섹션과 공동 작업자의 **[!UICONTROL 받은 대상자]** 섹션에 표시됩니다.

**[!UICONTROL 공동 작업]**(으)로 이동하여 프로젝트를 연 다음 **[!UICONTROL 활성화]** 탭을 선택합니다.

**[!UICONTROL 대상자를 [공동 작업자]]**(으)로 보냈습니다. 섹션에서 추가 아이콘(![추가 아이콘.](/help/assets/icons/plus.png))을 선택합니다. 대상자가 전송되지 않은 경우 대신 빈 디스플레이에서 **[!UICONTROL 대상자 보내기]**&#x200B;를 선택하십시오.

![대상자가 전송되지 않았을 때의 프로젝트 수준 활성화 탭입니다. 빈 표시 메시지는 대상자를 보내지 않았음을 설명하고 대상자 보내기 단추를 표시합니다.](/help/assets/collaborate/activate/activate-new-audiences.png){zoomable="yes"}

**[!UICONTROL 대상자 보내기]** 워크플로우가 열립니다. 대상 선택기를 사용하여 대상을 찾거나 **[!UICONTROL 대상 찾아보기]**&#x200B;를 선택하여 사용 가능한 대상을 비교합니다.

>[!IMPORTANT]
>
>겹치는 ID가 1000개가 넘는 대상자만 활성화할 수 있습니다. 대상 겹침이 1000 ID 임계값 근처에 있는 경우 활성화가 실패할 수 있습니다.

![대상자 선택기와 대상자 찾아보기 단추를 사용하여 대상자 보내기 워크플로우입니다. 이 워크플로우를 통해 보낸 사람이 일치 키 및 액세스 설정을 구성하기 전에 대상을 선택할 수 있습니다.](/help/assets/collaborate/activate/audience-activation.png){zoomable="yes"}

**[!UICONTROL 대상자 찾아보기]** 대화 상자에서 각 대상자에 대해 **[!UICONTROL ID 개수]**, **[!UICONTROL 중복 ID]** 및 **[!UICONTROL 중복 %]**&#x200B;을 검토합니다.

![ID 수, 겹치는 ID 수 및 겹치는 비율로 사용 가능한 대상을 나열하는 대상자 찾아보기 대화 상자](/help/assets/collaborate/activate/browse-audiences.png){zoomable="yes"}

>[!IMPORTANT]
>
>대상자가 여러 일치 키를 사용하는 경우 선택한 모든 일치 키는 필수 중복 임계값을 충족해야 합니다. 대상자를 보내기 전에 대상자가 중복 요구 사항을 충족하는지 확인하려면 [검색 탭](./discover.md)을 사용하세요.

보낼 대상을 선택한 다음 **[!UICONTROL 저장]**&#x200B;을 선택합니다.

선택한 대상자가 워크플로우에 ID 및 중복 정보와 함께 표시됩니다.

![ID 수, 중복 ID 수, 중복 백분율, 일치 키 및 일치 키 편집 옵션을 표시하는 선택한 대상을 포함하는 대상 전송 워크플로우입니다.](/help/assets/collaborate/activate/audience-selected.png){zoomable="yes"}

### 일치 키 편집 {#edit-match-keys}

Collaborator 연결에 대해 구성된 일치 키를 사용하거나 대상에 적용되지 않는 일치 키를 제거합니다.

선택한 대상자에서 **[!UICONTROL 일치 키 편집]**&#x200B;을 선택합니다.

![일치 키 편집 옵션이 강조 표시된 대상자 보내기 워크플로우에서 선택한 대상자입니다.](/help/assets/collaborate/activate/edit-match-keys.png){zoomable="yes"}

**[!UICONTROL 일치 키 편집]** 대화 상자가 나타납니다. 사용하지 않을 일치 키를 끈 다음 **[!UICONTROL 저장]**&#x200B;을 선택합니다.

>[!NOTE]
>
>일치 키를 하나 이상 선택한 상태로 유지해야 합니다.

![Collaborator 연결 및 저장 단추를 통해 사용할 수 있는 일치 키에 대한 토글 컨트롤이 있는 일치 키 편집 대화 상자.](/help/assets/collaborate/activate/edit-match-keys-selection.png){zoomable="yes"}

### 대상자 액세스 구성 {#configure-audience-access}

대상자를 보내는 방법과 공동 작업자가 대상자에 액세스할 수 있는 기간을 구성합니다.

**[!UICONTROL 액세스 기간]** 컨트롤을 사용하여 다음 옵션 중 하나를 선택하십시오.

- **[!UICONTROL 지금 보내기(1회)]**: 대상자를 한 번 보냅니다. 수신 공동 작업자가 한 번 활성화할 수 있습니다.
- **[!UICONTROL 반복 대상 전송을 예약합니다]**: 지정된 액세스 기간 동안 대상을 새로 고치십시오. **[!UICONTROL 날짜 범위]** 컨트롤을 사용하여 시작 날짜와 종료 날짜를 선택하십시오.

![대상자 보내기 워크플로우의 액세스 기간 단계이며 대상자를 한 번 보내거나 되풀이되는 대상자 보내기를 예약하는 옵션이 있습니다. 반복 옵션은 액세스 기간을 정의하기 위한 날짜 컨트롤을 표시합니다.](/help/assets/collaborate/activate/activation-frequency.png)

### 자동 활성화 일정 선택 {#auto-activation-schedule}

Collaborator가 연결에 대해 자동 활성화 대상을 구성한 경우 **[!UICONTROL 활성화]** 섹션은 **[!UICONTROL 자동 활성화]**&#x200B;이 활성화되었음을 나타냅니다. 수신자가 선택한 대상이 읽기 전용으로 표시됩니다. 발신자는 **[!UICONTROL 빈도]**&#x200B;를 사용하여 활성화가 실행되는 시기를 선택하십시오.

- **[!UICONTROL 지금 활성화(1회)]**: 대상자를 받으면 활성화를 한 번 실행합니다.
- **[!UICONTROL 일회성 대상자 활성화를 예약합니다]**: 선택한 미래 날짜 및 시간에 활성화를 한 번 실행합니다.
- **[!UICONTROL 반복 활성화를 예약합니다]**: 선택한 날짜 범위 동안 구성한 일정에 따라 활성화를 실행합니다.

![자동 활성화가 활성화된 대상자 전송 워크플로우와 [빈도] 메뉴에 즉시, 향후 일회성 및 반복 활성화 옵션이 표시됩니다.](/help/assets/collaborate/activate/choose-auto-activation-schedule.png){zoomable="yes"}

반복 활성화의 경우 활성화 일정, 시작 시간 및 날짜 범위를 구성합니다. 자동 활성화는 즉시, 향후 일회성 또는 반복 일정을 지원합니다. 반복은 필요하지 않습니다.

![매일 반복되는 활성화 일정, 시작 시간 및 날짜 범위로 구성된 대상자 보내기 워크플로우입니다.](/help/assets/collaborate/activate/configure-recurring-auto-activation.png){zoomable="yes"}

대상자 및 액세스 설정이 완료되면 **[!UICONTROL 보내기]**&#x200B;를 선택하세요.

대상자가 **[!UICONTROL 대상자를 [공동 작업자]]** 섹션으로 보냈습니다. 공동 작업자는 **[!UICONTROL 받은 대상]** 섹션에서 검토할 수 있습니다. 자동 활성화가 활성화되면 Collaboration이 수신기에 대한 활성화도 생성하고 활성화는 선택한 일정에 따라 실행됩니다.

## 보낸 대상자 보기 {#view-sent-audiences}

[공동 작업자에게 **[!UICONTROL 보낸 대상]]** 섹션을 사용하여 보낸 대상을 검토하고 현재 액세스 상태를 모니터링합니다.

각 보낸 대상자는 다음 정보를 표시합니다.

| 열 | 설명 |
|---|---|
| **[!UICONTROL 대상 이름]** | 보낸 대상자의 이름입니다. |
| **[!UICONTROL 상태]** | 대상자의 현재 액세스 상태입니다. |
| **[!UICONTROL ID 개수]** | 대상자의 ID 수입니다. |
| **[!UICONTROL 중복 ID]** | 공동 작업자의 인벤토리와 겹치는 ID의 수입니다. |
| **[!UICONTROL 생성일]** | 대상자를 처음 보낸 날짜 및 시간입니다. |
| **[!UICONTROL 마지막으로 보냄]** | 대상 데이터가 가장 최근에 공동 작업자에게 전송된 날짜와 시간입니다. |
| **[!UICONTROL 액세스 기간]** | 대상자를 전송할 때 구성된 액세스 설정입니다. |
| **[!UICONTROL 키 일치]** | 대상자를 보낼 때 사용되는 일치 키입니다. |

### 보낸 대상자 삭제 {#delete-sent-audience}

보낸 대상자를 삭제하면 보낸 대상자 목록에서 제거되고 공동 작업자의 액세스를 취소할 수 있습니다.

삭제 아이콘(![삭제 아이콘](/help/assets/icons/delete.png))을 선택합니다. **[!UICONTROL 대상자를 [공동 작업자]]** 섹션으로 보냈습니다.

![대상자 행 옆에 삭제 아이콘이 표시된 보낸 대상자 섹션입니다.](/help/assets/collaborate/activate/delete-sent-audiences.png){zoomable="yes"}

확인 대화 상자가 나타납니다. **[!UICONTROL 삭제]**&#x200B;를 선택하여 확인합니다.

![취소 및 삭제 단추와 함께 대상이 제거되고 공동 작업자의 액세스 권한이 상실됨을 설명하는 보낸 사람 대상 삭제 확인 대화 상자가 표시됩니다.](/help/assets/collaborate/activate/delete-sent-audiences-confirmation.png)

대상자가 섹션에서 제거되며 공동 작업자는 해당 섹션에 액세스할 수 없습니다.

## 수신한 대상자 보기 {#received-audiences}

**[!UICONTROL 받은 대상]** 섹션을 사용하여 공동 작업자가 보낸 대상을 검토합니다. 대상이 전송되기 전에 자동 활성화 대상이 구성된 경우 Collaboration은 대상이 수신되면 자동으로 활성화를 만듭니다. 자동 활성화가 반복되는 경우 다른 대상에 대한 추가 수동 활성화를 만들 수도 있습니다. 자세한 내용은 [받은 대상을 수동으로 활성화](#activate-received-audience)를 참조하십시오. 자동 활성화 대상이 구성되지 않은 경우 대상을 수동으로 활성화합니다.

수신된 각 대상에는 다음 정보가 표시됩니다.

| 열 | 설명 |
|---|---|
| **[!UICONTROL 대상 이름]** | 받은 대상자의 이름입니다. |
| **[!UICONTROL 상태]** | 대상자의 현재 액세스 상태입니다. |
| **[!UICONTROL ID 개수]** | 대상자의 ID 수입니다. |
| **[!UICONTROL 중복 ID]** | 인벤토리와 겹치는 ID 수입니다. |
| **[!UICONTROL 마지막 데이터 흐름 실행]** | 대상에 대해 가장 최근 데이터 흐름이 실행된 날짜 및 시간입니다. |
| **[!UICONTROL 액세스 기간]** | 대상자를 보낸 공동 작업자가 구성한 액세스 설정입니다. |
| **[!UICONTROL 키 일치]** | 대상자에 사용되는 일치 키입니다. |

![활성 및 만료된 대상자 규모가 있는 수신된 대상자 섹션입니다. 각 대상 행에는 해당 이름, 상태, ID 정보, 마지막 데이터 흐름 실행, 액세스 기간, 일치 키 및 활성화를 시작하는 데 사용되는 추가 아이콘이 표시됩니다.](/help/assets/collaborate/activate/received-audiences-section.png){zoomable="yes"}

### 수신된 대상자 수동 활성화 {#activate-received-audience}

수신된 대상을 수동으로 활성화하여 구성된 대상 중 하나로 해당 데이터를 전송합니다.

**[!UICONTROL 받은 대상]** 섹션에서 추가 아이콘(![추가 아이콘](/help/assets/icons/plus.png))을 선택합니다. 활성화할 대상 옆에 있습니다.

**[!UICONTROL 대상자 활성화]** 대화 상자가 나타납니다.

대상 데이터를 받는 대상을 선택하려면 **[!UICONTROL 대상]**&#x200B;을 사용하십시오. 대상 목록이 비어 있으면 계속하기 전에 대상을 구성합니다. 지침은 [대상 개요](../destinations/overview.md)를 참조하십시오.

활성화 실행 시기와 빈도를 선택하도록 **[!UICONTROL 빈도]** 및 사용 가능한 일정 컨트롤을 구성합니다. **[!UICONTROL 활성화]**&#x200B;를 선택합니다.

다음 예제에서는 **[!UICONTROL Northstar 대상 내보내기]**&#x200B;를 대상으로 선택한 수동 활성화 워크플로를 보여 줍니다.

![Northstar 대상 내보내기를 선택하고 일별 일정, 시작 시간 및 날짜 범위를 구성한 Northstar 가을 캠페인 고객을 위한 수동 대상자 활성화 대화 상자의 예입니다.](/help/assets/collaborate/activate/manually-activate-received-audience.png){zoomable="yes"}

>[!NOTE]
>
>반복 자동 활성화가 있는 받은 대상의 경우 해당 대상에 대한 추가 활성화를 다른 대상에 수동으로 만들 수 있습니다. 자동 활성화는 독립적으로 계속됩니다.

대화 상자가 닫히고 **[!UICONTROL 활성화된 대상자]** 섹션에 활성화가 표시됩니다. 받은 대상자는 **[!UICONTROL 받은 대상자]** 섹션에서 액세스 권한이 활성화된 상태로 유지됩니다.

## 활성화된 대상자 보기 {#activated-audiences}

**[!UICONTROL 활성화된 대상]** 섹션을 사용하여 자동 또는 수동으로 생성된 활성화를 받은 대상을 확인하고 대상 및 게재 상태를 검토할 수 있습니다. 자동으로 생성된 활성화는 수신자가 수동 활성화 워크플로를 완료할 필요 없이 여기에 표시됩니다.

![받은 대상의 Northstar Fall Campaign 고객을 표시하는 활성화 탭과 활성화된 대상의 Northstar 대상 내보내기에 대해 자동으로 생성된 일일 활성화.](/help/assets/collaborate/activate/view-auto-activated-audience.png){zoomable="yes"}

활성화된 각 대상에는 다음 정보가 표시됩니다.

| 열 | 설명 |
|---|---|
| **[!UICONTROL 대상 이름]** | 활성화된 대상자의 이름입니다. |
| **[!UICONTROL 상태]** | 현재 활성화 상태입니다. |
| **[!UICONTROL 활성화된 개수]** | 대상에 활성화된 ID의 수입니다. |
| **[!UICONTROL 마지막으로 새로 고침]** | 활성화된 대상이 가장 최근에 새로 고침된 날짜 및 시간입니다. |
| **[!UICONTROL 대상]** | 대상 데이터를 수신하는 대상. |
| **[!UICONTROL 빈도]** | 활성화 빈도(예: 일회성 또는 반복 일정). |
| **[!UICONTROL 날짜]** | 활성화가 실행되는 날짜 또는 날짜 범위입니다. |
| **[!UICONTROL 키 일치]** | 활성화된 대상자에 포함된 일치 키. |

![활성, 보관 및 일시 중지된 활성화 횟수가 있는 활성화된 대상자 섹션입니다. 각 행에는 대상 이름, 상태, 활성화된 수, 마지막으로 새로 고친 날짜, 대상, 빈도, 활성화 날짜, 일치 키 및 삭제 아이콘이 표시됩니다.](/help/assets/collaborate/activate/activated-audiences-section.png){zoomable="yes"}

### 활성화된 대상자 삭제 {#delete-activated-audience}

활성화된 대상을 삭제하여 **[!UICONTROL 활성화된 대상]** 섹션에서 활성화를 제거합니다.

삭제 아이콘(![삭제 아이콘](/help/assets/icons/delete.png))을 선택합니다. 활성화된 대상 옆에 있습니다.

확인 대화 상자가 나타납니다. **[!UICONTROL 삭제]**&#x200B;를 선택하여 확인합니다.

![취소 및 삭제 단추를 사용하여 대상을 활성화된 대상 목록에서 제거하고 나중에 다시 활성화할 수 있음을 설명하는 활성화된 대상 삭제 확인 대화 상자가 표시됩니다.](/help/assets/collaborate/activate/delete-activated-audience-confirmation.png)

활성화가 목록에서 제거됩니다. 액세스가 활성 상태를 유지하는 동안 받은 대상을 다시 활성화할 수 있습니다.

## 다음 단계 {#next-steps}

대상자를 보내거나 활성화한 후 **[!UICONTROL 대상자를 [공동 작업자]]** 및 **[!UICONTROL 활성화된 대상자]** 섹션으로 보냈습니다. 캠페인이 완료되면 Adobe 지원 및 엔지니어링 팀과 협력하여 측정 데이터를 업로드하고 해당 [측정 보고서](./measure.md)를 확인하십시오.
