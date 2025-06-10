---
title: 광고주 또는 게시자와 연결
description: 잠재적 공동 작업자를 발견한 후 연결을 설정하고 프로젝트에 대한 공동 작업을 시작하는 방법에 대해 알아보십시오.
audience: admin, publisher, advertiser
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 3fed93f7-1854-440c-802e-6b47e82918c9
source-git-commit: 3615d969ff6e0ff95304a02346845909f3f8258c
workflow-type: tm+mt
source-wordcount: '1401'
ht-degree: 6%

---

# 광고주 또는 게시자와 연결

{{limited-availability-release-note}}

공동 작업자(일반적으로 광고주와 게시자)가 캠페인에 대해 함께 작업하려면 먼저 연결을 설정해야 합니다. 이 연결을 통해 대상자를 활성화하고, 프로젝트를 만들고, 캠페인 성과에 대한 보고서를 실행할 수 있습니다.

## 높은 수준 워크플로

광고주와 게시자 간에 연결을 설정하려면 다음 단계를 수행해야 합니다.

1. 광고주가 [게시자를 검색하고](/help/guide/connect/discover-publishers.md)게시자가 작업하려는 게시자를 검색합니다.
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

![특정 게시자에서 연결 옵션이 강조 표시된 연결 대시보드입니다.](/help/assets/connect/establish-connection/connect-selection.png){zoomable="yes"}

초대가 전송되면 연결 설정을 미리 볼 수 있지만 편집할 수는 없습니다. **[!UICONTROL 내 연결]** 탭에서 보류 중인 초대를 봅니다. 연결 상태가 **[!UICONTROL 초대가 전송됨]**(으)로 표시됩니다.

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
>abstract="이 섹션에서는 Real-Time CDP Collaboration 내에서 해당 활동에 대해 지불하는 사용자를 결정합니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_creditsplit_audiencesharing"
>title="대상자 공유"
>abstract="대상자 활성화 크레딧은 활성화를 위해 준비된 일치하는 ID 수에 따라 사용됩니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_creditsplit_measurement"
>title="측정"
>abstract="활동을 실행하여 캠페인 성과 보고서와 통찰력을 생성합니다. 크레딧은 모든 캠페인의 캠페인 보고서 행 수 및 보고 빈도를 기반으로 사용됩니다(매일, 3일마다 또는 매주)."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_legalagreement"
>title="법적 계약"
>abstract="두 당사자 간에 데이터 공유 계약이 있는지 확인합니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_advertisername"
>title="광고주 이름"
>abstract="<p>선택적 설정입니다. 광고주가 게시자에게 알려진 이름 및 ID를 나타냅니다.</p><p>여기에 추가하는 광고주 이름은 프로젝트 만들기 단계에서 미리 채워집니다.</p><ul><li>게시자가 여러 이름을 구성한 경우 목록에서 하나를 선택합니다.</li><li>이름이 하나만 구성된 경우 자동으로 미리 선택됩니다.</li><li>구성된 이름이 없으면 필드에 Real-Time CDP Collaboration의 광고주 계정 이름이 미리 채워집니다.</li></ul>"
>additional-url="https://experienceleague.adobe.com/en/docs/real-time-cdp-collaboration/using/collaborate/manage-projects#create-project" text="프로젝트 만들기"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_audience_activation"
>title="대상자 활성화"
>abstract="대상 활성화를 사용하면 대상 활성화를 시작할 수 있는 공동 작업자를 선택할 수 있습니다."

<!-- Move and update the above popover when bidirectional is active. -->

초대가 전송되면 연결 설정을 미리 볼 수 있습니다. 연결 설정을 완료하려면 먼저 초대를 수락해야 합니다.

![미리 보기 상태의 연결 설정 보기입니다.](/help/assets/connect/establish-connection/preview-connection-settings.png){zoomable="yes"}

### 광고주 연결 설정 {#advertiser-connection-settings}

공동 작업자가 연결을 수락하면 연결 설정을 설정합니다. 이러한 설정은 작업할 사용 사례, 프로젝트의 일치 키 및 기타 구성을 포함한 공동 작업 조건을 정의합니다.

시작하려면 **[!UICONTROL 내 연결]**(으)로 이동합니다. **[!UICONTROL 보류 중]** 상태의 모든 연결에 대해 **[!UICONTROL 연결 설정]**&#x200B;을 선택하여 연결 설정을 구성할 수 있습니다.

![보류 중인 연결 및 연결 설정 옵션이 강조 표시된 내 연결 작업 영역입니다.](/help/assets/connect/establish-connection/pending-connection.png){zoomable="yes"}

아래 필드를 편집하고 정의할 수 있습니다.

![채우기 전 연결 설정 작업 영역입니다.](/help/assets/connect/establish-connection/connection-view.png){zoomable="yes"}

+++사용 사례

사용 사례에는 사용 가능한 모든 옵션이 미리 채워져 있습니다. 이를 사용자 지정하려면 **[!UICONTROL 사용 사례]** 섹션에서 **[!UICONTROL 편집]**&#x200B;을(를) 선택하고 원하지 않는 항목을 끕니다. 선택한 사용 사례는 [프로젝트 내에서 사용할 수 있는 보기 및 옵션](../collaborate/manage-projects.md#project-use-cases)을 결정합니다.

![연결 설정 작업 영역의 사용 사례 설정입니다.](/help/assets/connect/establish-connection/view-use-cases.png){zoomable="yes"}

+++

+++키 일치

일치 키는 [조직을 설정하는 동안](/help/guide/setup/onboard-organization.md#set-up-match-keys)선택한 키로 미리 채워집니다. 사용하지 않을 일치 키를 전환할 수 있지만 조직 설정 중에 선택되지 않은 일치 키는 추가할 수 없습니다.

![연결 설정 작업 영역의 일치 키 설정입니다.](/help/assets/connect/establish-connection/match-keys.png){zoomable="yes"}

+++

+++크레딧 분할

신용 분할 섹션을 사용하여 두 협업 당사자 중 어느 쪽이 활동 비용을 부담할지 결정합니다. 신용 분할 옵션은 연결에 대해 선택한 사용 사례에 따라 결정됩니다. **[!UICONTROL Measurement]** 사용 사례에서는 한 당사자가 비용을 부담해야 하지만 **[!UICONTROL 활성화 - 일치]** 사용 사례에서는 각 당사자가 자신의 비용을 부담하도록 하는 추가 옵션을 제공합니다. 비용 분류에 대한 자세한 내용은 [신용 활동 유형](/help/guide/setup/my-activity.md#types-of-activities) 안내서를 참조하십시오.

>[!NOTE]
>
>대상자 - 이그레스는 항상 대상자를 받는 공동 작업자가 적용하므로 선택할 필요가 없습니다.

![연결 작업 영역에 옵션이 있는 신용 분할 대화 상자.](/help/assets/connect/establish-connection/credit-split.png){zoomable="yes"}
+++

+++계약

이 연결을 계속 진행하려면 먼저 두 당사자 간의 데이터 공유 계약이 있음을 확인해야 합니다.

![법률 계약 섹션이 연결 작업 영역에서 강조 표시되고 확인되었습니다.](/help/assets/connect/establish-connection/legal-agreement.png){zoomable="yes"}

+++

선택을 마치면 **[!UICONTROL 제출]**&#x200B;을 선택하여 제안된 설정을 공동 작업자에게 보내어 검토하십시오.

### 게시자 연결 설정 {#publisher-connection-settings}

그러면 게시자는 연결 설정을 검토하고 이를 수락 또는 거부해야 합니다. 연결 설정을 검토하려면 **[!UICONTROL 내 연결]**(으)로 이동하여 연결 카드에서 **[!UICONTROL 연결 설정 검토]**&#x200B;를 선택하십시오.

![내 연결 보기에서 강조 표시된 연결 설정 검토 옵션입니다.](/help/assets/connect/establish-connection/review-connection-settings.png){zoomable="yes"}

공동 작업자가 제안한 설정을 검토합니다. 연결 설정을 수락하기 전에 귀하와 공동 작업자 사이에 법적 계약이 있음을 확인해야 합니다. 또한 시스템에서 광고주가 알려지는 광고주 이름을 추가할 수 있습니다.

![공동 작업자의 제안된 설정과 광고주 이름 및 계약 섹션이 강조 표시된 연결 설정 작업 영역입니다.](/help/assets/connect/establish-connection/publisher-connection-settings.png){zoomable="yes"}

+++광고주 이름

연결 설정을 작업 중인 게시자는 시스템에서 광고주가 알고 있는 광고주 이름을 추가하도록 선택할 수 있습니다. 게시자는 함께 일하는 광고주가 여러 지역에 있는 경우 등 여러 광고주 이름을 연결에 추가할 수 있습니다. 나중에 [공동 작업할 프로젝트를 만들기](/help/guide/collaborate/manage-projects.md#create-project)하면 귀하 또는 공동 작업자가 프로젝트와 연결할 광고주 이름을 선택할 수 있습니다.

![연결 설정 작업 영역의 광고주 이름 대화 상자입니다.](/help/assets/connect/establish-connection/add-advertiser-names-modal.png)

다음은 프로젝트를 만들 때 광고주 이름 선택이 작동하는 방식입니다.

1. **광고주 이름이 설정되지 않음**: 광고주 이름이 추가되지 않으면 Real-Time CDP Collaboration에서 광고주 이름으로 광고주 이름을 사용하는 것으로 기본 설정됩니다.
2. **광고주 이름 집합 하나**: 단일 광고주 이름이 추가되면 Real-Time CDP Collaboration은 자동으로 해당 이름을 프로젝트의 광고주 이름으로 사용합니다.
3. **여러 광고주 이름 집합**: 둘 이상의 광고주 이름이 추가되면 프로젝트를 만들 때 사용자 또는 공동 작업자가 제공된 이름을 선택할 수 있습니다.

![광고주 이름 섹션이 채워진 연결 설정 작업 영역입니다.](/help/assets/connect/establish-connection/advertiser-names.png)

+++

>[!NOTE]
>
> 연결 설정을 수락하면 더 이상 광고주 이름을 추가하거나 편집할 수 없습니다.

제안된 연결 설정에 만족하면 **[!UICONTROL 수락]**&#x200B;을 선택하여 연결을 설정하십시오. 연결 설정 변경을 요청하려면 **[!UICONTROL 거부]**&#x200B;를 선택합니다. 그런 다음 공동 작업자가 연결 설정을 수정하고 다시 보내어 검토할 수 있습니다.

## 연결 삭제 {#delete-connections}

계속 작업하지 않으려는 공동 작업자와의 연결을 삭제할 수 있습니다. 기존 연결을 삭제하려면 **[!UICONTROL 연결]**(으)로 이동합니다. 그러면 광고주가 **[!UICONTROL 내 연결]**(으)로 이동해야 합니다. 삭제할 연결을 열려면 연결 카드에서 **[!UICONTROL 연결 보기]**&#x200B;를 선택하십시오.

![내 연결 보기에서 강조 표시된 연결 보기 옵션입니다.](/help/assets/connect/establish-connection/delete-view-connection.png){zoomable="yes"}

연결을 삭제하려면 연결 작업 영역에서 삭제 아이콘 ![삭제 아이콘](/help/assets/common/delete.svg)을(를) 선택하십시오.

![연결 작업 영역에서 강조 표시된 삭제 아이콘입니다.](/help/assets/connect/establish-connection/delete-option.png){zoomable="yes"}

연결 삭제를 확인하는 확인 대화 상자가 나타납니다. **[!UICONTROL 삭제]**&#x200B;를 선택하여 삭제를 확인합니다.

![연결을 삭제하는 확인 대화 상자입니다.](/help/assets/connect/establish-connection/delete-confirmation-dialog.png){zoomable="yes"}

>[!WARNING]
>
>연결이 삭제되면 더 이상 공동 작업자와 연결되지 않으며 공동 작업에 포함된 모든 기존 프로젝트가 영구적으로 삭제되고 복구할 수 없습니다.

## 다음 단계

이제 공동 작업자와 연결을 설정한 후 귀하와 공동 작업자는 [프로젝트를 만들](/help/guide/collaborate/manage-projects.md#create-project)수 있습니다.
