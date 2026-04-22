---
title: Collaboration [!DNL Starter] 온보딩에 대한 권한 제어 구성
description: Adobe Experience Cloud의 사용 권한을 사용하여 Adobe Real-Time CDP Collaboration [!DNL Starter] 에 대한 사용 권한을 구성하는 방법에 대해 알아봅니다.
audience: users invited to Real-Time CDP Collaboration [!DNL Starter]
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 4e50b6cc-58f7-4a0c-8b6d-f5aa4f092e9f
source-git-commit: 147fd5847bc5074e4b4f8a05a9a1c3afc089be56
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 4%

---

# Collaboration [!DNL Starter] 온보딩에 대한 권한 제어 구성

Adobe Experience Platform 제품에 대한 관리자 및 사용자 액세스 권한을 설정한 후에는 Real-Time CDP Collaboration에 대한 적절한 권한이 있는 사용자 자신의 역할을 할당해야 합니다. Collaboration 기능에 액세스하고 관리할 수 있도록 Experience Cloud 권한 인터페이스를 통해 계정에 올바른 역할을 추가하는 방법을 배우려면 이 안내서를 참조하십시오.

Collaboration 리소스에 포함된 표준 역할 및 사용 가능한 권한에 대한 자세한 내용은 [역할 관리 방법 안내서](../permissions/manage-roles.md)를 참조하세요.

## 전제 조건 {#prerequisites}

Adobe Experience Platform 제품에 대해 **관리자 권한**&#x200B;과 **사용자 액세스 권한**&#x200B;이 모두 있는지 확인하십시오. 이러한 액세스 수준을 아직 설정하지 않은 경우 [관리자 액세스 안내서](./starter-admin-access.md)에서 단계별 지침을 참조하십시오.

## 권한 설정 {#setup-permissions}

Collaboration에 필요한 권한을 설정하려면 아래 단계를 따르십시오. 먼저 자격 증명을 사용하여 [Adobe Experience Cloud](https://experience.adobe.com/)에 로그인합니다.

### 액세스 권한 {#access-permissions}

로그인한 후 **[!UICONTROL 빠른 액세스]** 섹션으로 이동하여 **[!UICONTROL 권한]**&#x200B;을 선택하십시오. 필요한 역할을 직접 할당할 수 있는 권한 대시보드가 열립니다.

![빠른 액세스 섹션 내에서 사용 권한이 강조 표시된 Experience Cloud 홈 페이지.](../../assets/setup/starter/access-permissions.png){zoomable="yes"}

### 사용자 선택 {#select-user}

**[!UICONTROL 권한]** 대시보드의 왼쪽 패널에서 **[!UICONTROL 사용자]**&#x200B;를 선택합니다. 그런 다음 사용자 테이블에서 계정을 선택합니다.

>[!NOTE]
>
> 조직에서 Experience Platform에 처음 액세스하는 사용자는 **사용자** 표에 나열된 유일한 사용자일 수 있습니다. 추가 팀원을 초대하려면 [사용자 액세스 구성 안내서](../permissions/manage-user-access.md#administrators-configure-user-access-to-experience-platform)의 단계를 따르십시오.

![권한 대시보드에 사용자 계정이 강조 표시된 사용자 테이블이 표시됩니다.](../../assets/setup/starter/select-user.png){zoomable="yes"}

### 역할 할당 {#assign-roles}

해당 **[!UICONTROL 사용자]** 작업 영역에서 **[!UICONTROL 역할]** 탭으로 이동합니다. **[!UICONTROL 역할 추가]**&#x200B;를 선택합니다.

![해당 사용자 작업 영역에 [역할 추가] 옵션이 강조 표시된 [역할] 탭이 표시됩니다.](../../assets/setup/starter/add-roles.png){zoomable="yes"}

**[!UICONTROL 역할 추가]** 대화 상자에 사용 가능한 역할 테이블이 표시됩니다. 테이블의 각 행은 다음 정보가 있는 역할을 나타냅니다.

| **열** | **설명** |
|---------------|--------------------------------------------------------|
| **이름** | 역할의 이름입니다. |
| **설명** | 역할의 기능에 대한 간단한 요약입니다. 읽기 전용 역할은 사용자 정의할 수 없습니다. |
| **샌드박스** | 역할이 액세스를 제공하는 샌드박스(예: `Prod`)를 지정합니다. |
| **수정됨** | 역할을 마지막으로 업데이트한 날짜입니다. |

{style="table-layout:auto"}

특정 역할 및 해당 권한에 대한 자세한 개요는 [역할에 대한 권한 관리](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/abac/permissions-ui/permissions) 안내서를 참조하십시오.

정보를 검토하고 계정에 할당할 역할을 선택합니다. 완료되면 **[!UICONTROL 저장]**&#x200B;을 선택합니다.

![역할 추가 대화 상자에 선택한 역할과 저장 옵션이 강조 표시됩니다.](../../assets/setup/starter/add-roles-dialog.png){zoomable="yes"}

확인 대화 상자에서 새 역할이 추가되었음을 확인합니다.

사용 권한이 올바르게 설정되었는지 확인하려면 [Experience Cloud](https://experience.adobe.com/) 홈 페이지로 돌아가십시오. **[!UICONTROL 빠른 액세스]** 내에서 **[!UICONTROL Real-Time CDP Collaboration]**&#x200B;을(를) 선택하십시오. Collaboration 작업 영역에 액세스하고 [!DNL Starter] 계정에 사용할 수 있는 기능을 사용할 수 있어야 합니다.

## 다음 단계 {#next-steps}

사용 권한이 설정되면 Collaboration에 액세스할 수 있습니다. 다음으로, 다음과 같은 작업을 수행할 수 있습니다.

* [다양한 액세스 수준을 관리하기 위해 특정 권한으로 사용자 지정 역할을 만듭니다](../permissions/manage-roles.md#create-specific-access-roles).
* [사용 권한의 한 역할에 여러 사용자를 할당](../permissions/manage-user-access.md#assign-a-role).
* [Collaboration 계정을 설정하고 초대 공동 작업자와 연결을 설정합니다](../overview/starter-overview.md#set-up-connections).
* [Collaboration의 신용 사용 및 소비에 대해 자세히 알아보세요 [!DNL Starter]](./starter-credit-usage.md).

Real-Time CDP Collaboration 및 주요 기능에 대한 전체 개요를 보려면 [개요 안내서](../home.md)를 읽어 보십시오.
