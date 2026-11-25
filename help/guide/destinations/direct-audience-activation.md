---
title: 직접 대상 활성화(1P Audience Activation) - Beta
description: 프로젝트 없이 자체 또는 공유 자사 대상을 활성화하고, 대상을 선택하고, 필드 매핑을 검토하고, 활성화 일정을 설정하는 방법을 알아봅니다.
badgeBeta: label="Beta" type="Informative"
source-git-commit: 5f823194a18468b9205f64853551719ae8a3752f
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 1%
---

# 직접 대상자 활성화(1P Audience Activation) {#activate-audiences-directly}

[!DNL Adobe Real-Time CDP Collaboration]에서 직접 자사(1P) 대상 활성화를 사용하여 프로젝트를 만들지 않고 대상을 대상으로 보냅니다. 자신이 소유한 대상자 또는 자신과 공유한 대상자를 활성화하여 자사 용도로 사용할 수 있습니다.

구성된 대상 또는 **[!UICONTROL 활성화된 대상]**&#x200B;에서 시작한 다음 대상을 선택하고 활성화 일정을 설정합니다.

공동 작업 프로젝트를 통해 대상자를 보내고 활성화하려면 [프로젝트에서 대상자 보내기 및 활성화](/help/guide/collaborate/activate.md)를 참조하십시오.

## 활성화를 위한 대상자 액세스 {#audience-access-for-activation}

활성화 전에 부여가 필요한지 여부를 결정하려면 대상 소스를 확인하십시오.

| 대상자 소스 | 액세스 요구 사항 |
| --- | --- |
| 자신의 대상자 | 사용자가 대상자를 소유합니다. |
| 나와 공유된 대상자 | 직접 활성화 권한이 있는 활성 부여가 필요합니다. 제공자는 소유권을 유지합니다. |

{style="table-layout:auto"}

가상 대상 부여를 사용하면 데이터를 이동하지 않고도 참조를 통해 공유 대상에 액세스할 수 있습니다. 그런 다음 대상을 활성화하여 선택한 대상에 데이터를 전송할 수 있습니다.

권한 부여 및 공급자 제어에 대한 자세한 내용은 [가상 대상 액세스(대상 권한 부여)](/help/guide/setup/virtual-audience-access.md)를 참조하십시오.

## 사전 요구 사항 {#prerequisites}

시작하기 전에 다음을 확인합니다.

* 귀하가 보유하거나 자격을 갖춘 자사(1P) 부여를 통해 공유한 대상자.
* 직접 활성화를 지원하고 사용자가 제어하는 구성된 대상입니다.
* 대상에 대해 하나 이상의 일치 키 필드 매핑.

공유 대상을 활성화하려면 활성 연결 범위 부여가 [자격 조건](#check-shared-audience-access)을 충족하는지 확인하십시오. **[!UICONTROL 활성화]** 작업 영역을 사용합니다. 프로젝트가 필요하지 않습니다.

### 공유 대상자 자격 요건 {#check-shared-audience-access}

권한 부여는 직접 활성화를 지원하기 위한 각 조건을 충족해야 합니다.

| 요구 사항 | 조건 |
| --- | --- |
| 대상자 권한 | 부여에는 직접 활성화 권한이 포함됩니다. |
| 액세스 기간 | 부여가 무기한으로 또는 지정된 날짜 범위 내에서 활성 상태입니다. |

{style="table-layout:auto"}

별도의 **[!UICONTROL 새 대상 만들기]** 권한을 사용하면 공유 대상을 집단 대상 만들기에 사용할 수 있습니다. 직접 활성화에는 이 권한이 필요하지 않습니다.

### 대상 필드 매핑 {#review-destination-field-mappings}

직접 활성화는 대상에 대해 구성된 일치 키 매핑을 사용합니다. 활성화 중에는 일치 키를 선택하지 않습니다.

대상을 구성하려면 [대상 개요](../destinations/overview.md)를 참조하십시오.

## 직접 활성화 시작 {#start-direct-activation}

구성된 대상 또는 활성화된 대상자 목록에서 시작합니다. Adobe Experience Platform 대상은 자사 활성화를 지원하지 않습니다.

### 대상에서 시작 {#start-from-a-destination}

대상을 선택한 상태로 워크플로우를 열려면 구성된 대상에서 시작합니다. 먼저 **[!UICONTROL 활성화]** 작업 영역을 열고 **[!UICONTROL 대상]**&#x200B;을 선택합니다.

그런 다음 사용할 대상에 대한 작업에서 **[!UICONTROL 대상자 활성화]**&#x200B;를 선택합니다.

대상이 선택된 상태로 워크플로우가 열립니다. 그런 다음 [활성화를 구성](#configure-the-activation)합니다.

### 활성화된 대상자에서 시작 {#start-from-activated-audiences}

워크플로우에서 대상을 선택하려면 활성화된 대상자 목록에서 시작하십시오. 먼저 **[!UICONTROL 활성화]** 작업 영역을 열고 **[!UICONTROL 활성화된 대상]**&#x200B;을 선택합니다.

다음으로 페이지에서 **[!UICONTROL 대상자 활성화]**&#x200B;를 선택하거나 추가 아이콘(![대상자 활성화를 추가](/help/assets/icons/plus.png))을 선택하여 워크플로우를 시작합니다. **[!UICONTROL 대상자를 활성화]**&#x200B;합니다.

대상이 선택되지 않은 상태로 워크플로우가 열립니다. 그런 다음 [활성화를 구성](#configure-the-activation)합니다.

## 활성화 구성 {#configure-the-activation}

자체 대상자 또는 사용자와 공유된 대상자에서 활성화당 한 명의 대상자를 선택합니다. 미리 선택된 대상을 사용하거나, 선택된 대상이 없는 경우 구성된 대상을 선택합니다. 워크플로는 해당 대상에 대해 구성된 [기존 매핑](#review-destination-field-mappings)을(를) 적용합니다.

활성화 실행 시기를 선택한 다음, 제출하기 전에 선택한 대상자, 대상 및 일정을 검토하십시오.

## 변경 사항 및 예약된 실행에 액세스 {#access-changes-and-scheduled-runs}

공급자가 액세스 권한을 부여하는 동안에만 공유 대상을 활성화합니다.

| 액세스 변경 | 효과 |
| --- | --- |
| 부여가 만료됨 | 시스템은 시간별로 만료를 처리합니다. 만료가 처리된 후 수신자는 가상 대상자 액세스 권한을 잃게 됩니다. |
| 제공자는 부여를 취소합니다 | 수신자는 즉시 가상 대상자 액세스 권한을 잃게 됩니다. |
| 예약된 활성화가 실행됩니다 | 시스템이 부여를 확인합니다. 취소되거나 만료된 부여가 있는 대상은 활성화할 수 없습니다. |

{style="table-layout:auto"}

만료 또는 취소는 대상에 이미 전달된 대상 데이터를 제거하지 않습니다.

## 다음 단계 {#next-steps}

대상을 활성화한 후 이러한 안내서를 사용하여 대상 또는 공동 작업자 연결을 관리합니다.

* [대상 구성 및 관리](/help/guide/destinations/manage-destinations.md)
* [Collaborator 연결 관리](/help/guide/connect/manage-connections.md)
