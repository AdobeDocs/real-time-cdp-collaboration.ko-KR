---
title: 데이터 연결 관리
description: Real-Time CDP Collaboration의 일치 키, 예약, 사용 사례 및 대상 필터링을 포함하여 데이터 연결을 관리하는 방법을 알아봅니다
audience: administrator, data engineer
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: d142d3ed-f56a-4150-a885-571728a73ac8
source-git-commit: dd1386f9371cb40285315d11e07b139d3115e147
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 16%

---

# 데이터 연결 관리

{{limited-availability-release-note}}

## 개요

Real-Time CDP Collaboration의 데이터 연결을 사용하여 다양한 소스에서 대상을 가져옵니다. 기존 데이터 연결에 대해 일치 키를 관리하고 데이터 가져오기를 예약하는 방법을 알아봅니다. 또한 다양한 속성으로 대상자를 필터링하여 보다 세부적인 통찰력을 얻을 수 있습니다.

## 데이터 연결 보기

기존 데이터 연결을 보려면 **[!UICONTROL 설정]**(으)로 이동한 다음 **[!UICONTROL 내 데이터 연결]** 탭을 선택하십시오. 모든 현재 데이터 연결이 표시되어 각 연결에 대한 간략한 개요를 보여 줍니다. 일치 키, 예약 세부 정보 및 대상을 포함하여 데이터 연결 정보를 모두 보려면 해당 연결에서 **[!UICONTROL 데이터 연결 보기]**&#x200B;를 선택하십시오.

![내 데이터 연결 탭 보기가 표시되고 강조 표시된 작업 영역을 설정합니다.](/help/assets/setup/manage-data-connection/my-data-connections.png){zoomable="yes"}

### 일치 키 {#match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_matchkeys"
>title="일치 키"
>abstract="일치 키는 다양한 소스의 데이터를 어떻게 일치시킬지 결정합니다. 본인의 사용 사례와 개인 정보 지침에 가장 적합한 일치 키를 선택합니다."

일치 키는 서로 다른 데이터 소스의 대상자 간에 멤버를 조정하는 데 사용되는 식별자입니다. 데이터 연결을 위해 처음에 선택한 일치 키는 편집할 수 없습니다.

사용 가능한 일치 키는 다음과 같습니다.

- **해시된 이메일**

![일치 키 섹션이 강조 표시된 데이터 연결 작업 영역입니다.](/help/assets/setup/manage-data-connection/view-data-connection-match-keys.png){zoomable="yes"}

### 예약 {#scheduling}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_scheduling"
>title="예약"
>abstract="이 보기에는 데이터 연결에 대해 처음 선택한 일정 옵션이 표시됩니다."

데이터 연결을 위해 처음에 선택한 예약 옵션은 편집할 수 없습니다. 예약 옵션에 대한 자세한 내용은 대상 가져오기 워크플로 문서에서 [예약 섹션](/help/guide/setup/onboard-audiences.md#schedule)을(를) 참조하십시오.

![일정 섹션이 강조 표시된 데이터 연결 작업 영역입니다.](/help/assets/setup/manage-data-connection/view-data-connection-scheduling.png){zoomable="yes"}

## 데이터 연결 삭제

데이터 연결을 삭제하면 플랫폼에서 모든 기본 대상, 관련 설정 및 사용이 제거됩니다. 이 작업은 취소할 수 없습니다.

기존 데이터 연결을 삭제하려면 개별 데이터 연결의 작업 영역에서 삭제 아이콘(![삭제 아이콘](/help/assets/common/delete.svg))을 선택하십시오.

![삭제 옵션이 강조 표시된 데이터 연결 작업 영역입니다.](/help/assets/setup/manage-data-connection/delete-data-connection.png){zoomable="yes"}

확인 대화 상자가 나타납니다. 데이터 연결 삭제를 완료하려면 **[!UICONTROL 삭제]**&#x200B;을(를) 선택하십시오.

![삭제 옵션이 강조 표시된 데이터 연결 삭제 대화 상자입니다.](/help/assets/setup/manage-data-connection/delete-data-connection-confirm.png){zoomable="yes"}

## 대상자 관리 {#manage-audiences}

데이터 연결에 첨부된 대상자 목록이 작업 영역 하단에 표시됩니다. 이 목록에는 상태, 소스 및 연결 액세스를 포함하여 각 대상에 대한 간략한 개요가 표시됩니다. 대상자의 카테고리, 연결 액세스 또는 메타데이터 가시성을 편집하려면 대상자의 이름을 선택합니다. 대상자 관리에 대한 전체 안내서는 [개별 대상자 보기](./onboard-audiences.md#view-individual-audiences) 안내서를 참조하십시오.

![대상이 강조 표시된 데이터 연결 작업 영역입니다.](/help/assets/setup/manage-data-connection/view-data-connection-manage-audiences.png){zoomable="yes"}

## 다음 단계

데이터 연결을 관리한 후 대상자와 공동 작업자가 검색할 수 있도록 만든 대상 간의 [겹침 검색](/help/guide/collaborate/discover.md)을 수행할 수 있습니다.
