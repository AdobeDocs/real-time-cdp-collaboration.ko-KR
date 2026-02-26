---
title: 데이터 연결 관리
description: Real-Time CDP Collaboration의 일치 키, 예약, 사용 사례 및 대상 필터링을 포함하여 데이터 연결을 관리하는 방법을 알아봅니다
audience: administrator, data engineer
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: d142d3ed-f56a-4150-a885-571728a73ac8
source-git-commit: 46d2596bd0ccdc5da32067493968945c61f8acc4
workflow-type: tm+mt
source-wordcount: '1132'
ht-degree: 5%

---

# 데이터 연결 관리

{{limited-availability-release-note}}

## 개요

Real-Time CDP Collaboration의 데이터 연결을 사용하여 다양한 플랫폼에서 대상을 소스화할 수 있습니다. 기존 데이터 연결에 대해 일치 키를 관리하고 데이터 새로 고침을 예약하는 방법에 대해 알아봅니다. 또한 다양한 속성으로 대상자를 필터링하여 보다 세부적인 통찰력을 얻을 수 있습니다.

## 데이터 연결 보기

기존 데이터 연결을 보려면 **[!UICONTROL 설정]**(으)로 이동한 다음 **[!UICONTROL 내 데이터 연결]** 탭을 선택하십시오. 모든 현재 데이터 연결이 표시되어 각 연결에 대한 간략한 개요를 보여 줍니다. 일치 키, 예약 세부 정보 및 대상을 포함하여 데이터 연결 정보를 모두 보려면 해당 연결에서 **[!UICONTROL 데이터 연결 보기]**&#x200B;를 선택하십시오.

![내 데이터 연결 탭 보기가 표시되고 강조 표시된 작업 영역을 설정합니다.](/help/assets/setup/manage-data-connection/my-data-connections.png){zoomable="yes"}

### 일치 키 {#match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_matchkeys"
>title="일치 키"
>abstract="일치 키는 다양한 소스의 데이터를 어떻게 일치시킬지 결정합니다. 아래에 표시된 일치 키는 소스 필드를 매핑한 대상 필드입니다."

일치 키는 [소스 필드를 &#x200B;](./onboard-audiences.md#map-fields)에 매핑한 대상 필드입니다. 일치 키가 작동하는 방법에 대한 자세한 내용은 [일치 키](./onboard-account.md#set-up-match-keys) 안내서를 참조하세요.

![일치 키 섹션이 강조 표시된 데이터 연결 작업 영역입니다.](/help/assets/setup/manage-data-connection/view-data-connection-match-keys.png){zoomable="yes"}

### 일정 조정 {#scheduling}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_scheduling"
>title="일정 조정"
>abstract="데이터 연결에 대한 예약 세부 사항을 보고 필요한 경우 구성을 편집합니다."

데이터 연결에 대한 예약 설정을 보고 관리합니다. 예약은 대상을 새로 고치는 빈도를 결정합니다.

데이터 연결이 만들어지면 데이터 연결 작업 영역의 **[!UICONTROL 예약]** 섹션에서 바로 새로 고침 빈도, 시작 날짜 및 종료 날짜를 업데이트할 수 있습니다.

>[!NOTE]
>
>Adobe Experience Platform에서 대상을 소싱할 때 데이터 연결이 설정된 후 24시간 내에 대상을 사용할 수 있습니다. 초기 소싱 후 대상 데이터는 정의된 빈도에 따라 새로 고쳐집니다.

예약에 대한 자세한 내용은 대상자 구성 안내서에서 [예약 섹션](/help/guide/setup/onboard-audiences.md#schedule)을 참조하십시오.

![일정 섹션이 강조 표시된 데이터 연결의 작업 영역입니다.](/help/assets/setup/manage-data-connection/view-data-connection-scheduling.png){zoomable="yes"}

## 데이터 연결 편집 {#edit-data-connection}

기존 데이터 연결의 일치 키 및 예약 설정을 업데이트하는 방법에 대해 알아보려면 다음 섹션을 참조하십시오.

### 일치 키 편집 {#edit-match-keys}

>[!IMPORTANT]
>
>데이터 연결에 대한 일치 키를 편집하기 전에 다음을 참고하십시오.
>
>* 계정에 대해 구성된 일치 키만 데이터 연결에 사용할 수 있습니다.
>* 이때 데이터 연결에 일치 키를 추가할 수 있지만 일치 키가 활성화되면 제거할 수 없습니다.

**[!UICONTROL 키 일치]** 섹션에서 **[!UICONTROL 편집]**&#x200B;을(를) 선택합니다.

![편집 옵션이 강조 표시된 키 일치 섹션.](/help/assets/setup/manage-data-connection/edit-match-keys.png){zoomable="yes"}

데이터 연결에 대한 모든 변경 사항이 연결된 모든 대상에 적용됨을 설명하는 확인 대화 상자가 나타납니다. **[!UICONTROL 확인]**&#x200B;을(를) 선택하여 확인합니다. 나중에 이 확인을 건너뛰도록 선택할 수 있습니다.

![데이터 연결에 대한 변경 내용이 연결된 모든 대상에 적용됨을 보여 주는 확인 대화 상자입니다.](/help/assets/setup/manage-data-connection/confirm-data-connection-changes.png){zoomable="yes"}

**[!UICONTROL 일치 키]** 대화 상자에서 원본 필드와 해당 대상 필드(일치 키) 간의 기존 매핑을 볼 수 있습니다. 매핑된 소스 필드를 업데이트하여 일치 키를 편집하거나 추가 매핑 필드 행을 추가하여 새 일치 키를 채울 수 있습니다.

![원본 필드와 해당 대상 필드 간의 기존 매핑을 보여 주는 일치 키 대화 상자입니다.](/help/assets/setup/manage-data-connection/match-keys-dialog.png){zoomable="yes"}

#### 일치 키 추가 {#add-match-keys}

새 필드 행을 추가하려면 **[!UICONTROL 필드 추가]**&#x200B;를 선택하십시오.

![필드 추가를 선택하면 [키 일치] 대화 상자에 입력할 수 있는 비어 있는 새 매핑 필드가 표시됩니다.](/help/assets/setup/manage-data-connection/add-new-field.png){zoomable="yes"}

그런 다음 빈 소스 필드를 선택합니다. **[!UICONTROL 원본 필드 선택]** 대화 상자에 **[!UICONTROL ID 네임스페이스]** 및 **[!UICONTROL 프로필 특성]** 옵션이 표시됩니다. 목록을 필터링하고 검색 옵션을 사용하여 원하는 소스 필드를 찾을 수 있습니다.

원하는 소스 필드를 선택한 후 **[!UICONTROL 선택]**&#x200B;을(를) 선택하십시오.

![GAID 옵션이 선택된 소스 필드 선택 대화 상자입니다.](/help/assets/setup/manage-data-connection/select-source-field.png){zoomable="yes"}

**[!UICONTROL 키 일치]** 대화 상자에서 드롭다운 메뉴를 사용하여 새 소스 필드를 대상 필드에 매핑합니다. 사용 가능한 모든 대상 필드는 Collaborator 계정에 대해 구성된 일치 키입니다. 필요한 대상 필드가 없으면 [계정의 일치 키를 편집](./onboard-account.md#edit-match-keys)하여 추가하십시오.

**[!UICONTROL 해시된 이메일]** 대상 필드에 일반 텍스트 이메일 소스 필드를 매핑할 때와 같이 해시되지 않은 필드를 해시된 대상 필드에 소싱하려면 **[!UICONTROL 변환 적용]** 옵션을 사용하십시오.

![드롭다운 메뉴에 사용 가능한 모든 대상 필드가 표시되어 새 원본 필드와 매핑됩니다.](/help/assets/setup/manage-data-connection/select-target-field.png){zoomable="yes"}

필드 매핑을 완료한 후 업데이트를 검토하고 **[!UICONTROL 확인]**&#x200B;을 선택하여 변경 내용을 적용합니다.

![확인 옵션이 강조 표시된 업데이트된 필드 매핑을 표시하는 키 일치 대화 상자입니다.](/help/assets/setup/manage-data-connection/review-and-confirm.png){zoomable="yes"}

확인 대화 상자에서 일치 키가 성공적으로 업데이트되었는지 확인합니다.

### 예약 편집 {#edit-scheduling}

데이터 연결이 만들어지면 데이터 연결 작업 영역의 **[!UICONTROL 예약]** 섹션에서 바로 새로 고침 빈도, 시작 날짜 및 종료 날짜를 업데이트할 수 있습니다.

기존 데이터 연결의 빈도를 편집하여 대상을 새로 고치는 빈도를 더 잘 제어할 수 있습니다. 일정을 편집하려면 일정 카드의 데이터 연결에서 **[!UICONTROL 편집]**&#x200B;을 선택하세요.

![편집 옵션이 강조 표시된 예약 섹션입니다.](/help/assets/setup/manage-data-connection/edit-scheduling.png){zoomable="yes"}

데이터 연결에 대한 모든 변경 사항이 연결된 모든 대상에 적용됨을 설명하는 확인 대화 상자가 나타납니다. **[!UICONTROL 확인]**&#x200B;을(를) 선택하여 확인합니다. 나중에 이 확인을 건너뛰도록 선택할 수 있습니다.

![데이터 연결에 대한 변경 내용이 연결된 모든 대상에 적용됨을 보여 주는 확인 대화 상자입니다.](/help/assets/setup/manage-data-connection/confirm-data-connection-changes.png){zoomable="yes"}

**[!UICONTROL 예약]** 대화 상자에서 드롭다운 메뉴를 선택하여 **[!UICONTROL 빈도]**&#x200B;를 업데이트합니다. 새로 고침 빈도를 매일 또는 2~6일마다 실행되도록 설정합니다.

![빈도 드롭다운이 확장된 예약 대화 상자에서 대상 새로 고침 빈도 옵션을 표시합니다.](../../assets/setup/manage-data-connection/edit-frequency.png){zoomable="yes"}

그런 다음 대상자가 채워지고 새로 고쳐지는 기간을 업데이트하려면 **[!UICONTROL 날짜 범위]**&#x200B;를 선택하십시오.

![대상 모집단과 새로 고침의 시작 날짜와 종료 날짜를 편집하기 위해 날짜 범위 드롭다운을 표시하는 예약 대화 상자가 확장되었습니다.](../../assets/setup/manage-data-connection/edit-date-range.png){zoomable="yes"}

완료되면 업데이트를 검토하고 **[!UICONTROL 저장]**&#x200B;을 선택하여 변경 내용을 적용합니다.

![업데이트 및 저장 옵션을 강조 표시하는 예약 대화 상자](../../assets/setup/manage-data-connection/scheduling-dialog.png){zoomable="yes"}

## 데이터 연결 삭제

데이터 연결을 삭제하면 Collaboration에서 모든 기본 대상, 관련 설정 및 사용이 제거됩니다. 이 작업은 실행 취소할 수 없습니다.

기존 데이터 연결을 삭제하려면 개별 데이터 연결의 작업 영역에서 삭제 아이콘(![삭제 아이콘](/help/assets/common/delete.svg))을 선택하십시오.

![삭제 옵션이 강조 표시된 데이터 연결 작업 영역입니다.](/help/assets/setup/manage-data-connection/delete-data-connection.png){zoomable="yes"}

확인 대화 상자가 나타납니다. 데이터 연결 삭제를 완료하려면 **[!UICONTROL 삭제]**&#x200B;을(를) 선택하십시오.

![삭제 옵션이 강조 표시된 데이터 연결 삭제 대화 상자입니다.](/help/assets/setup/manage-data-connection/delete-data-connection-confirm.png){zoomable="yes"}

## 대상자 관리 {#manage-audiences}

데이터 연결에 첨부된 대상자 목록이 작업 영역 하단에 표시됩니다. 목록에는 상태, 소스 및 연결 액세스를 포함하여 각 대상에 대한 간략한 개요가 표시됩니다. 대상자의 카테고리, 연결 액세스 또는 메타데이터 가시성을 편집하려면 대상자의 이름을 선택합니다. 대상자 관리에 대한 전체 안내서는 [개별 대상자 보기](./onboard-audiences.md#view-individual-audiences) 안내서를 참조하십시오.

![대상이 강조 표시된 데이터 연결 작업 영역입니다.](/help/assets/setup/manage-data-connection/view-data-connection-manage-audiences.png){zoomable="yes"}

## 다음 단계

데이터 연결을 관리한 후 대상자와 공동 작업자가 검색할 수 있도록 만든 대상 간의 [겹침 검색](/help/guide/collaborate/discover.md)을 수행할 수 있습니다.
