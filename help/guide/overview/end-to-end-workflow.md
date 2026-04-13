---
title: 전체 워크플로
description: 공동 작업 패턴을 기반으로 Real-Time CDP Collaboration 사용에 대한 전체적인 워크플로를 이해합니다.
audience: admin, publisher, advertiser
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/kr/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 90f9341e-5dd7-4521-a602-edb0263838c5
source-git-commit: 901b17c7493e76b17e780b6f7b05a69fa22303d2
workflow-type: tm+mt
source-wordcount: '1738'
ht-degree: 0%

---

# 전체 워크플로

{{limited-availability-release-note}}

Adobe Real-Time CDP Collaboration에서 통합 워크플로우는 선택하는 공동 작업 패턴에 따라 다릅니다. 이 워크플로에서는 계정 및 소싱 대상 만들기에서 연결 형성 및 프로젝트 만들기에 이르기까지 공동 작업 프로젝트 설정 및 실행과 관련된 단계를 간략하게 설명합니다. 이 워크플로를 이해하는 것은 마케팅 목표를 달성하기 위해 플랫폼의 기능을 효과적으로 활용하는 데 필수적입니다.

## 시작

시작하기 전에 다음 주요 개념을 확실히 이해해야 합니다.

- **Collaboration 패턴**: 이러한 패턴은 공동 작업자가 함께 작업하는 방법을 정의합니다. 다음과 같은 5가지 패턴이 있습니다.
   - [advertiser-to-publisher](./collaboration-patterns.md#advertiser-to-publisher)
   - [브랜드 대 브랜드](./collaboration-patterns.md#brand-to-brand)
   - [advertiser-to-data 파트너](./collaboration-patterns.md#advertiser-to-data-partner)
   - [에이전시 투 퍼블리셔](./collaboration-patterns.md#agency-to-publisher)
   - [광고주-에이전시 플랫폼](./collaboration-patterns.md#advertiser-to-agency-platform)
- **계정 역할**: 계정 역할이 플랫폼 내의 기능을 결정합니다. 조직의 목표, 브랜드 및 목표에 부합해야 합니다. 네 가지 계정 역할이 있습니다. [광고주](./roles.md#advertiser), [게시자](./roles.md#publisher), [에이전시](./roles.md#agency) 및 [데이터 파트너](./roles.md#data-partner).
- **사용 사례**: 사용 사례는 Collaboration을 활용하여 마케팅 목표를 달성할 수 있는 방법을 정의합니다. 세 가지 공동 작업 사용 사례가 있습니다. [검색](./use-cases.md#discover), [활성화](./use-cases.md#activate) 및 [측정](./use-cases.md#measure).

이 안내서에서는 세 명의 모의 공동 작업자를 사용하여 전체적인 워크플로를 보여 줍니다.

- **[!UICONTROL Luma]**: 운동복 브랜드입니다. 타깃팅된 마케팅 캠페인을 통해 특정 대상에게 연결하고자 하는 광고주입니다.
- **[!UICONTROL TV Tube]**: 디지털 스트리밍 공급자입니다. 광고주가 사용할 수 있도록 대상 데이터를 제공하는 게시자입니다.
- **[!UICONTROL 의류 맞춤]**: 다른 운동복 브랜드. 또한 향상된 마케팅 활동을 위해 대상 데이터와 통찰력을 공유하기 위해 공동 작업을 원하는 두 번째 광고주입니다.
- **[!UICONTROL Agency99]**: 미디어 에이전시입니다. 작업 영역 내에서 여러 클라이언트 계정을 관리하고 게시자 및 광고주와 연결합니다.
- **[!UICONTROL DataM8]**: 타사 데이터 공급자입니다. 광고주가 사용할 대상 데이터를 제공합니다.
- **[!UICONTROL Holdco]**: 내부 에이전시 팀에서 클라이언트 캠페인을 관리하는 데 사용하는 회사 마케팅 및 광고 서비스 플랫폼입니다.

## 광고주-게시자 간 워크플로 {#advertiser-to-publisher-workflow}

운동 소매 회사인 [!UICONTROL Luma]이(가) 타깃팅된 마케팅 캠페인을 통해 특정 대상자에게 도달하기 위해 디지털 스트리밍 공급자인 [!UICONTROL TV Tube]와(과) 연결을 만들려고 합니다.

먼저 [!UICONTROL Luma]은(는) 광고주 역할로 [계정을 만들어야](../setup/onboard-account.md)하지만 [!UICONTROL TV Tube]은(는) 게시자 역할로 계정을 만듭니다.

계정을 설정한 후에는 [!UICONTROL Luma] 및 [!UICONTROL TV Tube]에서 모두 [데이터 연결 및 소스 대상을 만들기](../setup/onboard-audiences.md)해야 합니다. [!UICONTROL TV Tube]만 마케팅 캠페인에 대한 대상을 활성화하므로 [대상을 구성](../setup/manage-destinations.md)해야 합니다.

두 공동 작업자가 계정을 설정한 후에는 플랫폼 내에서 [연결을 형성](../connect/establishing-connections.md)할 준비가 되었습니다. [!UICONTROL Luma]은(는) [공동 작업자 검색](../connect/discover-collaborators.md) 기능을 사용하여 [!UICONTROL TV Tube]를 찾아 연결 요청을 시작합니다. [!UICONTROL TV Tube]에서 연결 요청을 수락하면 [!UICONTROL Luma]은(는) 공동 작업 방법을 정의하기 위해 연결 설정을 구성합니다. [!UICONTROL TV Tube]에서 두 브랜드 간의 보안 연결을 설정하기 위해 연결 요청을 수락합니다.

연결이 설정되면 [!UICONTROL Luma] [프로젝트를 만들고](../collaborate/manage-projects.md) [!UICONTROL TV Tube]와(과) 공동 작업을 시작합니다. 프로젝트 설정 중에 목표에 가장 적합한 공동 작업 사용 사례를 선택합니다. [검색](../collaborate/discover.md), [활성화](../collaborate/activate.md) 및 [측정](../collaborate/measure.md).

[!UICONTROL Luma]은(는) [Discover](../collaborate/discover.md) 사용 사례를 활용하여 [!UICONTROL TV Tube]의 대상 데이터에 대한 통찰력을 얻습니다. [!UICONTROL Luma]이(가) 대상 대상 세그먼트를 식별하면 이 대상을 [활성화](../collaborate/activate.md)합니다.

대상을 활성화한 후 [!UICONTROL TV Tube]에서 타깃팅된 마케팅 캠페인을 실행하고 [측정](../collaborate/measure.md)에 결과를 업로드하여 캠페인의 효과를 평가합니다.

## 브랜드 간 워크플로우 {#brand-to-brand-workflow}

스포츠 의류 브랜드인 [!UICONTROL Fit Apparel]은(는) 다른 스포츠 의류 브랜드인 [!UICONTROL Luma]과(와) 협력하여 향상된 마케팅 노력을 위한 대상 데이터 및 통찰력을 공유하려고 합니다.

계정을 설정한 후 [!UICONTROL Fit Apparel]과(와) [!UICONTROL Luma]을(를) 모두 [데이터 연결 및 소스 대상을 만들기](../setup/onboard-audiences.md)해야 합니다. [!UICONTROL 의류 맞춤]과(와) [!UICONTROL Luma] 모두 마케팅 캠페인에 대해 대상을 활성화하므로 둘 다 [대상을 구성](../setup/manage-destinations.md)해야 합니다.

대상을 소싱한 후 [!UICONTROL Apparel] 및 [!UICONTROL Luma] [연결을 형성하여](../connect/establishing-connections.md) 플랫폼 내에서 대상 데이터를 안전하게 공유합니다. 이렇게 하려면 [개인 연결 초대](../connect/establishing-connections.md#private-connection-invite) 기능을 사용해야 합니다. [!UICONTROL Luma]은(는) 연결 코드를 [!UICONTROL Fit Apparel]과(와) 공유하며, 사용자는 이를 사용하여 연결 요청을 시작합니다. [!UICONTROL Luma]이(가) 연결 요청을 수락하면 [!UICONTROL Fit Apparel]은(는) 공동 작업 방법을 정의하는 연결 설정을 구성합니다. 구성에서 [!UICONTROL 의류 맞춤]은 두 공동 작업자가 모두 마케팅 캠페인에 대한 대상을 활성화할 수 있도록 지정합니다. 연결을 완료하려면 [!UICONTROL Luma]이(가) 두 브랜드 간의 보안 링크 설정 요청을 수락합니다.

연결이 설정되면 [!UICONTROL Apparel 맞춤] [프로젝트를 만들어](../collaborate/manage-projects.md) [!UICONTROL Luma]와(과) 공동 작업을 시작합니다. 프로젝트 설정 중에 목표에 가장 적합한 공동 작업 사용 사례를 선택합니다. [검색](../collaborate/discover.md), [활성화](../collaborate/activate.md) 및 [측정](../collaborate/measure.md).

[!UICONTROL 의류 맞춤] 및 [!UICONTROL Luma] 모두 [검색](../collaborate/discover.md) 사용 사례를 사용하여 서로의 대상 데이터에 대한 통찰력을 얻을 수 있습니다. 중요한 대상 세그먼트를 식별한 후에는 마케팅 캠페인에 대해 선택한 대상을 [활성화](../collaborate/activate.md)합니다.

마지막으로 두 브랜드는 캠페인을 실행한 후 결과를 [측정값](../collaborate/measure.md)에 데이터를 업로드하고 공동 작업의 효과를 평가합니다.

## 광고주-광고 플랫폼 워크플로 {#advertiser-to-advertising-platform-workflow}

운동 소매 회사인 [!UICONTROL Luma]이(가) [!DNL AMC]의 ID 확인 및 타깃팅 도구를 활용하여 마케팅 기능을 개선하기 위해 [!DNL Amazon Marketing Cloud]&#x200B;([!DNL AMC])과(와) 연결하려고 합니다. Luma에 이미 활성 [!DNL Amazon Advertising] 계정이 있으며 [!DNL AMC]을(를) 사용하도록 승인되었습니다.

시작하려면 [!UICONTROL Luma]에서 광고주 역할을 사용하여 [계정을 만들고](../setup/onboard-account.md)해야 합니다. 계정을 설정한 후 [!UICONTROL Luma]은(는) [데이터 연결 및 원본 대상을 만들어야](../setup/onboard-audiences.md)합니다. [!UICONTROL Luma]은(는) 마케팅 캠페인에 대한 대상을 활성화하므로 [대상을 구성](../setup/manage-destinations.md)해야 합니다.

[!UICONTROL Luma]의 계정이 설정되면 플랫폼 내에서 [!DNL AMC]와(과) [연결을 구성](../connect/establishing-connections.md)할 준비가 되었습니다. [!UICONTROL Luma]은(는) [공동 작업자 검색](../connect/discover-collaborators.md) 기능을 사용하여 [!UICONTROL Amazon Marketing Cloud] 및 [연결 요청을 시작](../connect/advertising-platforms/amc.md)합니다. [!DNL Amazon] 로그인 페이지를 통해 연결을 인증하고 인증하면 [!DNL AMC]에 연결됩니다.

연결이 설정되면 [!UICONTROL Luma] [프로젝트를 만듭니다](../collaborate/manage-projects.md). [!DNL AMC]과의 공동 작업을 시작합니다. 사용 사례를 포함한 연결 설정은 광고 플랫폼에 따라 사전 구성됩니다. [!DNL AMC]의 사용 사례는 [검색](../collaborate/advertising-platforms/amc.md#discover)입니다.

[!UICONTROL Luma]은(는) [Discover](../collaborate/advertising-platforms/amc.md#discover) 사용 사례를 활용하여 [!DNL AMC]에서 인사이트 및 대상 데이터를 얻습니다. 이러한 통찰력을 사용하여 [!UICONTROL Luma]은(는) 마케팅 전략을 최적화하고 캠페인 효과를 향상시킬 수 있습니다.

## 광고주-데이터 파트너 워크플로 {#advertiser-to-data-partner-workflow}

운동 소매 회사인 [!UICONTROL Luma]은(는) 서드파티 데이터 공급자인 [!UICONTROL DataM8]과(와) 공동 작업을 수행하여 고객 프로필을 강화하고 대상 타깃팅을 개선하려고 합니다.

먼저 [!UICONTROL Luma]은(는) 광고주 역할로 [계정을 만들어야](../setup/onboard-account.md)하지만 [!UICONTROL DataM8]은(는) 데이터 파트너 역할로 계정을 만듭니다.

계정을 설정한 후 [!UICONTROL Luma]와(과) [!UICONTROL DataM8]을(를) 모두 [데이터 연결 및 소스 대상을 만듭니다](../setup/onboard-audiences.md). 두 공동 작업자는 마케팅 캠페인에 대해 대상을 활성화할 수 있으므로 각각 [대상을 구성](../setup/manage-destinations.md)해야 합니다.

두 공동 작업자가 계정을 설정한 후에는 플랫폼 내에서 [연결을 형성](../connect/establishing-connections.md)할 준비가 되었습니다. [!UICONTROL Luma]은(는) [공동 작업자 검색](../collaborate/discover.md) 기능을 사용하여 [!UICONTROL DataM8]을(를) 찾고 연결 요청을 시작합니다. [!UICONTROL DataM8]이(가) 연결 요청을 수락하면 [!UICONTROL Luma]은(는) 공동 작업 방법을 정의하기 위해 연결 설정을 구성합니다. [!UICONTROL DataM8]은(는) 두 공동 작업자 간의 보안 링크를 설정하기 위해 연결 요청을 수락합니다.

연결이 설정되면 [!UICONTROL Luma] [프로젝트를 만듭니다](../collaborate/manage-projects.md). [!UICONTROL DataM8]과의 공동 작업을 시작합니다. 프로젝트 설정 중에 목표에 가장 적합한 공동 작업 사용 사례를 선택합니다. [검색](../collaborate/discover.md), [활성화](../collaborate/activate.md) 및 [측정](../collaborate/measure.md).

[!UICONTROL Luma]은(는) [Discover](../collaborate/discover.md) 사용 사례를 활용하여 [!UICONTROL DataM8]의 대상 데이터에 대한 통찰력을 얻습니다. [!UICONTROL Luma]이(가) 대상 대상 세그먼트를 식별하면 이 대상을 [활성화](../collaborate/activate.md)합니다.

[!UICONTROL DataM8]에서도 대상을 [!UICONTROL Luma]에 [활성화](../collaborate/activate.md)할 수 있습니다. [!UICONTROL Luma]은(는) 이러한 기능을 사용하여 타사 특성을 고객 프로필에 추가하고 대상 구성을 분석합니다. CDP에서 바로 사용할 수 있는 보강된 데이터를 통해 [!UICONTROL Luma]은(는) 더 정밀한 대상을 작성하고 데이터를 관리 환경 외부로 이동하지 않고 유료 미디어 대상으로 활성화할 수 있습니다.

## 에이전시-게시자 간 워크플로 {#agency-to-publisher-workflow}

미디어 에이전시인 [!UICONTROL Agency99]이(가) 디지털 스트리밍 공급자인 [!UICONTROL TV Tube]과(와) 협력하여 타깃팅된 마케팅 캠페인을 통해 특정 대상에게 연결하려고 합니다.

먼저 [!UICONTROL Agency9]은(는) 에이전시 역할로 [계정을 만들어야](../setup/onboard-account.md)하지만, [!UICONTROL TV Tube]은(는) 게시자 역할로 계정을 만듭니다.

계정을 설정한 후 [!UICONTROL Agency9]와(과) [!UICONTROL TV Tube]를 모두 [데이터 연결 및 소스 대상을 만들기](../setup/onboard-audiences.md)해야 합니다. [!UICONTROL Agency99]은(는) 작업 영역에서 클라이언트 하위 계정 및 소스 클라이언트 데이터를 설정합니다. [!UICONTROL TV Tube]만 마케팅 캠페인에 대한 대상을 활성화하므로 [대상을 구성](../setup/manage-destinations.md)해야 합니다.

두 공동 작업자가 계정을 설정한 후에는 플랫폼 내에서 [연결을 형성](../connect/establishing-connections.md)할 준비가 되었습니다. [!UICONTROL Agency99]은(는) [공동 작업자 검색](../collaborate/discover.md) 기능을 사용하여 [!UICONTROL TV Tube]를 찾아 연결 요청을 시작합니다. [!UICONTROL Agency99]에서 [!UICONTROL TV Tube]와(과) 공동 작업하려는 하나 이상의 클라이언트를 위해 이 작업을 수행합니다. [!UICONTROL TV Tube]에서 연결 요청을 수락하면 [!UICONTROL Agency99]에서 각 공동 작업 방법을 정의하는 연결 설정을 구성합니다. [!UICONTROL TV Tube]에서 두 브랜드 간의 보안 연결을 설정하기 위한 연결 요청을 수락합니다.

연결이 설정되면 [!UICONTROL Agent99] [프로젝트를 만들어](../collaborate/manage-projects.md) 각 클라이언트 하위 계정에서 [!UICONTROL TV Tube]와(과) 공동 작업을 시작합니다. 프로젝트 설정 중에 목표에 가장 적합한 공동 작업 사용 사례를 선택합니다. [검색](../collaborate/discover.md), [활성화](../collaborate/activate.md) 및 [측정](../collaborate/measure.md).

[!UICONTROL Agency99]은(는) [Discover](../collaborate/discover.md) 사용 사례를 활용하여 [!UICONTROL TV Tube]의 대상 데이터에 대한 통찰력을 얻습니다. [!UICONTROL Agency99]이(가) 대상 대상 세그먼트를 식별하면 해당 대상을 [활성화](../collaborate/activate.md)합니다.

대상을 활성화한 후 [!UICONTROL TV Tube]에서 타깃팅된 마케팅 캠페인을 실행하고 [측정값](../collaborate/measure.md)에 결과를 업로드하여 캠페인의 효과를 평가합니다.

## 광고주-에이전시 플랫폼 워크플로 {#advertiser-to-agency-platform-workflow}

운동 소매 회사인 [!UICONTROL Luma]이(가) 에이전시 플랫폼인 [!UICONTROL Holdco]과(와) 협력하여 데이터를 공유하고 유료 미디어 인사이트를 받기를 원합니다.

먼저 [!UICONTROL Luma]은(는) 광고주 역할로 [계정을 만들어야](../setup/onboard-account.md)하지만 [!UICONTROL Holdco]은(는) 에이전시 역할로 계정을 만듭니다. 

계정을 설정한 후에는 [!UICONTROL Luma]와 [!UICONTROL Holdco]이(가) 모두 [데이터 연결을 만들고 소스 대상을 만들기](../setup/onboard-audiences.md)해야 합니다. 두 공동 작업자는 마케팅 캠페인에 대해 대상을 활성화할 수 있으므로 각각 [대상을 구성](../setup/manage-destinations.md)해야 합니다. 

두 공동 작업자가 계정을 설정한 후에는 플랫폼 내에서 [연결을 형성](../connect/establishing-connections.md)할 준비가 되었습니다. [!UICONTROL Luma]은(는) [공동 작업자 검색](../collaborate/discover.md) 기능을 사용하여 [!UICONTROL Holdco]을(를) 찾고 연결 요청을 시작합니다. [!UICONTROL Holdco]이(가) 연결 요청을 수락하면 [!UICONTROL Luma]이(가) 연결 설정을 구성하여 공동 작업 방법을 정의합니다.

[!UICONTROL Holdco]이(가) 연결 요청을 수락하여 두 공동 작업자 간의 보안 연결을 설정할 수 있습니다.

연결이 설정되면 [!UICONTROL Luma] [프로젝트를 만들고](../collaborate/manage-projects.md) [!UICONTROL Holdco]와의 공동 작업을 시작합니다. 프로젝트 설정 중에 목표에 가장 적합한 공동 작업 사용 사례를 선택합니다. [검색](../collaborate/discover.md), [활성화](../collaborate/activate.md) 및 [측정](../collaborate/measure.md).

[!UICONTROL Luma]은(는) [Discover](../collaborate/discover.md) 사용 사례를 활용하여 [!UICONTROL Holdco]의 대상 데이터에 대한 통찰력을 얻습니다. [!UICONTROL Luma]이(가) 대상 대상 세그먼트를 식별하면 이 대상을 [활성화](../collaborate/activate.md)합니다.

[!UICONTROL Holdco]에서도 대상을 [!UICONTROL Luma]에 [활성화](../collaborate/activate.md)할 수 있습니다. [!UICONTROL Luma]은(는) 이러한 기능을 사용하여 인사이트를 위한 에이전시가 실행하는 캠페인에서 유료 미디어 인사이트를 받고 CDP 프로필이 추가되고 소유한 미디어 오케스트레이션을 제공합니다.
