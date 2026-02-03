---
title: 계정 구성 및 관리
description: Real-Time CDP Collaboration에서 계정의 다양한 측면을 구성하고 관리하는 방법에 대해 알아봅니다
audience: admin, publisher, advertiser
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: a95e932a-9681-48f2-bf34-6fe5a50597d7
source-git-commit: 873af5b0ef5e4e0c937c540de4697ec314624669
workflow-type: tm+mt
source-wordcount: '1373'
ht-degree: 11%

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
>abstract="팀 또는 역할 기반의 이메일(예: **collaboration@yourcompany.com**)을 입력해 주십시오. 개인 또는 개별 이메일 주소는 사용할 수 없습니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_setup_connect_code"
>title="연결 코드"
>abstract="연결 코드는 계정의 고유 식별자입니다. Real-Time CDP Collaboration에서 다른 공동 작업자와의 연결을 구축하는 데 사용됩니다."

계정 구성을 시작하려면 먼저 계정 세부 사항을 설정해야 합니다. 이 경우 다음 정보를 추가해야 합니다.

* 브랜드를 명확하게 나타내는 **[!UICONTROL 계정 이름]**&#x200B;을(를) 추가합니다.
* 브랜드에 대한 **[!UICONTROL 설명]**&#x200B;을(를) 추가합니다. 이는 선택 사항이지만 다른 공동 작업자가 브랜드를 더 잘 이해하는 데 도움이 됩니다.
* **[!UICONTROL 역할]**&#x200B;을(를) 선택하십시오. **[!UICONTROL Advertiser]**&#x200B;에서 **[!UICONTROL Publisher]** 중 하나를 선택할 수 있습니다. 두 계정 역할 유형 간의 워크플로에서 유사점과 약간의 차이점을 확인하려면 [역할](/help/guide/overview/roles.md) 안내서를 읽어 보십시오.
* 계정의 **[!UICONTROL 업종]**&#x200B;을 선택하세요. 일부 예로는 **[!UICONTROL 소매]**, **[!UICONTROL 통신]** 또는 **[!UICONTROL 금융 서비스]**&#x200B;가 있습니다.
* **[!UICONTROL Region]**&#x200B;은(는) Adobe Experience Cloud 계정을 기반으로 자동으로 설정됩니다. 이는 언제든지 변경할 수 없습니다.
* 계정에 대해 **[!UICONTROL 연락처 전자 메일]**&#x200B;을(를) 추가합니다. 팀 또는 역할 기반 이메일 주소여야 합니다. 개인 이메일 주소를 제공해서는 안 됩니다.
* 계정에 대한 **[!UICONTROL 로고]**&#x200B;를 업로드하십시오. 현재 SVG 유형의 이미지가 지원됩니다. 이는 선택 사항이지만 로고를 업로드하면 Collaboration 인터페이스에서 브랜드를 시각적으로 나타낼 수 있습니다
* 계정 헤더 사진에 대한 이미지를 선택합니다.

>[!NOTE]
>
>이러한 세부 정보의 대부분을 언제든지 편집할 수 있지만 초기 설정 후에는 **[!UICONTROL 역할]**&#x200B;을(를) 편집할 수 없습니다. 완료되면 **[!UICONTROL 다음]**&#x200B;을 사용하여 다음 페이지로 이동하여 조직에서 사용할 일치 키를 선택하십시오.

![세부 정보 섹션이 표시되고 다음 옵션이 강조 표시된 계정 작업 영역 설정.](/help/assets/setup/manage-account/add-account-details.png){zoomable="yes"}

### 매칭 키 설정 {#set-up-match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_matchkeys"
>title="일치 키"
>abstract="일치 키는 서로 다른 데이터 소스의 대상자 프로필을 조정하는 데 사용되는 식별자입니다. 브랜드에서 사용할 수 있는 모든 일치 키를 포함합니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_setup_match_keys"
>title="일치 키"
>abstract=""

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_peopleIDs"
>title="자사 사용자 ID"
>abstract="해시된 이메일 주소, 해시된 전화번호 또는 CRM ID와 같은 자사 사용자 ID는 개별 프로필에 직접 연결됩니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_deviceIDs"
>title="자사 디바이스 ID"
>abstract="ECID 또는 IP 주소와 같은 자사 디바이스 ID는 여러 개인 간에 공유할 수 있는 디바이스에 직접 연결됩니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_partnerIDs"
>title="지원되는 파트너 ID"
>abstract="파트너 ID는 대상자 조정을 위해 외부 파트너가 제공하는 식별자입니다. 파트너 ID는 개별 프로필에 직접 연결되지 않습니다."

![지원되는 일치 키.](/help/assets/setup/manage-account/match-keys.png){zoomable="yes"}

>[!IMPORTANT]
>
>계정 설정 중에 선택하는 일치 키에 따라 연결 내에서 사용할 수 있는 일치 키가 결정됩니다. 연결 설정 중에 [원치 않는 일치 키를 제거](../connect/establishing-connections.md#connection-settings)할 수 있지만 연결이 설정된 후에는 일치 키를 추가할 수 없습니다. 계정 설정 중에 향후 캠페인에서 사용할 **모두** 일치 키를 선택하는 것이 중요합니다.

일치 키 를 사용하면 정확하고 개인 정보 보호 중심의 데이터 동기화를 활성화하여 공동 작업자가 공동 작업을 수행할 수 있으므로 보다 정확한 대상 타기팅 및 측정이 가능합니다. 계정 설정 중에 선택한 일치 키는 향후 연결에서 사용할 수 있는 일치 키를 결정합니다. 대상을 소싱할 때 데이터 연결에서 Collaboration의 대상 필드에 필드를 [매핑](./onboard-audiences.md#map-fields)하는 데에도 사용됩니다.

대상 프로필을 조정할 때 사용할 일치 키를 선택합니다. 미래를 계획하고, 함께 작업하고 향후 캠페인에서 사용을 예상할 수 있는 모든 일치 키를 포함합니다. 나중에 계정에 대해 추가 일치 키를 선택해야 하는 경우 [계정 편집](#edit-account) 워크플로우에서 선택할 수 있습니다. 그러나 초기 설정 후 추가된 일치 키는 기존 연결에서 사용할 수 없습니다.

#### 지원되는 일치 키 {#supported-match-keys}

Collaboration은 자사 사용자 ID, 자사 디바이스 ID 및 파트너 ID의 세 가지 일치 키 유형을 지원합니다. 모든 일치 키는 다음 요구 사항을 충족해야 합니다.

* 일치 키는 **트리밍**, **소문자화**&#x200B;여야 합니다.
* 해시된 일치 키는 **SHA256-hashed**&#x200B;여야 합니다.
* 대문자를 사용하는 해시된 값을 제공하면 Collaboration에서 자동으로 소문자로 변환합니다.
* 소스에 **일반 텍스트 식별자**&#x200B;이(가) 포함된 경우 **[!UICONTROL 데이터 연결 설정]**&#x200B;에서 [변환 적용](./manage-data-connection.md#match-keys) 옵션을 사용하여 해시를 적용하세요. 이 옵션은 Experience Platform에서 대상을 소싱할 때만 사용할 수 있으며 클라우드 기반 소스에는 지원되지 않습니다.

##### 자사 사용자 ID

자사 사용자 ID는 개별 프로필에 직접 연결됩니다. 현재 지원되는 ID:

* **[!UICONTROL 해시된 이메일]**
* **[!UICONTROL 해시된 휴대폰]**
* **[!UICONTROL CRM ID]**
* **[!UICONTROL 충성도 ID]**
<!-- * **[!UICONTROL Custom ID]**: Custom identifiers -->

##### 자사 디바이스 ID

자사 디바이스 ID는 특정 디바이스에 연결된 식별자입니다. 현재 지원되는 ID:

* **[!UICONTROL 해시된 IPv4]**: 해시된 IPv4 주소
* **[!UICONTROL IDFA]**: Apple iOS 장치에서 사용되는 IDFA(광고주용 식별자)입니다.
* **[!UICONTROL GAID]**: Android 장치에서 사용되는 Google 광고주 ID

##### 파트너 ID

파트너 ID는 대상자 조정을 위해 외부 파트너가 제공하는 식별자입니다. 현재 지원되는 ID:

* **[!UICONTROL AdFixus ID]**

>[!NOTE]
>
>Adobe과 [!DNL AdFixus]의 통합은 각 계정에 대한 고유한 [!UICONTROL AdFixus ID]를 일반적인 Adobe 인코딩 형식으로 매핑합니다. 이러한 매핑은 공동 작업자 간의 중복을 식별하는 데 사용됩니다. **[!UICONTROL AdFixus ID]**&#x200B;을(를) 사용하여 대상을 활성화할 때 원래 ID가 사용됩니다. Adobe으로 인코딩된 형식은 Collaboration을 떠나지 않습니다.

**[!UICONTROL AdFixus ID]**&#x200B;을(를) 선택할 때 **[!UICONTROL 계정 자격 증명]** 섹션에서 외부 파트너에게 해당 ID를 제공해야 합니다. 이 옵션은 *AdFixus ID*&#x200B;에서 전환하여 **[!UICONTROL after]**&#x200B;에만 사용할 수 있습니다. **[!UICONTROL 계정 ID]** 필드에 AdFixus ID를 입력하여 값의 정확성을 다시 확인합니다.

![AdFixus ID가 있는 키 일치 대화 상자가 켜지고 계정 자격 증명 섹션이 강조 표시됩니다.](/help/assets/setup/manage-account/adfixus-settings.png){zoomable="yes"}

원하는 일치 키를 모두 선택한 후 **[!UICONTROL 완료]**&#x200B;를 선택하여 계정 설정 워크플로를 완료합니다.

![일치 키 섹션이 표시된 계정 작업 영역 설정.](/help/assets/setup/manage-account/add-account-match-keys.png){zoomable="yes"}

## 계정 편집 {#edit-account}

계정을 설정한 후 언제든지 세부 정보를 편집하고 키를 일치시킬 수 있습니다.

### 세부 정보 편집 {#edit-details}

**[!UICONTROL 역할]**&#x200B;을(를) 제외하고 언제든지 계정의 세부 정보를 편집할 수 있습니다. 지역은 Adobe Experience Cloud 계정을 기반으로 자동으로 설정되며 변경할 수 없습니다.

계정을 편집하려면 **[!UICONTROL 설정]** 작업 영역의 **[!UICONTROL 내 계정]** 섹션에서 **[!UICONTROL 편집]**&#x200B;을(를) 선택하십시오.

![[내 계정] 탭과 [편집] 옵션이 강조 표시된 설치 작업 영역입니다.](/help/assets/setup/manage-account/edit-account.png){zoomable="yes"}

이제 계정 세부 사항을 편집할 수 있습니다. 변경할 필드를 업데이트한 다음 **[!UICONTROL 저장]**&#x200B;을 선택하여 변경 내용을 확인합니다.

![계정 세부 정보 편집 대화 상자](/help/assets/setup/manage-account/editable-options.png){zoomable="yes"}

### 일치 키 편집 {#edit-match-keys}

>[!IMPORTANT]
>
>일치 키를 편집해도 기존 연결에는 영향을 주지 않습니다. 연결이 설정되면 연결 설정 중에 선택한 일치 키가 수정됩니다. 계정 설정 중에 향후 캠페인에서 사용할 **모두** 일치 키를 선택하는 것이 중요합니다.

계정을 만들 때 처음에 선택한 일치 키도 업데이트할 수 있습니다. 이러한 일치 키는 향후 연결에 사용할 수 있는 일치 키를 결정합니다.

**[!UICONTROL 키 일치]** 섹션에서 **[!UICONTROL 편집]**&#x200B;을(를) 선택합니다.

![계정의 일치 키 섹션 내에서 [편집] 옵션이 강조 표시된 설치 작업 영역입니다.](/help/assets/setup/manage-account/edit-match-keys.png){zoomable="yes"}

**[!UICONTROL 키 일치]** 대화 상자가 나타납니다. 일치 키를 켜거나 끄거나 **[!UICONTROL AdFixus ID]**&#x200B;에 대한 [!UICONTROL 계정 ID]을(를) 업데이트한 다음 **[!UICONTROL 저장]**&#x200B;을(를) 선택하여 변경 내용을 확인합니다.

>[!IMPORTANT]
>
>[!UICONTROL AdFixus ID]을(를) 변경해도 일치 키를 사용하여 기존 데이터 연결에 대해 [데이터 스케치](../glossary.md#sketches) 새로 고침이 트리거되지 않습니다. 데이터가 스케치되면 [!UICONTROL 데이터 연결 일정] 설정에 따라 다음 대상자가 새로 고쳐질 때까지 [AdFixus ID](./manage-data-connection.md#scheduling)에 대한 변경 내용이 반영되지 않습니다. 다음 새로 고침 전에 변경해야 하는 경우 데이터 연결을 삭제하고 다시 만들 수 있습니다.

![저장 옵션이 강조 표시된 키 일치 대화 상자입니다.](/help/assets/setup/manage-account/match-key-dialog.png){zoomable="yes"}

## 다음 단계

계정을 설정한 후에는 Real-Time CDP Collaboration에 [소스 대상자](/help/guide/setup/onboard-audiences.md)를 추가할 준비가 되었습니다.
