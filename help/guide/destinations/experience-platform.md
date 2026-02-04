---
title: Adobe Experience Platform을 대상으로 구성
description: Real-Time CDP Collaboration에서 대상으로 Adobe Experience Platform을 구성하고 관리하는 방법에 대해 알아봅니다.
audience: admin, publisher, advertiser
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/kr/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 594610a0-9102-448a-b59b-ec162ef9dd57
source-git-commit: 0dead396657c97cec47ddd64c8ec3c349f541a8f
workflow-type: tm+mt
source-wordcount: '1489'
ht-degree: 11%

---

# Adobe Experience Platform을 대상으로 구성

{{limited-availability-release-note}}

프로젝트에서 Adobe Experience Platform으로 대상을 활성화하도록 이 대상을 구성합니다. 대상을 Adobe Experience Platform으로 활성화하면 다양한 마케팅 채널에서 대상 세분화, 분석 및 활성화를 위해 플랫폼의 기능을 활용할 수 있습니다. Adobe Experience Platform에 대한 자세한 내용은 [Experience Platform 개요](https://experienceleague.adobe.com/ko/docs/experience-platform/landing/home){target="_blank"}를 참조하세요.

>[!WARNING]
>
>대상을 만든 후에는 업데이트할 수 없습니다. 설정을 변경해야 하는 경우 기존 대상을 삭제하고 새 대상을 만들어야 합니다.

## 대상 구성 {#configure-destination}

Adobe Experience Platform을 대상으로 구성하려면 **[!UICONTROL 설정]**(으)로 이동한 다음 **[!UICONTROL 내 대상]** 탭을 선택합니다. Adobe Experience Platform에 대해 **[!UICONTROL 설정]**&#x200B;을 선택합니다.

![Adobe Experience Platform 대상에 대해 [설정] 옵션이 강조 표시된 내 대상 작업 영역입니다.](/help/assets/destinations/adobe-experience-platform/setup-aep.png)

**[!UICONTROL 대상 만들기]** 워크플로가 나타납니다.

![Adobe Experience Platform에 대한 대상 워크플로우를 만듭니다.](/help/assets/destinations/adobe-experience-platform/create-destination.png)

### 샌드박스 구성 {#configure-sandbox}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_audience_expiration"
>title="대상자 만료"
>abstract="이 기간이 지나면 Adobe Experience Platform에서 더 이상 대상자를 사용할 수 없습니다. 기본 만료일은 30일이며, 1일에서 30일 사이의 값으로 설정할 수 있습니다."

먼저 대상 데이터를 전송할 샌드박스를 선택해야 합니다.

>[!IMPORTANT]
>
>사용자가 액세스할 수 있는 샌드박스만 선택할 수 있습니다. 기본적으로 모든 Collaboration 사용자는 **Prod** 샌드박스에 액세스할 수 있습니다. 추가 샌드박스에 대한 액세스 권한을 얻으려면 관리자가 사용자에게 할당된 역할에 추가 샌드박스를 추가해야 합니다. 역할 관리에 대한 자세한 내용은 [역할 관리](../permissions/manage-roles.md) 안내서를 참조하세요.

**[!UICONTROL 샌드박스 구성]** 섹션에서 **[!UICONTROL 샌드박스]** 드롭다운을 선택하거나 샌드박스 이름을 입력합니다.

![대상 만들기 워크플로에서 강조 표시된 샌드박스 드롭다운입니다.](/help/assets/destinations/adobe-experience-platform/select-sandbox.png)

또는 **[!UICONTROL 샌드박스 찾아보기]**&#x200B;를 선택하여 사용 가능한 모든 샌드박스와 **[!UICONTROL 유형]**, **[!UICONTROL 상태]** 및 **[!UICONTROL 지역]**&#x200B;을 볼 수 있습니다. 사용할 샌드박스를 선택한 다음 **[!UICONTROL 저장]**&#x200B;을 선택합니다.

그런 다음 **[!UICONTROL 대상 만료]**&#x200B;을(를) 구성합니다. 기본적으로 대상 만료는 30일로 설정됩니다. 만료를 1일에서 30일 사이로 설정하도록 선택할 수 있습니다. 만료 날짜 이후, Adobe Experience Platform에서는 더 이상 대상을 사용할 수 없습니다.

![대상 만들기 워크플로에서 강조 표시된 대상 만료 섹션입니다.](/help/assets/destinations/adobe-experience-platform/audience-expiration.png)

### 활성화 매핑 만들기 {#create-activation-mapping}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_activation_matchkeys"
>title="활성화 매칭 키"
>abstract="활성화 매칭 키는 조직을 생성할 때 선택한 매칭 키를 기준으로 표시됩니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_activation_mapping"
>title="자세히 보기"
>abstract=""

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_target_namespaces"
>title="대상 네임스페이스"
>abstract="대상 네임스페이스는 Adobe Experience Platform에서 일치 키가 매핑될 ID 네임스페이스를 지정합니다. 해시 처리된 일치 키는 해시 값을 지원하는 대상 네임스페이스에 매핑되어야 합니다."

계정에 대해 활성화된 모든 일치 키는 기본적으로 활성화 매핑에 포함됩니다. 일치 키를 대상 네임스페이스에 직접 매핑하지 않으려면 연결된 키 옵션을 사용하여 다른 일치 키로 바꿀 수 있습니다. 연결된 키에 대한 자세한 내용은 아래 [섹션](#linked-keys)을 참조하세요.

#### 타겟 네임스페이스 매핑 {#map-target-namespaces}

각 일치 키를 대상 네임스페이스에 매핑하려면 일치 키 옆에 있는 **[!UICONTROL 대상 네임스페이스]** 필드를 선택합니다. **[!UICONTROL 소스 필드 선택]** 대화 상자가 나타납니다. 목록에서 대상 네임스페이스를 찾거나 특정 네임스페이스를 검색합니다. 일치 키에 사용할 대상 네임스페이스를 선택한 다음 **[!UICONTROL 선택]**&#x200B;을(를) 선택합니다.

>[!IMPORTANT]
>
>해시된 일치 키는 해시된 값을 지원하는 대상 네임스페이스에 매핑되어야 합니다. 예를 들어 **[!UICONTROL 해시된 이메일]** 일치 키는 Adobe Experience Platform의 **[!UICONTROL 이메일(SHA256, 소문자)]** ID 네임스페이스에 매핑되어야 합니다. **[!UICONTROL 해시된 이메일]** 일치 키를 **[!UICONTROL 이메일]** ID 네임스페이스에 매핑할 수 없습니다. 이 네임스페이스는 해시된 값을 지원하지 않습니다.

![선택 옵션이 강조 표시된 원본 필드 선택 대화 상자..](/help/assets/destinations/adobe-experience-platform/select-target-namespace.png)

활성화 매핑에 포함할 각 일치 키에 대해 이 프로세스를 반복합니다. 일치 키를 포함하지 않으려는 경우 해당 키를 제거하거나 연결된 키 옵션을 사용하여 다른 일치 키로 바꿀 수 있습니다.

#### 링크된 키 {#linked-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_linked_key"
>title="링크된 키"
>abstract="링크된 키를 사용하면 활성화 중에 원래 일치 키 대신 다른 일치 키를 사용하도록 지정할 수 있습니다. 프로필을 활성화하려면 원래 일치 키와 링크된 키 모두에 대한 값이 있어야 합니다."

링크된 키를 사용하면 활성화 중에 원래 일치 키 대신 다른 일치 키를 사용하도록 지정할 수 있습니다. 연결된 키가 작동하는 방식을 더 잘 이해하려면 다음 예를 고려하십시오.

retailer은 활성화된 데이터를 Experience Platform에서 해당 CRM 시스템으로 보내려고 합니다. retailer은 해시된 IP를 계정의 일치 키로 활성화하여 대상을 활성화할 때 일치율을 높였습니다. 그러나 retailer의 CRM 시스템은 해시된 IP를 ID 네임스페이스로 지원하지 않으므로 Experience Platform에 대상을 활성화할 때 대신 CRM ID 일치 키를 사용하려고 합니다. retailer은 연결된 키 옵션을 사용하여 해시된 IP 대신 CRM ID를 사용하여 Experience Platform에 대상을 활성화할 수 있습니다.

>[!NOTE]
>
>프로필이 활성화되려면 원래 일치 키와 연결된 일치 키 모두에 대한 값이 있어야 합니다. 예를 들어 해시된 ID가 CRM ID에 연결되어 있는 경우 프로필에는 활성화하려는 해시된 ID와 CRM ID에 대한 값이 있어야 합니다. 두 값 중 하나가 누락된 경우 프로필은 활성화되지 않습니다.

연결된 키를 사용하려면 해당 위치에 사용할 일치 키 옆의 **[!UICONTROL 연결된 키]** 옵션을 켜십시오. **[!UICONTROL 연결된 키]** 섹션이 표시되어 매핑을 만들도록 요청합니다.

![대상 만들기 워크플로에서 강조 표시된 연결된 키 옵션 및 섹션입니다.](/help/assets/destinations/adobe-experience-platform/linked-key.png)

드롭다운 메뉴에서 사용할 **[!UICONTROL 연결된 키]**&#x200B;를 선택합니다. 위의 예제에 따라 retailer은 **[!UICONTROL CRM ID]**&#x200B;을 연결된 키로 선택합니다.

![대상 만들기 워크플로에서 강조 표시된 연결된 키 드롭다운입니다.](/help/assets/destinations/adobe-experience-platform/select-linked-key.png)

다음으로, 아직 지정하지 않은 경우 연결된 키의 대상 네임스페이스를 지정합니다. **[!UICONTROL 활성화 매핑 만들기]** 섹션에서 일치 키에 대한 대상 네임스페이스를 이미 선택한 경우 자동으로 채워집니다. 연결된 키에 대한 대상 네임스페이스를 아직 선택하지 않은 경우 지금 선택할 수 있습니다.

연결된 키 옆의 **[!UICONTROL 대상 네임스페이스]** 필드를 선택합니다. **[!UICONTROL 소스 필드 선택]** 대화 상자가 나타납니다. 목록에서 대상 네임스페이스를 찾거나 특정 네임스페이스를 검색합니다. 연결된 키에 사용할 대상 네임스페이스를 선택한 다음 **[!UICONTROL 선택]**&#x200B;을(를) 선택합니다.

![소스 필드 선택 대화 상자](/help/assets/destinations/adobe-experience-platform/select-linked-key-target-namespace.png)

이제 연결된 키가 구성되었습니다.

>[!NOTE]
>
>활성화 매핑당 연결된 키 대상 네임스페이스는 하나만 사용할 수 있습니다. 예를 들어 해시된 ID를 CRM ID에 연결하는 경우 다른 필드에 대해 연결된 키 옵션을 토글하면 CRM ID에도 연결됩니다.

모든 일치 키 매핑을 완료했으면 설정을 검토하십시오. **[!UICONTROL 미리 보기]** 섹션에서 구성에 대한 요약을 제공합니다.

![대상 만들기 워크플로의 미리 보기 섹션입니다.](/help/assets/destinations/adobe-experience-platform/preview.png)

>[!IMPORTANT]
>
>현재 각 일치 키는 별도의 대상으로 Experience Platform에 대해 활성화됩니다. 예를 들어 일치 키로 [!UICONTROL 해시된 이메일] 및 [!UICONTROL 해시된 전화]가 있는 경우 대상이 활성화되면 Audience Portal에 두 개의 개별 대상이 만들어집니다.

구성에 만족하면 **[!UICONTROL 대상 만들기]**&#x200B;를 선택하세요. 대상이 성공적으로 생성되었음을 나타내는 확인 메시지가 나타납니다.

## Adobe Experience Platform을 대상으로 사용

Experience Platform을 대상으로 구성하면 프로젝트를 통해 플랫폼에 대한 [대상자 활성화](../collaborate/activate.md)를 시작할 수 있습니다. 현재 활성화 프로세스는 공동 작업자가 시작한 단일 단계 프로세스입니다. 예를 들어 광고주가 대상을 활성화하면 게시자의 사전 구성된 대상(Experience Platform)으로 전송됩니다. 대상자를 대상으로 보내기 위해 게시자가 추가적인 단계를 수행할 필요가 없습니다. 브랜드 간 공동 작업 패턴도 마찬가지입니다.

>[!IMPORTANT]
>
>**해야** Experience Platform을 대상으로 *이전*(으)로 구성해야 합니다. 대상이 구성되지 않은 경우 대상자가 사용자에게 전송되고 프로젝트 내의 **[!UICONTROL 활성화]** 탭에 표시되지만 Experience Platform에는 활성화되지 않습니다.

대상자가 활성화되면 Real-Time CDP Collaboration을 원본으로 하는 Experience Platform의 [대상자 포털](#audience-portal)에서 사용할 수 있습니다.  그런 다음 이러한 대상을 캠페인 및 고객 참여에 사용할 수 있습니다.

### 대상자 포털 {#audience-portal}

Adobe Experience Platform을 대상으로 구성했으므로 이제 대상자 포털에서 활성화된 대상자를 볼 수 있습니다. 대상 포털은 대상을 보고 관리할 수 있는 Adobe Experience Platform 내의 중앙 허브입니다. 이제 대상 포털에서 대상을 필터링할 때 Real-Time CDP Collaboration을 원본으로 제공합니다.

>[!IMPORTANT]
>
>Adobe Experience Platform에 활성화한 대상에 필요한 데이터 사용 레이블을 적용할 책임이 있습니다. 자세한 내용은 [데이터 사용 레이블](https://experienceleague.adobe.com/ko/docs/experience-platform/data-governance/labels/overview){target="_blank"} 안내서를 참조하십시오.

![필터 옵션에서 Real-Time CDP Collaboration을 원본으로 사용하는 대상 포털입니다.](/help/assets/destinations/adobe-experience-platform/audience-portal.png)

Audience Portal에 대한 자세한 내용은 [Audience Portal 개요](https://experienceleague.adobe.com/ko/docs/experience-platform/segmentation/ui/audience-portal#manage-audiences){target="_blank"} 안내서를 참조하십시오.
