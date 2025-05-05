---
title: 데이터 연결 관리
description: Real-Time CDP Collaboration의 일치 키, 예약, 사용 사례 및 대상 필터링을 포함하여 데이터 연결을 관리하는 방법을 알아봅니다
audience: administrator, data engineer
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/kr/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: d142d3ed-f56a-4150-a885-571728a73ac8
source-git-commit: acaaaa1e1fab981d874210639c16e76e48fc3394
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 17%

---

# 데이터 연결 관리

{{limited-availability-release-note}}

## 개요

Real-Time CDP Collaboration의 데이터 연결을 사용하여 다양한 소스에서 대상을 가져옵니다. 기존 데이터 연결에 대해 일치 키를 관리하고 데이터 가져오기를 예약하는 방법을 알아봅니다. 또한 다양한 속성으로 대상자를 필터링하여 보다 세부적인 통찰력을 얻을 수 있습니다.

여기에서 데이터 연결을 관리하려면 먼저 [대상자 온보딩 워크플로](./onboard-audiences.md) 동안 데이터 연결을 설정해야 합니다. 이렇게 하면 Real-Time CDP Collaboration에서 사용할 수 있도록 올바른 데이터 소스가 연결됩니다.

## 데이터 연결 보기

>[!IMPORTANT]
>
>데이터 연결 삭제는 현재 Real-Time CDP Collaboration 사용자 인터페이스에서 지원되지 않습니다. 데이터 연결을 삭제하려면 Adobe 담당자에게 연락하거나 [고객 지원 티켓을 만드십시오](https://experienceleague.adobe.com/home?lang=ko&amp;support-tab=open-ticket#support){target="_blank"}.

기존 데이터 연결을 보려면 **[!UICONTROL 설정]** > **[!UICONTROL 내 대상]**(으)로 이동한 다음 **[!UICONTROL 데이터 연결 관리]**&#x200B;를 선택하십시오.

![데이터 연결 관리가 강조 표시된 작업 영역을 설정합니다.](/help/assets/setup/manage-data-connection/manage-data-connection-highlighted.png){zoomable="yes"}

이렇게 하면 각 대상자 수, 데이터 연결 소스 등에 대한 정보가 포함된 현재 설정된 모든 데이터 연결 보기가 표시됩니다. 이 데이터 연결에 포함된 일치 키, 일정 및 대상에 대한 정보를 보려면 **[!UICONTROL 데이터 연결 보기]**&#x200B;를 선택하십시오.

![연결을 사용하여 데이터 연결 작업 영역 관리 ](/help/assets/setup/manage-data-connection/view-data-connection-highlighted.png){zoomable="yes"}

### 일치 키 {#match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_matchkeys"
>title="일치 키"
>abstract="일치 키는 다양한 소스의 데이터를 어떻게 일치시킬지 결정합니다. 본인의 사용 사례와 개인 정보 지침에 가장 적합한 일치 키를 선택합니다."

일치 키는 서로 다른 데이터 소스의 대상자 간에 멤버를 조정하는 데 사용되는 식별자입니다. 사용 가능한 일치 키는 다음과 같습니다.

- **해시된 이메일**

이 데이터 연결에 사용된 일치 키는 편집할 수 없습니다.

![일치 키 섹션이 강조 표시된 데이터 연결 작업 영역입니다.](/help/assets/setup/manage-data-connection/view-data-connection-match-keys.png){zoomable="yes"}

### 예약 {#scheduling}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_scheduling"
>title="예약"
>abstract="이 보기에는 데이터 연결에 대해 처음 선택한 일정 옵션이 표시됩니다."

데이터 연결을 위해 처음에 선택한 예약 옵션은 편집할 수 없습니다. 예약 옵션에 대한 자세한 내용은 대상 가져오기 워크플로 문서에서 [예약 섹션](/help/guide/setup/onboard-audiences.md#schedule)을(를) 참조하십시오.

![일정 섹션이 강조 표시된 데이터 연결 작업 영역입니다.](/help/assets/setup/manage-data-connection/view-data-connection-scheduling.png){zoomable="yes"}

## 대상자 관리 {#manage-audiences}

데이터 연결에서 대상자 목록을 볼 때 대상자를 보고, 해당 범주를 편집하거나, 데이터 연결에서 대상자를 제거하도록 선택할 수 있습니다.

![대상이 강조 표시된 데이터 연결 작업 영역입니다.](/help/assets/setup/manage-data-connection/view-data-connection-manage-audiences.png){zoomable="yes"}

## 다음 단계

데이터 연결을 관리한 후 대상자와 공동 작업자가 검색할 수 있도록 만든 대상 간의 [겹침 검색](/help/guide/collaborate/discover.md)을 수행할 수 있습니다.
