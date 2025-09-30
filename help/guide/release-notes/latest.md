---
title: 최신 Real-Time CDP Collaboration 릴리스 노트
description: Real-Time CDP Collaboration의 최신 릴리스를 따르십시오.
audience: admin, publisher, advertiser
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 8513c648-1cc1-4544-b86d-2ee3193ab60f
source-git-commit: 36f43d9d34ce7851a1c7093e0891f9c87e56387c
workflow-type: tm+mt
source-wordcount: '1231'
ht-degree: 2%

---

# 최신 Real-Time CDP Collaboration 릴리스 노트

{{limited-availability-release-note}}

**마지막 업데이트**: 2025년 8월.

이러한 릴리스 노트는 Adobe Real-Time CDP Collaboration에 릴리스된 기능을 다룹니다. Collaboration 릴리스는 연속 게재 모델에서 작동하므로 대략적인 월별 릴리스 케이던스를 사용할 수 있습니다. 이러한 릴리스 노트는 자주 업데이트되므로 정기적으로 확인하십시오.

## 2025년 8월 {#august-2025}

이제 **캐나다**&#x200B;의 고객이 Real-Time CDP Collaboration을 사용할 수 있습니다. 이러한 지역의 Real-Time CDP Prime 및 Ultimate 고객이 자동으로 사용할 수 있습니다.

* Collaboration은 이제 다음 [일치 키](../setup/onboard-account.md#supported-match-keys)를 지원합니다.
   * 해시된 이메일
   * 해시된 전화번호
   * CRM ID
   * 충성도 ID
   * 해시된 IPv4
   * AdFixus ID
* 이제 Collaboration 전체에서 여러 일치 키를 사용할 수 있으므로 대상 크기를 확장하고 일치율을 향상시킬 수 있습니다. 대상을 소싱하고, 연결을 설정하고, 대상을 활성화할 때 여러 일치 키를 사용할 수 있습니다. 여러 일치 키 사용에 대한 자세한 내용은 [일치 키 설정](../setup/onboard-account.md) 및 [소싱 대상](../setup/onboard-audiences.md#map-fields) 안내서를 참조하십시오.

>[!IMPORTANT]
>
>여러 일치 키가 사용되는 대상을 활성화할 때 하나(또는 그 이상) 일치 키에 겹침이 없거나 대상 수가 없거나 임계값 미만이면 전체 활성화가 실패합니다. 활성화하기 전에 대상이 충분히 겹치고 모든 일치 키에서 최소 1000 ID 임계값을 충족하는지 확인하십시오.

* 이제 Adobe Experience Platform 대상이 여러 일치 키로 대상 활성화를 지원합니다. 또한 이제 활성화 중에 전송되는 일치 키를 지정하기 위해 대상의 매핑을 구성할 때 연결된 키를 사용할 수 있습니다. 자세한 내용은 [Experience Platform 대상](../destinations/experience-platform.md#linked-keys) 안내서를 참조하십시오.
* 이제 공동 작업자가 여러 대상을 한 번에 편집할 수 있습니다. 이제 일괄 편집 도구를 사용하여 여러 대상에 대한 대상 메타데이터, 연결 액세스, 이름, 설명 및 범주를 편집할 수 있습니다. 대상자 편집에 대한 자세한 내용은 [대상자 관리](../setup/onboard-audiences.md#edit-audiences) 안내서를 참조하십시오.

## 2025년 7월 {#july-2025}

Real-Time CDP Collaboration은 이제 브랜드 간 공동 작업을 지원합니다. 이제 공동 작업자는 광고주인지 게시자인지에 관계없이 연결을 형성할 수 있습니다. 이를 통해 보다 유연한 공동 작업 기회를 얻을 수 있으며 브랜드가 서로의 데이터와 통찰력을 활용할 수 있습니다. 브랜드 간 공동 작업과 광고주 간 공동 작업의 차이점에 대해 자세히 알아보려면 [공동 작업 패턴](../overview/collaboration-patterns.md) 안내서를 읽어 보십시오.

* 공동 작업자는 이제 [개인 연결 초대](../connect/establishing-connections.md#private-connection-invites)를 사용하여 서로 연결할 수 있습니다. 계정의 고유 연결 코드를 공동 작업자와 공유하면 공동 작업자가 이를 사용하여 사용자와 직접 연결할 수 있습니다. 이는 브랜드 간 공동 작업의 핵심 기능으로, 공동 작업자는 **[!UICONTROL 공동 작업자 검색]** 디렉터리를 탐색하는 광고주를 넘어 연결을 설정할 수 있습니다.
* 이제 [셀프 서비스 대상](../setup/manage-destinations.md)을 광고주와 게시자 모두에서 사용할 수 있습니다.
* 이제 [계정 역할](../overview/roles.md)에 관계없이 연결된 두 공동 작업자에 대해 대상 활성화를 사용할 수 있습니다. 대상 활성화 설정은 [연결을 설정하는 동안](../connect/establishing-connections.md#configure-connection-settings)구성되어 대상을 활성화할 수 있는 공동 작업자를 지정할 수 있습니다. 대상자 활성화에 대한 자세한 내용은 [대상자 활성화](../collaborate/activate.md) 안내서를 참조하십시오.
* 브랜드 간 공동 작업을 지원하도록 **[!UICONTROL 활성화]** 사용 사례를 다시 구성했습니다. 이제 프로젝트 내의 **[!UICONTROL 활성화]** 탭에 공동 작업자에게 전송된 대상과 공동 작업자가 대상으로 활성화한 대상이 표시됩니다. 자세한 내용은 [대상자 활성화](../collaborate/activate.md) 안내서를 참조하십시오. <br> ![대상자 및 대상자 활성화 섹션이 있는 대시보드 활성화.](/help/assets/release-notes/2025/activate-dashboard.png){zoomable="yes"}
* 이제 프로젝트의 **[!UICONTROL 검색]** 탭에서 대상 인덱스 점수를 사용할 수 있습니다. 대상 색인 점수는 대상이 공동 작업자의 대상과 얼마나 잘 일치하는지 측정하는 것입니다. 이 점수는 기본 대상 수 및 중복을 기반으로 계산됩니다. 대상 색인 점수에 대한 자세한 내용은 [대상 색인 점수](../collaborate/discover.md#audience-index-score) 안내서를 참조하십시오.

## 2025년 5월 {#may-2025}

* 이제 **호주** 및 **뉴질랜드**&#x200B;의 고객이 Real-Time CDP Collaboration을 사용할 수 있습니다. 이러한 지역의 Real-Time CDP Prime 및 Ultimate 고객이 자동으로 사용할 수 있습니다.
* 이제 Real-Time CDP Collaboration에서 [설정](../setup/manage-destinations.md) 섹션의 **[!UICONTROL 내 대상]** 탭을 통해 **[!UICONTROL 셀프 서비스 대상]**&#x200B;을 제공합니다. 대상을 사용하면 광고 네트워크 또는 데이터 관리 플랫폼과 같은 서드파티 플랫폼에서 대상을 활성화하여 다양한 채널에서 고객에게 도달할 수 있습니다. 현재 Adobe Experience Platform 대상만 지원됩니다. 다른 대상을 구성하는 데 관심이 있는 경우 Adobe 담당자에게 문의하십시오. 대상에 대한 자세한 내용은 [대상 개요](../destinations/overview.md) 안내서를 참조하십시오.
   * 대상에는 [Collaboration 대상 포털](https://experienceleague.adobe.com/en/docs/experience-platform/segmentation/ui/audience-portal.md#manage-audiences)에서 Adobe Experience Platform 대상을 볼 수 있는 지원도 추가됩니다.
* 이제 Collaboration에서 기존 데이터 연결의 대상 새로 고침 빈도를 편집할 수 있습니다. 현재 대상자를 매일 또는 2~6일마다 새로 고치도록 선택할 수 있습니다. 대상 새로 고침 빈도를 편집하는 방법에 대한 자세한 내용은 [데이터 연결 관리](../setup/manage-data-connection.md#scheduling) 안내서를 참조하십시오.
* 이제 연결 내에서 선택한 각 사용 사례에 대해 공동 작업자 간의 크레딧 분할이 설정됩니다. 각 사용 사례에 대해 서로 다른 크레딧 소비 규칙을 설정하여 크레딧이 사용되는 방식을 보다 효과적으로 제어할 수 있습니다. 크레딧 분할 기능에 대해 자세히 알아보려면 [연결 설정](../connect/establishing-connections.md#connection-settings) 안내서를 읽어 보십시오. 크레딧 사용 방법에 대한 자세한 내용은 [크레딧 활동 유형](../setup/my-activity.md#types-of-activities) 안내서를 참조하십시오. <br> ![크레딧 분할 기능을 표시하는 연결 설정 화면입니다.](/help/assets/release-notes/2025/credit-split.png){zoomable="yes"}
* 이제 게시자는 광고주로부터 연결 설정을 수락하기 전에 광고주 이름과 ID를 설정할 수 있습니다. 게시자는 광고주의 이름 및 ID와 다를 수 있는 내부 시스템에 맞는 이름 및 ID를 설정할 수 있습니다. 광고주 이름 및 ID 추가에 대한 자세한 내용은 [연결 설정](../connect/establishing-connections.md#connection-settings.md) 안내서를 참조하십시오. <br> ![게시자 설정 광고주 이름 및 ID를 표시하는 연결 설정 화면입니다.](/help/assets/release-notes/2025/add-advertiser-names-modal.png){zoomable="yes"}

## 2025년 4월 {#april-2025}

* 새 **[!UICONTROL 입력 처리됨]** 열이 신용 소비 활동 테이블에 추가되었습니다. 이 열에는 각 활동에 대해 처리된 총 입력 수(예: ID 또는 행)가 표시됩니다. [자세히 보기](/help/guide/setup/my-activity.md#inputs-processed). <br> ![내 활동 보기에서 처리된 입력 열이 강조 표시되었습니다.](/help/assets/release-notes/2025/inputs-processed-column.png){zoomable="yes"}
* 새 연락처 이메일 옵션이 계정 만들기에 추가되었습니다. 이렇게 하면 파트너 공동 작업자가 연결 프로세스 중에 필요에 따라 연락할 수 있습니다. [자세히 보기](../setup/onboard-account.md).

## 2025년 3월 {#march-2025}

* 이제 [대상을 Collaboration에 소싱](/help/guide/setup/onboard-audiences.md)할 때 **대상 관리 크레딧 활동**&#x200B;을 더 잘 관리하기 위해 [1일에서 6일마다](/help/guide/setup/my-activity.md#types-of-activities)의 대상 새로 고침 빈도를 설정할 수 있습니다. 자세한 내용은 [대상자 관리](https://experienceleague.adobe.com/en/docs/experience-platform/segmentation/ui/audience-portal.md#manage-audiences) 안내서를 참조하십시오. <br> ![대상자 멤버십을 업데이트하기 위한 다른 빈도 간격을 보여 주는 예약 화면입니다.](/help/assets/setup/add-manage-audiences/audience-scheduling-frequency.png "대상자 멤버십을 업데이트하기 위한 다른 빈도 간격을 보여 주는 예약 화면"){width="250" align="center" zoomable="yes"}
* 이제 공동 작업자와 연결을 설정할 때 사전 정의된 **사용 사례**&#x200B;에서 선택할 수 있습니다. 선택한 사용 사례에 따라 사용 가능한 프로젝트 섹션과 제품 기능이 결정됩니다. 자세한 내용은 [프로젝트 관리](/help/guide/collaborate/manage-projects.md#project-use-cases) 안내서를 참조하십시오.
   * *Measurement*&#x200B;에서 **Measure** 프로젝트 섹션을 사용하도록 설정합니다.
   * *대상 검색*&#x200B;에서 **검색** 프로젝트 섹션을 사용하도록 설정합니다.
   * *대상 활성화*&#x200B;를 통해 **활성화** 프로젝트 섹션 <br>을(를) 사용할 수 있습니다.
* 이제 더 이상 함께 작업하지 않으려는 공동 작업자와의 연결을 삭제할 수 있습니다. 연결을 삭제하는 방법에 대해 알아보려면 [연결 삭제](/help/guide/connect/establishing-connections.md#delete-connections) 안내서를 참조하십시오.

## 2025년 2월 {#february-2025}

광고주와 게시자가 서드파티 쿠키 없이 고부가가치 대상을 검색, 활성화 및 측정할 수 있도록 특별히 제작된 Adobe Real-Time CDP Collaboration은 현재 미국에서 일반적으로 사용할 수 있습니다.

### 시작하기

1. **액세스 설정**: 시스템 관리자는 사용자에 대한 액세스 권한을 구성합니다. 액세스 권한 구성에 대한 자세한 내용은 [사용자 액세스 관리](/help/guide/permissions/manage-user-access.md#RTCDP-collaboration-access) 안내서를 참조하십시오.
2. **데이터 원본 연결**: Collaboration에서 사용할 Source 대상입니다. 대상자 소싱을 시작하려면 [소스 및 대상자 관리](/help/guide/setup/onboard-audiences.md) 안내서를 읽어 보세요.
3. **연결 설정**: 신뢰할 수 있는 광고주 또는 게시자와 공동 작업을 시작합니다. 연결 형성에 대한 자세한 내용은 [연결 설정](/help/guide/connect/establishing-connections.md) 안내서를 참조하십시오.
4. **검색 및 활성화**: 캠페인에서 활성화할 중요한 대상을 식별하는 프로젝트를 만듭니다. 프로젝트 만들기에 대한 자세한 내용은 [프로젝트 관리](/help/guide/collaborate/manage-projects.md) 안내서를 참조하십시오.

### 가용성

* Adobe Real-Time CDP Collaboration은 현재 미국 고객만 사용할 수 있습니다.
* Adobe Real-Time CDP Prime 및 Ultimate 고객에게 자동으로 제공됩니다

자세한 내용은 다음을 참조하십시오.

* [Collaboration 개요](/help/guide/home.md)
* [전체 워크플로](/help/guide/overview/end-to-end-workflow.md)
* [권한 개요](/help/guide/permissions/overview.md)
