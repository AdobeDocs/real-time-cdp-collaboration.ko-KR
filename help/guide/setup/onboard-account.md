---
title: 계정 구성 및 관리
description: Real-Time CDP Collaboration에서 계정의 다양한 측면을 구성하고 관리하는 방법에 대해 알아봅니다
audience: admin, publisher, advertiser
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: a95e932a-9681-48f2-bf34-6fe5a50597d7
source-git-commit: 608706d00124372ac59209478ab551a3a6ce0226
workflow-type: tm+mt
source-wordcount: '937'
ht-degree: 13%

---

# 계정 구성 및 관리

{{limited-availability-release-note}}

Real-Time CDP Collaboration에서 계정을 설정하여 다른 공동 작업자와의 연결을 준비하는 방법에 대해 알아봅니다. 이 안내서에서는 계정 세부 정보 추가, 일치 키 선택 및 계정 설정 관리를 포함하여 계정의 초기 설정을 다룹니다.

![구성된 계정을 표시하는 설치 작업 영역입니다.](/help/assets/setup/manage-account/my-account.png){zoomable="yes"}

## 계정 설정 {#set-up-account}

Collaboration에 처음 액세스하면 계정을 설정하라는 메시지가 표시됩니다. 계정 세부 정보를 구성하고 키를 일치시킬 수 있는 일회성 프로세스입니다. 조직의 첫 번째 계정인 경우 [계정 세부 정보](#set-up-details) 설정을 시작으로 온보딩 프로세스를 즉시 진행합니다.

조직을 추가하려면 왼쪽 레일에서 **[!UICONTROL 설정]**(으)로 이동하여 추가 아이콘(![추가 아이콘)을 선택하십시오.](/help/assets/icons/plus.png))을(를) 오른쪽 위 모서리에서 찾을 수 있습니다. **[!UICONTROL 계정]**&#x200B;을(를) 선택합니다.

![[내 계정] 탭과 [계정] 옵션이 강조 표시된 설치 작업 영역입니다.](/help/assets/setup/manage-account/add-new-account.png){zoomable="yes"}

### 세부 정보 설정 {#set-up-details}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_setup_contact_email"
>title="연락처 이메일"
>abstract="팀 또는 역할 기반 전자 메일을 제공하십시오(예: **collaboration@yourcompany.com**). 개인 또는 개별 이메일 주소는 사용할 수 없습니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_setup_connect_code"
>title="연결 코드"
>abstract="연결 코드는 계정의 고유 식별자입니다. Real-Time CDP Collaboration의 다른 공동 작업자와 연결을 설정하는 데 사용됩니다."

<!-- Move the above popover to new section for invite on this page when its created -->

계정 구성을 시작하려면 먼저 계정 세부 사항을 설정해야 합니다. 이 경우 다음 정보를 추가해야 합니다.

* 브랜드를 명확하게 나타내는 **[!UICONTROL 계정 이름]**&#x200B;을(를) 추가합니다.
* 브랜드에 대한 **[!UICONTROL 설명]**&#x200B;을(를) 추가합니다. 이는 선택 사항이지만 다른 공동 작업자가 브랜드를 더 잘 이해하는 데 도움이 됩니다.
* **[!UICONTROL 역할]**&#x200B;을(를) 선택하십시오. **[!UICONTROL Advertiser]**&#x200B;에서 **[!UICONTROL Publisher]** 중 하나를 선택할 수 있습니다. [통합 워크플로 문서](/help/guide/end-to-end-workflow.md)를 읽고 두 조직 역할 유형 간의 워크플로에서 유사점과 약간의 차이점을 확인하십시오.
<!-- The above will need to be updated when I update things for B2B -->
* 계정의 **[!UICONTROL 업종]**&#x200B;을 선택하세요. 일부 예로는 **[!UICONTROL 소매]**, **[!UICONTROL 통신]** 또는 **[!UICONTROL 금융 서비스]**&#x200B;가 있습니다.
* **[!UICONTROL Region]**&#x200B;은(는) Adobe Experience Cloud 계정을 기반으로 자동으로 설정됩니다. 이는 언제든지 변경할 수 없습니다.
* 계정에 대해 **[!UICONTROL 연락처 전자 메일]**&#x200B;을(를) 추가합니다. 팀 또는 역할 기반 이메일 주소여야 합니다. 개인 이메일 주소를 제공해서는 안 됩니다.
* 계정에 대한 **[!UICONTROL 로고]**&#x200B;를 업로드하십시오. 현재 SVG 유형의 이미지가 지원됩니다. 이는 선택 사항이지만 로고를 업로드하면 Collaboration 인터페이스에서 브랜드를 시각적으로 나타낼 수 있습니다
* 계정 헤더 사진에 대한 이미지를 선택합니다.

>[!NOTE]
>
>이러한 세부 정보의 대부분을 언제든지 편집할 수 있지만 초기 설정 후에는 **[!UICONTROL 역할]**&#x200B;을(를) 편집할 수 없습니다. 완료되면 **[!UICONTROL 다음]**&#x200B;을 사용하여 다음 페이지로 이동하여 조직에서 사용할 일치 키를 선택하십시오.

![세부 정보 섹션이 표시되고 다음 옵션이 강조 표시된 계정 작업 영역 설정.](/help/assets/setup/manage-account/add-account-details.png){zoomable="yes"}

### 일치 키 설정 {#set-up-match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_matchkeys"
>title="일치 키"
>abstract="일치 키는 서로 다른 데이터 소스의 대상자 간에 멤버를 조정하는 데 사용되는 식별자입니다. 내 브랜드와 함께 사용할 수 있는 모든 일치 키를 포함합니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_peopleIDs"
>title="자사 사람 ID"
>abstract="해시된 이메일 주소나 전화번호와 같은 자사 사람 ID는 개인 프로필에 직접 연결됩니다. 현재 지원되는 ID는 해시된 이메일과 전화번호입니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_deviceIDs"
>title="자사 디바이스 ID"
>abstract="ECID나 IP 주소와 같은 자사 디바이스 ID는 여러 개인이 공유할 수 있는 디바이스에 직접 연결됩니다. IPv4는 현재 지원되는 유일한 자사 디바이스 ID입니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_partnerIDs"
>title="지원되는 파트너 ID"
>abstract="프로필과 연결된 파트너 ID는 특정 프로필에 대한 도달 범위를 확장합니다."

>[!IMPORTANT]
>
>계정 설정 중에 선택하는 일치 키는 다른 공동 작업자와 만드는 연결에 사용할 수 있는 일치 키를 결정합니다. 연결 설정 중에 일치 키를 제거할 수 있지만 새 일치 키를 추가할 수는 없습니다. 계정 설정 중에 향후 캠페인에서 사용할 **모두** 일치 키를 선택해야 합니다.

이메일 주소, 장치 ID 또는 고객 ID와 같은 일치 키를 사용하면 정확하고 개인 정보 보호 중심의 데이터 동기화를 활성화하여 공동 작업자가 함께 작업할 수 있으므로 보다 정확한 대상 타기팅 및 측정을 수행할 수 있습니다.

![Collaboration의 첫 번째 릴리스에 대해 사용 가능한 식별자를 보여 주는 슬라이드.](/help/assets/setup/manage-account/available-identifiers.png)

<!-- Eventually replace this image above to match branding better. -->

대상 프로필을 조정할 때 사용할 일치 키를 선택합니다. 작업할 수 있는 모든 일치 키를 포함합니다. 미래를 계획하고 향후 캠페인에서 사용할 것으로 예상되는 일치 키를 선택합니다. 나중에 계정에 대해 추가 일치 키를 선택해야 하는 경우 [계정 편집](#edit-account) 워크플로우에서 선택할 수 있습니다.

사용할 일치 키를 최대 5개까지 선택하십시오. 나중에 연결을 설정할 때 원하지 않는 일치 키를 제거할 수 있지만 새 일치 키를 추가할 수는 없습니다.

사용 가능한 일치 키에는 세 가지 유형이 있습니다.

* 자사 사람 ID
* 자사 디바이스 ID
* 파트너 ID

>[!IMPORTANT]
>
>현재 지원되는 일치 키는 해시된 이메일뿐입니다.

준비되면 **[!UICONTROL 완료]**&#x200B;를 선택하여 조직 설정 워크플로를 완료합니다.

![일치 키 섹션이 표시된 조직 작업 영역 설정입니다.](/help/assets/setup/manage-account/add-account-match-keys.png){zoomable="yes"}

## 계정 편집 {#edit-account}

계정을 설정한 후에는 언제든지 해당 계정의 특정 측면과 세부 사항을 편집할 수 있습니다. 계정을 편집하려면 **[!UICONTROL 설정]** 작업 영역&#x200B;**[!UICONTROL 의]**&#x200B;내 계정&#x200B;**[!UICONTROL 섹션에서 &#x200B;]편집**&#x200B;을(를) 선택하십시오.

![[내 계정] 탭과 [편집] 옵션이 강조 표시된 설치 작업 영역입니다.](/help/assets/setup/manage-account/edit-account.png){zoomable="yes"}

이제 **[!UICONTROL 역할]**&#x200B;을(를) 제외하고 계정 세부 정보를 편집할 수 있습니다. 지역은 Adobe Experience Cloud 계정을 기반으로 자동으로 설정되며 언제든지 변경할 수 없습니다.

![계정 세부 정보 편집 대화 상자](/help/assets/setup/manage-account/editable-options.png){zoomable="yes"}

조직에 온보딩할 때 처음에 선택한 일치 키도 업데이트할 수 있습니다. 원하는 일치 키를 추가하려면 **[!UICONTROL 일치 키]** 섹션에서 **[!UICONTROL 편집]**&#x200B;을(를) 선택하십시오.

![계정의 일치 키 섹션 내에서 [편집] 옵션이 강조 표시된 설치 작업 영역입니다.](/help/assets/setup/manage-account/edit-match-keys.png){zoomable="yes"}

## 다음 단계

계정을 설정한 후에는 Real-Time CDP Collaboration에 [소스 대상자](/help/guide/setup/onboard-audiences.md)를 추가할 준비가 되었습니다.
