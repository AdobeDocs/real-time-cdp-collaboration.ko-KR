---
title: 권한을 통해 역할 관리
description: Real-Time CDP Collaboration UI 내의 다양한 구성 요소에 대한 액세스를 제공하는 사용 가능한 모든 역할 리소스를 이해합니다.
audience: admin
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 59cf5bf2-421b-4ebc-beab-30eafb098649
TQID: https://experienceleague.adobe.com/dB7nEQtEGG8PvCSE7eDDelH-ml2EhKOQ8ovvGXG1Ejg
product_v2: id: fdddec33-c9cb-4459-b8b6-2664395a6f10
feature_v2: id: ba929a52-9339-4154-9487-317dc875a3c7
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: c1579802-ddd4-4214-8a91-97b2066abe11id: c2be0313-b3ae-45e0-b454-d20bf54b23f2id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 3ce7e66b31332836fd6cc6137c94622436505cc9
workflow-type: tm+mt
source-wordcount: 623
ht-degree: 3%

---

# 역할 관리 {#manage-roles}

{{limited-availability-release-note}}

Adobe Real-Time CDP Collaboration UI의 다양한 구성 요소에 대한 사용자 액세스를 관리하기 위해 [관리자](./manage-user-access.md#system-admin-gain-access)는 역할을 정의하고 할당할 수 있습니다. 역할은 관리자 또는 사용자가 조직의 [리소스](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/home#permissions){target="_blank"}에 대한 액세스 권한을 정의합니다. 이 안내서에서는 Real-Time CDP Collaboration에서 제공하는 표준 역할과 사용자 지정 역할에 할당할 수 있는 개별 권한에 대한 정보를 제공합니다.

역할 관리를 시작하려면 관리자가 Experience Platform 제품에 액세스해야 합니다. 관리 액세스 권한 획득 또는 Experience Platform 액세스 권한에 대한 자세한 내용은 [사용자 액세스 관리](./manage-user-access.md#manage-user-access-through-permissions) 안내서를 참조하십시오.

## 표준 역할 {#standard-roles}

두 가지 공통 액세스 제어 사용 사례를 채우는 두 가지 표준 역할이 제공됩니다. 이는 사용자 정의할 수 없음을 의미하는 &quot;읽기 전용&quot; 역할입니다.

| 역할 이름 | 역할 설명 | 권한 |
| --- | --- | --- |
| Collaboration 관리자 | 15개의 모든 권한을 포함하는 모든 액세스 권한입니다. 이를 통해 사용자는 모든 데이터를 읽고, 만들고, 편집할 수 있습니다. 또한 Experience Platform의 **[!UICONTROL Prod]** 샌드박스에 액세스할 수 있으므로 대상을 Real-Time CDP Collaboration으로 가져올 수 있습니다. | 모두 아래 표에서 가져온 것입니다. |
| Collaboration 뷰어 | 읽기 전용 액세스 권한입니다. 사용자는 데이터, 활동, 연결 등을 읽고 검색할 수 있습니다. 또한 Experience Platform의 **[!UICONTROL Prod]** 샌드박스에 액세스할 수 있으므로 대상을 Real-Time CDP Collaboration으로 가져올 수 있습니다. | 아래 표의 모든 읽기 권한입니다. |

{style="table-layout:auto"}

## 특정 액세스 역할 만들기 {#specific-access-roles}

다양한 사용자에게 다양한 수준의 액세스 권한을 제공하기 위해 추가 역할을 만들 수 있습니다. 역할을 만들 때 **[!UICONTROL 공동 작업]** 리소스 내에서 특정 권한을 선택하여 다양한 액세스 수준을 관리할 수 있습니다. 역할을 만들고 관리하는 방법은 [역할](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/abac/permissions-ui/roles#create-new-role){target="_blank"} 안내서를 참조하세요.

>[!NOTE]
> Collaboration에 액세스하려면 사용자가 Adobe Experience Platform의 **[!UICONTROL Prod]** 샌드박스에 액세스할 수 있어야 합니다. 사용자에게 이 샌드박스에 대한 액세스 권한을 부여하려면 **[!UICONTROL Sandboxes]** 리소스에서 **[!UICONTROL Prod]** 권한이 포함된 역할에 할당되어야 합니다.

다음은 Collaborations 리소스 내에서 사용 가능한 권한 목록입니다.

| 높은 수준 권한 | 설명 |
| --- | --- |
| Collaboration 인스턴스 관리 | 조직의 공동 작업 인스턴스를 보고, 만들고, 업데이트하고, 삭제합니다. 다른 조직의 공동 작업 인스턴스를 검색합니다. |
| Collaboration 인스턴스 읽기 | 조직의 공동 작업 인스턴스를 읽고 다른 조직의 공동 작업 인스턴스를 검색합니다. |
| 연결 초대 관리 | 조직에서 시작한 연결 초대를 보고, 만들고, 삭제합니다. 다른 조직에서 시작한 연결 초대를 수락 및 거부합니다. |
| 연결 초대 읽기 | 연결 초대 보기. |
| Collaboration 연결 관리 | 공동 작업자는 설정을 보고 만들고 업데이트하며 연결을 제출하고 삭제할 수 있습니다. |
| Collaboration 연결 읽기 | 연결 보기. |
| 대상 데이터 관리 | 온보딩하고 대상자를 검색합니다. 공개, 비공개 및 사용자 지정 대상을 업데이트하고 대상 인벤토리 메타데이터 설정을 관리합니다. |
| 대상 데이터 읽기 | Read and discover audiences. |
| Manage Measurement Data | Onboard, update, and delete measurement data. |
| Read Measurement Data | Read measurement data. |
| Manage Projects | View, create, update, and delete projects for any of the discover, activate, and measurement activities. |
| Read Projects | View projects for any of the discover, activate, and measurement activities. |
| Read User Activities | Read user activities. |
| Export User Activities | Export user activities. |
| Read Collaboration Credit Monitoring | Credit monitoring at the organization and instance level. |

{style="table-layout:auto"}

## 다음 단계

After creating roles that define access to Collaboration, you&#39;ll need to [assign the roles](./manage-user-access.md#assign-a-role) to administrators and users. Refer to the [manage permissions for a role](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/abac/permissions-ui/permissions) guide for a complete overview of managing roles.
