---
title: 광고주 또는 게시자와 연결
description: 잠재적 공동 작업자를 발견한 후 연결을 설정하고 프로젝트에 대한 공동 작업을 시작하는 방법에 대해 알아보십시오.
audience: admin, publisher, advertiser
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 3fed93f7-1854-440c-802e-6b47e82918c9
source-git-commit: cc74b26091a4f764e200c9cae91316492874551a
workflow-type: tm+mt
source-wordcount: '1191'
ht-degree: 12%

---

# 광고주 또는 게시자와 연결

{{limited-availability-release-note}}

Real-Time CDP Collaboration에서 캠페인을 함께 작업하는 회사에 대해 두 협업 당사자(가장 일반적으로 광고주와 게시자) 간의 연결을 설정하는 것이 전제 조건입니다. 게시자와 광고주 모두 연결을 설정할 수 있습니다. 나중에 연결을 시작하는 상대는 *연결 소유자*&#x200B;가 됩니다.

## 높은 수준 워크플로

높은 수준에서 광고주와 게시자 간에 연결을 설정하려면 워크플로가 다음과 같습니다.

1. 광고주가 함께 작업하려는 게시자를 [검색하고](/help/guide/connect/discover-publishers.md)검색합니다.
2. 광고주가 연결 초대를 보냅니다.
3. 게시자가 초대를 수락합니다.
4. 광고주가 일치 키 등을 포함한 연결 설정을 보냅니다. 이러한 연결 설정은 공동 작업의 제품 내 용어를 나타냅니다.
5. 게시자가 연결 설정을 허용합니다. 원하는 경우 게시자는 초기 연결 설정을 거부하고 광고주가 수정된 연결 설정을 제출하도록 요청할 수 있습니다.

![광고주-게시자 연결 프로세스의 높은 수준 다이어그램입니다.](/help/assets/connect/establish-connection/advertiser-publisher-connection-process.png){zoomable="yes"}

위의 항목이 완료되면 공동 작업자는 [프로젝트 만들기](/help/guide/collaborate/manage-projects.md#create-project)로 진행하여 [중복 보고서를 실행](/help/guide/collaborate/discover.md)하고 광고 캠페인을 시작할 수 있습니다.

>[!IMPORTANT]
>
>두 공동 작업자 간의 연결이 설정되면 연결 설정을 더 이상 수정할 수 없습니다.

## 초대 보내기 {#send-invite}

연결을 설정하려면 게시자 검색 화면에서 게시자 인벤토리를 검색할 때 **[!UICONTROL 연결]**&#x200B;을 선택하십시오.

![연결 선택기](/help/assets/connect/establish-connection/connect-selection.png){zoomable="yes"}

이제 초대가 종료되어 연결 설정을 미리 볼 수 있지만 편집할 수는 없습니다. **[!UICONTROL 내 연결]** 탭에서 보류 중인 초대를 볼 수 있습니다. 연결 상태는 **[!UICONTROL 초대 보냄]**&#x200B;입니다.

![게시자에게 보낸 보류 중인 초대가 내 연결 보기에 표시됩니다.](/help/assets/connect/establish-connection/pending-invite-sent.png){zoomable="yes"}

공동 작업자가 초대를 수락하면 연결 설정을 구성하고 검토 및 수락하도록 공동 작업자에게 보낼 수 있습니다.

## 연결 설정 {#connection-settings}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_usecases"
>title="사용 사례"
>abstract="사용 사례에는 모든 옵션이 미리 채워져 있습니다. 연결 설정을 제출하기 전에 사용 사례를 편집할 수 있습니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_matchkeys"
>title="일치 키"
>abstract="일치 키는 조직 수준에서 선택한 키로 미리 채워집니다. 이 연결에서 사용하지 않으려는 일치 키를 끌 수 있습니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_creditsplit"
>title="크레딧 분할"
>abstract="이 섹션에서는 Real-Time CDP Collaboration 내 해당 활동에 대한 비용을 누가 지불하는지 확인합니다. 현재는 대상자 공유 사용 사례만 구성할 수 있습니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_creditsplit_audiencesharing"
>title="대상자 공유"
>abstract="대상자 공유는 당사자가 공동 작업 파트너에게 일치하는 데이터를 활성화해 달라고 요청할 때 하는 활동입니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_creditsplit_measurement"
>title="측정"
>abstract="이 사용 사례를 사용하면 Real-Time CDP Collaboration에서 활동을 실행하여 캠페인 성과 보고서와 통찰력을 생성할 수 있습니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_legalagreement"
>title="법적 계약"
>abstract="두 당사자 간에 데이터 공유 계약이 있는지 확인합니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_advertisername"
>title="광고주 이름"
>abstract="<p>선택적 설정입니다. 광고주가 게시자에게 알려진 이름 및 ID를 나타냅니다.</p><p>여기에 추가하는 광고주 이름은 프로젝트 만들기 단계에서 미리 채워집니다.</p><ul><li>게시자가 여러 이름을 구성한 경우 목록에서 하나를 선택합니다.</li><li>이름이 하나만 구성된 경우 자동으로 미리 선택됩니다.</li><li>구성된 이름이 없으면 필드에 Real-Time CDP Collaboration의 광고주 계정 이름이 미리 채워집니다.</li></ul>"
>additional-url="https://experienceleague.adobe.com/en/docs/real-time-cdp-collaboration/using/collaborate/manage-projects#create-project" text="프로젝트 만들기"

초대가 전송되면 연결 설정을 미리 볼 수 있습니다. 연결 설정을 완료하려면 먼저 초대를 수락해야 합니다.

![미리 보기 상태의 연결 설정 보기입니다.](/help/assets/connect/establish-connection/preview-connection-settings.png){zoomable="yes"}

이제 공동 작업자가 연결을 수락하면 연결에 대한 연결 설정을 시작할 수 있습니다. 연결 설정은 함께 수행할 사용 사례, 프로젝트에서 사용할 일치 키 등과 같은 공동 작업 조건을 정의합니다.

연결 설정을 설정하고 공동 작업자와 공유하려면 **[!UICONTROL 내 연결]**(으)로 이동합니다. **[!UICONTROL 보류 중]** 상태의 모든 연결에 대해 **[!UICONTROL 연결 설정]**&#x200B;을 선택하여 연결 설정을 구성할 수 있습니다.

![보류 중인 연결이 있는 내 연결 보기와 연결 설정 옵션이 강조 표시되어 있습니다.](/help/assets/connect/establish-connection/pending-connection.png){zoomable="yes"}

아래 필드를 편집하고 정의할 수 있습니다.

![연결 보기 설정](/help/assets/connect/establish-connection/connection-view.png){zoomable="yes"}

+++사용 사례

사용 사례는 사용 가능한 모든 사용 사례로 미리 채워집니다. **[!UICONTROL 편집]**&#x200B;을(를) 선택하고 원하지 않는 사용 사례를 전환하여 연결에서 사용할 사용 사례를 선택할 수 있습니다. 선택한 사용 사례는 프로젝트 내에서 [사용할 수 있는 보기 및 옵션에 영향을 줍니다](../collaborate/manage-projects.md#project-use-cases).

![사용 사례](/help/assets/connect/establish-connection/view-use-cases.png){zoomable="yes"}

+++

+++키 일치

일치 키는 [조직 수준](/help/guide/setup/onboard-organization.md#set-up-match-keys)에서 선택한 키로 미리 채워집니다. 이 연결에 사용하지 않으려는 일치 키를 전환할 수 있지만 조직을 설정할 때 선택하지 않은 일치 키는 추가할 수 없습니다.

![키 일치](/help/assets/connect/establish-connection/match-keys.png)

+++

+++크레딧 분할

신용 분할 섹션을 사용하여 두 협업 당사자 중 어느 쪽이 활동 비용을 부담할지 결정합니다.

![크레딧 분할](/help/assets/connect/establish-connection/edit-billing-ownership.png)

+++

+++계약

이 연결을 계속 진행하려면 먼저 두 당사자 간의 데이터 공유 계약이 있음을 확인해야 합니다.

![법적 계약.](/help/assets/connect/establish-connection/legal-agreement.png)

+++

+++광고주 이름

연결 설정을 작업 중인 게시자는 시스템에서 광고주가 알고 있는 광고주 이름을 추가하도록 선택할 수 있습니다. 게시자는 함께 일하는 광고주가 여러 지역에 있는 경우 등 여러 광고주 이름을 연결에 추가할 수 있습니다. 나중에 [공동 작업할 프로젝트를 만들기](/help/guide/collaborate/manage-projects.md#create-project)하면 귀하 또는 공동 작업자가 프로젝트와 연결할 광고주 이름을 선택할 수 있습니다.

![광고주 이름 추가 모달](/help/assets/connect/establish-connection/add-advertiser-names-modal.png)

다음은 프로젝트를 만들 때 광고주 이름 선택이 작동하는 방식입니다.

1. **광고주 이름이 설정되지 않음**: 광고주 이름이 추가되지 않으면 Real-Time CDP Collaboration에서 광고주 이름으로 광고주 이름을 사용하는 것으로 기본 설정됩니다.
2. **광고주 이름 집합 하나**: 단일 광고주 이름이 추가되면 Real-Time CDP Collaboration은 자동으로 해당 이름을 프로젝트의 광고주 이름으로 사용합니다.
3. **여러 광고주 이름 집합**: 둘 이상의 광고주 이름이 추가되면 프로젝트를 만들 때 사용자 또는 공동 작업자가 제공된 이름을 선택할 수 있습니다.

![광고주 이름](/help/assets/connect/establish-connection/advertiser-names.png)

+++

선택을 마치면 **[!UICONTROL 제출]**&#x200B;을 선택하여 제안된 설정을 공동 작업자에게 보내 검토하도록 합니다.

공동 작업자로부터 제안된 연결 설정을 받는 경우 해당 설정을 **[!UICONTROL 수락]**&#x200B;하거나 **[!UICONTROL 거부]**&#x200B;할 수 있습니다. 연결 설정을 수락하기 전에 귀하와 공동 작업자 간에 법적 계약이 적용되었는지 확인하고 승인해야 합니다. 연결 설정을 거부하는 경우 제품 외부에 있는 공동 작업자에게 연락하여 연결 설정을 어떻게 수정해야 수락할 수 있는지 논의하십시오.

## 연결 삭제 {#delete-connections}

계속 작업하지 않으려는 공동 작업자와의 연결을 삭제할 수 있습니다. 기존 연결을 삭제하려면

1. **[!UICONTROL 연결]** > **[!UICONTROL 내 연결]**(으)로 이동합니다.
2. 삭제할 연결에 액세스하려면 연결 카드에서 **[!UICONTROL 연결 보기]**&#x200B;를 선택하십시오.
3. 삭제 아이콘 ![삭제 아이콘](/help/assets/common/delete.svg)을 선택하여 연결 삭제 확인 대화 상자를 표시합니다.
   ![연결 삭제 아이콘이 강조 표시되어 있습니다.](/help/assets/connect/establish-connection/delete-icon-highlighted.png){zoomable="yes"}
4. **[!UICONTROL 삭제]**&#x200B;를 선택하여 삭제를 확인합니다.
   ![연결 삭제를 확인하는 대화 상자. ](/help/assets/connect/establish-connection/delete-connection-dialog.png){zoomable="yes"}

>[!WARNING]
>
>연결이 삭제되면 더 이상 공동 작업자와 연결되지 않으며 공동 작업에 포함된 모든 기존 프로젝트가 영구적으로 삭제되고 복구할 수 없습니다.

## 다음 단계

이제 공동 작업자와 연결을 설정한 후 귀하와 공동 작업자는 [프로젝트를 만들](/help/guide/collaborate/manage-projects.md#create-project)수 있습니다.
