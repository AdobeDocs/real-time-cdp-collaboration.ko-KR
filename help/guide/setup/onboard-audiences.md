---
title: Source 및 대상자 관리
description: Adobe Real-Time CDP Collaboration에서 대상자를 소스 및 관리하는 방법 알아보기
audience: admin, publisher, advertiser
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 0a5158fa-73d3-4406-af20-2b6c7be9934e
source-git-commit: 0dead396657c97cec47ddd64c8ec3c349f541a8f
workflow-type: tm+mt
source-wordcount: '3502'
ht-degree: 16%

---

# Source 및 대상자 관리

{{limited-availability-release-note}}

대상자는 다양한 속성에 따라 세그먼트화된 사용자 또는 고객의 특정 그룹입니다. 이를 통해 공동 작업자는 보다 효과적인 광고 캠페인을 위해 타기팅된 마케팅 및 개인화된 경험에 대해 공동 작업을 수행할 수 있습니다. 이 안내서에서는 대상을 Real-Time CDP Collaboration에 소스, 대상 대시보드 보기 및 개별 대상을 관리하는 방법을 다룹니다.

## Source 대상자를 Collaboration으로 {#source-audiences}

>[!IMPORTANT]
>
>소스 대상을 만들려면 사용자는 두 개의 프로필 관리 권한(**[!UICONTROL 프로필 보기]** 및 **[!UICONTROL 세그먼트 보기]**)이 포함된 역할에 할당되어야 합니다. 필요한 권한 할당에 대한 자세한 내용은 권한의 [대상 소싱](../permissions/overview.md#audience-sourcing) 안내서를 참조하십시오.

공동 작업자를 통해 대상자를 활성화하고 중복 계산을 실행하려면 먼저 대상자를 Collaboration에 소싱해야 합니다. 대상을 소싱하려면 아래 섹션의 워크플로 단계를 따르십시오.

**[!UICONTROL 설정]** 작업 영역의 **[!UICONTROL 내 대상]** 탭에서 추가 아이콘(![추가 아이콘)을 선택합니다.](/help/assets/icons/plus.png))을(를) 선택한 다음 **[!UICONTROL 대상]**&#x200B;을 선택합니다. 첫 번째 대상자인 경우 **[!UICONTROL 추가] 옵션**&#x200B;을 선택할 수도 있습니다.

![대상자 추가 옵션과 대상자 옵션이 강조 표시된 내 대상자 작업 영역입니다.](/help/assets/setup/add-manage-audiences/add-audiences.png){zoomable="yes"}

### 데이터 연결 선택 {#select-data-connection}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_marketing_actions"
>title="마케팅 액션"
>abstract="<p>마케팅 액션을 사용하여 Experience Platform에서 Real-Time CDP Collaboration으로 가져올 대상자 고객 데이터를 제어합니다. <strong>데이터 협업</strong> 마케팅 액션은 C4, C5, C9 데이터 사용 레이블을 지원합니다. <strong>데이터 과학</strong> 마케팅 액션은 C9 데이터 사용 레이블을 지원합니다.</p> <p> <ul><li> 확인란이 <em>표시</em>되어 있는 경우, Experience Platform에서 위에 언급된 레이블로 표시된 모든 데이터는 제외되며 Real-Time CDP Collaboration으로 이동되지 <strong>않습니다</strong>.</li><li> 확인란이 <em>비활성화된 </em> 경우, Experience Platform에서 Real-Time CDP Collaboration으로 가져올 수 있는 데이터에 제한이 없습니다.</li></ul></p>"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/data-governance/labels/overview.html?lang=ko" text="데이터 사용 레이블 개요"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/data-governance/labels/reference.html" text="데이터 사용 레이블 용어"

>[!IMPORTANT]
>
>첫 번째 데이터 연결을 설정하고 첫 번째 대상을 소싱한 후 기존 데이터 연결에서 여러 대상을 소싱할 수 있습니다. 데이터 연결이 이미 설정되었으므로 대상을 추가할 때는 [대상 선택](#select-audiences) 단계부터 시작합니다.

데이터 연결은 대상을 소싱하고 있는 위치의 데이터 소스입니다. 현재 지원되는 데이터 연결은 Adobe Experience Platform 뿐입니다.

데이터 연결에 대해 구성하는 모든 설정은 이 데이터 연결에서 가져온 모든 대상에 적용됩니다.

>[!TIP]
>
>데이터 연결을 보고 편집할 수 있는 별도의 워크플로우가 있습니다. 자세한 내용은 [데이터 연결 관리](/help/guide/setup/manage-data-connection.md) 안내서를 참조하십시오.

데이터 연결을 추가하려면 **[!UICONTROL 새 데이터 연결 추가]**&#x200B;를 선택한 후 **[!UICONTROL 다음]**&#x200B;을 선택합니다.

![새 데이터 연결 추가 옵션이 강조 표시된 대상자 추가 작업 영역입니다.](/help/assets/setup/add-manage-audiences/add-data-connection.png){zoomable="yes"}

#### 데이터 소스 선택

그런 다음 데이터 연결의 소스를 선택합니다. 사용 가능한 소스는 다음과 같습니다.

* **Adobe Experience Platform**: Adobe Experience Platform에서 대상을 가져오려면 이 옵션을 선택하십시오.
* **CSV 파일**(향후 릴리스): 빠르고 간단한 데이터 수집을 위해 대상 데이터가 포함된 CSV 파일을 업로드합니다.
* **Amazon Web Services**(향후 릴리스): Amazon S3 저장소에 연결하여 S3 버킷에서 직접 대상 데이터를 소싱합니다.
* **Snowflake**(향후 릴리스): Snowflake 데이터 웨어하우스를 사용하여 대상 데이터를 원활하게 가져올 수 있습니다.
* **Google Cloud Platform**(향후 릴리스): Google Cloud Storage에 연결하여 GCS 버킷에서 직접 대상 데이터를 소싱합니다.

데이터 원본을 선택한 후 **[!UICONTROL 다음]**&#x200B;을(를) 선택하십시오.

![Adobe Experience Platform 옵션이 강조 표시된 대상자 추가 작업 영역입니다.](/help/assets/setup/add-manage-audiences/select-data-connection-source.png){zoomable="yes"}

#### 샌드박스 선택

데이터 소스를 선택한 후 Collaboration에 사용할 대상을 포함하는 샌드박스를 선택해야 합니다. 사용 가능한 샌드박스 목록에서 샌드박스를 선택한 후 **[!UICONTROL 다음]**&#x200B;을 선택합니다.

![샌드박스가 선택된 대상 추가 작업 영역입니다.](/help/assets/setup/add-manage-audiences/select-sandbox.png){zoomable="yes"}

#### 거버넌스 정책 및 시행 액션 {#governance-policy-and-enforcement-actions}

그런 다음 소스 데이터에 올바른 마케팅 작업이 설정되어 있는지 확인해야 합니다. 또한 Experience Platform에서 가져온 데이터가 데이터 공동 작업에 사용될 수 있도록 동의해야 합니다.

마케팅 작업을 사용하여 Experience Platform에서 Collaboration으로 가져올 대상 데이터를 제어합니다. **[!UICONTROL 데이터 협업]** 마케팅 액션은 C4, C5, C9 데이터 사용 레이블을 지원합니다. **[!UICONTROL 데이터 과학]** 마케팅 액션은 C9 데이터 사용 레이블을 지원합니다.

[C4, C5 및 C9 데이터 사용 레이블](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/labels/reference#contract){target="_blank"}에 대해 자세히 알아보십시오.

* 확인란이 ***enabled***&#x200B;이면 위에서 설명한 대로 Experience Platform에서 레이블이 지정된 데이터는 제외되며 **not**&#x200B;이(가) Collaboration으로 전송됩니다.
* 확인란 ***비활성화됨***&#x200B;을 사용하면 Experience Platform에서 가져온 데이터에 제한이 없습니다.

Experience Platform 설명서에서 데이터 사용 레이블에 대해 자세히 알아보십시오.

* [데이터 사용 레이블 개요](https://experienceleague.adobe.com/ko/docs/experience-platform/data-governance/labels/overview){target="_blank"}
* [데이터 사용 레이블 용어집](https://experienceleague.adobe.com/ko/docs/experience-platform/data-governance/labels/reference){target="_blank"}

또한 Collaboration으로 소싱되는 데이터에 적용할 동의 규칙을 선택할 수 있습니다.

![거버넌스 정책 및 구현 작업 섹션에서 대상 추가 작업 영역입니다.](/help/assets/setup/add-manage-audiences/data-collaboration-consent.png){zoomable="yes"}

마케팅 작업 및 동의 규칙을 선택한 후 **[!UICONTROL 다음]**&#x200B;을(를) 선택하여 다음 단계로 진행합니다. 약관에 동의하라는 확인 대화 상자가 나타납니다. 확인란을 선택한 다음 **[!UICONTROL 확인]**&#x200B;을 선택하여 확인합니다.

![확인란과 확인 옵션이 강조 표시된 거버넌스 정책 및 구현 작업 대화 상자.](/help/assets/setup/add-manage-audiences/data-collaboration-consent-confirmation.png){zoomable="yes"}

### 세부 정보 입력

그런 다음 데이터 연결의 이름과 설명을 입력합니다. 이 정보는 나중에 데이터 연결을 식별하는 데 도움이 됩니다.

![이름 및 설명을 제공하는 옵션이 있는 대상 추가 작업 영역입니다.](/help/assets/setup/add-manage-audiences/data-connection-details.png){zoomable="yes"}

### 필드 매핑 {#map-fields}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_source_fields"
>title="소스 필드"
>abstract="소스 필드는 Experience Platform 구현의 ID 네임스페이스와 속성입니다. 이를 공동 작업에 정의된 대상 필드에 매핑할 수 있습니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_target_fields"
>title="대상 필드"
>abstract="대상 필드는 계정 설정 중에 선택한 일치 키입니다. 기본적으로 선택한 모든 일치 키를 사용할 수 있습니다."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_apply_transformation"
>title="변환 적용"
>abstract="소스에서 *해시되지 않은* 필드를 가져오는 경우, 이 옵션을 사용하면 공동 작업에서 해싱을 적용하고 일반 필드를 해시된 필드로 변환합니다."

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

다음으로 Collaboration의 대상 필드에 매핑할 소스 필드를 선택합니다. 사용 가능한 대상 필드는 계정 설정 중에 선택한 일치 키를 기반으로 합니다.

>[!IMPORTANT]
>
>현재, 새 맵 필드를 포함하도록 데이터 연결을 편집할 수 없습니다. 데이터 연결이 만들어진 후 계정에 새 일치 키를 추가하면 해당 키에 매핑할 새 데이터 연결을 만들어야 합니다.

![대상 필드에 소스 필드를 매핑하는 옵션이 있는 대상 추가 작업 영역입니다.](/help/assets/setup/add-manage-audiences/add-map-fields.png){zoomable="yes"}

>[!TIP]
>
>여러 소스 필드를 동일한 대상 필드에 매핑할 수 있습니다. 예를 들어, Experience Platform의 두 개의 별도 필드에 이메일 주소가 있는 경우, 각각의 주소를 **[!UICONTROL 해시된 이메일]** 대상 필드에 두 개의 별도 행으로 매핑할 수 있습니다. **[!UICONTROL 필드 추가]** 옵션을 사용하여 추가 매핑 행을 추가하십시오.

>[!BEGINSHADEBOX]

**[!UICONTROL Source 필드]**&#x200B;은(는) Experience Platform의 ID 네임스페이스 및 특성입니다. 여기에는 [standard](https://experienceleague.adobe.com/docs/experience-platform/identity/features/namespaces.html#standard){target="_blank"} 및 [custom](https://experienceleague.adobe.com/docs/experience-platform/identity/features/namespaces.html#create-namespaces){target="_blank"} ID 네임스페이스가 모두 포함됩니다. 또한 [유니온 스키마](https://experienceleague.adobe.com/docs/experience-platform/profile/union-schemas/union-schema.html){target="_blank"}에 있고 XDM 개별 프로필 클래스에 속하는 프로필 특성도 포함됩니다.

Source 필드는 Collaboration에 정의된 대상 필드에 매핑됩니다.

**[!UICONTROL 대상 필드]**&#x200B;은(는) ID가 Collaboration에서 참조되는 방식을 나타냅니다. 대상 필드는 계정 설정 중에 선택한 일치 키입니다. 기본적으로 선택한 모든 일치 키를 사용할 수 있습니다.

해시된 필드에 **[!UICONTROL 해시되지 않은]** 필드를 소싱할 때 *변환 적용* 옵션을 사용하십시오. Collaboration은 해싱을 적용하고 필드를 변환합니다. Adobe에서 사용하는 해싱 알고리즘은 SHA256입니다.

>[!ENDSHADEBOX]

필드 매핑을 시작하려면 대상 필드 옆에 있는 빈 소스 필드를 선택합니다. **[!UICONTROL 소스 필드 선택]** 대화 상자가 나타납니다. **[!UICONTROL ID 네임스페이스]**&#x200B;와(과) **[!UICONTROL 프로필 속성]** 옵션 중에서 선택하여 원하는 소스 필드를 찾은 다음 목록에서 필드를 선택합니다. 검색 옵션을 사용하여 원하는 필드를 찾을 수도 있습니다.

![전자 메일 옵션이 표시된 원본 필드 선택 대화 상자입니다.](/help/assets/setup/add-manage-audiences/select-source-field.png){zoomable="yes"}

해시되지 않은 필드를 해시된 대상 필드에 소싱하려면 **[!UICONTROL 변환 적용]** 옵션을 사용하십시오. 예를 들어 두 번째 전자 메일 필드를 추가하려면 **[!UICONTROL 필드 추가]** 옵션을 선택하여 새 행을 추가한 다음 대상 필드에 대해 **[!UICONTROL 해시된 전자 메일]**&#x200B;을 선택합니다. 해시되지 않은 전자 메일 원본 필드를 선택한 다음 **[!UICONTROL 변환 적용]**&#x200B;을 선택합니다.

![전자 메일 원본 필드가 대상 필드에 매핑된 대상자 추가 작업 영역입니다. 변환 적용 이 켜진 상태로 있습니다.](/help/assets/setup/add-manage-audiences/apply-transformation.png){zoomable="yes"}

각 대상 필드에 대한 매핑 쌍을 계속 추가합니다. 일치 키를 사용하지 않으려면 필드 옆에 있는 삭제(![삭제 아이콘](/help/assets/icons/delete.png)) 아이콘을 사용하여 제거할 수 있습니다. 일치 키가 제거되면 연결에서 대상을 소싱할 때 일치 키를 사용할 수 없습니다.

![대상 필드 옆에 삭제 옵션이 강조 표시된 대상 추가 작업 영역입니다.](/help/assets/setup/add-manage-audiences/remove-target-field.png){zoomable="yes"}

필드 매핑을 마치면 **[!UICONTROL 다음]**&#x200B;을(를) 선택하여 계속하십시오.

![맵 필드가 채워져 있고 다음 옵션이 강조 표시된 대상자 추가 작업 영역입니다.](/help/assets/setup/add-manage-audiences/confirm-field-mapping.png){zoomable="yes"}

### 예약 {#schedule}

다음으로 대상자 채우기를 시작하고 종료할 시기를 예약합니다. 대상자는 이 일정에 따라 새로 고쳐집니다.

![예약 옵션이 표시된 대상 추가 작업 영역입니다.](/help/assets/setup/add-manage-audiences/audience-scheduling.png){zoomable="yes"}

>[!IMPORTANT]
>
>대상 업데이트 빈도를 조정하면 대상 새로 고침에 따라 계산되는 [대상 관리 크레딧 활동](/help/guide/setup/my-activity.md#types-of-activities)을 관리하는 데 도움이 됩니다. 더 높은 빈도를 선택하면 대상 검색 보고서와 대상 활성화에 사용할 수 있는 데이터의 최신 상태가 영향을 줄 수 있습니다.

**[!UICONTROL 빈도]** 드롭다운에서 대상 새로 고침 빈도를 선택하십시오.

![빈도 드롭다운이 열려 있는 작업 영역을 예약하는 대상 추가.](/help/assets/setup/add-manage-audiences/audience-scheduling-frequency.png){zoomable="yes"}

그런 다음 **[!UICONTROL 날짜 범위]**&#x200B;를 선택합니다. 시작 날짜는 대상자가 프로필로 채우기를 시작하는 날짜이고 종료 날짜는 대상자가 새로 고침을 중지하는 날짜입니다.

![날짜 범위 옵션이 표시된 작업 영역을 예약하는 대상 추가.](/help/assets/setup/add-manage-audiences/audience-scheduling-date-range.png){zoomable="yes"}

>[!IMPORTANT]
>
>날짜 범위의 종료 날짜 이후, 이 데이터 연결에서 가져온 모든 대상의 새로 고침이 중지됩니다. 연결을 갱신하려면 [데이터 연결 관리](/help/guide/setup/manage-data-connection.md) 안내서를 따르십시오.

### 대상자 선택 {#select-audiences}

대상 소스를 선택한 후 포함할 특정 대상을 선택합니다. 검색 및 필터 옵션을 사용하여 데이터 연결에서 관련 대상을 찾습니다. 원하는 대상을 선택한 후 **[!UICONTROL 다음]**&#x200B;을 선택합니다.

![사용 가능한 대상 목록이 있는 대상 추가 작업 영역입니다.](/help/assets/setup/add-manage-audiences/select-audience.png){zoomable="yes"}

### 검토

대상자 추가를 완료하기 전에 모든 구성 및 설정을 검토하십시오. 모든 세부 정보가 올바른지 확인한 다음 **[!UICONTROL 완료]**&#x200B;를 선택하여 데이터 연결 만들기를 완료합니다.

![모든 선택 구성이 표시된 대상자 추가 작업 영역입니다.](/help/assets/setup/add-manage-audiences/review-connection.png){zoomable="yes"}

## 대상자 대시보드 보기 {#view-audiences-dashboard}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_missing_identities"
>title="누락된 ID"
>abstract="구성된 일정에 따라 다음 데이터 연결이 새로 고쳐진 후에 ID 개수를 확인할 수 있습니다. 일반적으로 데이터 연결이 설정된 후 24시간 이내에 최초 새로 고침이 이루어집니다. 구성된 일정에 따라 지속적인 새로 고침이 진행됩니다."

대상을 소싱하면 **[!UICONTROL 내 대상]** 작업 영역에 Collaboration에 현재 소싱되어 있는 모든 대상이 표시됩니다.

![모든 대상이 소스로 제공되는 내 대상 작업 영역입니다.](/help/assets/setup/add-manage-audiences/audiences-workspace.png)

각 대상에는 다음 정보에 대한 개요가 포함되어 있습니다.

| 항목 | 설명 |
|----------|---------|
| **[!UICONTROL 이름]** | 대상자의 이름입니다. |
| **[!UICONTROL ID]** | 이 대상에 있는 ID의 수를 나타냅니다. 동일한 프로필에 두 개 이상의 ID가 있고 이러한 ID가 프로젝트에서 일치 키로 사용되는 경우 프로필이 카운트에 두 번 표시됩니다. |
| **[!UICONTROL 상태]** | 대상이 활성 상태이고 프로젝트에서 사용할 수 있는지 여부를 나타냅니다. **[!UICONTROL 보류 중]** 상태는 대상이 최근에 소싱되었으며 ID가 아직 채워지지 않았음을 나타냅니다. 소스 대상은 초기 새로 고침 후 프로필로 채워집니다. 이 프로필은 일반적으로 데이터 연결이 설정된 후 24시간 이내에 발생합니다. |
| **[!UICONTROL Source]** | 대상자를 가져온 위치를 나타냅니다. 현재 Collaboration 릴리스에서는 Experience Platform이 유일한 지원 소스입니다. |
| **[!UICONTROL 데이터 연결]** | 대상자에 대한 데이터 연결은 출처입니다. 데이터 연결을 보기 위한 이름을 선택할 수 있습니다. |
| **[!UICONTROL 연결 액세스]** | 대상자가 비공개인지 아니면 공용인지 정의합니다. 공개 대상은 중복 보고서에서 검색할 수 있으며 프로젝트 내에서 활성화할 수 있습니다. |
| **[!UICONTROL 생성일]** | 대상이 처음에 Collaboration으로 소싱되었을 때를 나타냅니다. |
| **[!UICONTROL 마지막으로 업데이트됨]** | Collaboration에서 대상이 마지막으로 업데이트된 날짜 및 시간을 나타냅니다. 이는 대상을 마지막으로 새로 고친 때가 아니라 대상의 구성 또는 메타데이터가 마지막으로 변경된 때를 나타냅니다. |

![모든 대상이 소스로 제공되는 내 대상 작업 영역입니다.](/help/assets/setup/add-manage-audiences/audiences-workspace.png){zoomable="yes"}

대상자에 대해 빠른 작업을 수행하려면 대상자 이름 옆에 있는 생략 부호 **..**&#x200B;을(를) 선택하십시오. 다음 옵션을 사용할 수 있습니다.

* **[!UICONTROL 범주 편집]**&#x200B;을 통해 대상에 다른 범주 태그를 추가할 수 있습니다. 자세한 내용은 아래의 [범주](#categories) 섹션을 참조하십시오.
* **[!UICONTROL 삭제]**&#x200B;하면 데이터 연결에서 대상이 삭제됩니다.

![줄임표 메뉴가 열려 있고 범주 편집 및 삭제 옵션이 강조 표시된 내 대상 작업 영역입니다.](/help/assets/setup/add-manage-audiences/audiences-ellipsis-menu.png){zoomable="yes"}

## 개별 대상자 보기 {#view-individual-audiences}

개별 대상에 대한 정보를 보고 업데이트하려면 **[!UICONTROL 내 대상]** 작업 영역에서 대상을 선택하십시오. 대상 작업 공간에는 세부 사항, ID, 카테고리, 연결 액세스 및 메타데이터 가시성 설정을 포함하여 선택한 대상에 대한 자세한 정보가 표시됩니다.

### 대상자 세부 정보

각 개별 대상자에 대해 다음 정보가 표시됩니다.

| 항목 | 설명 |
|----------|---------|
| **[!UICONTROL 상태]** | 대상이 활성 상태이고 프로젝트에서 사용할 수 있는지 여부를 나타냅니다. |
| **[!UICONTROL Source]** | 대상자를 가져온 위치를 나타냅니다. 현재 Collaboration 릴리스에서는 Experience Platform이 유일한 지원 소스입니다. |
| **[!UICONTROL 데이터 연결]** | 대상자에 대한 데이터 연결은 출처입니다. |
| **[!UICONTROL 마지막으로 업데이트됨]** | Collaboration에서 대상이 마지막으로 업데이트된 날짜 및 시간을 나타냅니다. 이는 대상을 마지막으로 새로 고친 때가 아니라 대상의 구성 또는 메타데이터가 마지막으로 변경된 때를 나타냅니다 |
| **[!UICONTROL 마지막으로 업데이트한 사람]** | 대상자를 마지막으로 업데이트한 사용자를 나타냅니다. |
| **[!UICONTROL 생성일]** | 대상이 처음에 Collaboration으로 소싱되었을 때를 나타냅니다. |
| **[!UICONTROL 만든 사람]** | 대상을 Collaboration으로 가져온 사용자를 나타냅니다. |

![개별 대상자의 작업 영역입니다.](/help/assets/setup/add-manage-audiences/audience-details.png){zoomable="yes"}

#### ID {#identities}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_identities"
>title="ID"
>abstract="이 대상자를 구성하는 ID를 일치 키로 구분하여 분석한 결과입니다."

**[!UICONTROL ID]** 섹션은 대상자에 있는 ID의 수를 나타냅니다. 또한 섹션에는 대상자의 구성을 이해하는 데 도움이 되는 일치 키별 ID 분류가 포함되어 있습니다.

![개별 대상자의 작업 영역에 있는 ID 섹션입니다.](/help/assets/setup/add-manage-audiences/audience-details-identities.png){zoomable="yes"}

일치 키 분류의 개별 섹션 위로 마우스를 가져가면 관련 키에 대한 정확한 ID 카운트가 제공됩니다.

![일치 키 분류와 함께 개별 대상자의 작업 영역에 있는 ID 섹션입니다.](/help/assets/setup/add-manage-audiences/audience-details-identities.png)

#### 카테고리 {#categories}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_categories"
>title="카테고리"
>abstract="대상자에 태그를 지정하면 쉽게 구성, 필터링 및 검색할 수 있습니다. 여러 개의 카테고리로 대상자에 태그를 지정한 다음 이 카테고리 태그를 사용하여 제품의 다른 영역에서 원하는 대상자를 필터링할 수 있습니다."

대상자를 쉽게 구성하고, 필터링하고, 검색할 수 있도록 대상자에 태그를 지정할 수 있습니다. 대상 중복 보고서를 실행할 때 여러 범주가 있는 대상에 태그를 지정한 다음 이러한 범주 태그를 사용하여 [discover](/help/guide/collaborate/discover.md) 제품 영역에서 원하는 대상을 필터링할 수 있습니다.

범주를 추가하려면 **[!UICONTROL 범주]** 섹션 내에서 **[!UICONTROL 편집]** 옵션을 선택하십시오.

![개별 대상자의 작업 영역에 있는 범주 섹션입니다.](/help/assets/setup/add-manage-audiences/audience-details-categories.png){zoomable="yes"}

대상자에 추가할 범주를 선택할 수 있는 **[!UICONTROL 범주]** 대화 상자가 나타납니다. 개별 범주를 선택하려면 범주 이름 옆에 있는 확인란을 선택합니다.


#### 연결 액세스 {#connection-access}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_connection_access"
>title="연결 액세스"
>abstract="<p>대상자는 공개, 비공개, 사용자 정의 등 세 가지 유형으로 나눌 수 있습니다.</p><p> 공동 작업자가 있는 프로젝트에서 사용 가능한지 여부는 연결 액세스 설정에 따라 다릅니다.</p>"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_access"
>title="자세히 보기"
>abstract=""

공동 작업자가 있는 프로젝트에서 대상을 사용할 수 있는지는 연결 액세스 설정에 따라 다릅니다. **[!UICONTROL 연결 액세스]** 섹션에서 대상자가 개인 대상인지, 공용 대상인지 또는 특정 연결에만 사용할 수 있는지 선택할 수 있습니다. 공용 대상은 연결에서 사용 가능하고 검색 가능합니다.

대상자의 연결 액세스를 업데이트하려면 **[!UICONTROL 연결 액세스]** 섹션 내에서 **[!UICONTROL 편집]** 옵션을 선택하십시오.

![개별 대상자 작업 영역의 연결 액세스 섹션입니다.](/help/assets/setup/add-manage-audiences/audience-details-connection-access.png){zoomable="yes"}

사용 가능한 연결 액세스 옵션이 세 개 있는 **[!UICONTROL 연결 액세스]** 대화 상자가 나타납니다.

* **[!UICONTROL 개인 대상자]**. 이러한 대상은 중복 보고서에서 사용하거나 공동 작업자와의 연결에서 활성화할 수 *없음*&#x200B;입니다. 공동 작업자가 보거나 사용할 수 있는 대상은 아니지만, 대상의 모집단은 여전히 **[!UICONTROL 대상 비교 섹션]**&#x200B;의 [모든 대상](/help/guide/collaborate/discover.md#compare-audiences) 보기에서 총 모집단에 기여합니다. 공동 작업자와 연결에서 대상을 사용하려면 설정을 공개 또는 사용자 지정으로 변경하십시오.
* **[!UICONTROL 공개 대상]**. 이러한 대상은 중복 보고서에서 사용하고 공동 작업자와의 연결에서 활성화할 수 있습니다.
* **[!UICONTROL 사용자 지정 대상]**. 이러한 대상은 중복 보고서에서 사용할 수 있으며 지정된 연결에서만 활성화할 수 있습니다. 공동 작업자가 보거나 사용할 수 있는 대상은 아니지만, 대상의 모집단은 여전히 **[!UICONTROL 대상 비교 섹션]**&#x200B;의 [모든 대상](/help/guide/collaborate/discover.md#compare-audiences) 보기에서 총 모집단에 기여합니다.

원하는 연결 액세스 옵션을 선택한 다음 **[!UICONTROL 저장]**&#x200B;을 선택하여 변경 내용을 적용합니다.

![사용 가능한 옵션이 표시된 연결 액세스 대화 상자입니다.](/help/assets/setup/add-manage-audiences/audience-details-connection-access-dialog.png){zoomable="yes"}

>[!IMPORTANT]
>
>액세스 상태(공개, 비공개 또는 사용자 지정)에 관계없이 모든 대상의 모집단은 프로젝트 내의 **[!UICONTROL 대상 비교]** 섹션에서 **[!UICONTROL 모든 대상]** 모집단에 기여합니다.

공동 작업자가 있는 프로젝트에서 사용할 수 있는 대상 가용성은 연결 액세스 설정에 따라 다릅니다.

#### 메타데이터 가시성 {#metadata-visibility}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_metadata_visibility"
>title="메타데이터 가시성"
>abstract="<p>다른 공동 작업자가 귀하와 연결하거나 프로젝트 보기에서 해당 대상자의 메타데이터 중 어떤 것을 볼 수 있는지를 나타냅니다.</p> <p> **ID 수**&#x200B;는 검색 탭에서 중복 보고서를 볼 때 공동 작업자가 대상자의 ID 수를 볼 수 있는지 여부를 제어합니다.</p><p> **대상자 중복 비율**&#x200B;은 공동 작업자가 자신의 대상자와 귀하의 대상자 간의 중복 비율을 확인할 수 있는지 여부를 제어합니다.</p><p> **[!UICONTROL 대상자 색인]**&#x200B;은 공동 작업자가 프로젝트 내에서 대상자 색인을 볼 수 있는지 여부를 제어합니다. 이 기능은 활성 대상자가 3명 이상인 경우에만 사용할 수 있습니다.</p> <br> 메타데이터 가시성 설정을 적용하려면 대상자를 공개 또는 사용자 지정으로 설정해야 합니다."

>[!NOTE]
>
>공동 작업자가 모든 대상을 전용으로 설정한 경우 **[!UICONTROL 검색]** 작업 영역에서 프로젝트의 **[!UICONTROL 관련 대상]** 섹션이 비어 있습니다. 자세한 내용은 [검색](/help/guide/collaborate/discover.md#relevant-audiences) 안내서를 참조하십시오.

메타데이터 가시성은 대상자가 사용자와 연결되기 전 또는 다른 프로젝트 보기 내에서 대상자의 메타데이터를 다른 공동 작업자에게 가시적으로 보여 줍니다. 대상자의 메타데이터 가시성을 업데이트하려면 **[!UICONTROL 메타데이터 가시성]** 섹션 내에서 **[!UICONTROL 편집]** 옵션을 선택하십시오.

![개별 대상자의 작업 영역에 있는 메타데이터 가시성 섹션입니다.](/help/assets/setup/add-manage-audiences/audience-details-metadata-visibility.png){zoomable="yes"}

대상에 대한 가시성 설정을 구성할 수 있는 **[!UICONTROL 메타데이터 가시성]** 대화 상자가 나타납니다. 각 대상에 대해 구성할 수 있는 두 가지 메타데이터 가시성 설정이 있습니다.

**[!UICONTROL ID 개수 표시]**: 이 설정은 프로젝트 내의 [검색 탭에서 중복 보고서를 볼 때](/help/guide/collaborate/discover.md#discover-overlaps) 공동 작업자가 대상의 ID 개수를 볼 수 있는지 여부를 제어합니다.

**[!UICONTROL 대상 겹치기 표시 %]**: 이 설정은 공동 작업자가 대상자와 대상 간의 겹치기 비율을 [검색](/help/guide/collaborate/discover.md#compare-audiences)할 수 있는지 여부를 제어합니다.

**[!UICONTROL 대상 인덱스]**: true로 설정하면 공동 작업자가 프로젝트 내에서 [대상 인덱스](/help/guide/collaborate/discover.md#audience-index-score)을(를) 볼 수 있습니다. 이 기능은 활성 대상자가 3명 이상인 경우에만 사용할 수 있습니다.

>[!NOTE]
>
>메타데이터 가시성 설정을 적용하려면 대상을 공개 또는 사용자 지정으로 설정해야 합니다.

![사용 가능한 옵션이 표시된 메타데이터 가시성 대화 상자입니다.](/help/assets/setup/add-manage-audiences/audience-details-metadata-dialog.png){zoomable="yes"}

## 여러 대상 편집 {#edit-audiences}

대상 대시보드에서 여러 대상을 한 번에 편집할 수 있습니다. 이렇게 하려면 이름 옆에 있는 상자를 선택하여 편집할 대상을 선택합니다. 대상자를 선택하면 편집 메뉴에 있는 옵션을 사용하여 작업을 수행할 수 있습니다.

![두 대상이 선택되어 있고 편집 메뉴가 강조 표시된 내 대상 작업 영역입니다.](/help/assets/setup/add-manage-audiences/audiences-bulk-edit.png)

### 메타데이터 가시성 일괄 편집 {#bulk-edit-metadata-visibility}

대상자 대시보드에서 대상자를 선택한 상태에서 편집 메뉴에서 **[!UICONTROL 메타데이터 가시성 편집]**&#x200B;을 선택합니다.

![메타데이터 가시성 편집 옵션이 강조 표시된 내 대상 작업 영역입니다.](/help/assets/setup/add-manage-audiences/audiences-bulk-edit-metadata.png)

선택한 대상에 대한 가시성 설정을 구성할 수 있는 **[!UICONTROL 메타데이터 가시성]** 대화 상자가 나타납니다. 기본적으로 옵션이 선택되지 않습니다. 선택한 모든 대상에 적용할 옵션을 선택한 다음 **[!UICONTROL 저장]**&#x200B;을 선택합니다.

![사용 가능한 옵션이 표시된 메타데이터 가시성 대화 상자입니다.](/help/assets/setup/add-manage-audiences/audience-details-metadata-dialog.png)

### 연결 액세스 일괄 편집 {#bulk-edit-connection-access}

대상자 대시보드에서 대상자를 선택한 상태에서 편집 메뉴에서 **[!UICONTROL 연결 액세스 편집]**&#x200B;을 선택합니다.

![연결 액세스 편집 옵션이 강조 표시된 내 대상 작업 영역입니다.](/help/assets/setup/add-manage-audiences/audiences-bulk-edit-connection-access.png)

선택한 대상에 대한 액세스 설정을 구성할 수 있는 **[!UICONTROL 연결 액세스]** 대화 상자가 나타납니다. 기본적으로 **[!UICONTROL 개인 대상]** 옵션이 선택됩니다. 선택한 모든 대상에 적용할 옵션을 선택한 다음 **[!UICONTROL 저장]**&#x200B;을 선택합니다.

![사용 가능한 옵션이 표시된 연결 액세스 대화 상자입니다.](/help/assets/setup/add-manage-audiences/audience-details-connection-access-dialog.png)

### 대상자 이름 및 설명 벌크 편집 {#bulk-edit-audience-names-descriptions}

대상자 대시보드에서 대상자를 선택한 상태에서 편집 메뉴에서 **[!UICONTROL 이름 및 설명 편집]**&#x200B;을(를) 선택하십시오.

![이름 및 설명 편집 옵션이 강조 표시된 내 대상 작업 영역입니다.](/help/assets/setup/add-manage-audiences/audiences-bulk-edit-name-description.png)

선택한 각 대상자의 이름과 설명을 구성할 수 있는 **[!UICONTROL 이름 및 설명]** 대화 상자가 나타납니다. 기본적으로 각 대상에 대해 현재 이름과 설명이 표시됩니다. 변경한 다음 **[!UICONTROL 저장]**&#x200B;을 선택합니다.

![사용 가능한 옵션이 표시된 이름 및 설명 대화 상자입니다.](/help/assets/setup/add-manage-audiences/audiences-bulk-edit-name-description-dialog.png)

### 범주 일괄 편집 {#bulk-edit-categories}

대상자 대시보드에서 대상자를 선택한 상태에서 편집 메뉴에서 **[!UICONTROL 범주 편집]**&#x200B;을 선택합니다.

![범주 편집 옵션이 강조 표시된 내 대상 작업 영역입니다.](/help/assets/setup/add-manage-audiences/audiences-bulk-edit-categories.png)

선택한 각 대상에 대해 범주를 구성할 수 있는 **[!UICONTROL 범주]** 대화 상자가 나타납니다. 기본적으로 범주가 선택되지 않습니다. 범주를 선택하려면 먼저 기본 범주를 선택한 다음 포함할 하위 범주를 선택합니다. 변경한 다음 **[!UICONTROL 저장]**&#x200B;을 선택합니다.

![사용 가능한 옵션이 표시된 범주 대화 상자입니다.](/help/assets/setup/add-manage-audiences/audiences-bulk-edit-categories-dialog.png)

## 다음 단계

대상을 소싱한 후 프로젝트에서 공동 작업을 수행하기 위해 공동 작업자를 [연결](/help/guide/connect/establishing-connections.md)할 차례입니다.
