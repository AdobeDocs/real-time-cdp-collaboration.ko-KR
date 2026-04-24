---
title: RTCDP Collaboration 스타터 개요
description: Adobe Real-Time CDP Collaboration Starter를 사용하여 전체 Real-Time CDP 라이선스를 구입하지 않고도 라이선스가 있는 파트너와의 개인정보 보호 중심 공동 작업을 확장하고 강화하는 방법에 대해 알아봅니다.
audience: publisher, advertiser, invited users to Real-Time CDP Collaboration Starter
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 7ae0bd3d-eee9-48c0-9f18-a56033fee52d
source-git-commit: c759496b528ed6c1e173f1ca1f1469da572c85df
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 4%

---

# Adobe Real-Time CDP Collaboration [!DNL Starter] 개요

Adobe Real-Time CDP Collaboration [!DNL Starter]을(를) 사용하여 라이선스가 있는 파트너와 개인 정보 중심 데이터 프로젝트에 대해 공동 작업하십시오. 참여하기 위해 자체 Collaboration 라이선스가 필요하지 않습니다.

라이선스가 있는 파트너가 귀하를 Collaboration에 초대하고 크레딧을 사용하여 광고주별-게시자별 및 브랜드별 패턴 모두에서 공동 워크플로우에 자금을 조달합니다. 이러한 패턴과 작동 방식에 대해 자세히 알아보려면 [공동 작업 패턴](./collaboration-patterns.md) 및 [통합 워크플로](./end-to-end-workflow.md) 안내서를 읽어 보십시오.

초대된 [!DNL Starter] 사용자는 다음 작업을 수행할 수 있습니다.

* [!DNL Starter] 계정에서 공동 작업 데이터를 온보딩하고 관리합니다.
* Source 및 공동 프로젝트에서 사용할 대상 유지 관리
* 효과적인 타기팅 및 캠페인 측정을 지원하기 위해 대상자와 파트너가 겹친다는 점에 대한 통찰력을 얻으십시오.
* 대상을 활성화하고 이를 파트너와 공유하여 공동 캠페인 활성화 및 참여를 유도하십시오.

## 전제 조건 {#prerequisites}

Collaboration [!DNL Starter]을(를) 시작하려면 조직과 라이선스 파트너가 모두 동일한 지역에 있는지 확인하십시오. Real-Time CDP Prime, Ultimate 또는 Collaboration 라이선스를 보유하고 있는 파트너의 초대를 받아야 합니다.

초대를 시작하려면 라이선스가 있는 파트너에게 다음 정보를 제공하십시오.

* 연락처 이름
* 연락처 이메일
* 회사
* 역할(광고주/게시자): 광고주
* 업계

초대를 받고 수락하면 조직에서 Collaboration [!DNL Starter]에 액세스하려면 Adobe으로 무비용 판매 주문을 검토하고 서명해야 합니다. 초대 프로세스에 대한 자세한 내용은 [공동 작업자를 Collaboration에 초대 [!DNL Starter]](../connect/establishing-connections.md#invite-collaborator) 안내서를 참조하십시오.

## 가드레일 {#guardrails}

[!DNL Starter] 계정에 적용되는 주요 보호 기능에 대해 이해하려면 다음 표를 참조하십시오. 여기에는 대상 소싱, 데이터 볼륨, 새로 고침 빈도, 대상 중복 및 활성화 기능에 대한 제한이 포함됩니다.

| 가드레일 | 설명 |
|----------| ------------|
| 대상자 소스 | **[!DNL Amazon S3]**&#x200B;을(를) 소스로 사용하여 대상 데이터를 Collaboration으로 가져올 수 있습니다. 단계별 지침은 [대상 소싱을 구성하는 방법 [!DNL Amazon S3] 을 참조하십시오](../setup/configure-aws-s3-audience-sourcing.md). |
| 대상자 | [!DNL Starter] 계정은 최대 다음 수를 사용할 수 있습니다.<ul><li>[!DNL AWS S3] 버킷에서 가져온 대상자 10명</li><li>총 5,000만 개의 id(대상 데이터의 행 수로 계산)</li><li>6일마다 대상당 1회 새로 고침</li></ul> |
| 대상자 중복 및 통찰력 | 대상 간 대상 중복 및 통찰력을 실행할 수 있는 빈도에는 사용 제한이 없습니다. [겹침을 검색하고 대상을 비교하는 방법](../collaborate/discover.md)을 알아보세요. |
| 활성화 | [!DNL Starter] 사용자는 귀하를 초대한 파트너와만 대상을 활성화하고 공유할 수 있습니다. 외부 플랫폼에 대한 대상을 구성할 수 없습니다. [대상자 활성화](../collaborate/activate.md)에 대해 자세히 알아보세요. |

{style="table-layout:auto"}

## 시작 {#getting-started}

[초대를 수락하고 약관에 동의하면](../connect/establishing-connections.md#accept-invitation-sign-terms) 자격 증명을 사용하여 [Adobe Experience Cloud](https://experience.adobe.com/){target="_blank"}에 로그인합니다. Collaboration을 사용하려면 먼저 계정에 적절한 액세스 권한과 역할이 부여되어야 합니다.

이 워크플로우를 사용하여 [!DNL Starter] 계정을 설정하고 파트너와 공동 작업을 시작합니다.

### 관리자 액세스 설정 {#setup-admin-access}

먼저 **관리자 액세스** 작업 영역을 사용하여 자신에게 필요한 액세스 권한을 부여합니다. 이렇게 하면 Experience Platform 제품에 대한 관리 권한과 사용자 액세스 권한이 모두 부여됩니다. 초기 액세스를 설정하는 방법에 대한 자세한 단계는 [관리자 액세스 지침](../setup/starter-admin-access.md)을 참조하세요.

완료되면 [Adobe Experience Cloud](https://experience.adobe.com/){target="_blank"} 홈 페이지의 **[!UICONTROL 빠른 액세스]** 섹션에 **[!UICONTROL 권한]**, **[!UICONTROL Experience Platform]** 및 **[!UICONTROL Real-Time CDP Collaboration]**&#x200B;이 표시됩니다.

![제품 관리자 액세스 설정 후 사용 권한, Experience Platform 및 Real-Time CDP Collaboration을 표시하는 Adobe Experience Cloud 작업 영역입니다.](/help/assets/overview/starter/setup-admin-access.png){zoomable="yes"}

액세스 역할 및 다양한 Adobe Experience Cloud 제품에 대한 자세한 내용은 [액세스 제어 개요](../permissions/overview.md)를 참조하십시오.

### 권한 구성 {#configure-permissions}

이제 관리자 권한이 있으므로 자신과 조직의 다른 사용자에게 역할과 권한을 할당할 수 있습니다. 이 단계는 Real-Time CDP Collaboration에 액세스하거나 다른 사람이 사용할 수 있도록 허용하기 전에 필요합니다. 자세한 지침은 [사용 권한을 구성하는 방법](../setup/starter-permission-controls.md)을 참조하세요. Collaboration에서 사용할 수 있는 다양한 역할 및 권한에 대한 자세한 내용은 [역할 관리](../permissions/manage-roles.md) 설명서를 참조하십시오.

역할 및 권한이 할당되면 Collaboration에 액세스할 수 있는지 확인합니다. [Adobe Experience Cloud](https://experience.adobe.com/){target="_blank"}(으)로 이동한 다음 **[!UICONTROL 빠른 액세스]** 섹션에서 **[!UICONTROL Real-Time CDP Collaboration]**&#x200B;을(를) 선택합니다. 이렇게 하면 Collaboration 기능을 사용할 수 있는 **[!UICONTROL Adobe Real-Time CDP Collaboration]** 작업 영역이 열립니다.

### 연결 설정 {#set-up-connections}

다음으로, 다음 안내서의 단계에 따라 연결을 설정하고 파트너와 공동 작업을 시작합니다.

* [Collaboration 계정 설정](../setup/onboard-account.md)
* [초대 공동 작업자와 연결 설정](../connect/overview.md)
* [새 프로젝트를 만들고 파트너와 공동 작업 시작](../collaborate/overview.md)

### 신용 사용 이해 {#understand-credit-usage}

모든 Collaboration [!DNL Starter] 활동에서 크레딧을 사용합니다. 그러나 초대된 사용자는 이러한 크레딧을 구매하거나 관리할 필요가 없습니다. 귀하를 초대한 공동 작업자는 귀하의 활동과 연관된 모든 신용 사용을 다룹니다. 자세한 내용은 Collaboration의 [신용 사용 및 소비 [!DNL Starter]](../setup/starter-credit-usage.md) 설명서를 참조하세요.

## 다음 단계 {#next-steps}

이제 초기 설정을 완료하고 보안 공동 작업을 위해 조직을 구성했습니다. 다음으로 다음 리소스를 탐색하여 대상 소싱 및 Collaboration 내의 다양한 프로젝트 사용 사례에 대해 알아보십시오.

* [Source 및 대상자 관리](../setup/onboard-audiences.md)
* [프로젝트 사용 사례](../collaborate/overview.md#project-use-cases):
   * [중복 검색 및 대상 비교](../collaborate/discover.md)
   * [대상자 활성화](../collaborate/activate.md)
   * [캠페인 성과 측정](../collaborate/measure.md)
