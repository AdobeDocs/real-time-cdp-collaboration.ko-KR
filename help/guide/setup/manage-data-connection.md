---
title: 데이터 연결 관리
description: Real-Time CDP Collaboration의 일치 키, 예약, 사용 사례 및 대상 필터링을 포함하여 데이터 연결을 관리하는 방법을 알아봅니다
audience: administrator, data engineer
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: d142d3ed-f56a-4150-a885-571728a73ac8
source-git-commit: c76259c1a5a684e69e4b5ac8bfdecc9026fe0939
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 10%

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

일치 키는 [소스 필드를 ](./onboard-audiences.md#map-fields)에 매핑한 대상 필드입니다. 데이터 연결을 위해 처음에 선택한 일치 키는 편집할 수 없습니다. 일치 키를 업데이트하려면 새 데이터 연결을 만들어야 합니다. 일치 키가 작동하는 방법에 대한 자세한 내용은 [일치 키](./onboard-account.md#set-up-match-keys) 안내서를 참조하세요.

![일치 키 섹션이 강조 표시된 데이터 연결 작업 영역입니다.](/help/assets/setup/manage-data-connection/view-data-connection-match-keys.png){zoomable="yes"}

### 예약 {#scheduling}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_scheduling"
>title="예약"
>abstract="데이터 연결에 대한 일정 세부 정보를 보고, 필요한 경우 새로 고침 빈도를 편집합니다."

데이터 연결에 대한 예약 설정을 보고 관리합니다. 예약은 대상을 새로 고치는 빈도를 결정합니다.

데이터 연결이 만들어지면 데이터 연결 작업 영역의 **[!UICONTROL 예약]** 섹션에서 바로 새로 고침 빈도를 업데이트할 수 있습니다.

>[!NOTE]
>
>Adobe Experience Platform에서 대상을 소싱할 때 데이터 연결이 설정된 후 24시간 내에 대상을 사용할 수 있습니다. 초기 소싱 후 대상 데이터는 정의된 빈도에 따라 새로 고쳐집니다.

예약에 대한 자세한 내용은 대상자 구성 안내서에서 [예약 섹션](/help/guide/setup/onboard-audiences.md#schedule)을 참조하십시오.

![일정 섹션이 강조 표시된 데이터 연결의 작업 영역입니다.](/help/assets/setup/manage-data-connection/view-data-connection-scheduling.png){zoomable="yes"}

#### 예약 편집 {#edit-scheduling}

기존 데이터 연결의 빈도를 편집하여 대상을 새로 고치는 빈도를 더 잘 제어할 수 있습니다. 일정을 편집하려면 일정 카드의 데이터 연결에서 **[!UICONTROL 편집]**&#x200B;을 선택하세요.

예약은 데이터 연결에서 가져온 모든 대상에 영향을 줍니다.

**[!UICONTROL 예약]** 대화 상자에서 드롭다운 메뉴를 선택하여 **[!UICONTROL 빈도]**&#x200B;를 업데이트합니다. 새로 고침 빈도를 매일 또는 2~6일마다 실행되도록 설정합니다. 완료되면 **[!UICONTROL 저장]**&#x200B;을 선택하여 변경 내용을 적용합니다.

![예약 대화 상자, 빈도 및 날짜 범위를 설정하는 옵션을 표시합니다.](../../assets/setup/manage-data-connection/scheduling-dialog.png){zoomable="yes"}

## 데이터 연결 삭제

데이터 연결을 삭제하면 Collaboration에서 모든 기본 대상, 관련 설정 및 사용이 제거됩니다. 이 작업은 취소할 수 없습니다.

기존 데이터 연결을 삭제하려면 개별 데이터 연결의 작업 영역에서 삭제 아이콘(![삭제 아이콘](/help/assets/common/delete.svg))을 선택하십시오.

![삭제 옵션이 강조 표시된 데이터 연결 작업 영역입니다.](/help/assets/setup/manage-data-connection/delete-data-connection.png){zoomable="yes"}

확인 대화 상자가 나타납니다. 데이터 연결 삭제를 완료하려면 **[!UICONTROL 삭제]**&#x200B;을(를) 선택하십시오.

![삭제 옵션이 강조 표시된 데이터 연결 삭제 대화 상자입니다.](/help/assets/setup/manage-data-connection/delete-data-connection-confirm.png){zoomable="yes"}

## 대상자 관리 {#manage-audiences}

데이터 연결에 첨부된 대상자 목록이 작업 영역 하단에 표시됩니다. 목록에는 상태, 소스 및 연결 액세스를 포함하여 각 대상에 대한 간략한 개요가 표시됩니다. 대상자의 카테고리, 연결 액세스 또는 메타데이터 가시성을 편집하려면 대상자의 이름을 선택합니다. 대상자 관리에 대한 전체 안내서는 [개별 대상자 보기](./onboard-audiences.md#view-individual-audiences) 안내서를 참조하십시오.

![대상이 강조 표시된 데이터 연결 작업 영역입니다.](/help/assets/setup/manage-data-connection/view-data-connection-manage-audiences.png){zoomable="yes"}

## 다음 단계

데이터 연결을 관리한 후 대상자와 공동 작업자가 검색할 수 있도록 만든 대상 간의 [겹침 검색](/help/guide/collaborate/discover.md)을 수행할 수 있습니다.
