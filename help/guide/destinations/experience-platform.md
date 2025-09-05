---
title: Adobe Experience Platform을 대상으로 구성
description: Real-Time CDP Collaboration에서 대상으로 Adobe Experience Platform을 구성하고 관리하는 방법에 대해 알아봅니다.
audience: admin, publisher, advertiser
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/kr/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 594610a0-9102-448a-b59b-ec162ef9dd57
source-git-commit: f13b0996c35bcb6060c583ca328c2c04daaf8abc
workflow-type: tm+mt
source-wordcount: '874'
ht-degree: 11%

---

# Adobe Experience Platform을 대상으로 구성

{{limited-availability-release-note}}

프로젝트에서 Adobe Experience Platform으로 대상을 활성화하도록 이 대상을 구성합니다. 대상을 Adobe Experience Platform으로 활성화하면 다양한 마케팅 채널에서 대상 세분화, 분석 및 활성화를 위해 플랫폼의 기능을 활용할 수 있습니다. Adobe Experience Platform에 대한 자세한 내용은 [Experience Platform 개요](https://experienceleague.adobe.com/ko/docs/experience-platform/landing/home){target="_blank"}를 참조하세요.

## 대상 구성 {#configure-destination}

Adobe Experience Platform을 대상으로 구성하려면 **[!UICONTROL 설정]**(으)로 이동한 다음 **[!UICONTROL 대상]** 탭을 선택합니다. Adobe Experience Platform에 대해 **[!UICONTROL 설정]**&#x200B;을 선택합니다.

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
>title="활성화 일치 키"
>abstract="활성화 일치 키는 조직을 생성할 때 선택한 일치 키를 기준으로 표시됩니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_target_namespaces"
>title="대상 네임스페이스"
>abstract="대상 네임스페이스는 Adobe Experience Platform에서 일치 키가 매핑될 ID 네임스페이스를 지정합니다. 해시 처리된 일치 키는 해시 값을 지원하는 대상 네임스페이스에 매핑되어야 합니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_linked_key"
>title="링크된 키"
>abstract="연결된 주요 상황별 도움말에 대한 자리 표시자"

다음으로, 대상자 데이터가 Adobe Experience Platform으로 전송되는 방법을 정의하기 위해 활성화 매핑을 만들어야 합니다. 조직을 만드는 동안 선택한 각 [일치 키](../setup/onboard-account.md#set-up-match-keys)를 대상 네임스페이스에 매핑할 수 있습니다. 대상 네임스페이스는 Adobe Experience Platform에서 일치 키가 매핑될 [ID 네임스페이스](https://experienceleague.adobe.com/ko/docs/experience-platform/identity/features/namespaces#standard){target="_blank"}를 지정합니다.

>[!IMPORTANT]
>
>해시된 일치 키는 해시된 값을 지원하는 대상 네임스페이스에 매핑되어야 합니다. 예를 들어 **[!UICONTROL 해시된 이메일]** 일치 키는 Adobe Experience Platform의 **[!UICONTROL 이메일(SHA256, 소문자)]** ID 네임스페이스에 매핑되어야 합니다. **[!UICONTROL 해시된 이메일]** 일치 키를 **[!UICONTROL 이메일]** ID 네임스페이스에 매핑할 수 없습니다. 이 네임스페이스는 해시된 값을 지원하지 않습니다.

각 일치 키 옆에 있는 **[!UICONTROL 대상 네임스페이스]** 필드를 선택합니다. **[!UICONTROL 소스 필드 선택]** 대화 상자가 나타납니다. 목록에서 대상 네임스페이스를 찾거나 특정 네임스페이스를 검색합니다. 일치 키에 사용할 대상 네임스페이스를 선택한 다음 **[!UICONTROL 선택]**&#x200B;을(를) 선택합니다.

![선택 옵션이 강조 표시된 원본 필드 선택 대화 상자..](/help/assets/destinations/adobe-experience-platform/select-target-namespace.png)

모든 일치 키 매핑을 마쳤으면 설정을 검토한 다음 **[!UICONTROL 만들기]**&#x200B;를 선택하여 대상 만들기를 완료합니다.

## Adobe Experience Platform을 대상으로 사용

Adobe Experience Platform을 대상으로 구성하면 프로젝트를 통해 플랫폼에 대한 [대상자 활성화](../collaborate/activate.md)를 시작할 수 있습니다. 현재 활성화 과정은 광고주가 시작한 단일 단계 과정이다. 광고주가 대상을 활성화하면 게시자의 사전 구성된 대상(이 경우 Adobe Experience Platform)으로 전송됩니다. 대상자를 대상으로 보내기 위해 게시자가 추가적인 단계를 수행할 필요가 없습니다.

>[!IMPORTANT]
>
>**해야** Adobe Experience Platform을 대상으로 *이전*(으)로 구성해야 합니다. 대상이 구성되지 않은 경우 대상자가 사용자에게 전송되고 프로젝트 내의 **[!UICONTROL 활성화]** 탭에 표시되지만 Adobe Experience Platform에는 활성화되지 않습니다.

대상자가 활성화되면 Real-Time CDP Collaboration을 원본으로 하는 Experience Platform의 [대상자 포털](#audience-portal)에서 사용할 수 있습니다.  그런 다음 이러한 대상을 캠페인 및 고객 참여에 사용할 수 있습니다.

### 대상자 포털 {#audience-portal}

Adobe Experience Platform을 대상으로 구성했으므로 이제 대상자 포털에서 활성화된 대상자를 볼 수 있습니다. 대상 포털은 대상을 보고 관리할 수 있는 Adobe Experience Platform 내의 중앙 허브입니다. 이제 대상 포털에서 대상을 필터링할 때 Real-Time CDP Collaboration을 원본으로 제공합니다.

>[!IMPORTANT]
>
>Adobe Experience Platform에 활성화한 대상에 필요한 데이터 사용 레이블을 적용할 책임이 있습니다. 자세한 내용은 [데이터 사용 레이블](https://experienceleague.adobe.com/ko/docs/experience-platform/data-governance/labels/overview){target="_blank"} 안내서를 참조하십시오.

![필터 옵션에서 Real-Time CDP Collaboration을 원본으로 사용하는 대상 포털입니다.](/help/assets/destinations/adobe-experience-platform/audience-portal.png)

Audience Portal에 대한 자세한 내용은 [Audience Portal 개요](https://experienceleague.adobe.com/ko/docs/experience-platform/segmentation/ui/audience-portal#manage-audiences){target="_blank"} 안내서를 참조하십시오.
