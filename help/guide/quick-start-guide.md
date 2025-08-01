---
title: Real-Time CDP Collaboration 빠른 시작 안내서
description: 역할 및 조직 설정, 대상 소싱, 활성화 및 측정을 포함하여 Real-Time CDP Collaboration에서 조직을 온보딩하는 방법을 알아봅니다. 이 안내서는 공동 작업자가 대상자를 안전하고 효율적으로 사용하도록 연결 설정을 구성할 수 있도록 도와줍니다.
audience: admin, publisher, advertiser
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/kr/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 68e5095e-ece5-4f64-9056-10f3b216cf0c
source-git-commit: d460cb12b43b6c250a5fb491c1efc223c53abb23
workflow-type: tm+mt
source-wordcount: '1408'
ht-degree: 0%

---

# Real-Time CDP Collaboration 빠른 시작 안내서

{{limited-availability-release-note}}

조직을 구성하고, 대상을 소싱하고, 개인 정보 중심의 활성화 및 측정을 활성화하여 Real-Time CDP Collaboration을 시작하십시오.

## 전제 조건

시작하기 전에 다음을 확인하십시오.

- 활성 Real-Time CDP Collaboration 라이선스.
- [Adobe Experience Platform에 대한 시스템 또는 제품 관리자 액세스](./permissions/overview.md).
- [최종 사용자에 대해 프로비전된 액세스](./permissions/manage-user-access.md).
- [조직에 대해 만들어지고 사용자에게 할당된 역할](./permissions/manage-roles.md).
- 조직의 이름, 로고 및 배너와 같은 브랜딩 자산에 대한 액세스 권한.
- [정의된 일치 키 전략](./setup/onboard-account.md#set-up-match-keys)(현재 해시된 이메일만 지원되는 일치 키).
- (선택 사항) 대상 관리에 Experience Platform을 사용하지 않는 경우 지원되는 클라우드 소스(Amazon S3 또는 Snowflake)에 액세스합니다.

## 1단계: 역할 기반 설정 완료 {#complete-role-based-setup}

조직의 액세스 역할은 사용자가 Collaboration에서 보고 수행할 수 있는 작업을 결정합니다. 계속하기 전에 역할 기반 권한이 올바르게 설정되어 있는지 확인하여 플랫폼에서 적절한 액세스 및 가시성을 보장하십시오.

**리소스:**

- [사용자 액세스 설명서](./permissions/manage-user-access.md)
- [역할 설정 설명서](./permissions/manage-roles.md)


이 비디오를 통해 Admin Console 및 Experience Platform을 사용하여 Collaboration에 대한 제품 액세스 및 권한을 할당하는 방법에 대해 알아보십시오.

>[!VIDEO](https://video.tv.adobe.com/v/3452237/?learn=on&enablevpops&captions=kor)

## 2단계: Collaboration 계정 설정 {#set-up-your-account}

대상을 소스화하려면 먼저 Collaboration에서 계정을 구성해야 합니다. 이는 표시되는 방식과 인터페이스에서 액세스할 수 있는 내용을 제어합니다.

필요한 액세스 권한이 없는 경우 1단계로 돌아가거나 조직의 관리자에게 문의하여 이 설정을 완료하십시오.

Collaboration에서 계정의 역할을 정의하고, 브랜딩 자산을 제공하며, 연결 간에 대상자를 정렬하도록 일치 키를 구성합니다.

>[!NOTE]
>
>설치하는 동안 하나 이상의 계정(예: 광고주 및 게시자)을 만들 수 있습니다. 브랜딩 자산 및 연락처 전자 메일과 같은 특정 필드는 나중에 **[!UICONTROL 설정]** 작업 영역에서 업데이트할 수 있습니다.

- **역할 할당** - 계정이 광고주인지 게시자인지를 결정합니다. 귀하의 역할은 Collaboration에서 보유하고 있는 기능을 정의합니다. 역할이 공동 작업 워크플로에 미치는 영향에 대한 자세한 내용은 [역할](./overview/roles.md) 안내서를 참조하세요.
- **브랜딩 자산** - 계정에 다음 내용을 추가하십시오.
   - 계정 이름(최대 100자)
   - 설명(최대 1,000자)
   - 로고(SVG &lt;20KB, 이상적인 사각형)

>[!NOTE]
>
>게시자 계정을 만들 때 Collaboration의 연결 카탈로그에 공개적으로 표시되도록 하려면 Adobe 계정 담당자에게 문의하십시오. 게시자 계정에는 사용자 지정 브랜드 배너(JPG 2688x1536)가 필요합니다. 이 파일은 담당자에게 직접 공유할 수 있습니다.

- **연락처 전자 메일** - 연결이 설정된 후 공동 작업자가 사용할 비즈니스 전자 메일을 제공합니다.
- **일치 키 구성** - 대상 일치에 사용되는 식별자를 선택합니다(현재 해시된 이메일만 지원되는 일치 키).

역할을 정의하고, 브랜딩 자산을 업로드하고, 일치 키를 구성하는 방법을 포함하여 초기 계정 설정에 대한 자세한 내용은 [초기 계정 설정](./setup/onboard-account.md#initial-account-setup){target="_blank"} 안내서를 참조하십시오.

이 비디오를 통해 계정 만들기, 브랜딩 및 일치 키 구성을 포함한 광고주 설정에 대한 단계별 설명을 살펴보십시오.

>[!VIDEO](https://video.tv.adobe.com/v/3452264/?learn=on&enablevpops)

## 3단계: Source 대상(Experience Platform 또는 클라우드 소스) {#source-audiences}

계정이 만들어지고 브랜딩 및 일치 키가 구성되면 대상자 소싱을 시작할 수 있습니다. 데이터 저장소 및 비즈니스 요구 사항에 따라 다음 소싱 방법 중 하나를 선택합니다.

### 옵션 A: Experience Platform의 Source

[Collaboration을 사용하여 대상이 포함된 샌드박스를 연결합니다](./setup/onboard-audiences.md). 이 셀프서비스 메서드를 사용하여 Experience Platform 인스턴스 내에서 기존 대상 세그먼트를 참조합니다.

#### 대상자 구성

연결에서 사용할 대상을 준비, 일치 및 제어하는 방법을 구성합니다.

- **대상 선택** *(Experience Platform만 해당)* - 지원되는 식별자가 있는 대상 세그먼트를 선택합니다.
- **일치 키 매핑** - 대상 필드를 구성된 일치 키와 맞춥니다.
- **변환 적용** - 필요한 경우 해시 일반 텍스트 값(예: 이메일)입니다.
- **새로 고침 예약** - 업데이트 주기(예: 매일)를 정의합니다.
- **동의 설정 구성** - 동의 모드(옵트인, 옵트아웃 또는 없음)를 선택하여 연결에 포함할 수 있는 프로필을 결정합니다.

>[!NOTE]
>
>Collaboration에서 대상을 추가하거나 제거하고 새로 고침 일정을 직접 업데이트할 수 있습니다. 일치 키 또는 동의 모드와 같은 다른 설정을 변경하려면 데이터 연결을 삭제하고 다시 만들어야 합니다.

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
>소스에 **일반 텍스트 식별자**&#x200B;이(가) 포함된 경우 **[!UICONTROL 변환 적용]** 옵션을 사용하여 해싱을 적용하십시오. 이 옵션은 Experience Platform에서 대상을 소싱할 때만 사용할 수 있으며 클라우드 기반 소스에는 지원되지 않습니다.
>
>자세한 내용은 소스 및 대상자 관리 안내서의 [필드 매핑](./setup/onboard-audiences.md#map-fields) 섹션을 참조하십시오.

Collaboration을 사용하여 대상을 소싱하는 방법에 대한 전체 연습을 보려면 아래 비디오를 시청하십시오.

>[!VIDEO](https://video.tv.adobe.com/v/3452217/?learn=on&enablevpops)

또는 [Collaboration의 소싱 대상](./setup/onboard-audiences.md#source-and-manage-audiences)에 대한 문서를 참조하십시오.

### 옵션 B: Snowflake 또는 Amazon S3의 Source

클라우드 소스(예: [!DNL AWS S3] 또는 [!DNL Snowflake])를 구성하려면 다음 [대상 사양 PDF](../assets/quick-start/RTCDP_Collaboration_Audience_Onboarding_Spec_v1.0.pdf)을 사용하여 대상 데이터를 준비하십시오. 완료되면 또는 질문이 있는 경우 Adobe 계정 담당자에게 문의하여 설정을 완료합니다. 이 방법은 셀프서비스가 아니며 Adobe 지원이 필요합니다.

>[!IMPORTANT]
>
>클라우드 기반 대상 파일은 대상 사양 PDF에 요약된 필수 스키마를 따라야 합니다. 파일에는 해시된 식별자(소문자화된 SHA256), 필수 메타데이터 필드(예: `segment_name` 및 `activation_id`)가 포함되어야 하며 지원되는 형식(예: CSV 또는 Parquet)을 사용해야 합니다. Adobe은 활성화 전에 데이터를 정규화하지 않습니다. TTL은 대상자의 수명에 따라 강제 적용됩니다.
>
>업로드된 파일의 모든 대상은 이 단계에서 완전히 소싱됩니다. [대상 가시성 설정](/help/guide/setup/onboard-audiences.md#metadata-visibility)은 공동 작업자가 대상을 볼 수 있는지, 그리고 Collaboration UI를 통해 관리되는지 여부를 결정합니다.

## 4단계: 대상자 활성화 (Experience Platform 또는 클라우드 대상) {#activate-audiences}

그런 다음 Experience Platform 인스턴스 또는 클라우드 대상에 대상을 활성화합니다.

### 옵션 A: Experience Platform에 활성화

[Adobe Experience Platform을 대상으로 구성](/help/guide/destinations/experience-platform.md) 안내서에 설명된 다음 단계를 완료합니다.

- **대상 만들기** - UI를 사용하여 Experience Platform 대상(샌드박스 수준)을 설정합니다.
- **일치 키 매핑** - 식별자를 선택합니다(예: `hashedEmail`).
- **TTL 정의** - 만료 설정(1~30일).
- **Audience Portal에서 확인** - 공동 작업자가 대상자를 보내면 원본 &quot;[!UICONTROL Real-Time CDP Collaboration]&quot; 아래의 Audience Portal에 표시되는지 확인하십시오.

### 옵션 B: 클라우드에 활성화

클라우드 대상(예: [!DNL AWS S3] 또는 [!DNL Snowflake])을 구성하려면 Adobe 계정 담당자에게 문의하여 설정 프로세스를 시작하십시오. 클라우드 대상에 따라 파일 경로, 자격 증명, 계정 로케이터 등 클라우드 대상 세부 정보를 제공해야 합니다. 필요한 정보가 제공되면 Adobe에서 클라우드 대상 설정을 구성합니다.

클라우드 대상으로 전송된 대상 데이터는 사전 정의된 스키마를 따릅니다. 필수 필드 및 형식에 대한 자세한 설명은 [Collaboration Audience Activation 안내서](../assets/quick-start/RTCDP_Collaboration_Audience_Activation_Spec_v1.0.pdf)를 다운로드하십시오.

## 5단계: 측정 설정(선택 사항) {#set-up-measurement}

>[!AVAILABILITY]
>
>이 기능은 **베타**&#x200B;에 있으며 제한된 가용성 프로그램에서 고객만 사용할 수 있습니다. 액세스 권한을 요청하려면 Adobe 담당자에게 문의하십시오.

>[!IMPORTANT]
>
>**[!UICONTROL 측정]** 작업 영역은 연결 프로세스 **[!UICONTROL 에서]**&#x200B;측정[ 사용 사례를 사용하도록 설정한 경우 ](./connect/establishing-connections.md#connection-settings)에만 사용할 수 있습니다. 사용 사례에 대한 자세한 내용은 [프로젝트 관리](./collaborate/manage-projects.md#project-use-cases) 안내서를 참조하세요.

Collaboration은 캠페인 도달 범위, 빈도 및 효과를 분석하는 다양한 보고서를 제공합니다. UI에서 **[!UICONTROL 측정]** 작업 영역을 사용할 수 있지만 전체 보고 기능을 사용하려면 백 엔드를 활성화해야 할 수 있습니다.

측정 보고서를 보고 해석하는 방법은 [측정 가이드](./collaborate/measure.md)를 참조하세요. 여기에는 속성, 캠페인 요약 지표 및 도달 곡선 및 빈도 분포와 같은 대시보드가 포함됩니다.

<!-- 
Commenting out the below information as this workflow is not yet in Beta but will be imminently. A guided measurement configuration workflow will be available in a future release."

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
   - Submit the report. It will run on the selected date and populate within 24 hours. 
-->

## 6단계: 공동 작업자와 연결 {#connect-with-collaborators}

설정이 완료되면 이제 조직에서 초대를 보내거나 수락하고 승인을 위해 프로젝트 설정을 제출하여 공동 작업자와 연결할 준비가 되었습니다. 이 연결 프로세스에는 초대장 보내기 또는 받기, 연결 설정(사용 사례 및 신용 사용 등) 검토 및 제출, 연결 확인 등이 포함됩니다.

광고주는 왼쪽 탐색 메뉴에서 **[!UICONTROL 연결]** 작업 영역을 사용하여 사용 가능한 게시자를 찾아봅니다. 또는 공동 작업자가 [개인 연결 초대](./connect/establishing-connections.md#private-connection-invite){target="_blank"}를 통해 서로 직접 연결할 수 있습니다.

>[!NOTE]
>
>현재는 광고주만 게시자를 검색할 수 있습니다. 게시자는 광고주를 찾아보거나 광고주와의 연결을 시작할 수 없습니다.

이 흐름에 대한 개요는 [연결 설정 안내서](./connect/establishing-connections.md){target="_blank"}를 참조하십시오. 공동 작업자 탐색 및 연결 설정 관리를 포함한 연결 프로세스에 대한 시각적 설명은 [advertiser 계정 설정 비디오](https://experienceleague.adobe.com/ko/docs/platform-learn/tutorials/collaboration/connect-with-publishers){target="_blank"}를 시청하십시오.

## 다음 단계

이제 초기 설정을 완료하고 보안 공동 작업을 위해 조직을 구성했습니다. 다음으로 다음 리소스를 탐색하여 활성화, 측정 및 데이터 거버넌스에 대해 깊이 있게 이해합니다.

- [대상자 활성화 워크플로 설명서](./collaborate/activate.md)
- [측정 사용 사례](./collaborate/measure.md)
- [Collaboration 거버넌스 모범 사례](./setup/onboard-audiences.md#governance-policy-and-enforcement-actions)
