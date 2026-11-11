---
title: '[!DNL The Trade Desk] (Alpha)의 유료 미디어 신호로 프로필 보강'
description: 유료 미디어 강화 속성을 내보내고, 전달된 CSV를 수집하며, 대상 구축 및 개인화를 위해 자사 프로필을 업데이트하는 방법을 알아봅니다.
audience: advertiser
hide: true
badge: Alpha
source-git-commit: d090aff6ea091f60c9b3bbaf2ca72fcf8017d7d1
workflow-type: tm+mt
source-wordcount: '1503'
ht-degree: 0%
---

# Trade Desk 프로필 강화(Alpha)

[!DNL The Trade Desk]의 REDS(원시 이벤트 데이터 스트림) 노출 로그 데이터 피드를 사용하여 데이터 보강 특성 및 유료 미디어 컨텍스트를 자사 프로필로 내보냅니다.

CSV 파일이 [!DNL Amazon S3] 내보내기 대상에 도착한 후 [!DNL Adobe Real-Time CDP]&#x200B;(으)로 수집하십시오. 이 릴리스에서 파일을 내보내도 프로필이 자동으로 업데이트되거나 경험이 활성화되지 않습니다. [!DNL Adobe Real-Time CDP]에 대한 자동 프로필 보강은 후속 릴리스의 기능입니다.

광고 노출은 고객 프로필에 컨텍스트를 추가합니다. 참여, 구매 의도 또는 장기 관심사를 확인하지 않습니다.

## 데이터 보강 준비 {#prepare-for-enrichment}

시작하기 전에 관리자, 미디어 팀 및 데이터 팀과 협력하여 다음을 확인합니다.

* [!DNL Adobe Real-Time CDP Collaboration]에 대한 액세스 권한과 서명된 참여 계약입니다.
* REDS 피드 프로비저닝을 승인하기 위해 액세스 편지를 [!DNL The Trade Desk]&#x200B;(으)로 완료했습니다.
* 해시된 이메일 주소 또는 해시된 전화 번호를 사용하는 [!DNL Adobe Real-Time CDP Collaboration]에서 사용할 수 있는 자사 대상자입니다. 다른 식별자는 이 릴리스에서 지원되지 않습니다.
* 데이터 보강 출력을 받도록 구성된 [!DNL Amazon S3] 대상입니다.
* 전달된 파일을 [!DNL Adobe Real-Time CDP]&#x200B;(으)로 수집하는 프로세스입니다.

### 소스 피드 승인 {#authorize-source-feed}

[!DNL The Trade Desk]이(가) 제공한 액세스 편지를 완료하여 [!DNL The Trade Desk]이(가) REDS 로그를 Adobe으로 직접 보내도록 승인합니다.

[!DNL The Trade Desk]에서 원본 피드를 프로비저닝하고 Adobe에서 액세스 및 수집을 구성합니다. 프로젝트를 만들기 전에 연결이 활성 상태이고 피드가 준비되었는지 확인하십시오.

처리 후 데이터 보강 출력 파일이 내보내기 대상에 도착합니다.

### 다운스트림 수집 준비 {#prepare-downstream-ingestion}

게재 후 [!DNL Adobe Real-Time CDP] 관리자 또는 기술 지원 팀에 문의하여 파일을 수집하십시오.

## 프로젝트 연결 및 만들기 {#connect-create-projects}

연결 대화 상자에서 액세스 문자를 완료하고 파트너 ID를 저장합니다. 프로젝트를 생성하기 전에 Adobe에서 REDS 로그 수신을 확인할 때까지 기다립니다. 프로젝트를 만들면 데이터 보강 작업이 시작되며, 이를 위해서는 파트너 ID와 로그가 모두 필요합니다.

### 파트너와 연결 {#connect-partner}

[!DNL The Trade Desk]에 연결하고 광고주 정보를 추가하십시오.

1. **[!UICONTROL 연결]**&#x200B;에서 **[!UICONTROL 공동 작업자 검색]**&#x200B;을 엽니다.
1. [!DNL The Trade Desk] 검색
   ![Collaborator 카탈로그에 [!DNL The Trade Desk] 및 해당 [!UICONTROL 연결] 옵션이 나열됩니다.](../../../assets/collaborate/advertising-platforms/discover-collaborators-trade-desk.png){zoomable="yes"}
1. [!DNL The Trade Desk]에 대해 **[!UICONTROL 연결]**&#x200B;을 선택하고 연결 대화 상자의 지침을 따릅니다.
   ![연결 대화 상자에서 [!DNL The Trade Desk]에 대한 REDS 인증 및 파트너 ID 설정을 설명합니다.](../../../assets/collaborate/advertising-platforms/trade-desk-connection-instructions.png){zoomable="yes"}
1. 연결이 활성 상태가 되면 **[!UICONTROL 연결 설정]**&#x200B;을 여십시오. **[!UICONTROL 광고주 정보]**&#x200B;에서 **[!UICONTROL 편집]**&#x200B;을 선택하여 기존 정보를 업데이트하거나 **[!UICONTROL 추가]**&#x200B;를 선택하여 새 정보를 입력하십시오.
   ![활성 연결 설정에 [!UICONTROL 광고주 정보] 및 [!UICONTROL 편집] 컨트롤이 표시됩니다.](../../../assets/collaborate/advertising-platforms/trade-desk-connection-settings.png){zoomable="yes"}
1. **[!UICONTROL 파트너 ID]** 및 **[!UICONTROL 파트너 이름]**&#x200B;에 파트너 ID와 파트너 이름을 입력한 다음 **[!UICONTROL 저장]**&#x200B;을 선택합니다. **[!UICONTROL 시트 식별자]**&#x200B;의 [!DNL The Trade Desk] 계정에서 파트너 ID를 찾으십시오.
   ![광고주 정보 대화 상자에 필요한 파트너 ID 및 파트너 이름 필드와 [!UICONTROL 저장] 컨트롤이 있습니다.](../../../assets/collaborate/advertising-platforms/trade-desk-advertiser-partner-info-dialog.png){zoomable="yes"}

연결이 활성화되고 광고주 정보를 저장한 후 Adobe이 REDS 로그를 수신했는지 확인할 때까지 기다립니다. 그런 다음 프로젝트를 만듭니다.

### 프로젝트 만들기 {#create-project}

연결을 위한 프로젝트 만들기:

1. **[!UICONTROL 공동 작업]**&#x200B;에서 **[!UICONTROL 내 프로젝트]**&#x200B;를 선택하세요.
1. **[!UICONTROL 프로젝트 만들기]** 또는 추가 아이콘(![프로젝트 추가.](/help/assets/icons/plus.png))을 선택하십시오.
1. **[!UICONTROL 프로젝트 만들기]**&#x200B;에서 **[!UICONTROL 공동 작업자]**&#x200B;에서 [!DNL The Trade Desk]을(를) 선택하십시오.
   ![[!UICONTROL 프로젝트 만들기] 양식에서 [!DNL The Trade Desk]을(를) 나열하고 프로젝트 이름, 설명 및 이미지 필드를 포함합니다.](../../../assets/collaborate/advertising-platforms/trade-desk-create-project.png){zoomable="yes"}
1. **[!UICONTROL 프로젝트 이름]** 및 **[!UICONTROL 설명]**&#x200B;을 입력한 다음 프로젝트를 식별할 이미지를 선택하십시오.
1. **[!UICONTROL 만들기]**&#x200B;를 선택합니다.

일반적인 프로젝트 관리에 대해서는 [프로젝트 만들기 및 관리 가이드](/help/guide/collaborate/manage-projects.md)를 참조하십시오.

## 속성 선택 및 내보내기 {#select-export-attributes}

프로젝트에서 데이터 보강 속성 내보내기:

<!-- TODO: Replace the destination screenshot with one showing the [!UICONTROL Export Attributes] action. -->

1. 프로젝트를 열고 **[!UICONTROL 강화]**&#x200B;를 선택합니다.
1. 각 속성에 대한 적용 범위 값을 검토하여 신호 가용성을 파악합니다.
1. 데이터 보강에 사용할 속성을 선택합니다.
   ![[!UICONTROL 강화] 페이지는 선택 가능한 신호를 범주별로 그룹화하고 범위 값을 표시합니다.](../../../assets/collaborate/advertising-platforms/enrich-attribute-selection.png){zoomable="yes"}
1. 데이터 보강 출력에 대해 구성된 [!DNL Amazon S3] 내보내기 대상을 선택하십시오. 대상을 구성하려면 [클라우드 저장소 대상 구성 및 관리](/help/guide/destinations/manage-destinations.md)를 참조하십시오.
   <!-- ![The [!UICONTROL Choose a destination] screen lists a destination and the [!UICONTROL Export Attributes] action.](../../../assets/collaborate/advertising-platforms/enrich-choose-destination.png){zoomable="yes"} -->
1. 선택한 특성과 대상을 검토한 다음 **[!UICONTROL 특성 내보내기]**&#x200B;를 선택하십시오.
   <!-- ![The destination screen confirms that enrichment has started.](../../../assets/collaborate/advertising-platforms/enrich-request-confirmation.png){zoomable="yes"} -->

대상이 올바르게 구성된 경우 내보내기 제출이 게재를 시작합니다. [!DNL Adobe Real-Time CDP Collaboration] 외부에서 파일을 성공적으로 배달했는지 확인하십시오.

Adobe은 사용자가 프로젝트를 만든 다음 매주 데이터 보강 속성을 처리합니다. 각 실행은 사용 가능한 [!DNL The Trade Desk]개의 최근 90일 데이터를 사용합니다. 각 내보내기에는 가장 최근에 완료된 실행에서 선택한 속성이 포함됩니다. 새로 고친 속성을 내보내려면 나중에 실행이 완료된 후 다른 내보내기를 요청합니다.

### 사용 가능한 데이터 보강 신호 {#available-signals}

4개의 카테고리에 걸쳐 18개의 조정된 신호 중에서 선택합니다. 사용자 지정 데이터 보강 표현식은 지원되지 않습니다.

| 카테고리 | 신호 | 설명 |
| --- | --- | --- |
| 코어 | [!UICONTROL 마지막으로 노출된 날짜] | ID가 가장 최근에 광고에 노출된 날짜입니다. |
| 코어 | [!UICONTROL 노출 수] | 노출 빈도 범주(원시 노출 수가 아님). |
| 코어 | [!UICONTROL 전망 및 재타겟팅] | 잠재 고객 또는 리마케팅으로 노출 분류 유추. |
| 코어 | [!UICONTROL 제품 범주 표시] | 광고에서 홍보된 제품에 대해 유추된 범주. |
| 코어 | [!UICONTROL 주요 인벤토리 채널] | 광고 노출과 연계된 기본 인벤토리 채널. |
| 코어 | [!UICONTROL 상위 장치 유형] | 광고 노출과 관련된 기본 디바이스 유형입니다. |
| Geography | [!UICONTROL 구/군/시] | 확인된 위치가 아니라 광고 컨텍스트에서 파생된 도시 정보입니다. |
| Geography | [!UICONTROL 지역/상태] | 광고 컨텍스트의 지역 또는 상태 정보입니다. |
| Geography | [!UICONTROL DMA] | 광고 컨텍스트에서 파생된 DMA(지정 시장 지역) 정보입니다. |
| 연결된 텔레비전(CTV) | [!UICONTROL CTV 노출됨] | 연결된 TV 장치에서 광고 노출. |
| 연결된 텔레비전(CTV) | [!UICONTROL 실시간 스트림 뷰어] | 시청 증명이나 참여 증명이 아닌 라이브 스트림 인벤토리의 광고 노출. |
| 연결된 텔레비전(CTV) | [!UICONTROL PMP/프리미엄 노출] | 개별적으로 검증된 프리미엄 재고가 아닌 개인 시장(PMP) 또는 개인 계약 노출. |
| 컨텐츠 선호도 | [!UICONTROL 연결된 TV/스트리밍] | 스트리밍 콘텐츠와 연계된 광고 노출. |
| 컨텐츠 선호도 | [!UICONTROL 게이머] | 게임 콘텐츠, 사이트 또는 앱과 관련된 광고 노출. |
| 컨텐츠 선호도 | [!UICONTROL 스포츠 팬] | 스포츠 콘텐츠, 사이트 또는 앱과 관련된 광고 노출. |
| 컨텐츠 선호도 | [!UICONTROL 뉴스 팔로워] | 뉴스 콘텐츠, 사이트 또는 앱과 관련된 광고 노출. |
| 컨텐츠 선호도 | [!UICONTROL 음악 애호가] | 음악 콘텐츠, 사이트 또는 앱과 관련된 광고 노출. |
| 컨텐츠 선호도 | [!UICONTROL 콘텐츠 장르] | 광고 노출과 관련된 콘텐츠 장르. |

지리 신호는 확인된 집 또는 현재 위치보다는 광고 컨텍스트를 설명합니다. 콘텐츠 선호도 신호는 개인의 관심사나 선호도를 확인하지 않는다. 소스 정보를 사용할 수 없는 경우 일부 속성에 값이 포함되지 않을 수 있습니다.

### 속성 범위 {#attribute-coverage}

적용 범위에서는 처리된 레코드에 속성 값이 포함된 빈도를 설명합니다. 예/아니요 신호(예: **[!UICONTROL CTV 노출됨]**)의 경우 적용 범위는 true 값이 있는 레코드를 계산합니다. 적용 범위에는 ID 일치율 또는 속성을 받을 자사 프로필의 비율이 표시되지 않습니다.

ID 일치, 소스-신호 가용성 및 수집은 프로필 업데이트에 영향을 줍니다. 적용 범위에서 내보내기 완료 또는 프로필 업데이트를 확인하지 않습니다.

### 워크플로 범위 {#workflow-scope}

조정된 카탈로그를 사용하여 [!DNL The Trade Desk]에서 데이터를 보강합니다. 원시 로그를 내보내거나 사용자 지정 속성 표현식을 만들 수 없습니다. 다른 수요측 플랫폼(DSP) 및 공급측 플랫폼(SSP) 통합은 지원되지 않습니다.

이 워크플로우는 데이터 보강 기회 검색, 대상 중복 분석 또는 속성 및 증분 측정을 지원하지 않습니다.

## 결과 수집 및 유효성 검사 {#ingest-validate-results}

게재 후 [!DNL Adobe Real-Time CDP] 관리자 또는 기술 지원 팀에 문의하여 파일을 수집하십시오.

### 출력 파일 {#output-file}

내보내기가 구성된 [!DNL Amazon S3] 대상에 CSV 파일을 전달합니다.

<!-- 
TODO: replace this placeholder with the engineering-confirmed output specification:
* Required hashing and normalization for each identifier, including whether email requires SHA-256 after trimming and lowercasing.
* Exact CSV headers, the file naming pattern, and the delivery bucket and path.
* Each identifier column in the delivered file and the identity namespace to map that column to during ingestion.
Do not treat example formats or supported input match keys as confirmed output requirements.
-->

프로필 업데이트와 별도로 내보내기를 확인합니다.

1. CSV 파일이 의도한 [!DNL Amazon S3] 위치에 도착했는지 확인하십시오.
1. 파일에 예상 식별자와 선택한 속성이 포함되어 있는지 확인합니다.
1. 대상 샌드박스 및 데이터 세트에 대해 확인된 ID 및 스키마 매핑을 사용하여 파일을 수집합니다.
1. 수집 결과를 검토하고 예상 프로필 샘플에 데이터 보강 속성이 포함되어 있는지 확인합니다.

파일을 내보내도 수집이 업데이트된 프로필을 확인하지 않습니다. 나중에 내보낼 각각을 개별적으로 수집하여 프로필을 업데이트합니다.

## 데이터 보강 문제 해결 {#troubleshoot-enrichment}

다음 검사를 사용하여 소스 데이터, 내보내기 및 수집 문제를 해결할 수 있습니다.

| 문제 | 확인할 사항 |
| --- | --- |
| 연결 또는 **[!UICONTROL 강화]**&#x200B;를 사용할 수 없습니다. | 관리자에게 문의하여 연결 및 프로젝트 액세스를 확인하십시오. 소스 피드 설정이 완료되었는지 확인합니다. |
| 내보내기 대상을 사용할 수 없음 | 관리자에게 문의하여 대상이 구성되어 있고 데이터 보강 출력에 사용할 수 있는지 확인하십시오. |
| 특성에 범위가 제한되어 있습니다. | 미디어 팀과 함께 소스 데이터 가용성을 검토합니다. 적용 범위를 프로필 일치율로 해석하지 마십시오. |
| 내보내기가 요청되었지만 파일이 없습니다. | 데이터 팀에 의도한 대상을 확인합니다. 요청 제출이 게재를 확인하지 않습니다. |
| 전달된 파일이 프로필을 업데이트하지 않았습니다. | 수집 결과를 검토하고 ID 및 스키마 매핑을 확인합니다. 내보내기와 수집은 별개의 작업입니다. |
| 내보내기를 요청할 수 없습니다. | 하나 이상의 속성과 대상을 선택하십시오. 내보내기가 이미 처리 중인 경우 다른 내보내기를 요청하기 전에 완료될 때까지 기다리십시오. |
| 범위가 높지만 속성을 받는 프로필은 거의 없습니다. | 적용 범위가 ID 일치율이 아닙니다. 소스 피드가 준비되었고, 대상자가 지원되는 일치 키를 사용하며, 수집 중에 ID 매핑이 올바른지 확인합니다. |
| 프로젝트를 만든 후에는 속성 또는 범위가 표시되지 않습니다 | 프로젝트 설정은 만들 때 수정됩니다. 해당 시점에 Adobe이 [!DNL The Trade Desk]에서 REDS 로그를 받지 못한 경우 나중에 해당 로그를 사용할 수 없습니다. Adobe에서 로그 수신을 확인한 후 새 프로젝트를 만듭니다. |
| 프로필에는 속성이 있지만 대상자 또는 경험은 이를 반영하지 않습니다 | 대상 평가, ID, 동의 및 다운스트림 경험 타깃팅 규칙을 확인합니다. |

## 다음 단계 {#next-steps}

특성을 수집 및 확인한 후 데이터 보강 신호를 자사 데이터와 결합하여 [!DNL Adobe Real-Time CDP]에 대상을 빌드합니다. 자세한 내용은 [대상 빌더 안내서](https://experienceleague.adobe.com/en/docs/experience-platform/segmentation/ui/audience-builder){target="_blank"}를 참조하십시오.

대상, 개인화 또는 고객 여정에 대해 대상을 활성화하려면 [대상 활성화 안내서](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/ui/activate/activation-overview){target="_blank"}를 참조하십시오.
