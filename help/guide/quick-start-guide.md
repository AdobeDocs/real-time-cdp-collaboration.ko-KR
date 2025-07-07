---
title: Real-Time CDP Collaboration 온보딩 빠른 시작
description: 역할 및 조직 설정, 대상 소싱, 활성화 및 측정을 포함하여 Real-Time CDP Collaboration에서 조직을 온보딩하는 방법을 알아봅니다. 이 안내서는 광고주와 게시자가 공동 작업 설정을 구성하고 공유 대상을 안전하고 효율적으로 사용할 수 있도록 지원합니다.
audience: admin, publisher, advertiser
exl-id: 68e5095e-ece5-4f64-9056-10f3b216cf0c
source-git-commit: 5b17bcfbab02e8d24009a875ddea15cbd49c1506
workflow-type: tm+mt
source-wordcount: '1605'
ht-degree: 0%

---

# Real-Time CDP Collaboration 온보딩 빠른 시작

조직을 구성하고, 대상을 소싱하고, 개인 정보 중심의 활성화 및 측정을 활성화하여 Real-Time CDP Collaboration을 시작하십시오.

## 전제 조건

시작하기 전에 다음을 확인하십시오.

- 활성 Real-Time CDP Collaboration 라이선스.
- [Adobe Experience Platform에 대한 시스템 또는 제품 관리자 액세스](./permissions/overview.md#use-cases).
- [최종 사용자에 대해 프로비전된 액세스](./permissions/manage-user-access.md).
- [조직에 대해 만들어지고 사용자에게 할당된 역할](./permissions/manage-roles.md).
- 조직의 이름, 로고 및 배너와 같은 브랜딩 자산에 대한 액세스 권한.
- [정의된 일치 키 전략](./setup/onboard-organization.md#set-up-match-keys)(현재 해시된 이메일만 지원되는 일치 키).
- (선택 사항) Experience Platform을 대상으로 사용하지 않는 경우 지원되는 클라우드 소스(Amazon S3 또는 Snowflake)에 액세스합니다.

## 1단계: 역할 기반 설정 완료 {#complete-role-based-setup}

>[!NOTE]
>
>이 단계는 광고주와 게시자 모두에 적용됩니다.

조직의 액세스 역할은 사용자가 Real-Time CDP Collaboration에서 보고 수행할 수 있는 작업을 결정합니다. 계속하기 전에 역할 기반 권한이 올바르게 설정되어 있는지 확인하여 플랫폼에서 적절한 액세스 및 가시성을 보장하십시오.

**리소스:**

- [사용자 액세스 설명서](./permissions/manage-user-access.md)
- [역할 설정 설명서](./permissions/manage-roles.md)


이 비디오를 통해 Admin Console 및 Experience Platform UI를 사용하여 Collaboration에 대한 제품 액세스 및 권한을 할당하는 방법에 대해 알아보십시오.

>[!VIDEO](https://video.tv.adobe.com/v/3452216/?learn=on&enablevpops)

## 2단계: Real-Time CDP Collaboration 조직 설정 {#set-up-your-organization}

>[!NOTE]
>
>이 단계는 광고주와 게시자 모두에 적용됩니다.

대상을 추가하려면 먼저 Collaboration에서 조직을 구성해야 합니다. 이는 조직이 인터페이스에서 나타나고 행동하는 방식을 제어합니다.

Experience Platform에 대한 관리자 액세스 권한이 없는 경우 조직의 관리자에게 문의하여 이 설정을 완료하십시오.

Collaboration에서 조직의 역할을 정의하고, 브랜딩 자산을 제공하고, 연결 간에 대상자를 정렬하도록 일치 키를 구성합니다. 그런 다음 아래 단계를 완료하여 설정을 완료하고 조직이 연결에 참여할 수 있도록 준비하십시오.

>[!NOTE]
>
>설치하는 동안 한 명 이상의 공동 작업자(예: 광고주 또는 게시자 프로필)를 만들 수 있습니다. 브랜딩 자산 및 연락처 전자 메일과 같은 특정 필드는 나중에 **[!UICONTROL 설정]** 작업 영역에서 업데이트할 수 있습니다. 일치 키는 프로젝트 수준에서 제거할 수 있지만 추가되지는 않으므로 신중하게 계획하십시오.

- **역할 할당** - 조직이 광고주, 게시자 또는 둘 다 역할을 하는지 여부를 결정합니다. 역할은 대상자 공유 시작(광고주) 또는 대상자 사용 가능(게시자)과 같은 협업 기능을 정의합니다. 역할이 공동 작업 워크플로에 미치는 영향에 대해 자세히 알아보려면 [전체 워크플로 안내서](./end-to-end-workflow.md)를 참조하세요.
- **브랜딩 자산** - 계정에 다음 내용을 추가하십시오.
   - 브랜드 이름(최대 100자)
   - 브랜드 설명(최대 1,000자)
   - 브랜드 로고 (SVG &lt;20KB, 이상적인 사각형)
   - 브랜드 배너(JPG 2688x1536 또는 유사)
- **연락처 전자 메일** - 연결이 설정된 후 공동 작업자가 사용할 비즈니스 전자 메일을 제공합니다.

  >[!NOTE]
  >
  >게시자 계정을 만들 때 Collaboration의 연결 카탈로그에 공개적으로 표시되도록 하려면 Adobe 계정 담당자에게 문의하십시오. 게시자 계정에는 사용자 지정 브랜드 배너(JPG 2688x1536)가 필요합니다. 이 파일은 담당자에게 직접 공유할 수 있습니다.

- **일치 키 구성** - 대상 일치에 사용되는 식별자를 선택합니다(현재 해시된 이메일만 지원되는 일치 키).

조직이 만들어지고 브랜딩 및 일치 키가 구성되면 조직에서 대상을 소싱하고 데이터를 활성화할 수 있습니다.

역할을 정의하고, 브랜딩 자산을 업로드하고, 일치 키를 구성하는 방법을 포함하여 초기 조직 설정에 대한 자세한 내용은 [초기 조직 설정 문서](./setup/onboard-organization.md#initial-organization-setup){target="_blank"}를 참조하십시오.

계정 만들기, 브랜딩 및 일치 키 구성을 포함한 광고주 설정에 대한 단계별 설명을 살펴보십시오.

>[!VIDEO](https://video.tv.adobe.com/v/3452264/?learn=on&enablevpops)

## 3단계: Source 대상(Experience Platform 또는 클라우드 소스) {#source-audiences}

소스 대상에 대해 다음 데이터 저장소 중 하나 또는 모두를 선택합니다. Collaboration UI를 사용하거나 Adobe과 협력하여 개인 정보 보호 형식으로 대상자를 소스화합니다.

### 옵션 A: Experience Platform의 Source

[Collaboration 대상 UI를 사용하여 대상이 포함된 샌드박스를 연결합니다](./setup/onboard-audiences.md). 이 셀프서비스 메서드를 사용하여 Experience Platform 인스턴스 내에서 기존 대상 세그먼트를 참조합니다.

### 옵션 B: Snowflake 또는 Amazon S3의 Source

클라우드 소스(예: [!DNL AWS S3] 또는 [!DNL Snowflake])를 구성하려면 다음 [대상 사양 PDF](../assets/quick-start/RTCDP_Collaboration_Audience_Onboarding_Spec_v1.0.pdf)을 사용하여 대상 데이터를 준비하십시오. 완료되면 또는 질문이 있는 경우 Adobe 계정 담당자에게 문의하여 설정을 완료합니다. 이 방법은 셀프서비스가 아니며 Adobe 지원이 필요합니다.

>[!IMPORTANT]
>
>클라우드 기반 대상 파일은 대상 사양 PDF에 요약된 필수 스키마를 따라야 합니다. 파일에는 해시된 식별자(소문자화된 SHA256), 필수 메타데이터 필드(예: `segment_name` 및 `activation_id`)가 포함되어야 하며 지원되는 형식(예: CSV 또는 Parquet)을 사용해야 합니다. Adobe은 활성화 전에 데이터를 정규화하지 않습니다. TTL은 대상자의 수명에 따라 강제 적용됩니다.
>
>업로드된 파일의 모든 대상은 이 단계에서 완전히 소싱됩니다. 특정 파트너 조직에 대한 액세스는 Collaboration UI를 통해 별도로 제공됩니다.

### 대상자 구성

연결에서 사용할 대상을 준비, 일치 및 제어하는 방법을 구성합니다.

- **대상 선택** *(Experience Platform만 해당)* - 지원되는 식별자가 있는 대상 세그먼트를 선택합니다.
- **일치 키 매핑** - 대상 필드를 구성된 일치 키와 맞춥니다.
- **변환 적용** - 필요한 경우 해시 일반 텍스트 값(예: 이메일)입니다.
- **새로 고침 예약** - 업데이트 주기(예: 매일)를 정의합니다.
- **동의 설정 구성** - 동의 모드(옵트인, 옵트아웃 또는 없음)를 선택하여 연결에 포함할 수 있는 프로필을 결정합니다.

>[!NOTE]
>
>Collaboration UI에서 대상을 추가하거나 제거하고 새로 고침 일정을 직접 업데이트할 수 있습니다. 일치 키 또는 동의 모드와 같은 다른 설정을 변경하려면 데이터 연결을 삭제하고 다시 만들어야 합니다.

>[!IMPORTANT]
>
>**공동 작업자 역할당 최대 대상 수:**
>
>- **광고주**&#x200B;는 최대 25개의 대상을 소싱할 수 있습니다.
>- **게시자**&#x200B;는 최대 250개의 대상(각각 최소 5,000개의 ID를 가짐)을 검색할 수 있습니다.

>[!IMPORTANT]
>
>**주요 요구 사항 일치:**
>
>모든 일치 키는 **트림됨**, **소문자화** 및 **SHA256-hashed**&#x200B;여야 합니다.\
>대문자를 사용하는 해시된 값을 제공하면 Collaboration에서 자동으로 소문자로 변환합니다.\
>소스에 **일반 텍스트 식별자**&#x200B;이(가) 포함된 경우 UI의 **[!UICONTROL 변환 적용]** 옵션을 사용하여 해싱을 적용합니다. 이 옵션은 Experience Platform에서 대상을 소싱할 때만 사용할 수 있으며 클라우드 기반 소스에는 지원되지 않습니다.
>
>자세한 내용은 대상자 가져오기 및 관리 안내서의 [필드 매핑](./setup/onboard-audiences.md#map-fields) 섹션을 참조하십시오.

Collaboration UI를 사용하여 대상을 참조하는 방법에 대한 전체 연습을 보려면 아래 Collaboration 대상 참조 데모 비디오를 시청하십시오.

>[!VIDEO](https://video.tv.adobe.com/v/3452217/?learn=on&enablevpops)

또는 [Real-Time CDP Collaboration에서 대상을 사용할 수 있도록 설정](https://experienceleague.adobe.com/en/docs/real-time-cdp-collaboration/using/setup/onboard-audiences#import-audiences)에 대한 문서를 참조하십시오.

## 4단계: 대상자 활성화 (Experience Platform 또는 클라우드 대상) {#activate-audiences}

>[!NOTE]
>
>이 단계는 광고주와 게시자 모두에 적용됩니다.

Collaboration UI를 사용하여 Experience Platform 인스턴스 또는 클라우드 대상에 대한 대상을 활성화합니다.

### 옵션 A: Experience Platform에 활성화

[대상으로 Adobe Experience Platform 구성](https://experienceleague.adobe.com/en/docs/real-time-cdp-collaboration/using/destinations/experience-platform) 안내서에 설명된 다음 단계를 완료하십시오.

- **대상 만들기** - UI를 사용하여 Experience Platform 대상(샌드박스 수준)을 설정합니다.
- **일치 키 매핑** - 식별자를 선택합니다(예: `hashedEmail`).
- **TTL 정의** - 만료 설정(1~30일).
- **Audience Portal에서 확인** - 공동 작업자가 대상자를 보내면 원본 &quot;[!UICONTROL Real-Time CDP Collaboration]&quot; 아래의 Audience Portal에 표시되는지 확인하십시오.

### 옵션 B: 클라우드에 활성화

대상을 클라우드 대상(예: [!DNL AWS S3] 또는 [!DNL Snowflake])으로 활성화하려면 Adobe 계정 담당자에게 문의하여 설정 프로세스를 시작하십시오. 파일 경로, 자격 증명 및 예상 파일 형식 등 대상 세부 정보를 제공해야 합니다. 설정하는 동안 일치 키(예: `hashedEmail`)도 지정하고 원하는 TTL 및 새로 고침 케이던스를 정의해야 합니다. 구성이 완료되면 Adobe은 대상을 프로비저닝하고 데이터가 올바르게 전달되는지 확인합니다.

클라우드 대상으로 전송된 대상 데이터는 사전 정의된 스키마를 따릅니다. 필수 필드 및 형식에 대한 자세한 설명은 [Collaboration Audience Activation 안내서](../assets/quick-start/RTCDP_Collaboration_Audience_Activation_Spec_v1.0.pdf)를 다운로드하십시오.

### 주요 차이점

다음 목록에서는 Experience Platform과 클라우드 활성화 옵션 간의 차이점을 조명합니다.

- Experience Platform 활성화는 완전히 셀프서비스되며 Audience Portal에 표시됩니다.
- 클라우드 대상은 Adobe 조정이 필요하며 UI에 표시되지 않습니다.

## 5단계: 측정 설정(선택 사항) {#set-up-measurement}

>[!AVAILABILITY]
>
>이 기능은 **베타**&#x200B;에 있으며 제한된 가용성 프로그램에서 고객만 사용할 수 있습니다. 액세스 권한을 요청하려면 Adobe 담당자에게 문의하십시오.

>[!IMPORTANT]
>
>**[!UICONTROL 측정]** 작업 영역은 연결 프로세스 **[!UICONTROL 에서]**&#x200B;측정[ 사용 사례를 사용하도록 설정한 경우 ](./connect/establishing-connections.md#connection-settings)에만 사용할 수 있습니다. 사용 사례에 대한 자세한 내용은 [프로젝트 관리](./collaborate/manage-projects.md#project-use-cases) 안내서를 참조하세요.

Collaboration은 캠페인 도달 범위, 빈도 및 효과를 분석하는 다양한 보고서를 제공합니다. UI에서 **[!UICONTROL 측정]** 작업 영역을 사용할 수 있지만 전체 보고 기능을 사용하려면 백 엔드를 활성화해야 할 수 있습니다.

측정 보고서를 보고 해석하는 방법은 [측정 가이드](./collaborate/measure.md)를 참조하세요. 여기에는 속성, 캠페인 요약 지표 및 도달 곡선 및 빈도 분포와 같은 대시보드가 포함됩니다.

<!-- Commenting out the below information as this workflow is not yet in Beta but will be imminently. A guided measurement configuration workflow will be available in a future release."
### Configure measurement workflow

Collaboration supports two measurement workflows:

- **Attribution using Adobe Experience Platform datasets**
- **Campaign summary using only partner-provided data**

Choose the appropriate workflow below based on your campaign measurement goals.

#### Option A: Attribution using Experience Platform datasets

Use this workflow to measure conversion activity using datasets stored in Experience Platform.

1. **Create a measurement data connection**
   - Select the dataset that contains your conversion events.
   - Map identity fields from your dataset to the match keys used in Collaboration.
   - Manage consent and governance settings.
   - Define one or more conversion events to measure.
   - Review and confirm your setup.

2. **Run a measurement report**
   - Go to the **[!UICONTROL Measure]** workspace within the associated project.
   - Input the report name, date range, and report run date.
   - Select **[!UICONTROL Attribution]** as the report type.
   - Select the defined conversion event(s).
   - Submit the report. It will run on the specified date and populate within 24 hours.

#### Option B: Campaign summary using partner-provided data

Use this workflow to generate campaign summary insights based on advertiser-supplied identifiers (for example, campaign ID).

1. **Set up the connection**
   - In the connection settings, ensure **[!UICONTROL Measurement]** is selected as a use case.
   - Create a project under the connection with **[!UICONTROL Measurement]** as an activity.

2. **Provide campaign context**
   - Input required campaign identifiers (for example, **Campaign ID**) for the partner to reference.
   - Align with your partner on campaign scope and reporting timeline.

3. **Run a measurement report**
   - Navigate to the **[!UICONTROL Measure]** workspace within the project.
   - Input the report name, date range, and report run date.
   - Select **[!UICONTROL Campaign summary]** as the report type.
   - Submit the report. It will run on the selected date and populate within 24 hours. -->

## 확인

활성화 후에 대상이 성공적으로 전달되었는지 또는 적절한 대상에서 사용할 수 있게 되었는지 확인합니다.

- 대상이 Audience Portal에 표시되는지 확인합니다(Experience Platform 활성화의 경우).
- 외부 대상 로그 또는 확인을 통해 성공적인 클라우드 게재를 확인합니다.

## 6단계: 공동 작업자와 연결 {#connect-with-collaborators}

설정 및 데이터 프로비저닝이 완료되면 이제 조직에서 초대를 보내거나 수락하고 승인을 위해 프로젝트 설정을 제출하여 공동 작업자와 연결할 준비가 되었습니다. 이 연결 프로세스에는 초대장 보내기 또는 받기, 연결 설정(예: 사용 사례 및 신용 소비) 검토 및 제출, 관계 확인이 포함됩니다.

광고주는 Collaboration UI의 왼쪽 탐색 메뉴에서 **[!UICONTROL 연결]** 작업 영역을 사용하여 사용 가능한 게시자를 찾아봅니다.

>[!NOTE]
>
>현재는 광고주만 게시자를 검색할 수 있습니다. 게시자는 광고주를 찾아보거나 광고주와의 연결을 시작할 수 없습니다.

이 흐름에 대한 개요는 [광고주 또는 게시자와 연결 가이드](./connect/establishing-connections.md){target="_blank"}를 참조하십시오. 공동 작업자 탐색 및 연결 설정 관리를 포함한 연결 프로세스에 대한 시각적 설명은 [advertiser 계정 설정 비디오](https://experienceleague.adobe.com/ko/docs/platform-learn/tutorials/collaboration/connect-with-publishers){target="_blank"}를 시청하십시오.

## 다음 단계

이제 초기 설정을 완료하고 보안 공동 작업을 위해 조직을 구성했습니다. 다음으로 다음 리소스를 탐색하여 활성화, 측정 및 데이터 거버넌스에 대해 깊이 있게 이해합니다.

- [대상자 활성화 워크플로 설명서](./collaborate/activate.md)
- [측정 사용 사례](./collaborate/measure.md)
- [Collaboration 거버넌스 모범 사례](./setup/onboard-audiences.md#governance-policy-and-enforcement-actions)
