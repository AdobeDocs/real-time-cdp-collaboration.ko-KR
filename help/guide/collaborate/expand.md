---
title: 확장에서 확장 대상 만들기
description: Adobe Real-Time CDP Collaboration에서 공동 작업자의 대상 모집단을 사용하여 시드 대상에서 확장 대상을 만드는 방법을 알아봅니다.
source-git-commit: 88cd685742a4d85850cbf732ef93ab215287c22a
workflow-type: tm+mt
source-wordcount: '871'
ht-degree: 1%
---
# 확장에서 확장 대상 만들기

프로젝트 내의 **[!UICONTROL 확장]** 탭을 사용하여 대상자 중 하나에서 확장 대상자를 만듭니다. Collaboration은 공동 작업자의 대상 모집단을 사용하여 시드 대상과 유사한 프로필을 찾으므로 공동 작업자의 기본 대상 데이터를 노출하지 않고 새 잠재 고객에게 도달할 수 있습니다. 결과 확장 대상자는 활성화를 위해 공동 작업자에게 전송됩니다.

## 사전 요구 사항 {#prerequisites}

**[!UICONTROL 확장]** 탭을 사용하려면 먼저 다음을 수행해야 합니다.

* 시드 대상자로 사용할 하나 이상의 대상자를 [소스](/help/guide/setup/onboard-audiences.md)
* 공동 작업자가 있는 [연결됨](/help/guide/connect/establishing-connections.md)
* 해당 공동 작업자로 [프로젝트를 만듦](/help/guide/collaborate/manage-projects.md)
* 확장 대상을 받는 경우 활성화된 대상을 받도록 구성된 [대상](/help/guide/destinations/overview.md)입니다.

## 개요 확장 {#expand-overview}

**[!UICONTROL 공동 작업]** > **[!UICONTROL 내 프로젝트]**(으)로 이동하여 프로젝트를 열고 **[!UICONTROL 확장]** 탭을 선택합니다.

**[!UICONTROL 확장]** 페이지에는 이 공동 작업자를 위해 만들어진 확장 대상과 새 대상을 만드는 옵션이 표시됩니다.

![이름, 상태, 모델 크기, 대상 도달 및 마지막으로 업데이트된 열이 있는 확장 대상 테이블을 표시하는 확장 탭입니다.](/help/assets/collaborate/expand/expand-overview.png){zoomable="yes"}

**[!UICONTROL 확장 대상]** 표에는 프로젝트에서 만든 모든 확장 대상이 나열됩니다.

| 열 | 설명 |
|---|---|
| **[!UICONTROL 이름]** | 확장 대상자의 이름입니다. 편집할 때까지 기본값은 시드 대상 이름으로 설정됩니다. |
| **[!UICONTROL 상태]** | 확장 대상의 현재 상태입니다. 자세한 내용은 [확장 대상 상태](#expansion-audience-status)를 참조하십시오. |
| **[!UICONTROL 모델 크기]** | 생성된 확장 대상자의 크기입니다. 모델 처리가 완료될 때까지 사용할 수 없습니다. |
| **[!UICONTROL 대상자 도달]** | 확장 대상에 사용되는 대상 도달 범위 설정입니다. |
| **[!UICONTROL 마지막으로 업데이트됨]** | 확장 대상이 마지막으로 업데이트된 날짜 및 시간입니다. |

{style="table-layout:auto"}

### 확장 대상 상태 {#expansion-audience-status}

확장 대상자는 다음 상태로 이동합니다.

| 상태 | 설명 |
|---|---|
| **[!UICONTROL 처리 중]** | 확장 모델이 여전히 확장 대상자를 생성하고 있습니다. |
| **[!UICONTROL 초안]** | 모델이 완료되었으며 확장 대상자를 검토하여 공동 작업자에게 보낼 준비가 되었습니다. |
| **[!UICONTROL 활성]** | 확장 대상자를 공동 작업자에게 보냈습니다. |

{style="table-layout:auto"}

>[!NOTE]
>
>상태가 실시간으로 업데이트되지 않습니다. 최신 상태를 보려면 **[!UICONTROL 확장]** 탭을 다시 열거나 새로 고치십시오.

## 확장 대상 만들기 {#create-expansion-audience}

새 확장 대상을 만들려면 추가 아이콘(![추가 아이콘](/help/assets/icons/plus.png))을 선택합니다. **[!UICONTROL 확장]** 페이지에서 **[!UICONTROL 확장된 대상 만들기]**&#x200B;를 선택합니다.


**[!UICONTROL 확장 대상자 생성]** 대화 상자가 나타납니다. 모든 필드를 완료하여 확장 대상을 생성합니다.

![시드 대상, 대상 도달, 일치 키 및 시드 대상 구성원 필드가 있는 대상 확장 생성 대화 상자입니다.](/help/assets/collaborate/expand/generate-expansion-audience-dialog.png){zoomable="yes"}

### 시드 대상자 선택 {#select-seed-audience}

**[!UICONTROL 시드 대상 선택]** 드롭다운에서 고유한 대상 중 하나를 선택합니다. Collaboration에서는 이 대상을 공동 작업자 모집단에서 유사한 프로필을 찾기 위한 기반으로 사용합니다.

![대상 생성 확장 대화 상자의 시드 대상 필드입니다.](/help/assets/collaborate/expand/select-seed-audience.png){zoomable="yes"}

### 일치 키 선택 {#select-match-key}

확장 대상에 대해 하나의 일치 키를 활성화합니다. 두 개 이상을 활성화할 수 없습니다.

| 개인 ID | 디바이스 ID |
|---|---|
| **[!UICONTROL 해시된 이메일]** | **[!UICONTROL 해시된 IPv4]** |
| **[!UICONTROL 해시된 휴대폰]** | **[!UICONTROL GAID]** |
| **[!UICONTROL 충성도 ID]** | **[!UICONTROL IDFA]** |
| **[!UICONTROL CRM ID]** | **[!UICONTROL Demdex ID]** |

{style="table-layout:auto"}

>[!NOTE]
>
>시드 대상자에 지정된 일치 키가 포함되지 않은 경우 해당 옵션이 비활성화되어 선택으로 표시되지 않습니다.

![사용 가능한 일치 키 옵션이 있는 대상 확장 생성 대화 상자의 일치 키 섹션.](/help/assets/collaborate/expand/select-match-key.png){zoomable="yes"}

### 대상자 도달 범위 선택 {#select-audience-reach}

**[!UICONTROL 대상 도달]** 드롭다운을 사용하여 시드 대상 유사도와 전체 도달 범위의 균형을 맞춥니다. 시드 대상자에 대한 유사성과 전체 도달 범위 사이의 중간 지점은 **[!UICONTROL 균형]**&#x200B;을(를) 선택하십시오.

![[균형 조정] 옵션을 선택하고 설명 텍스트가 있는 대상 확장 생성 대화 상자의 대상 도달 필드입니다.](/help/assets/collaborate/expand/select-audience-reach.png){zoomable="yes"}

### 시드 대상자 포함 또는 제외 {#include-exclude-seed-audience}

**[!UICONTROL 시드 대상]** 라디오 단추를 사용하여 원본 시드 대상을 최종 확장 대상에 포함할지 또는 제외할지 선택합니다.

![예 및 아니요 라디오 단추가 있는 대상 확장 생성 대화 상자의 시드 대상 멤버 필드입니다.](/help/assets/collaborate/expand/include-exclude-seed-audience.png){zoomable="yes"}

### 확장 대상 생성 {#generate-expansion-audience}

모든 필드가 완료되면 **[!UICONTROL 확장 대상 생성]**&#x200B;을 선택하십시오. Collaboration에서 확장 대상을 만들고 있으며 **[!UICONTROL 확장]** 페이지에서 진행 상황을 추적할 수 있다는 확인 메시지가 표시됩니다.

## 확장 대상자 검토 및 보내기 {#review-send-expansion-audience}

확장 대상자의 상태가 **[!UICONTROL 초안]**(으)로 업데이트되면 **[!UICONTROL 확장 대상자]** 테이블에서 해당 이름을 선택하여 엽니다.

![대상 메타데이터, 모델 크기, 시드 대상 크기 및 전송 단추를 표시하는 확장 대상 세부 정보 페이지입니다.](/help/assets/collaborate/expand/expansion-audience-detail.png){zoomable="yes"}

이 보기에서 다음 작업을 수행할 수 있습니다.

* 확장 대상 이름 편집
* 생성 날짜 및 시간 보기
* 시드 대상 크기를 생성된 확장 대상 크기와 비교
* 대상자 생성에 사용되는 일치 키 검토

준비가 되면 **[!UICONTROL 파트너에게 보내기]**&#x200B;를 선택하여 확장 대상자를 공동 작업자에게 보냅니다. 대상자를 보낼 때까지 대상자가 **[!UICONTROL 초안]** 상태로 유지된 다음 **[!UICONTROL 활성]**(으)로 업데이트됩니다.

>[!NOTE]
>
>공동 작업자에게 구성된 대상이 없는 경우 **[!UICONTROL 파트너에게 보내기]**&#x200B;를 사용할 수 없습니다. 공동 작업자가 먼저 대상을 설정해야 한다는 메시지가 표시됩니다.

>[!IMPORTANT]
>
>확장 대상자는 공동 작업자에게 전송되지 않으면 생성된 후 7일 후에 만료됩니다.

## 확장 대상자 수신 및 활성화 {#receive-activate-expansion-audience}

확장 대상을 전송하면 Collaboration은 연결에 대해 구성된 활성화 설정에 따라 이를 공동 작업자에게 전달합니다.

* **자동 활성화**&#x200B;가 활성화된 경우 Collaboration은 Collaborator가 구성한 대상에 확장 대상을 자동으로 활성화하며 해당 [활성화 탭](./activate.md#activated-audiences)에 표시됩니다.
<!-- Beta release: automatic activation is the only available activation setting. Uncomment the manual activation guidance below when manual activation is introduced with the GA release. -->
<!-- * If **manual activation** is enabled, the expansion audience appears in your collaborator's [Received audiences](./activate.md#received-audiences) section of the **[!UICONTROL Activate]** tab, and your collaborator must manually activate it. -->

## 다음 단계

확장 대상을 보낸 후에는 [검색 탭](./discover.md)을 사용하여 다른 대상과 비교하거나 [활성화 탭](./activate.md)을 사용하여 활성화를 추적하세요.
