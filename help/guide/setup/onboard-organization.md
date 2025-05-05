---
title: 조직 온보드 및 관리
description: Real-Time CDP Collaboration에서 조직의 다양한 측면을 온보딩하고 관리하는 방법을 알아봅니다
audience: admin, publisher, advertiser
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/kr/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: a95e932a-9681-48f2-bf34-6fe5a50597d7
source-git-commit: 0de6ab9af8152975f8e0b0f75b1ee0116ed73584
workflow-type: tm+mt
source-wordcount: '853'
ht-degree: 14%

---

# 조직 온보드 및 관리

{{limited-availability-release-note}}

Real-Time CDP Collaboration에 조직을 온보딩하고 회사의 다양한 측면을 관리하는 방법을 알아봅니다. 이 페이지에서는 일치 키, 기본 ID 및 기타 옵션 설정을 포함하여 조직을 Adobe Real-Time CDP Collaboration에 온보딩하는 절차에 대해 설명합니다.

![페이지 설정](/help/assets/setup/manage-organization/my-organization.png){zoomable="yes"}

## 초기 조직 설정

먼저 조직 및 조직 세부 사항을 설정해야 합니다. 왼쪽 레일에서 **[!UICONTROL 설정]**(으)로 이동하고 오른쪽 상단 모서리에서 **+** 기호를 선택한 다음 **[!UICONTROL 계정]**&#x200B;을 선택합니다.

>[!TIP]
>
>작업할 초기 계정을 설정한 후 동일한 워크플로우를 사용하여 동일한 조직 내에서 추가 계정을 설정할 수 있습니다.

![Real-Time CDP Collaboration에 새 조직을 추가할 계정 선택](/help/assets/setup/manage-organization/add-new-account.png){zoomable="yes"}

조직을 설정하는 워크플로에는 아래 두 페이지가 포함됩니다.

* [세부 정보 설정](#set-up-details)
* [일치 키 설정](#set-up-match-keys)

>[!IMPORTANT]
>
>조직 수준에서 선택하는 모든 *일치 키*&#x200B;는 광고주와 게시자 간의 공동 작업에서 [프로젝트 수준](/help/guide/collaborate/manage-projects.md)(으)로 적용됩니다. 그런 다음 프로젝트 수준에서 일치 키를 제거할 수 있지만 이 화면의 조직 수준에서 선택되지 않은 일치 키를 추가할 수 있는 기능은 *없음*&#x200B;입니다.

### 세부 정보 설정 {#set-up-details}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_setup_contact_email"
>title="연락처 이메일"
>abstract="팀 또는 역할 기반 전자 메일을 제공하십시오(예: `collaboration@yourcompany.com`). 개인 또는 개인 이메일 주소를 사용해서는 안 됩니다."

![조직을 설정하는 세부 정보 및 사용 사례 단계](/help/assets/setup/manage-organization/add-organization-details.png){zoomable="yes"}

1. 회사에 대한 **[!UICONTROL 조직 이름]**&#x200B;을(를) 추가합니다.
2. 회사에 대한 **[!UICONTROL 설명]**&#x200B;을(를) 추가합니다.
3. **[!UICONTROL 회사 역할]**&#x200B;을 선택하세요. **[!UICONTROL Advertiser]**&#x200B;에서 **[!UICONTROL Publisher]** 중 하나를 선택할 수 있습니다. [통합 워크플로 문서](/help/guide/end-to-end-workflow.md)를 읽고 두 조직 역할 유형 간의 워크플로에서 유사점과 약간의 차이점을 확인하십시오.
4. 조직의 **[!UICONTROL 업종]**&#x200B;을 선택하세요. 일부 예로는 **[!UICONTROL 소매]**, **[!UICONTROL 통신]** 또는 **[!UICONTROL 금융 서비스]**&#x200B;가 있습니다.
5. 조직의 **[!UICONTROL 지역]**&#x200B;을 선택하세요. 현재 버전의 제품에서 **[!UICONTROL 북미]**&#x200B;은(는) 사전 설정된 기본 선택입니다.
6. 조직의 **[!UICONTROL 연락처 전자 메일]**&#x200B;을(를) 추가합니다. 팀 또는 역할 기반 이메일 주소여야 합니다. 개인 이메일 주소를 제공해서는 안 됩니다.
7. <span class="preview"> 게시자 전용</span>: 게시자 조직을 설정할 때 게시자 카탈로그에서 광고주가 검색할 수 있음을 읽고 확인해야 합니다.
   ![게시자별 옵트인 메시지.](/help/assets/setup/manage-organization/publisher-specific-optin-message.png){zoomable="yes"}
8. 회사에 대한 **[!UICONTROL 로고]**&#x200B;를 업로드하십시오. 현재 SVG 유형의 이미지가 지원됩니다.
9. 회사 머리글 사진에 대한 이미지를 선택합니다.

선택에 만족하면 **[!UICONTROL 다음]**&#x200B;을 사용하여 다음 페이지로 이동하고 조직에서 사용해야 하는 일치 키를 선택하십시오.

### 일치 키 설정 {#set-up-match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_matchkeys"
>title="일치 키"
>abstract="일치 키는 서로 다른 데이터 소스의 대상자 간에 멤버를 조정하는 데 사용되는 식별자입니다. 회사에서 사용할 수 있는 모든 일치 키를 포함합니다."

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

이메일 주소, 장치 ID 또는 고객 ID와 같은 일치 키는 광고주와 게시자가 정확하고 개인정보 보호 중심의 데이터 동기화를 활성화하여 보다 정확한 대상 타기팅 및 측정을 허용함으로써 함께 작업하는 데 도움이 됩니다.

![Real-Time CDP Collaboration의 첫 번째 릴리스에 대해 사용 가능한 식별자를 보여 주는 슬라이드.](/help/assets/setup/manage-organization/available-identifiers.png)

게시자 및 광고주 대상의 멤버를 조정할 때 사용할 일치 키를 선택합니다. 회사에서 작업할 수 있는 모든 일치 키를 포함합니다. 미래를 계획하고 향후 게시자-광고주 캠페인에서 사용할 것으로 예상되는 일치 키를 선택합니다. 조직에 대해 추가 일치 키를 선택해야 하는 경우 나중에 [조직 편집](#edit-organization) 워크플로우에서 해당 작업을 수행할 수도 있습니다.

![키 일치 선택 단계입니다.](/help/assets/setup/manage-organization/add-organization-match-keys.png){zoomable="yes"}

사용할 일치 키를 최대 5개까지 선택하십시오. 나중에 연결을 설정할 때 원하지 않는 일치 키를 제거할 수 있지만 새 일치 키를 추가할 수는 없습니다.

Real-Time CDP Collaboration에서 사용할 수 있는 일치 키는 다음 세 가지 유형일 수 있습니다.

* 자사 사람 ID
* 자사 디바이스 ID
* 파트너 ID

Real-Time CDP Collaboration의 첫 번째 릴리스에서 사용할 수 있는 일치 키는 다음과 같습니다.

* 해시된 이메일

<!--

not available in the Limited GA release

* Hashed phone
* IPv4

-->

준비되면 **[!UICONTROL 완료]**&#x200B;를 선택하여 조직 설정 워크플로를 완료합니다.

## 조직 편집 {#edit-organization}

처음에 조직을 설정한 후에는 언제든지 조직의 특정 측면 및 세부 정보를 편집할 수 있습니다. 조직을 편집하려면 **[!UICONTROL 내 조직]** 보기에서 **[!UICONTROL 편집]**&#x200B;을 선택하세요.

![조직 컨트롤 편집이 강조 표시되었습니다.](/help/assets/setup/manage-organization/edit-organization.png){zoomable="yes"}

이때 조직 이름, 설명, 로고 및 조직 프로필 사진을 업데이트할 수 있습니다.

![조직을 위한 편집 가능한 옵션](/help/assets/setup/manage-organization/editable-options.png){zoomable="yes"}

조직 온보딩 시 처음에 선택한 일치 키와 대상 중복 및 기타 제품 영역에서 표시 및 사용할 수 있는 일치 키에 해당하는 ID의 최소 임계값을 업데이트할 수도 있습니다. **[!UICONTROL 일치 키]** 탭에서 **[!UICONTROL 편집]**&#x200B;을 선택하여 원하는 일치 키를 추가하거나 ID 임계값을 업데이트합니다.

![일치 키 편집](/help/assets/setup/manage-organization/edit-match-keys.png){zoomable="yes"}

## 다음 단계

조직을 설정하고 나면 Real-Time CDP Collaboration에 [대상자를 가져올](/help/guide/setup/onboard-audiences.md)준비가 되었습니다.
