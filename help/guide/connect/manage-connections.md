---
title: 연결 관리
description: Real-Time CDP Collaboration에서 연결을 관리하는 방법을 알아봅니다.
audience: admin, publisher, advertiser
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/kr/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 50120839-4a20-4ec1-8887-9342bd17c52d
source-git-commit: 46d2596bd0ccdc5da32067493968945c61f8acc4
workflow-type: tm+mt
source-wordcount: '1079'
ht-degree: 1%

---

# 연결 관리 {#manage-connections}

{{limited-availability-release-note}}

**[!UICONTROL 내 연결]** 작업 영역은 연결을 관리할 중앙 위치를 제공합니다. **[!UICONTROL 기존 연결]** 섹션에서 기존 연결을 보고 **[!UICONTROL 작업 필요]** 섹션에서 작업이 필요한 연결을 확인할 수 있습니다.

## 연결 보기 {#view-connection}

기존 연결을 보려면 **[!UICONTROL 연결]** 작업 영역으로 이동합니다. 게시자는 기존 연결을 표시합니다. 광고주는 **[!UICONTROL 내 연결]**(으)로 이동해야 합니다.

![내 연결 작업 영역에서 연결에 대해 강조 표시된 연결 보기 옵션입니다.](/help/assets/connect/manage-connections/view-connection.png){zoomable="yes"}

연결 개요 작업 공간이 나타나고 연결 및 활성 프로젝트에 대한 세부 정보가 표시됩니다. 연결 설정을 보려면 **[!UICONTROL 연결 설정]**&#x200B;을 선택하십시오.

![연결 개요 작업 영역에서 강조 표시된 연결 설정 옵션입니다.](/help/assets/connect/manage-connections/connection-overview.png){zoomable="yes"}

사용자와 공동 작업자 간의 연결 세부 정보가 표시되는 연결 설정 작업 영역이 나타납니다. 여기에서 연결 프로세스 중에 선택한 모든 설정, 연결의 현재 상태, 연결 소유자 및 공동 작업자의 연락처 정보를 볼 수 있습니다. 특정 연결 설정에 대한 자세한 내용은 [연결 설정](/help/guide/connect/establishing-connections.md#connection-settings) 안내서를 참조하십시오.

![연결 설정 작업 영역에 연결 세부 정보가 표시됩니다.](/help/assets/connect/manage-connections/connection-settings.png){zoomable="yes"}

## 연결 삭제 {#delete-connection}

계속 작업하지 않으려는 공동 작업자와의 연결을 삭제할 수 있습니다. 연결을 삭제하려면 삭제하려는 연결로 이동한 다음 연결 작업 영역에서 삭제 아이콘 ![삭제 아이콘](/help/assets/common/delete.svg)을 선택합니다.

![연결 작업 영역에서 강조 표시된 삭제 아이콘입니다.](/help/assets/connect/establish-connection/delete-option.png){zoomable="yes"}

연결 삭제를 확인하는 확인 대화 상자가 나타납니다. **[!UICONTROL 삭제]**&#x200B;를 선택하여 삭제를 확인합니다.

![연결을 삭제하는 확인 대화 상자입니다.](/help/assets/connect/establish-connection/delete-confirmation-dialog.png){zoomable="yes"}

>[!WARNING]
>
>연결이 삭제되면 공동 작업의 기존 프로젝트가 모두 영구적으로 삭제되고 복구할 수 없습니다. 연결 요청은 **[!UICONTROL 내 연결]** 내의 **[!UICONTROL 작업 필요]** 섹션 내에서 보류 중인 상태로 유지되지만 연결 및 해당 구성은 더 이상 활성화되지 않습니다. 공동 작업자와 다시 연결하려면 연결을 다시 설정해야 합니다.

## 연결 편집 {#edit-connection}

공동 작업 연결의 소유자는 연결이 설정된 후 공동 작업자와 연결 설정을 편집할 수 있습니다. 다음과 같은 작업을 수행할 수 있습니다.

* 사용 사례 추가
* 일치 키를 추가합니다. 일치 키 제거는 향후 지원됩니다.
* 대상자 활성화 권한 업데이트
* 크레딧 분할 설정 업데이트

>[!IMPORTANT]
>
>사용 사례 또는 일치 키가 연결에 추가되면 제거할 수 없습니다.

>[!TIP]
>
>**owner**&#x200B;은(는) **recipient**&#x200B;에게 초대를 보내 연결을 시작하는 공동 작업자입니다. 자세한 내용은 [공동 작업자와 연결 설정 설명서](./establishing-connections.md)를 참조하십시오.

연결 설정을 편집하려면 연결 설정 작업 공간으로 이동합니다. 세 점 아이콘(![세 점 아이콘)을 선택합니다.](/help/assets/icons/more.png)) 사용 가능한 작업을 보려면 **[!UICONTROL 편집]**&#x200B;을 선택합니다.

![편집 옵션이 강조 표시된 연결 설정 작업 영역입니다.](/help/assets/connect/manage-connections/edit-connection.png){zoomable="yes"}

공동 작업자 검토를 위해 설정 변경 사항을 편집하고 제출하라는 대화 상자가 나타납니다. **[!UICONTROL 편집]**&#x200B;을 선택합니다.

![편집 옵션이 강조 표시된 연결 설정 편집 대화 상자입니다.](/help/assets/connect/manage-connections/edit-connection-settings-dialog.png){zoomable="yes"}

### 대상자 활성화 편집 {#edit-audience-activation}

대상 활성화 설정은 연결에서 대상을 대상에 활성화할 수 있는 공동 작업자를 결정합니다. 이 설정을 변경하려면 **[!UICONTROL 대상 활성화]** 섹션에서 **[!UICONTROL 편집]**&#x200B;을(를) 선택하십시오.

![대상자 활성화 섹션 및 편집 옵션을 표시하는 연결 설정 편집 화면입니다.](/help/assets/connect/manage-connections/edit-audience-activation.png){zoomable="yes"}

**[!UICONTROL 대상자 활성화]** 대화 상자에서 드롭다운 메뉴를 사용하여 대상자 활성화 권한을 업데이트합니다. 단일 공동 작업자를 선택하거나 두 공동 작업자가 대상을 활성화하도록 허용할 수 있습니다.

![대상자 활성화 권한 업데이트를 위해 대상자 활성화 대화 상자 강조 표시 드롭다운 메뉴가 확장되었습니다.](/help/assets/connect/manage-connections/audience-activation-dropdown-menu.png){zoomable="yes"}

완료되면 **[!UICONTROL 저장]**&#x200B;을 선택합니다.

![새 대상 활성화 권한과 저장 옵션을 보여 주는 대상 활성화 대화 상자입니다.](/help/assets/connect/manage-connections/audience-activation-dialog.png){zoomable="yes"}

### 사용 사례 추가 {#add-use-cases}

Collaboration에서 검색, 활성화 및 측정과 같은 사용 사례는 공동 작업자와 함께 사용할 수 있는 프로젝트 섹션 및 기능을 결정합니다. 향후 프로젝트를 위해 기존 연결에 추가 사용 사례를 추가할 수 있습니다. 자세한 내용은 [공동 작업 사용 사례](../overview/use-cases.md)를 참조하세요.

새 사용 사례를 추가하려면 **[!UICONTROL 사용 사례]** 섹션에서 **[!UICONTROL 편집]**&#x200B;을 선택하세요.

![사용 사례 섹션 및 편집 옵션이 강조 표시된 연결 설정 편집 화면입니다.](/help/assets/connect/manage-connections/edit-use-cases.png){zoomable="yes"}

**[!UICONTROL 사용 사례]** 대화 상자에서 추가하려는 새 사용 사례를 전환한 다음 **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

![사용 사례 대화 상자에 강조 표시된 저장 옵션이 표시됩니다.](/help/assets/connect/manage-connections/use-cases-dialog.png){zoomable="yes"}

>[!NOTE]
>
>[대상 활성화&quot; 또는 &quot;측정&quot;과 같은 새 사용 사례를 추가](#add-use-cases)하면 연결 설정 편집 화면이 업데이트되어 **[!UICONTROL 대상 활성화]** 및 **[!UICONTROL 크레딧 분할]** 섹션이 포함됩니다. 이러한 새로운 사용 사례에 적합한 설정을 구성해야 합니다. 자세한 내용은 [대상자 활성화](../connect/establishing-connections.md#audience-activation) 및 [크레딧 분할](../connect/establishing-connections.md#credit-split) 안내서를 참조하십시오.
>
>![새 사용 사례가 추가된 후 대상 활성화 및 크레딧 분할 섹션이 표시되는 연결 설정 편집 화면입니다.](/help/assets/connect/manage-connections/setup-audience-activation-credit-split.png){zoomable="yes"}

### 일치 키 추가 {#add-match-keys}

계정에 구성되어 있고 공동 작업자가 선택한 일치 키만 연결에 사용할 수 있습니다. [계정에 새 일치 키를 추가](../setup/onboard-account.md#edit-match-keys)하고 공동 작업자가 동일한 키를 선택하면 기존 연결 내에서 해당 키를 활성화할 수 있습니다.

연결 설정 편집 화면의 **[!UICONTROL 키 일치]** 섹션에서 **[!UICONTROL 편집]**&#x200B;을(를) 선택합니다.

![연결 설정 편집 화면에서 [키 일치] 섹션과 [편집] 옵션을 강조 표시합니다.](/help/assets/connect/manage-connections/edit-connection-match-keys.png){zoomable="yes"}

**[!UICONTROL 일치 키]** 대화 상자가 나타나고 연결에 대해 구성된 기존 일치 키를 표시합니다. 추가할 일치 키를 선택한 후 **[!UICONTROL 저장]**&#x200B;을 선택합니다.

![일치하는 키 대화 상자에 선택한 새 일치 키와 저장 옵션이 표시됩니다.](/help/assets/connect/manage-connections/connection-match-keys-dialog.png){zoomable="yes"}

### 신용 분할 편집 {#edit-credit-split}

크레딧 분할 설정은 연결의 각 사용 사례와 관련된 비용을 담당하는 공동 작업자를 지정합니다. 이 설정을 업데이트하려면 **[!UICONTROL 크레딧 분할]** 섹션에서 **[!UICONTROL 편집]**&#x200B;을(를) 선택하십시오.

![크레딧 분할 섹션과 편집 옵션을 강조 표시하는 연결 설정 편집 화면입니다.](/help/assets/connect/manage-connections/edit-credit-split.png){zoomable="yes"}

**[!UICONTROL 신용 분할]** 대화 상자에서 [!UICONTROL 활성화 일치] 및 [!UICONTROL 측정]에 대한 기본 설정을 선택합니다. 그런 다음 **[!UICONTROL 저장]**&#x200B;을 선택하여 확인합니다.

![크레딧 분할 설정 및 저장 옵션을 표시하는 크레딧 분할 대화 상자.](/help/assets/connect/manage-connections/credit-split-dialog.png){zoomable="yes"}

### 변경 사항 검토 및 제출 {#review-and-submit-changes}

연결 설정 편집을 완료하면 **[!UICONTROL 변경 내용 제출]**&#x200B;을 검토하고 선택합니다. 연결 설정 업데이트가 검토를 위해 공동 작업자에게 전송됩니다.

![업데이트 및 변경 내용 제출 옵션이 표시되는 연결 설정 편집 화면입니다.](/help/assets/connect/manage-connections/review-and-submit-changes.png){zoomable="yes"}

#### 연결 설정 변경 내용을 초안으로 저장

연결 설정 변경 사항을 초안으로 저장하고 언제든지 돌아가서 연결 설정 업데이트를 완료할 수 있습니다.

변경 내용을 초안으로 저장하려면 **[!UICONTROL 변경 내용 제출]** 옆에 있는 **[!UICONTROL 취소]**&#x200B;을(를) 선택하십시오. 그런 다음 **[!UICONTROL 제출되지 않은 변경 내용]** 대화 상자에서 **[!UICONTROL 나중에 계속]**&#x200B;을 선택하여 확인합니다.

![연결 설정 편집 화면](/help/assets/connect/manage-connections/unsubmitted-changes-dialog.png){zoomable="yes"}

이제 변경 사항이 초안으로 저장됩니다. 연결 설정 작업 영역에서 제출되지 않은 변경 사항이 있음을 나타내는 알림을 볼 수 있습니다. 추가로 업데이트하려면 **[!UICONTROL 편집 계속]**&#x200B;을 선택하세요.

![연결 설정 작업 영역의 알림에서 검토 및 제출 보류 중인 제출되지 않은 변경 내용이 있음을 보여 줍니다.](/help/assets/connect/manage-connections/continue-editing-connection.png){zoomable="yes"}
