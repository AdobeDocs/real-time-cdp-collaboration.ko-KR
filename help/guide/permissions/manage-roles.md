---
title: 권한을 통해 역할 관리
description: 실시간 CDP 협업 UI 내의 다양한 구성 요소에 대한 액세스를 제공하는 사용 가능한 모든 역할 리소스를 이해합니다.
audience: admin
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 59cf5bf2-421b-4ebc-beab-30eafb098649
source-git-commit: 56872a2cd91ae040aba51ed5784c86b055f88756
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 1%

---

# 역할 관리 {#manage-roles}

{{limited-availability-release-note}}

Real-Time CDP Collaboration UI의 다양한 구성 요소에 대한 사용자 액세스를 관리하기 위해 [관리자](./manage-user-access.md#system-admin-gain-access)는 역할을 정의하고 할당할 수 있습니다. 역할은 관리자 또는 사용자가 조직의 [리소스](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/home#permissions){target="_blank"}에 대한 액세스 권한을 정의합니다. 이 안내서에서는 Real-Time CDP Collaboration에서 제공하는 표준 역할과 사용자 지정 역할에 할당할 수 있는 개별 권한에 대한 정보를 제공합니다.

역할 관리를 시작하려면 관리자가 Experience Platform 제품에 액세스해야 합니다. 관리 액세스 권한을 얻는 방법 또는 Experience Platform 액세스 권한을 얻는 방법에 대한 자세한 내용은 관리 사용자 액세스](./manage-user-access.md#manage-user-access-through-permissions) 안내서 를 참조하십시오[.

## 표준 역할 {#standard-roles}

두 가지 공통 액세스 제어 사용 사례를 충족하는 두 가지 표준 역할이 제공됩니다. 이러한 역할은 &quot;읽기 전용&quot; 역할이므로 사용자 지정할 수 없습니다.

| 역할 이름 | 역할 설명 | 권한 |
| --- | --- | --- | 
| 협업 관리자 | 15가지 권한을 모두 포함하는 모든 액세스 권한입니다. 이렇게 하면 사용자 모두가 모든 데이터를 읽고, 만들고, 편집할 수 있습니다. 또한 Experience Platform 의 Prod ]**샌드박스에 액세스할**[!UICONTROL &#x200B;수 있으므로 대상을 Real-Time CDP Collaboration으로 가져올 수 있습니다. | 모두 아래 표의 내용입니다. |
| Collaboration 뷰어 | 읽기 전용 액세스 권한입니다. 사용자는 데이터, 활동, 연결 등을 읽고 검색할 수 있습니다. 또한 Experience Platform의 **[!UICONTROL Prod]** 샌드박스에 액세스할 수 있으므로 대상을 Real-Time CDP Collaboration으로 가져올 수 있습니다. | 아래 표의 모든 읽기 권한. |

{style="table-layout:auto"}

## 특정 액세스 역할 만들기 {#specific-access-roles}

다른 사용자에게 다양한 수준의 액세스를 제공하기 위해 추가 역할을 만들 수 있습니다. 역할을 만들 때 **[!UICONTROL 공동 작업]** 리소스 내에서 특정 권한을 선택하여 다양한 액세스 수준을 관리할 수 있습니다. 역할을 만들고 관리하는 방법은 [역할](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/abac/permissions-ui/roles#create-new-role){target="_blank"} 안내서를 참조하세요.

>[!NOTE]
> Real-Time CDP Collaboration에 액세스하려면 사용자가 Experience Platform의 **[!UICONTROL Prod]** 샌드박스에 액세스할 수 있어야 합니다. 사용자에게 이 샌드박스에 대한 액세스 권한을 부여하려면 **[!UICONTROL Sandboxes]** 리소스에서 **[!UICONTROL Prod]** 권한이 포함된 역할에 할당되어야 합니다.

다음은 Collaborations 리소스 내에서 사용 가능한 권한 목록입니다.

| 높은 수준 권한 | 설명 |
| --- | --- |
| 협업 인스턴스 관리 | 조직의 공동 작업 인스턴스를 보기, 생성, 업데이트 및 삭제합니다. 다른 조직의 공동 작업 인스턴스를 Discover 합니다. |
| 협업 인스턴스 읽기 | 조직의 공동 작업 인스턴스를 읽고 다른 조직의 공동 작업 인스턴스를 검색합니다. |
| 연결 초대 관리 | 조직에서 시작한 연결 초대를 보기, 만들기 및 삭제합니다. 다른 조직에서 시작한 연결 초대를 수락 및 거부합니다. |
| 연결 초대 읽기 | 연결 초대 보기. |
| 협업 연결 관리 | 광고주 역할은 설정을 보고, 만들고, 업데이트할 수 있을 뿐만 아니라 연결을 제출하고 삭제할 수도 있습니다. 게시자는 연결을 보거나, 수락하거나, 거부할 수 있습니다. |
| Collaboration 연결 읽기 | 연결 보기. |
| 대상 데이터 관리 | 대상을 온보딩하고 발견하십시오. 공개, 비공개 및 사용자 지정 대상을 업데이트하고 대상 인벤토리 메타데이터 설정을 관리합니다. |
| 대상 데이터 읽기 | 잠재 고객을 읽고 발견하십시오. |
| 측정 데이터 관리 | 측정 데이터를 온보딩, 업데이트 및 삭제합니다. |
| 측정 데이터 읽기 | 측정 데이터를 읽습니다. |
| 프로젝트 관리 | 검색, 공유, 활성화 및 측정 활동에 대한 프로젝트를 보기, 만들기, 업데이트 및 삭제합니다. |
| 프로젝트 읽기 | 검색, 공유, 활성화 및 측정 활동에 대한 프로젝트를 보기. |
| 사용자 활동 읽기 | 사용자 활동을 읽습니다. |
| 사용자 활동 내보내기 | 사용자 활동을 내보냅니다. |
| Collaboration 신용 모니터링 읽기 | 조직 및 인스턴스 레벨에서 신용 모니터링 |

{style="table-layout:auto"}

## 다음 단계

Real-Time CDP 공동 작업에 대한 액세스 권한을 정의하는 역할을 만든 후 관리자 및 사용자에게 [역할을 할당](./manage-user-access.md#assign-a-role)해야 합니다. 역할 관리에 대한 전체 개요는 [역할에 대한 권한 관리](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/abac/permissions-ui/permissions) 안내서를 참조하십시오.
