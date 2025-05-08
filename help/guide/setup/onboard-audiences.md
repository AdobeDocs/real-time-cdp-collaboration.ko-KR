---
title: 대상자 가져오기 및 관리
description: Adobe Real-Time CDP Collaboration에서 대상을 가져오고 관리하는 방법 알아보기
audience: admin, publisher, advertiser
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 0a5158fa-73d3-4406-af20-2b6c7be9934e
source-git-commit: 8fca38c8125cefae9fe52ecd168e3d0ff20f2936
workflow-type: tm+mt
source-wordcount: '2685'
ht-degree: 22%

---

# 대상자 가져오기 및 관리

{{limited-availability-release-note}}

대상자는 다양한 속성에 따라 세그먼트화된 사용자 또는 고객의 특정 그룹입니다. 이를 통해 광고주와 게시자는 보다 효과적인 광고 캠페인을 위해 타깃팅된 마케팅 및 개인화된 경험에 대해 공동 작업을 수행할 수 있습니다.

대상과 관련하여 볼 수 있는 모든 관련 지표와 대상자를 Adobe Real-Time CDP Collaboration으로 가져오는 워크플로 단계를 이해하려면 이 페이지를 이동으로 사용하십시오.

>[!TIP]
>
>이 화면의 정보를 사용하여 대상에 대해 필요한 모든 정보를 얻을 수 있으며 [검색 및 겹치는 화면](/help/guide/collaborate/discover.md)을 통해 게시자 인벤토리와 비교할 때 다양한 캠페인 유형에 가장 적합한 대상에 대한 통찰력을 얻을 수 있습니다.

>[!BEGINSHADEBOX]

이 설명서 페이지에 표시되는 내용:

* [Real-Time CDP Collaboration에 대상자 가져오기](#import-audiences)
* [대상자 대시보드 보기](#view-audiences-dashboard)
* [개별 대상자 보기](#view-individual-audiences)

>[!ENDSHADEBOX]

## Real-Time CDP Collaboration에 대상자 가져오기 {#import-audiences}

>[!IMPORTANT]
>
>대상자를 가져오려면 프로필 보기 및 세그먼트 보기, 이렇게 두 개의 프로필 관리 권한이 포함된 역할에 사용자를 할당해야 합니다. 필요한 권한 할당에 대한 자세한 내용은 [대상자 가져오기](../permissions/overview.md#audience-importation) 안내서를 참조하십시오.

공동 작업자와 대상을 공유하고 중복 계산을 실행하려면 먼저 대상을 Real-Time CDP Collaboration으로 가져와야 합니다. 대상자를 가져오려면 아래 섹션의 워크플로 단계를 따르십시오.

![조직에 대상이 추가되기 전에 내 대상 화면을 표시합니다.](/help/assets/setup/add-manage-audiences/org-without-audiences-added.png)

**[!UICONTROL 내 대상]** 탭에서 더하기 **+** 기호를 선택한 다음 **대상**&#x200B;을 선택합니다.

### 데이터 연결 선택 {#select-data-connection}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_marketing_actions"
>title="마케팅 액션"
>abstract="<p>마케팅 액션을 사용하여 Experience Platform에서 Real-Time CDP Collaboration으로 가져올 대상자 고객 데이터를 제어합니다. <strong>데이터 협업</strong> 마케팅 액션은 C4, C5, C9 데이터 사용 레이블을 지원합니다. <strong>데이터 과학</strong> 마케팅 액션은 C9 데이터 사용 레이블을 지원합니다.</p> <p> <ul><li> 확인란이 <em>표시</em>되어 있는 경우, Experience Platform에서 위에 언급된 레이블로 표시된 모든 데이터는 제외되며 Real-Time CDP Collaboration으로 이동되지 <strong>않습니다</strong>.</li><li> 확인란이 <em>표시되어 있지 않은</em> 경우, Experience Platform에서 Real-Time CDP Collaboration으로 가져올 수 있는 데이터에 제한이 없습니다.</li></ul></p>"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/data-governance/labels/overview.html?lang=ko" text="데이터 사용 레이블 개요"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/data-governance/labels/reference.html" text="데이터 사용 레이블 용어"

>[!IMPORTANT]
>
>첫 번째 데이터 연결에 연결하고 첫 번째 대상을 가져온 후 이 기존 데이터 연결에서 여러 대상을 가져오도록 선택할 수 있습니다. 이 경우 다른 단계의 모든 필수 구성 요소 정보를 기존 연결에서 가져오기 때문에 워크플로는 [대상 선택](#select-audience) 단계로 바로 이동합니다.

데이터 연결은 대상을 Real-Time CDP Collaboration으로 가져오는 위치의 데이터 소스입니다. Real-Time CDP Collaboration의 첫 번째 릴리스에서 지원되는 데이터 연결은 Adobe Experience Platform 뿐입니다.

데이터 연결에 대해 구성하는 ID 매핑 또는 예약과 같은 모든 설정은 이 데이터 연결에서 가져온 모든 대상에 적용됩니다.

>[!TIP]
>
>이 단계에서 추가한 모든 데이터 연결을 항상 보고 편집할 수 있는 별도의 워크플로우가 있습니다. [데이터 연결 관리](/help/guide/setup/manage-data-connection.md)에 대해 자세히 알아보세요.

![AEP RTCDP, CSV 파일, Amazon S3 및 Snowflake에 대한 옵션을 보여 주는 대상 소스 화면을 선택하십시오.](/help/assets/setup/add-manage-audiences/Step-Select-Audience-Source.png)

#### 데이터 소스 선택

이 단계에서는 대상 데이터의 소스를 선택합니다. 사용 가능한 소스는 다음과 같습니다.

* **Adobe Experience Platform**: Adobe Experience Platform Real-Time CDP에서 대상을 가져오려면 이 옵션을 선택하십시오.
* **CSV 파일**(향후 릴리스): 빠르고 간단한 데이터 수집을 위해 대상 데이터가 포함된 CSV 파일을 업로드합니다.
* **Amazon Web Services**(향후 릴리스): Amazon S3 저장소에 연결하여 S3 버킷에서 직접 대상 데이터를 가져옵니다.
* **Snowflake**(향후 릴리스): Snowflake 데이터 웨어하우스를 사용하여 대상 데이터를 원활하게 가져올 수 있습니다.

#### 샌드박스 선택

**Adobe Experience Platform**&#x200B;을(를) 데이터 소스로 선택한 후에는 가져올 대상이 포함된 샌드박스를 선택해야 합니다.

![대상자를 가져올 샌드박스 선택](/help/assets/setup/add-manage-audiences/import-audiences-select-sandbox.png)

원하는 샌드박스를 선택한 후 **[!UICONTROL 다음]**&#x200B;을 선택합니다.

#### 거버넌스 정책 및 시행 액션 {#governance-policy-and-enforcement-actions}

그런 다음 가져온 데이터에 올바른 마케팅 작업이 설정되어 있는지 확인해야 합니다. 또한 Real-Time CDP에서 가져온 데이터가 데이터 공동 작업에 사용되도록 동의해야 합니다.

마케팅 액션을 사용하여 Experience Platform에서 Real-Time CDP Collaboration으로 가져올 대상자 고객 데이터를 제어합니다. **데이터 협업** 마케팅 액션은 C4, C5, C9 데이터 사용 레이블을 지원합니다. **데이터 과학** 마케팅 액션은 C9 데이터 사용 레이블을 지원합니다.

[C4, C5 및 C9 데이터 사용 레이블](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/labels/reference#contract){target="_blank"}에 대해 자세히 알아보십시오.

* 확인란이 *표시*&#x200B;되어 있는 경우, Experience Platform에서 위에 언급된 레이블로 표시된 모든 데이터는 제외되며 Real-Time CDP Collaboration으로 이동되지 *않습니다*.
* 확인란이 *표시되어 있지 않은* 경우, Experience Platform에서 Real-Time CDP Collaboration으로 가져올 수 있는 데이터에 제한이 없습니다.

Experience Platform 설명서에서 데이터 사용 레이블에 대해 자세히 알아보십시오.

* [데이터 사용 레이블 개요](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/labels/overview){target="_blank"}
* [데이터 사용 레이블 용어집](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/labels/reference){target="_blank"}

![데이터 공동 작업에 필요한 마케팅 작업입니다.](/help/assets/setup/add-manage-audiences/data-collaboration-consent.png)

### 세부 정보 입력

그런 다음 나중에 이 데이터 연결을 인식하기 위해 이름과 설명을 입력합니다.

<!--

>[!IMPORTANT]
>
>Note a difference in terminology where the sandbox selected from Real-Time CDP is considered a dataset in the UI in Real-Time CDP Collaboration.

-->

### 필드 매핑 {#map-fields}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_source_fields"
>title="소스 필드"
>abstract="소스 필드는 기존 실시간 CDP 구현의 ID 네임스페이스와 속성입니다. 이를 Real-Time CDP Collaboration에 정의된 대상 필드에 매핑할 수 있습니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_target_fields"
>title="대상 필드"
>abstract="대상 필드는 회사에서 온보딩을 진행할 때 선택한 일치 키에 해당합니다. 현재 유일하게 지원되는 일치 키는 해시된 이메일입니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_apply_transformation"
>title="변환 적용"
>abstract="소스에서 *해시되지 않은* 필드를 가져오는 경우, 이 옵션을 사용하면 Real-Time CDP Collaboration에서 해싱을 적용하고 일반 필드를 해시된 필드로 변환합니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_identity_namespaces"
>title="ID 네임스페이스"
>abstract="Experience Platform 조직에서 사용할 수 있는 표준 및 사용자 정의 ID 네임스페이스에서 ID 네임스페이스를 선택합니다."
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/identity/features/namespaces.html#standard" text="Experience Platform의 표준 및 ID 네임스페이스"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_profile_attributes"
>title="프로필 속성"
>abstract="Experience Platform의 프로필 클래스에 대한 공용 구조체 스키마에서 속성을 선택합니다. 이 보기는 공용 구조체 스키마에 존재하고 XDM 개별 프로필 클래스에 속하는 속성을 표시합니다."
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/profile/union-schemas/union-schema.html" text="Experience Platform의 공용 구조체 스키마"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_target_namespaces"
>title="대상 네임스페이스"
>abstract="적절한 설명으로 채워집니다."

![대상 필드에 매핑된 원본 필드를 표시하는 필드 매핑 화면.](/help/assets/setup/add-manage-audiences/Step-Map-Fields.png)

필드 매핑 단계에서는 데이터 연결에서 가져온 프로필의 ID 필드를 조직에서 선택한 일치 키에 매핑하는 방법을 선택할 수 있습니다.

>[!TIP]
>
>여러 소스 필드를 동일한 대상 필드에 매핑할 수 있습니다. 예를 들어, Experience Platform의 두 개의 별도 필드에 이메일 주소가 있는 경우 두 주소를 **[!UICONTROL 해시된 이메일]** 대상 필드에 두 개의 별도 행으로 매핑할 수 있습니다.

>[!BEGINSHADEBOX]

**[!UICONTROL Source 필드]**&#x200B;은(는) 데이터를 가져오는 원본에서 ID가 참조되는 방식을 나타냅니다.

**[!UICONTROL 대상 필드]**&#x200B;은(는) ID가 Real-Time CDP Collaboration에서 참조되는 방식을 나타냅니다. 여기에서 선택할 수 있는 값은 회사 온보딩 워크플로우에서 설정한 일치 키에 해당합니다.

소스에서 *해시되지 않은* 필드를 가져올 때 **[!UICONTROL 변환 적용]** 옵션을 사용하십시오. 이 경우 Real-Time CDP Collaboration은 해싱을 적용하고 필드를 변환합니다. Adobe에서 사용하는 해싱 알고리즘이 SHA256입니다.

>[!ENDSHADEBOX]

필요한 만큼 매핑 쌍을 추가하고 **[!UICONTROL 다음]**&#x200B;을(를) 선택하여 다음 단계로 진행합니다.

<!--

In this step, you can also add any identity crosswalks that you would like to use.

Identity crosswalks will be supported after the beta release.

#### Add identity crosswalk

Use identity crosswalks to connect different identifiers across datasets to enrich your audience data with additional attributes or dimensions. 

TODO add GIF Identity crosswalks screen showing a list of available identity crosswalks with details.

Select **[!UICONTROL Add identity crosswalk]** to see a screen where you can choose from various identity crosswalks that you have previously [imported into Real-Time CDP Collaboration](/help/guide/setup/identity-crosswalk.md#import-crosswalk). Each entry includes details such as the table name, type, description, and creation date.

After selecting the desired crosswalk, use a source field join key to map to the crosswalk table join key. 

>[!NOTE]
>
>After selecting an identity crosswalk, the **[!UICONTROL Add identity crosswalk]** control is greyed out. 

For further reading about identity crosswalks, refer to the [glossary](/help/guide/glossary.md).

-->


<!-- will uncomment this part when Manage use cases part becomes available

### Manage use cases {#manage-use-cases}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_usecases"
>title="Use cases for identities"
>abstract="This control is disabled in the initial release of Real-Time CDP Collaboration"

![Manage use cases screen.](/help/assets/setup/add-manage-audiences/Step-manage-use-cases.png)

For every identity selected in the mapping step, select the use cases that you can use the identity for. Available use cases are: 

* Discover
* Share
* Activate
* Measure

Note that this control is disabled in the initial release of Real-Time CDP Collaboration.

After selecting the desired use cases for each identity, proceed to the next step. 

-->›

### 예약 {#schedule}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_audience_expiration"
>title="대상자 만료"
>abstract="대상자 만료에 대한 세부 정보."

대상자 채우기 및 새로 고침을 시작 및 종료하는 시점을 예약합니다. 대상 멤버십은 이 일정에 따라 새로 고쳐집니다.

![대상자를 채우는 시작 날짜와 종료 날짜를 표시하는 예약 화면입니다.](/help/assets/setup/add-manage-audiences/Step-Schedule.png)

대상에 대한 새로 고침 빈도를 선택합니다. 사용 가능한 옵션은 1일에서 6일 사이의 새로 고침 비율입니다.

>[!IMPORTANT]
>
>대상 업데이트 빈도를 조정하면 대상 구성원 새로 고침에 따라 계산되는 [대상 관리 크레딧 활동](/help/guide/setup/my-activity.md#types-of-activities)을 관리하는 데 도움이 됩니다. 이로 인해 대상 검색 보고서와 대상 공유 및 활성화에 덜 신선한 데이터를 사용할 수 있습니다.

![대상자 멤버십을 업데이트하기 위한 다른 빈도 간격을 보여 주는 예약 화면](/help/assets/setup/add-manage-audiences/Step-Schedule-Set-Frequency.png)

>[!IMPORTANT]
>
>날짜 범위의 종료 날짜 이후, 이 데이터 연결에서 가져온 모든 대상의 새로 고침이 중지됩니다. 연결을 갱신하려면 [데이터 연결 관리](/help/guide/setup/manage-data-connection.md)(으)로 이동하여 새 종료 날짜를 설정하십시오.

### 대상자 선택 {#select-audience}

대상 소스를 선택한 후 포함할 특정 대상을 선택합니다. 페이지의 검색 및 필터 옵션을 사용하여 선택한 데이터 소스에서 관련 대상을 찾을 수 있습니다.

![확인란을 사용하여 사용 가능한 대상 목록을 표시하는 대상 화면을 선택하십시오.](/help/assets/setup/add-manage-audiences/Step-Select-Audience.png)

### 검토

대상자 추가를 완료하기 전에 모든 구성 및 설정을 검토하십시오. 모든 세부 정보가 올바른지 확인하고 **[!UICONTROL 완료]**&#x200B;를 선택하여 프로세스를 완료합니다.

## 대상자 대시보드 보기 {#view-audiences-dashboard}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_missing_identities"
>title="누락된 ID"
>abstract="ID 카운트는 구성된 일정에 따라 다음 데이터 연결을 새로 고친 후 사용할 수 있습니다. 초기 새로 고침은 일반적으로 데이터 연결이 설정된 후 24시간 이내에 수행됩니다. 진행 중인 새로 고침은 구성된 일정을 따릅니다. "

대상을 Real-Time CDP Collaboration으로 가져온 다음에는 대시보드 보기에서 해당 대상에 대한 정보를 얻을 수 있습니다. **[!UICONTROL 내 대상]** 페이지의 기본 보기에는 조직에서 현재 Real-Time CDP Collaboration으로 가져온 모든 대상이 표시됩니다.

![광고주가 가져온 모든 대상을 표시하는 대상 개요 페이지](/help/assets/setup/add-manage-audiences/audiences-overview.png)

각 대상자에 대한 다음 관련 정보를 볼 수 있습니다.

| 항목 | 설명 |
|----------|---------|
| **[!UICONTROL ID]** | 이 대상에 있는 ID의 수를 나타냅니다. 동일한 프로필에 두 개 이상의 ID가 있고 이러한 ID가 프로젝트에서 일치 키로 사용되는 경우 프로필이 카운트에 두 번 표시됩니다. |
| **[!UICONTROL 상태]** | 대상이 활성 상태이고 프로젝트에서 사용할 수 있는지 여부를 나타냅니다. 보류 중 상태는 대상자를 최근에 가져왔으며 대상자 멤버가 아직 채워지지 않았음을 나타냅니다. 가져온 대상자는 구성된 일정에 따라 다음 데이터 연결을 새로 고치면 프로필로 채워집니다. 초기 새로 고침은 일반적으로 데이터 연결이 설정된 후 24시간 이내에 수행됩니다                                         . |
| **[!UICONTROL Source]** | 이 대상자를 가져온 소스를 나타냅니다. 현재 Real-Time CDP Collaboration 릴리스에서는 Adobe Experience Platform이 유일한 지원 소스입니다. |
| **[!UICONTROL 데이터 연결]** | 이 대상자를 가져온 위치에 대한 추가 드릴다운 정보입니다. 예를 들어 Experience Platform 소스에서 대상을 가져올 때 조직에서 액세스할 수 있는 개별 샌드박스가 데이터 연결로 간주됩니다. |
| **[!UICONTROL 연결 액세스]** | 이 대상이 비공개인지 아니면 공용인지 정의합니다. 공용 대상은 중복 보고서에서 검색할 수 있으며 공동 작업자와 공유할 수 있습니다. |
| **[!UICONTROL 생성일]** | 이 대상자를 Real-Time CDP Collaboration으로 가져온 시기를 나타냅니다. |
| **[!UICONTROL 마지막으로 업데이트됨]** | 이 대상자의 모든 측면이 업데이트된 마지막 날짜 및 시간을 나타냅니다. |

설정한 모든 데이터 연결을 보고 편집하려면 **[!UICONTROL 데이터 연결 관리]**를 선택하십시오.
대상자를 제거하려면 생략과 **[!UICONTROL 삭제]**를 선택하십시오.
대상에 다른 범주 태그를 추가하려면 엘리피스와 **[!UICONTROL 범주 편집]**&#x200B;을 선택하십시오. 아래의 [범주](/#categories) 섹션에서 자세한 내용을 확인하세요.
개별 대상을 검사하거나 편집하려면 대상 이름을 선택합니다.

## 개별 대상자 보기 {#view-individual-audiences}

대상 보기는 대상에 대한 추가 정보를 표시합니다.

![개별 대상자를 보고 검사합니다.](/help/assets/setup/add-manage-audiences/view-inspect-audience.png)

이 화면에서 볼 수 있는 지표는 아래에 설명되어 있습니다.

| 항목 | 설명 |
|----------|---------|
| **[!UICONTROL 상태]** | 대상이 활성 상태이고 프로젝트에서 사용할 수 있는지 여부를 나타냅니다. |
| **[!UICONTROL Source]** | 이 대상자를 가져온 소스를 나타냅니다. 현재 Real-Time CDP Collaboration 릴리스에서는 Adobe Experience Platform이 유일한 지원 소스입니다. |
| **[!UICONTROL 데이터 연결]** | 이 대상자를 가져온 위치에 대한 추가 드릴다운 정보입니다. 예를 들어 Experience Platform 소스에서 대상을 가져올 때 조직에서 액세스할 수 있는 개별 샌드박스가 데이터 연결로 간주됩니다. |
| **[!UICONTROL 마지막으로 업데이트됨]** | 이 대상자의 모든 측면이 업데이트된 마지막 날짜 및 시간을 나타냅니다. |
| **[!UICONTROL 마지막으로 업데이트한 사람]** | 이 대상자를 마지막으로 업데이트한 사용자를 나타냅니다. |
| **[!UICONTROL 생성일]** | 이 대상자를 Real-Time CDP Collaboration으로 가져온 시기를 나타냅니다. |
| **[!UICONTROL 만든 사람]** | 대상을 Real-Time CDP Collaboration으로 가져온 사용자를 나타냅니다. |


페이지에서 두 개의 추가 컨트롤을 사용하여 대상을 편집하거나 제거할 수 있습니다.

* **[!UICONTROL 삭제]**: 인벤토리에서 대상자를 제거합니다.
* **[!UICONTROL 편집]**: 이름 또는 설명과 같은 대상 메타데이터를 편집합니다.

![개별 대상자를 보고 검사합니다.](/help/assets/setup/add-manage-audiences/audiences-edit-delete-controls.png)

대상자에 대한 추가 정보는 아래 위젯에서 사용할 수 있으며 부분적으로 편집할 수 있습니다.

![개별 대상자를 보고 검사합니다.](/help/assets/setup/add-manage-audiences/audiences-further-info-boxes.png)

* [ID](#identities)
* [카테고리](#categories)
* [연결 액세스](#connection-access)
* [메타데이터 가시성](#metadata-visibility)

### ID {#identities}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_identities"
>title="ID"
>abstract="이 대상자를 구성하는 ID에 대한 분류 보기와 해당 ID가 있는 프로필의 총 개수를 확인합니다."

이 섹션은 대상자를 가져올 때 지정한 ID와 함께 대상자에 있는 프로필 수를 나타냅니다. 또한 섹션에는 ID 분류가 포함되어 있으므로 대상자 모집단의 대부분을 구성하는 ID를 파악할 수 있습니다.

### 카테고리 {#categories}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_categories"
>title="카테고리"
>abstract="대상자에 태그를 지정하면 쉽게 구성, 필터링 및 검색할 수 있습니다. 여러 개의 카테고리로 대상자에 태그를 지정한 다음 이 카테고리 태그를 사용하여 제품의 다른 영역에서 원하는 대상자를 필터링할 수 있습니다."

대상자를 쉽게 구성하고, 필터링하고, 검색할 수 있도록 대상자에 태그를 지정할 수 있습니다. 대상 중복 보고서를 실행할 때 여러 범주가 있는 대상에 태그를 지정한 다음 이러한 범주 태그를 사용하여 [discover](/help/guide/collaborate/discover.md) 제품 영역에서 원하는 대상을 필터링할 수 있습니다.

### 연결 액세스 {#connection-access}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_connection_access"
>title="연결 액세스"
>abstract="<p>대상자는 공개, 비공개, 사용자 정의 등 세 가지 유형으로 나눌 수 있습니다.</p><p> 공동 작업자가 있는 프로젝트에서 사용 가능한지 여부는 연결 액세스 설정에 따라 다릅니다. 연결 액세스를 비공개에서 공개로 언제든지 변경할 수 있지만 공동 작업자와 대상자를 공유한 후에는 기존 설정을 다시 변경할 수 없습니다.</p>"

대상이 귀하에게 비공개여야 하는지 또는 연결에서 사용 가능하고 검색 가능한지 여부를 선택합니다. 사용 가능한 세 가지 옵션은 다음과 같습니다.

* **[!UICONTROL 공개 대상]**. 이러한 대상은 중복 보고서에서 사용하고 공동 작업자와의 연결에서 공유 및 활성화할 수 있습니다.
* **[!UICONTROL 개인 대상자]**. 이러한 대상은 중복 보고서에서 사용하고 공동 작업자와의 연결에서 공유 및 활성화할 수 있는 *없음*&#x200B;입니다. 공동 작업자가 보거나 사용할 수는 없지만 이 대상자의 모집단은 여전히 [검색 및 겹치기 섹션](/help/guide/collaborate/discover.md#compare-audiences)의 **[!UICONTROL 모든 대상자]** 보기의 총 모집단에 기여합니다. 공동 작업자와 연결에서 대상을 사용하려면 설정을 공개 또는 사용자 지정으로 변경하십시오.
* **[!UICONTROL 사용자 지정 대상]**. 이러한 대상은 중복 보고서에서 사용하고 지정된 연결에서만 공유 및 활성화할 수 있습니다. 모든 공동 작업자가 보거나 사용할 수는 없지만 이 대상자의 모집단은 여전히 [검색 및 겹치기 섹션](/help/guide/collaborate/discover.md)의 **[!UICONTROL 모든 대상자]** 보기에서 총 모집단에 기여합니다.

>[!IMPORTANT]
>
>액세스 상태(공개, 비공개 또는 사용자 지정)에 관계없이, 대상 검색 겹침 분석 보기에서 대상의 모집단은 **[!UICONTROL 모든 대상]** 모집단에 기여합니다. <br> ![대상 검색 중복 분석의 시스템 생성 **모든 대상** 대상에 모든 연결 액세스 상태(공용, 개인, 사용자 지정)의 대상이 포함됩니다.](/help/assets/setup/add-manage-audiences/all-audiences-view.png "**Audience Discovery** 중복 분석의 시스템 생성 **모든 대상** 대상에는 모든 연결 액세스 상태(공용, 개인, 사용자 지정)의 대상이 포함됩니다."){width="100" zoomable="yes"}

공동 작업자가 있는 프로젝트에서 사용할 수 있는 대상 가용성은 연결 액세스 설정에 따라 다릅니다. 연결 액세스를 비공개에서 공개로 언제든지 변경할 수 있지만 공동 작업자와 대상자를 공유한 후에는 기존 설정을 다시 변경할 수 없습니다.

### 메타데이터 가시성 {#metadata-visibility}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_metadata_visibility"
>title="메타데이터 가시성"
>abstract="<p>귀하의 조직에 연결하기 전에 다른 조직에서 볼 수 있는 대상자 메타데이터 정보를 나타냅니다. </p> <p> **ID 수**&#x200B;는 검색 탭에서 중복 보고서를 볼 때 파트너가 대상자의 ID 수를 볼 수 있는지 여부를 제어합니다. **대상자 중복 비율**&#x200B;은 공동 작업자가 자신의 대상자와 귀하의 대상자 간의 중복 비율을 확인할 수 있는지 여부를 제어합니다."

>[!NOTE]
>
>공동 작업자가 모든 대상을 비공개로 설정한 경우 대상 인사이트의 **[!UICONTROL 관련 대상]** 보기가 비어 있습니다. [자세히 보기](/help/guide/collaborate/discover.md#relevant-audiences).

대상 메타데이터 정보 중 조직과 연결되기 전 또는 다른 프로젝트 보기 내에서 다른 조직에 표시되는 정보를 나타냅니다.

**[!UICONTROL ID 개수 표시]**: 이 설정은 [검색 탭에서 중복 보고서를 볼 때](/help/guide/collaborate/discover.md#discover-overlaps) 파트너가 대상의 ID 개수를 볼 수 있는지 여부를 제어합니다.

![ID 개수 표시 옵션이 선택 해제되고 선택된 병렬 이미지](/help/assets/setup/add-manage-audiences/show-identity-count.png)

**[!UICONTROL 대상 겹치기 표시 %]**: true로 설정하면 공동 작업자가 대상 및 사용자의 대상 간에 겹치는 비율을 [검색](/help/guide/collaborate/discover.md#compare-audiences)할 수 있습니다. 예를 들어 아래 기록에서 대상 `agora-advertiser-aud3`의 이 구성이 true로 설정되어 있고 공동 작업자는 해당 대상과 겹치는 비율을 볼 수 있습니다. 대상 `agora-advertiser-aud1`의 이 설정이 false로 설정되어 있으므로 공동 작업자가 겹침 백분율을 볼 수 없습니다.

![서로 다른 두 대상에 대한 대상 겹침 비율입니다.](/help/assets/setup/add-manage-audiences/audience-overlap-percentage.gif)

## 다음 단계

대상을 가져온 후 [연결](/help/guide/connect/establishing-connections.md) 섹션을 사용하여 연결할 게시자를 검색하고 프로젝트에 대한 공동 작업을 시작하십시오.
