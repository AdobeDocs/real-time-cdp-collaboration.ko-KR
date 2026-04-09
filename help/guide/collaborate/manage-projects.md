---
title: 프로젝트 만들기 및 관리
description: Adobe Real-Time CDP Collaboration에서 프로젝트를 만들고 관리하는 방법 알아보기
audience: admin, publisher, advertiser
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/kr/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: ae492846-bc0a-4422-86ca-577bcc1fa60c
source-git-commit: 0cf888e36ffc4730fc8de4d8adccae0e0fc2caa8
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 13%

---

# 프로젝트 만들기 및 관리

{{limited-availability-release-note}}

프로젝트는 Adobe Real-Time CDP Collaboration 워크플로의 중심입니다. 공동 작업자와 연결한 후 프로젝트를 만들어 대상 중복 계산을 실행하고 캠페인에 대한 관련 대상을 검색합니다.

>[!TIP]
>
>프로젝트는 일반적으로 단일 캠페인과 연결되어야 합니다.

![모든 현재 프로젝트를 표시하는 공동 작업 대시보드입니다.](/help/assets/collaborate/manage-view-projects/projects-overview-page.png){zoomable="yes"}

필터를 사용하여 아래와 같이 특정 공동 작업자로 시작한 프로젝트만 볼 수 있습니다.

![단일 공동 작업자가 있는 프로젝트의 필터링된 보기입니다.](/help/assets/collaborate/manage-view-projects/filtered-project-view.png){zoomable="yes"}

## 프로젝트 만들기 {#create-project}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_create_project_advertisername_amc"
>title="광고주 이름(Amazon Marketing Cloud)"
>abstract="Amazon Marketing Cloud(AMC) 연결의 경우 이 필드는 Amazon Ads 로그인이 액세스할 수 있는 AMC 인스턴스를 나타냅니다. 광고주 이름을 반영하지 않습니다. 필요한 인스턴스가 나열되지 않으면 Amazon Marketing Cloud 관리자에게 문의하여 액세스 권한을 요청합니다."

프로젝트를 만들려면 먼저 공동 작업자와 [연결을 설정](/help/guide/connect/establishing-connections.md)해야 합니다. 연결이 설정되면 해당 공동 작업자와 함께 프로젝트를 만들 수 있습니다.

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_projects_advertisername"
>title="광고주 이름"
>abstract="드롭다운 메뉴에서 광고주 이름을 선택하십시오. 이들 옵션은 시스템과의 호환성을 보장하기 위해 게시자가 연결 설정에서 미리 구성합니다."

**[!UICONTROL 공동 작업]**(으)로 이동한 다음 **[!UICONTROL 내 프로젝트]**(으)로 이동합니다. 첫 번째 프로젝트인 경우 **[!UICONTROL 프로젝트 만들기]**&#x200B;를 선택할 수 있습니다. 그렇지 않으면 추가 아이콘(![추가 아이콘](/help/assets/icons/plus.png))을 선택할 수 있습니다. 언제든지 새 프로젝트를 만들 수 있습니다.

![더하기 기호를 선택하거나 프로젝트를 만들어 새 프로젝트를 설정합니다.](/help/assets/collaborate/manage-view-projects/create-project.png){zoomable="yes"}

**[!UICONTROL 프로젝트 만들기]** 대화 상자가 나타납니다. 드롭다운을 통해 프로젝트를 만들 **[!UICONTROL 공동 작업자]**&#x200B;를 선택하십시오. 게시자이고 연결 설정 중에 광고주 이름을 설정한 경우 **[!UICONTROL 광고주 이름]**&#x200B;을 선택할 수 있습니다.

>[!NOTE]
>
> 연결 설정에서 단일 광고주 이름을 구성한 경우 기본적으로 표시됩니다. 설정된 광고주 이름이 없으면 광고주의 **[!UICONTROL 이름]**&#x200B;이(가) **[!UICONTROL 광고주 이름]**(으)로 미리 선택됩니다.

![공동 작업자가 선택되고 광고주 이름이 강조 표시된 프로젝트 만들기 대화 상자.](/help/assets/collaborate/manage-view-projects/create-project-advertiser-names.png){zoomable="yes"}

그런 다음 프로젝트에 대해 **[!UICONTROL 프로젝트 이름]** 및 **[!UICONTROL 설명]**&#x200B;을 추가하십시오. 그런 다음 프로젝트를 나타내는 이미지를 선택합니다. 이 이미지는 프로젝트 개요 페이지에서 프로젝트를 구별하는 데 도움이 됩니다. 완료되면 **[!UICONTROL 만들기]**&#x200B;를 선택하여 프로젝트를 만듭니다.

![새 프로젝트를 설정하는 데 필요한 옵션](/help/assets/collaborate/manage-view-projects/create-project-required-info.png){zoomable="yes"}

이제 연결 설정 중에 선택한 사용 사례에 따라 새 프로젝트, 세부 정보 및 사용 가능한 섹션을 볼 수 있습니다.

![프로젝트 개요 작업 영역입니다.](/help/assets/collaborate/manage-view-projects/project-overview.png){zoomable="yes"}

## 캠페인 ID 관리 {#manage-campaign-id}

**캠페인 ID**&#x200B;은(는) 프로젝트를 특정 캠페인에 연결하며 [측정 보고서를 생성](./measure.md#create-measurement-report)하는 데 필요합니다. 동일한 공동 작업자로 여러 캠페인을 실행하는 경우 한 프로젝트에 여러 캠페인 ID를 추가할 수 있습니다. 이러한 모든 캠페인은 보고에서 선택할 수 있습니다.

- **게시자**: 보고서를 실행하기 전에 Collaboration UI에서 Campaign ID와 관련 이름을 입력하거나 업데이트합니다.
- **광고주**: 필요에 따라 공동 작업자(게시자)에게 캠페인 ID를 추가하도록 요청하십시오.

캠페인 ID를 추가하거나 업데이트하려면 **[!UICONTROL 공동 작업]** 작업 영역으로 이동한 다음 관련 프로젝트 카드에서 **[!UICONTROL 보기]**&#x200B;를 선택하십시오.

![프로젝트 카드에서 보기 옵션을 강조 표시하는 공동 작업 영역입니다.](/help/assets/collaborate/manage-view-projects/view-project.png){zoomable="yes"}

해당 **[!UICONTROL 프로젝트 개요]** 작업 영역에 프로젝트에 연결된 모든 캠페인을 나열하는 **[!UICONTROL 캠페인 ID 및 이름]** 섹션이 나타납니다. 아직 캠페인을 추가하지 않은 경우 **[!UICONTROL 추가]**&#x200B;를 선택하십시오. 이미 캠페인이 있는 경우 **[!UICONTROL 편집]**&#x200B;을(를) 선택하여 세부 정보를 업데이트하거나 추가 캠페인을 추가하세요.

![프로젝트 개요 작업 영역에 [편집] 옵션이 강조 표시된 캠페인 ID 및 이름 섹션이 표시됩니다.](/help/assets/collaborate/manage-view-projects/edit-campaign-id.png){zoomable="yes"}

**[!UICONTROL 캠페인 ID 및 이름]** 대화 상자에서 **[!UICONTROL 캠페인 ID 추가]**&#x200B;를 선택하여 캠페인 세부 정보를 입력할 수 있는 새 행을 추가합니다.

![캠페인 ID 추가 옵션을 선택한 후 캠페인 ID 및 이름 대화 상자에 빈 캠페인 행이 표시됩니다.](/help/assets/collaborate/manage-view-projects/add-campaign-row.png){zoomable="yes"}

**[!UICONTROL 캠페인 ID]** 및 **[!UICONTROL 캠페인 이름]**&#x200B;을 입력한 다음 **[!UICONTROL 저장]**&#x200B;을 선택하십시오.

![새 캠페인 세부 정보와 [저장] 옵션이 강조 표시된 캠페인 ID 및 이름 대화 상자.](/help/assets/collaborate/manage-view-projects/save-campaign-id.png){zoomable="yes"}

최신 캠페인과 최근 변경 내용을 보려면 **[!UICONTROL 캠페인 ID 및 이름]** 섹션을 확인하십시오. 이제 새 Campaign ID를 사용하여 측정 보고서를 생성할 수 있습니다.

![업데이트된 캠페인 ID 및 이름 섹션을 표시하는 프로젝트 개요 작업 영역입니다.](/help/assets/collaborate/manage-view-projects/view-updated-campaigns.png){zoomable="yes"}
