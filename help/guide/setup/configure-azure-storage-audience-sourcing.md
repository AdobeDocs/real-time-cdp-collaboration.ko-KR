---
title: Real-Time CDP Collaboration의  [!DNL Azure] 저장소에서 Source 대상
description: Source Blob Storage 또는 Azure Data Lake Storage Gen2의 Azure 자사 대상 데이터를 Real-Time CDP Collaboration으로 가져옵니다.
keywords: Real-Time CDP Collaboration; 대상 소싱; [!DNL Azure Blob Storage]; [!DNL Azure Data Lake Storage] Gen2
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
source-git-commit: 3b62837cecf6cf7c288ce1633d43312ff6a92664
workflow-type: tm+mt
source-wordcount: '2050'
ht-degree: 4%

---

# Azure 스토리지의 Source 대상

활성화 및 중복 분석을 위해 [!DNL Azure Blob Storage] 또는 [!DNL Azure Data Lake Storage]&#x200B;(ADLS) Gen2를 Adobe Real-Time CDP Collaboration에 연결하여 자사 대상 데이터를 소싱합니다.

이 안내서를 사용하여 재사용 가능한 [!DNL Azure] 데이터 연결을 만들고 구성된 저장소 위치에서 1회 가져오기를 실행합니다. 시작하기 전에 대상 파일이 [대상 소싱 사양](../../assets/quick-start/RTCDP_Collaboration_Audience_Sourcing_Spec_v1_3.pdf)을 충족하는지 확인하십시오. 설정 프로세스 중에 Adobe에 Azure 스토리지에 대한 읽기 액세스 권한을 부여합니다.

## [!DNL Azure] 소스 유형 선택 {#choose-source-type}

Collaboration에서는 두 개의 [!DNL Azure] 수집 옵션을 지원합니다. 아래 표를 사용하여 대상자 파일의 위치와 일치하는 안내 경로를 선택하십시오.

| | **[!DNL Azure Blob Storage]** | **[!DNL Azure Data Lake Storage]Gen2** |
|---|---|---|
| **다음의 경우에 사용** | 저장소 계정의 표준 Blob **container**&#x200B;에 파일이 있습니다(계층 네임스페이스가 필요하지 않음). | **계층 구조 네임스페이스(ADLS Gen2)**&#x200B;가 활성화된 저장소 계정의 **파일 시스템**&#x200B;에 파일이 있습니다. |
| Collaboration의 **Source 옵션** | **[!DNL Azure Blob Storage]** | **[!DNL Azure Data Lake Storage]Gen2** |
| **Collaboration의 필수 필드** | 저장소 계정, **[!UICONTROL 컨테이너]**, **[!UICONTROL 경로]** | 저장소 계정, **[!UICONTROL 컨테이너]**(ADLS Gen2 파일 시스템), **[!UICONTROL 경로]** |
| **권한 섹션** | [[!DNL Azure Blob] 권한](#set-up-azure-blob-storage-permissions) | [[!DNL Azure Data Lake Storage] Gen2 권한](#set-up-adls-gen2-permissions) |

데이터 연결당 **하나의 원본 유형만 구성할 수 있습니다**. [!DNL Blob]과(와) ADLS에서 모두 검색하려면 별도의 데이터 연결을 만드십시오.

## 사전 요구 사항 {#prerequisites}

이 안내서를 따르려면 먼저 [계정 온보딩 및 설정](./onboard-account.md)을 완료하십시오. 그런 다음 구성 워크플로우를 시작하기 전에 이 섹션의 전제 조건을 완료하십시오.

일부 단계는 **[!DNL Azure]관리자**&#x200B;의 작업이 필요합니다. 조직의 [!DNL Azure] 관리자가 아닌 경우 시작하기 전에 적절한 사용자를 식별하십시오.

### [!DNL Azure] 액세스 및 권한 {#azure-access-and-permissions}

Collaboration에서 연결을 구성하기 전에 사용자 또는 [!DNL Azure] 관리자가 대상 파일이 포함된 저장소 컨테이너 또는 ADLS Gen2 파일 시스템에 대한 Adobe 읽기 액세스 권한을 부여해야 합니다. 권한 설정이 완료되면 Collaboration 구성 워크플로가 **[!UICONTROL 동의]** 단계 동안 액세스를 확인합니다.

### 대상자 데이터 준비 {#prepare-audience-data}

소싱이 시작되기 전에 대상 파일이 **[대상 소싱 사양(v1.2)](../../assets/quick-start/RTCDP_Collaboration_Audience_Sourcing_Spec_v1_3.pdf)**&#x200B;을 준수해야 합니다.

주요 요구 사항은 다음과 같습니다.

* **파일 형식:** CSV, 쉼표를 필드 구분 기호로 사용하고 파이프(`|`)를 단일 필드 내의 여러 값에 대한 구분 기호로 사용.
* **필수 필드:** 모든 레코드에는 `AUDIENCE_ID` 열과 지원되는 일치 키 열이 하나 이상 포함되어야 합니다.
* **지원되는 일치 키:** `HASHED_EMAIL_SHA_256`, `HASHED_PHONE_SHA_256`, `HASHED_IPV4_SHA_256`, `CRM_ID`, `LOYALTY_ID`, `ADFIXUS_ID`.
* **요구 사항 해시:** 업로드하기 전에 모든 일치 키 값을 트리밍하고, 소문자화하고, SHA256-해시해야 합니다. Collaboration은 수집 전에 데이터를 해시하거나 정규화하지 않습니다.
* **열 일관성:** 구성된 경로의 모든 파일은 동일한 열 구조를 사용해야 합니다.

대상 파일에 있는 모든 일치 키도 Collaboration 계정에 대해 활성화되어야 합니다. 지침은 [일치 키 설정](https://experienceleague.adobe.com/ko/docs/real-time-cdp-collaboration/using/setup/onboard-account#set-up-match-keys)을 참조하십시오.

>[!IMPORTANT]
>
> 데이터 연결에 대해 활성화된 일치 키는 연결을 만든 후 제거할 수 없습니다. 활성 일치 키 집합을 변경하려면 연결을 삭제하고 새 연결을 만들어야 합니다. 설정 워크플로를 시작하기 전에 일치 키 구성이 완료되었는지 확인하십시오.

### 시작하기 전에 필요한 값 {#values-required}

구성 워크플로를 시작하기 전에 다음 값을 준비하십시오.

| 값 | 설명 | Azure Blob 스토리지 예 | ADLS Gen2 예 |
| ------------------- | ------------------------ | -------------------------------------- | -------------------------------------- |
| **저장소 계정** | 대상 파일을 호스팅하는 [!DNL Azure] 저장소 계정의 이름입니다. | `customerdatastore` | `datalake-prod` |
| **컨테이너** | [!DNL Azure Blob Storage]의 경우 대상 파일이 포함된 저장소 컨테이너입니다. [!DNL Azure Data Lake Storage] Gen2의 경우 **[!UICONTROL Container]** 필드에 ADLS Gen2 파일 시스템 이름을 입력합니다. | `audience-ingest` | `audiences` |
| **경로** | 수집할 대상 파일이 포함된 컨테이너 또는 파일 시스템 내의 폴더 경로입니다. Collaboration은 구성된 경로 바로 아래에 있는 파일만 수집하며 중첩된 하위 폴더에서 파일을 수집하지 않습니다. | `sourcing/audiences/path1/` | `sourcing/inbound/` |
| **테넌트 ID** | [!DNL Azure] 저장소 계정과 연결된 Microsoft Entra 테넌트 ID입니다. | `00000000-0000-0000-0000-000000000000` | `00000000-0000-0000-0000-000000000000` |

## [!DNL Azure] 권한 설정 {#set-up-azure-permissions}

이 섹션의 단계를 완료하여 [!DNL Azure] 환경을 준비하십시오. Adobe 구성 워크플로에서 연결을 설정하려면 먼저 Collaboration에서 저장소 컨테이너에 대한 읽기 액세스 권한이 필요합니다. 이 작업은 [!DNL Azure] 포털에서 수행되며 [!DNL Azure] 관리자가 완료해야 할 수 있습니다.

이 섹션을 완료한 후 [연결 구성 [!DNL Azure] 을 진행합니다](#configure-your-azure-connection).

### Adobe의 [!DNL Azure] 서비스 사용자 식별자 얻기 {#obtain-principal-identifier}

아래 단계에서 역할 할당 단계를 완료하기 전에 Adobe 계정 팀에 문의하여 해당 지역(북미, EMEA, 호주 및 뉴질랜드)에 대한 [!DNL Azure] 서비스 사용자 식별자를 얻으십시오. 이 식별자를 사용하여 Adobe에 스토리지에 대한 읽기 액세스 권한을 부여합니다.

### [!DNL Azure Blob Storage] 권한 설정 {#set-up-azure-blob-storage-permissions}

>[!IMPORTANT]
>
> 저장소 계정 또는 컨테이너에서 역할을 할당하려면 권한이 필요합니다(예: **소유자** 또는 **사용자 액세스 관리자** 또는 동등).

1. [[!DNL Azure] 포털](https://portal.azure.com/)에서 저장소 계정을 연 다음 **[!UICONTROL 컨테이너]**(으)로 이동하여 대상 파일이 포함된 컨테이너를 선택하십시오.
2. **[!DNL Access control (IAM)]**&#x200B;을(를) 선택한 다음 **[!DNL Add role assignment]**&#x200B;을(를) 선택합니다.
3. 컨테이너 범위에서 Adobe의 주체에 **[!DNL Storage Blob Data Reader]** 역할을 할당하십시오.
4. **저장**&#x200B;을 선택합니다.

### ADLS Gen2 권한 설정 {#set-up-adls-gen2-permissions}

ADLS Gen2 연결의 경우 Collaboration의 **[!UICONTROL Container]** 필드는 [!DNL Azure]의 ADLS Gen2 파일 시스템에 해당합니다. 대상 파일이 포함된 파일 시스템을 사용합니다.

권한을 할당하기 전에 저장소 계정에 **계층 구조 네임스페이스가 사용**&#x200B;되어 있고 방화벽 또는 개인 끝점 규칙이 Adobe 액세스를 허용하는지 확인하십시오.

1. [[!DNL Azure] 포털](https://portal.azure.com/)에서 ADLS Gen2 파일 시스템이 포함된 저장소 계정을 엽니다.
2. 대상 파일이 포함된 파일 시스템을 엽니다.
3. **[!UICONTROL IAM(액세스 제어)]**&#x200B;을 선택한 다음 **[!UICONTROL 역할 할당 추가]**&#x200B;를 선택합니다.
4. 파일 시스템 또는 디렉터리 범위에서 Adobe의 주체에 **[!DNL Storage Blob Data Reader]** 역할을 할당합니다.
5. **[!UICONTROL 저장]**&#x200B;을 선택합니다.

소스 유형에 대한 권한 설정을 완료한 후 [연결 구성 [!DNL Azure] 2}을 진행합니다.](#configure-your-azure-connection)

## [!DNL Azure] 연결 구성 {#configure-your-azure-connection}

Collaboration 구성 워크플로를 사용하여 [!DNL Azure] 저장소 세부 정보의 유효성을 검사하고, Adobe 액세스를 확인하고, 자동으로 매핑된 ID 필드를 검토하고, 데이터 연결을 만듭니다.

### 새 데이터 연결 추가 {#add-new-data-connection}

**[!UICONTROL 설정]** > **[!UICONTROL 내 대상]**(으)로 이동한 다음 추가 아이콘(![추가 아이콘](/help/assets/icons/plus.png))을 선택합니다. **[!UICONTROL 대상]**&#x200B;을 선택하세요.

![새 대상 또는 데이터 연결을 만드는 데 사용되는 대상 추가 옵션을 표시하는 내 대상 보기입니다.](../../assets/setup/azure-sourcing/my-audiences-add-audience-entry-point.png){zoomable="yes"}

**[!UICONTROL 대상자 추가]** 워크플로가 나타납니다. **[!UICONTROL 새 데이터 연결 추가]**&#x200B;를 선택한 후 **[!UICONTROL 다음]**&#x200B;을 선택합니다.

![새 데이터 연결 추가 옵션을 선택하고 다음을 강조 표시한 내 대상 보기입니다.](../../assets/setup/azure-sourcing/add-new-data-connection.png){zoomable="yes"}

### [!DNL Azure] 데이터 원본 선택 {#select-azure-data-source}

**[!UICONTROL Azure Blob 저장소]** 또는 **[!UICONTROL Azure Data Lake 저장소 Gen2]**&#x200B;를 선택한 후 **[!UICONTROL 다음]**&#x200B;을 선택합니다.

![데이터 연결 유형으로 선택된 [!DNL Azure Blob Storage]을(를) 표시하는 대상자 추가 워크플로 및 온보딩 단계 자격 증명, 동의, 필드 매핑 및 검토.](../../assets/setup/azure-sourcing/azure-source-selection-step.png){zoomable="yes"}

나머지 단계를 계속 진행하여 Azure 연결의 유효성을 검사하고, Adobe 액세스를 확인하고, 필드 매핑을 검토하고, 데이터 연결을 만듭니다.

### 연결 자격 증명 입력 {#enter-connection-credentials}

**[!UICONTROL 자격 증명]** 단계에서 [!DNL Azure] 저장소 위치에 액세스하는 데 필요한 정보를 제공하십시오.

| 필드 | 설명 |
|---|---|
| **[!UICONTROL 저장소 계정]** | 대상 파일이 포함된 [!DNL Azure] 저장소 계정입니다. |
| **[!UICONTROL 컨테이너]** | 대상자 파일이 포함된 스토리지 컨테이너 또는 ADLS Gen2 파일 시스템 |
| **[!UICONTROL 경로]** | 대상 파일이 저장된 컨테이너 내의 폴더 경로입니다. |
| **[!UICONTROL 테넌트 ID]** | 저장소 계정과 연결된 [!DNL Azure] 테넌트 식별자입니다. |

필요한 값을 입력한 후 **[!UICONTROL Azure에 연결]**&#x200B;을 선택합니다.

연결이 성공적으로 설정되었음을 나타내는 확인 메시지가 표시됩니다. 계속하려면 **[!UICONTROL 다음]**&#x200B;을 선택합니다.

![완료된 저장소 계정, 컨테이너, 경로 및 테넌트 ID 필드를 표시하는 자격 증명 단계이며 [!DNL Azure]에 연결됨 확인 메시지가 있습니다.](../../assets/setup/azure-sourcing/azure-credentials-step.png){zoomable="yes"}

### [!DNL Azure] 저장소에 Adobe 액세스 권한 부여 {#grant-adobe-access}

**[!UICONTROL 동의]** 단계에서 Collaboration은 이전에 구성한 [!DNL Azure] 권한의 유효성을 검사합니다.

[!DNL Azure]에서 인증 워크플로를 열려면 **[!UICONTROL 동의 URL]** 옆에 있는 시작 아이콘을 선택하십시오. 저장소 위치에 대한 동의를 부여할 수 있는 권한이 있는 계정으로 로그인한 다음 구성된 저장소 위치에 Adobe 액세스를 부여하는 Azure 인증 프롬프트를 완료합니다. 인증이 완료되면 Collaboration으로 돌아가서 **[!UICONTROL 동의 확인]**&#x200B;을 선택하여 Adobe의 액세스 권한을 확인합니다.

>[!NOTE]
>
>[!DNL Azure]개의 역할 할당이 전파되는 데 몇 분이 걸릴 수 있습니다. 동의 유효성 검사가 즉시 성공하지 못할 경우 몇 분 정도 기다린 후 Adobe의 서비스 주체에 필요한 역할이 할당되었는지 확인한 다음 다시 시도하십시오.

동의 유효성 검사가 성공하면 **[!UICONTROL 동의함]** 확인 메시지가 나타납니다. 계속하려면 **[!UICONTROL 다음]**&#x200B;을 선택합니다.

![동의 URL, \[!DNL Azure\] 응용 프로그램 식별자 및 동의 부여 확인 메시지를 표시하는 동의 단계입니다.](../../assets/setup/azure-sourcing/azure-consent-granted-step.png){zoomable="yes"}

### 필드 매핑 검토 {#review-field-mappings}

**[!UICONTROL 필드 매핑]** 단계에서 Collaboration은 소스 파일에서 지원되는 ID 필드를 자동으로 매핑합니다.

수동 구성은 필요하지 않습니다.

>[!IMPORTANT]
>
> Collaboration은 대상 소싱 사양을 기반으로 ID 필드를 자동으로 매핑합니다. 표시된 매핑이 올바르지 않은 경우 온보딩 워크플로우를 완료하기 전에 소스 파일을 업데이트합니다.

표시된 매핑을 검토하고 소스 필드가 대상 파일의 ID 열과 일치하는지 확인하십시오. 계속하려면 **[!UICONTROL 다음]**&#x200B;을 선택합니다.

![수동 구성 없이 자동으로 매핑된 원본 필드와 대상 ID 필드를 표시하는 필드 매핑 단계입니다.](../../assets/setup/azure-sourcing/azure-field-mapping-step.png){zoomable="yes"}

### 연결 검토 및 완료 {#review-and-complete}

**[!UICONTROL 검토]** 단계에서 저장소 계정, 컨테이너, 원본 경로, 테넌트 ID 및 필드 매핑을 확인하십시오.

또한 검토 페이지는 현재 [!DNL Azure] 워크플로우가 단일 소싱 실행을 수행하고 반복 일정을 구성하지 않음을 나타냅니다.

구성이 올바르면 **[!UICONTROL 완료]**&#x200B;를 선택합니다.

![연결 세부 정보, 필드 매핑 및 대상 가져오기가 일정이 구성되지 않은 일회성 가져오기임을 나타내는 메시지를 표시하는 검토 단계입니다.](../../assets/setup/azure-sourcing/azure-review-connection-step.png){zoomable="yes"}

## 소스 대상자 연결 확인 및 모니터링 {#confirm-connection-and-monitor-audiences}

**[!UICONTROL 완료]**&#x200B;를 선택하면 Collaboration에서 데이터 연결을 만들고 **[!UICONTROL 설정]** > **[!UICONTROL 내 데이터 연결]**(으)로 이동합니다.

### 연결이 생성되었는지 확인 {#confirm-connection-created}

**[!UICONTROL 내 데이터 연결]**&#x200B;의 연결 카드에서 연결이 성공적으로 생성되었음을 확인합니다. 카드에 소스 유형(**[!UICONTROL Azure Blob 저장소]** 또는 **[!UICONTROL Azure 데이터 레이크 저장소] Gen2**), 생성 날짜, 일치 키, 대상자 규모 및 현재 연결 상태가 표시됩니다.

![연결 세부 정보, 일치 키, 대상자 규모 및 상태 정보가 있는 새로 만든 [!DNL Azure Blob Storage] 연결 카드를 표시하는 내 데이터 연결 보기입니다.](../../assets/setup/azure-sourcing/azure-data-connection-card.png){zoomable="yes"}

### 소스 대상자 보기 {#view-sourced-audiences}

연결이 만들어지면 Collaboration은 구성된 [!DNL Azure] 위치에서 대상자 소싱을 자동으로 시작합니다. 소싱 진행 상황을 모니터링하고 소싱 대상을 검토하려면 **[!UICONTROL 설정]** > **[!UICONTROL 내 대상]**(으)로 이동하십시오.

소스 대상이 **[!UICONTROL 내 대상]** 표에 나타납니다. 대상 상태, ID 수, 소스, 데이터 연결 및 마지막 업데이트 날짜를 사용하여 예상 대상이 [!DNL Azure] 연결에서 소싱되었는지 확인하십시오.

>[!TIP]
>
>소싱 시간은 데이터 볼륨에 따라 다릅니다. 24시간 후에도 대상이 나타나지 않으면 [문제 해결](#troubleshooting)을 참조하세요.

![테이블에서 강조 표시된 새 대상이 있는 설치 작업 영역의 내 대상 탭입니다.](../../assets/setup/azure-sourcing/view-sourced-audiences.png)

## 알려진 제한 사항 {#known-limitations}

Azure 데이터 연결을 만들거나 관리하기 전에 다음 제한 사항을 검토하십시오.

* **일치 키 제약 조건:** 일치 키는 기존 연결에서 제거할 수 없습니다. 활성 일치 키를 변경하려면 연결을 삭제하고 새 연결을 만듭니다.
* **소스 유형당 활성 연결 하나: [!DNL Azure]:** 계정당 활성 Blob 연결 하나와 활성 ADLS Gen2 연결 하나를 가질 수 있습니다. 저장소 위치를 변경하려면 기존 연결을 삭제하고 새 연결을 만듭니다.
* **하위 폴더 지원:** Collaboration은 구성된 경로 바로 아래에 있는 파일만 수집합니다. 중첩된 하위 폴더에서 파일을 수집하지 않습니다.
* **별도의 원본 형식:** Blob와 ADLS Gen2는 서로 다른 연결입니다. 단일 마법사 실행에서 두 연결 간의 구성을 혼합하지 마십시오.

## 문제 해결 {#troubleshooting}

### 대상이 나타나지 않거나 소싱이 느립니다. {#audiences-not-appearing}

연결을 만든 후 소스 대상이 나타나지 않으면 다음 작업을 완료하십시오.

* 대상 파일이 구성된 경로 바로 아래에 있으며 대상 소싱 사양을 준수하는지 확인합니다.
* **[!UICONTROL 내 데이터 연결]**&#x200B;에서 오류가 있는지 확인하십시오.
* 24시간 후에도 문제가 지속되는 경우 연결 이름, 저장소 계정 및 컨테이너 세부 정보를 사용하여 Adobe 지원 센터에 문의하십시오.

### 대상자 소스이지만 0개 또는 예기치 않은 ID를 표시 {#zero-identities}

소싱 후에 대상이 표시되지만 ID 수가 0이거나 예상보다 낮은 경우 다음 작업을 완료하십시오.

* 업로드하기 전에 대상 파일의 모든 일치 키 값이 트리밍되고, 소문자이고, SHA256-해시되었는지 확인하십시오. Collaboration은 수집 시 데이터를 해시하거나 정규화하지 않습니다.
* 파일에 있는 일치 키가 Collaboration 계정에 대해 활성화되어 있는지 확인합니다. [일치 키 설정](https://experienceleague.adobe.com/ko/docs/real-time-cdp-collaboration/using/setup/onboard-account#set-up-match-keys)을 참조하세요.

### 초기 성공 이후 연결 실패 {#connection-failed}

연결이 성공적으로 만들어졌지만 나중에 실패 상태가 되면 이러한 검사를 사용합니다.

* Adobe 주체에 대한 [!DNL Azure] RBAC 역할 할당이 제거되거나 좁혀지지 않았는지 확인하십시오.
* 파일이 경로에 계속 있고 사양과 일치하는지 확인합니다.

### 가져오기 또는 형식 오류 {#format-errors}

파일 구조, 해시 또는 열 형식 문제로 인해 소싱이 실패할 경우 이러한 검사를 사용합니다.

* 모든 파일이 초기 수집과 동일한 열 구조 및 해싱 규칙을 유지하는지 확인합니다.

## 다음 단계 {#next-steps}

소싱이 완료되면 **[!UICONTROL 내 대상]**&#x200B;에서 활성화, 중복 분석 및 측정 워크플로우에 대상을 사용할 수 있습니다. 공동 작업자를 통해 소스 대상을 활성화하려면 [대상 활성화](../collaborate/activate.md)를 참조하십시오.

사용 가능한 다른 소싱 방법에는 Experience Platform, [!DNL Amazon S3], [!DNL Google Cloud Storage], [!DNL Snowflake] 및 CSV 파일 업로드가 있습니다. 다른 대상 소싱 방법은 다음을 참조하십시오.

* [대상 소싱을 위한 Google 클라우드 스토리지 구성](./configure-gcs-audience-sourcing.md)
* [대상 소싱을 위한 Snowflake 구성](./configure-snowflake-audience-sourcing.md)
* [대상 소싱을 위한 AWS S3 구성](./configure-aws-s3-audience-sourcing.md)
* [Experience Platform의 Source 대상](./onboard-audiences.md)
* [대상자 소싱에 대한 CSV 파일 업로드](./upload-csv-audience-sourcing.md)
