---
title: 연결 개요
description: Real-Time CDP Collaboration의 연결에 대해 알아봅니다.
audience: publisher, advertiser
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
source-git-commit: 5c08738cdc8e1e208203ee1f9a1cf1891b5b07cb
workflow-type: tm+mt
source-wordcount: '754'
ht-degree: 0%

---

# 연결 개요

{{limited-availability-release-note}}

공동 작업자가 캠페인에 대해 함께 작업하려면 먼저 연결을 설정해야 합니다. 이 연결을 통해 대상자를 활성화하고, 프로젝트를 만들고, 캠페인 성과에 대한 보고서를 실행할 수 있습니다.

연결은 선택한 공동 작업 패턴을 기반으로 설정됩니다. Collaboration은 광고주부터 게시자까지, 브랜드까지 및 광고주부터 광고 플랫폼까지의 세 가지 주요 공동 작업 패턴을 지원합니다. 이러한 패턴에 대한 자세한 내용은 [공동 작업 패턴](/help/guide/overview/collaboration-patterns.md) 안내서를 참조하십시오.

연결 설정 방법에 대해 알아보려면 공동 작업 패턴에 해당하는 아래 섹션을 읽어 보십시오.

- [광고주-게시자 연결](#advertiser-to-publisher-connection)
- [브랜드 간 연결](#brand-to-brand-connection)
- [광고주와 광고 플랫폼 연결](#advertiser-to-advertising-platform-connection)

## 광고주-게시자 연결 {#advertiser-to-publisher-connection}

![광고주-게시자 연결 프로세스의 높은 수준 다이어그램입니다.](/help/assets/connect/establish-connection/advertiser-publisher-flow.png){zoomable="yes"}

광고주 대 게시자 패턴에서 광고주는 **[!UICONTROL 게시자 검색]** 작업 영역을 통해 작업할 게시자를 검색하고 연결 초대를 보냅니다. 그러면 게시자가 초대를 검토하고 수락하여 광고주가 연결 설정을 제안할 수 있습니다. 게시자가 연결 설정을 수락하면 연결이 설정되고 두 공동 작업자가 프로젝트에서 함께 작업을 시작할 수 있습니다.

### 높은 수준 개요

광고주와 게시자 간에 연결을 설정하려면 다음 단계를 따르십시오.

1. [게시자 검색](./discover-collaborators.md): 광고주는 공동 작업할 수 있는 게시자를 식별합니다.
2. [초대 보내기](./establishing-connections.md#send-invite): 광고주가 선택한 게시자에게 연결 초대를 보냅니다.
3. [초대 수락](./establishing-connections.md#accept-invite): 게시자가 초대를 검토하고 수락합니다.
4. [연결 설정 구성](./establishing-connections.md#configure-connection-settings): 광고주가 연결 설정을 구성하고 검토할 수 있도록 게시자에게 보냅니다.
5. [연결 설정 확인](./establishing-connections.md#review-connection-settings): 게시자가 연결 설정을 검토하고 이를 수락 또는 거부합니다. 수락되면 연결이 설정됩니다. 거부된 경우 게시자는 제품 외부의 수정 사항에 대한 피드백을 제공할 수 있습니다. 그런 다음 광고주는 설정을 수정하고 다시 보내어 검토할 수 있습니다.

연결 설정이 수락되면 연결이 설정되고 공동 작업자는 [프로젝트를 만들](/help/guide/collaborate/manage-projects.md#create-project) 준비가 되어 캠페인에 대한 공동 작업을 시작할 수 있습니다.

## 브랜드 간 연결 {#brand-to-brand-connection}

![브랜드 간 연결 프로세스의 높은 수준 다이어그램입니다.](/help/assets/connect/establish-connection/brand-to-brand-flow.png){zoomable="yes"}

>[!TIP]
>
>**brand** 용어는 Collaboration 외부의 회사 또는 브랜드를 가리키는 데 사용됩니다. **collaborator**&#x200B;이라는 용어는 광고주인지 게시자인지에 관계없이 Collaboration에서 연결을 구성할 수 있는 모든 계정을 의미합니다.

브랜드 간 패턴에서는 제품 외부에서 통신한 두 브랜드가 [개인 연결 초대](#private-connection-invite)를 사용하여 Collaboration에서 직접 연결할 수 있습니다. 브랜드는 광고주 또는 게시자일 수 있습니다. 이 패턴은 두 개의 광고주 또는 두 개의 게시자와 같이 기존 광고주-게시자 모델에 적합하지 않을 수 있는 브랜드에 특히 유용합니다.

먼저 공동 작업자가 다른 공동 작업자에게 개인 연결 초대를 보냅니다. 수신자가 초대를 검토하고 수락하여 소유자가 연결 설정을 제안할 수 있습니다. 수신자가 연결 설정을 수락하면 연결이 설정되고 두 공동 작업자가 프로젝트에서 함께 작업을 시작할 수 있습니다.

### 높은 수준 개요

>[!TIP]
>
>연결 프로세스에 대해 논의할 때 **소유자**&#x200B;와(과) **수신자** 사이에 차이가 있습니다. 소유자는 초대를 전송하여 연결을 시작하는 공동 작업자이고, 수신자는 초대를 받고 검토하는 공동 작업자입니다.

두 브랜드 간의 연결 과정에는 몇 가지 단계가 포함됩니다. 연결 프로세스가 시작되기 전에 몇 가지 전제 조건을 충족해야 합니다.

1. 두 브랜드가 제품 외부에서 소통하며 잠재적 연결에 대해 논의합니다.
1. 브랜드가 아직 Collaboration에 [계정을 만듭니다](/help/guide/setup/onboard-account.md). 아직 만들지 않은 경우 적절한 역할 유형(광고주 또는 게시자)을 선택하십시오.

전제 조건이 충족되면 연결 프로세스를 시작할 수 있습니다. 다음 단계는 프로세스에 대해 간략히 설명합니다.

1. [비공개 연결 초대 보내기](./establishing-connections.md#private-connection-invite): 한 공동 작업자가 다른 공동 작업자에게 비공개 연결 초대를 보냅니다.
2. [개인 연결 초대 수락](./establishing-connections.md#accept-invite): 받는 사람이 개인 연결 초대를 검토하고 수락합니다.
3. [연결 설정 구성](./establishing-connections.md#configure-connection-settings): 소유자가 연결 설정을 구성하고 검토 및 수락하기 위해 받는 사람에게 보냅니다.
4. [연결 설정 확인](./establishing-connections.md#review-connection-settings): 받는 사람이 연결 설정을 검토하고 이를 수락하거나 거부합니다.

연결 설정이 수락되면 연결이 설정되고 공동 작업자는 [프로젝트를 만들](/help/guide/collaborate/manage-projects.md#create-project) 준비가 되어 캠페인에 대한 공동 작업을 시작할 수 있습니다.

## 광고주와 광고 플랫폼 연결 {#advertiser-to-advertising-platform-connection}

광고주와 광고 플랫폼 간 연결 프로세스를 통해 광고주는 Amazon Marketing Cloud(AMC)와 같은 서드파티 광고 플랫폼과 연결하여 마케팅 기능을 향상시킬 수 있습니다.

### 높은 수준 개요

광고주와 광고 플랫폼 간의 연결 과정은 몇 가지 단계를 포함한다. 연결 프로세스가 시작되기 전에 광고 플랫폼에 대한 활성 계정이 있고 해당 서비스를 사용할 수 있는 권한이 있는지 확인하십시오. 다음 단계에서는 연결 프로세스에 대해 간략히 설명합니다.

1. [광고 플랫폼 살펴보기](./discover-collaborators.md): 광고주는 공동 작업할 수 있는 광고 플랫폼을 식별합니다.
2. [Advertising platform에 연결](./advertising-platforms/overview.md#advertising-platforms-overview): 광고주가 연결하려는 광고 플랫폼을 선택하여 연결 프로세스를 시작하고 프롬프트에 따라 연결을 인증하고 승인합니다.
