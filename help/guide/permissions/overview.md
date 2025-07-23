---
title: 액세스 제어 개요
description: Adobe Real-Time Customer Data Platform(CDP) Collaboration에 대한 액세스 권한을 얻는 방법에 대해 알아봅니다.
audience: admin
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: af48f5ea-8258-42a6-a39e-f4a4ca5b4a69
source-git-commit: 608706d00124372ac59209478ab551a3a6ce0226
workflow-type: tm+mt
source-wordcount: '954'
ht-degree: 2%

---

# 액세스 제어 개요

{{limited-availability-release-note}}

>[!IMPORTANT]
>
> Adobe Real-Time CDP Collaboration에 액세스하려는 최종 사용자의 경우 시스템 또는 제품 관리자에게 연락하여 기존 액세스를 확인하십시오. 시스템 관리자가 누구인지 모르는 경우 Adobe 담당자에게 문의하십시오.

Adobe Real-Time CDP Collaboration에 대한 액세스 제어는 [Adobe Experience Cloud](https://experience.adobe.com/){target="_blank"}의 Admin Console 및 권한을 통해 제공됩니다. 이 안내서에서는 사용 사례에 따라 자신 또는 팀의 다른 구성원에게 액세스 권한을 부여하는 방법을 알아봅니다.

## 액세스 제어 계층 {#hierarchy}

Collaboration에 대한 액세스 제어를 구성하려면 **반드시**&#x200B;시스템 또는 제품 관리자 권한이 있어야 합니다. 시스템 관리자에는 제한이 없으며 온보딩 프로세스 중에 프로비저닝됩니다. 한편 제품 관리자는 모든 제품에 할당된 관리 기능을 제공할 수 있습니다. 제품 관리자에게는 시스템 관리자가 제품 및 관리 액세스 권한을 부여해야 합니다.

이 안내서에서는 시스템 관리자, 제품 관리자 및 최종 사용자에 대한 액세스 구성에 대해 설명합니다. 역할 간의 주요 차이점을 이해하려면 아래 표를 참조하십시오.

| 역할 | 설명 |
| --- | --- | 
| 시스템 관리자 | 조직의 수퍼유저입니다. 관리자는 Admin Console에서 모든 관리 작업을 수행할 수 있으며 다른 사용자에게 관리 기능을 위임할 수 있는 권한이 있습니다. |
| 제품 관리자 | 조직에 할당된 제품 및 모든 관련 관리 기능(예: 조직에 사용자 추가, 제품 프로필에서 사용자 추가 또는 제거, 제품에서 다른 제품 관리자 추가 또는 제거)을 관리합니다. |
| 최종 사용자 | 제품을 사용하는 조직의 사용자입니다. |

{style="table-layout:auto"}

관리 역할에 대한 자세한 내용은 [Adobe 도움말 센터](https://helpx.adobe.com/enterprise/using/admin-roles.html)를 참조하십시오.

>[!TIP]
>
>이 안내서에서 **관리자**&#x200B;를 사용하면 **시스템 및 제품 관리자**&#x200B;가 됩니다.

## 추가 제품 {#products}

Collaboration에 대한 액세스 권한을 부여하려면 [사용 사례](#use-cases)에 따라 여러 제품에 액세스해야 합니다. 액세스 제어 가이드는 진행하면서 여러 사용자 인터페이스를 통해 작동할 수 있으며, 각 사용자 인터페이스는 액세스 구성 프로세스 내에서 특정 목적을 제공합니다. 각 제품의 용도를 자세히 이해하려면 아래 표를 참조하십시오.

| 제품 | 사용 |
| --- | --- |
| [관리 콘솔](https://adminconsole.adobe.com/) | 관리자는 이 옵션을 사용하여 사용자에게 제품 및/또는 관리자 액세스 권한을 할당합니다. |
| [사용 권한](https://experience.adobe.com/) | 관리자는 이 옵션을 사용하여 관리자 또는 최종 사용자 역할을 할당합니다. |
| [Experience Platform](https://platform.adobe.com/) | 관리자와 최종 사용자에게 Experience Platform 제품에 대한 액세스 권한을 부여하여 역할에 할당해야 합니다. |

## 시작 위치 {#use-cases}

이제 다양한 Experience Cloud 제품뿐만 아니라 사용자 및 관리 역할에 대해 더 깊이 이해했으므로 Collaboration에 대한 액세스 권한을 부여할 수 있습니다. 수행해야 하는 단계에 영향을 주는 두 가지 주요 요인이 있습니다.

- 관리자 또는 최종 사용자 액세스 권한을 할당하는 경우
- 사용자가 이미 Experience Platform 제품에 액세스할 수 있는 경우

액세스 제어 사용 사례에 따라 권한을 구성하는 데 필요한 사용자와 시작 위치를 결정하려면 아래 차트를 참조하십시오. **시작 위치에서 안내서의 끝까지 자습서를 따르십시오.**

>[!TIP]
>
> 수퍼 유저는 시스템 관리자가 얻을 수 있는 가장 높은 수준의 액세스 권한을 나타냅니다. 수퍼 사용자는 모든 관리 작업 및 사용자 기능을 수행할 수 있습니다. 시스템 관리자는 제품 기능을 즉시 사용할 수 없으며 아래 차트와 같이 자신에게 적절한 액세스 권한을 제공해야 합니다.

| 사용 사례 | 필수 역할 | 시작 위치 |
| --- | --- | --- | 
| 기존 Experience Platform 제품 액세스 권한이 없는 수퍼 유저. | 시스템 관리자. | [제품 관리자 액세스 구성](./manage-user-access.md#admin-access) |
| 기존 Experience Platform 시스템 관리자 **with** Experience Platform UI 액세스 권한을 가진 수퍼 유저. | 시스템 관리자. | [Collaboration 액세스 구성](./manage-user-access.md#RTCDP-collab-access) |
| Experience Platform UI 액세스 없이 **기존 Experience Platform 시스템 관리자의 수퍼 유저입니다.** | 시스템 관리자. | [제품 관리자 액세스 구성](./manage-user-access.md#admin-access) |
| 새 제품 관리자에 대한 제품 관리자 권한 및 Collaboration 액세스 권한. | 시스템 관리자. | [제품 관리자 액세스 구성](./manage-user-access.md#admin-access) |
| 기존 Experience Platform 제품 관리자 **Experience Platform UI 액세스**&#x200B;이(가) 있는 Collaboration 액세스 | 시스템 또는 제품 관리자. | [Collaboration 액세스 구성](./manage-user-access.md#RTCDP-collab-access) |
| Experience Platform UI 액세스 없이 기존 Experience Platform 제품 관리자 **의 Collaboration 액세스** | 시스템 또는 제품 관리자. | [사용자 액세스 구성](./manage-user-access.md#user-access) |
| 새 최종 사용자를 위한 Collaboration 액세스 권한. | 시스템 또는 제품 관리자. | [사용자 액세스 구성](./manage-user-access.md#user-access) |
| Experience Platform 액세스 권한이 있는 기존 사용자에 대한 Collaboration 액세스 권한. | 시스템 또는 제품 관리자. | [Collaboration 액세스 구성](./manage-user-access.md#RTCDP-collab-access) |

{style="table-layout:auto"}

## 추가 권한

Collaboration에 대한 액세스 권한을 얻으면 특정 기능에 대해 몇 가지 추가 Experience Platform 권한이 필요할 수 있습니다.

### 대상자 소싱 {#audience-sourcing}

공동 작업자에게 대상을 보내려면 먼저 Collaboration에 대상을 소싱해야 합니다. 현재 대상자 가져오기에 지원되는 셀프 서비스 데이터 연결은 Experience Platform뿐입니다. 먼저 대상자 온보딩을 관리하는 사용자에게 다음 **[!UICONTROL 프로필 관리]** 리소스 권한을 포함하는 역할을 할당해야 합니다.

| 사용 권한 | 설명 |
| ---- | ---- |
| [!UICONTROL 세그먼트 보기] | 사용자가 샌드박스에서 사용 가능한 대상 목록을 볼 수 있습니다. |
| [!UICONTROL 프로필 보기] | 공동 작업 필드에 매핑하는 데 사용할 수 있는 필드를 사용자가 볼 수 있도록 해줍니다. |

아래에서는 위의 권한이 추가된 예제 역할을 볼 수 있습니다. 역할 만들기 또는 할당에 대한 자세한 내용은 [역할 관리](./manage-roles.md) 안내서를 참조하세요.

![세그먼트 보기 및 프로필 보기 권한이 있는 권한의 리소스 작업 영역이 프로필 관리 리소스에 추가되었습니다.](../../assets/permissions/sample-audience-role.png)

>[!NOTE]
>
>사용자는 위의 권한 없이 소스가 제공된 후 Collaboration 내에서 대상자와 작업할 수 있습니다.

## 다음 단계

시작할 위치를 결정했으면 사용 사례의 링크에 따라 액세스 구성을 시작하십시오. 이러한 사용 사례 외에 관리자로서 Collaboration에 대한 액세스를 구성하는 방법에 대해 알아보려면 [사용자 액세스 관리](manage-user-access.md) 안내서를 참조하십시오. Collaboration의 다양한 구성 요소에 대한 액세스를 구성하는 역할과 그 부분에 대해 알아보려면 [역할 관리](manage-roles.md) 안내서를 참조하십시오.
