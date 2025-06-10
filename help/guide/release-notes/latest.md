---
title: 최신 Real-Time CDP Collaboration 릴리스 노트
description: Real-Time CDP Collaboration의 최신 릴리스를 따르십시오.
audience: admin, publisher, advertiser
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/kr/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 8513c648-1cc1-4544-b86d-2ee3193ab60f
source-git-commit: 691161cdc1f9338a470373988fbc0dee9a5be6db
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 3%

---

# 최신 Real-Time CDP Collaboration 릴리스 노트

{{limited-availability-release-note}}

**마지막 업데이트**: 2025년 4월.

이러한 릴리스 노트는 Real-Time Customer Data Platform Collaboration에 릴리스된 기능을 다룹니다. Real-Time CDP Collaboration 릴리스는 연속 게재 모델에서 작동하므로 대략적인 월별 릴리스 케이던스를 사용할 수 있습니다. 이러한 릴리스 노트는 자주 업데이트되므로 정기적으로 확인하십시오.

## 2025년 5월 {#may-2025}

* 이제 **호주** 및 **뉴질랜드**&#x200B;의 고객이 Real-Time CDP Collaboration을 사용할 수 있습니다. 이러한 지역의 Real-Time CDP Prime 및 Ultimate 고객이 자동으로 사용할 수 있습니다.
* 이제 Real-Time CDP Collaboration에서 **[!UICONTROL 설정]** 섹션의 **[!UICONTROL 내 대상]** 탭을 통해 [셀프 서비스 대상](../setup/manage-destinations.md)을 제공합니다. 대상을 사용하면 광고 네트워크 또는 데이터 관리 플랫폼과 같은 서드파티 플랫폼에서 대상을 활성화하여 다양한 채널에서 고객에게 도달할 수 있습니다. 현재 Adobe Experience Platform 대상만 지원됩니다. 다른 대상을 구성하는 데 관심이 있는 경우 Adobe 담당자에게 문의하십시오. 대상에 대한 자세한 내용은 [대상 개요](../destinations/overview.md) 안내서를 참조하십시오.

   * 대상에는 [Real-Time CDP Collaboration 대상 포털](https://experienceleague.adobe.com/ko/docs/experience-platform/segmentation/ui/audience-portal.md#manage-audiences.)에서 Adobe Experience Platform 대상을 볼 수 있는 지원도 추가됩니다.

* 이제 Real-Time CDP Collaboration에서 기존 데이터 연결의 대상 새로 고침 빈도를 편집할 수 있습니다. 현재 대상자를 매일 또는 2~6일마다 새로 고치도록 선택할 수 있습니다. 대상 새로 고침 빈도를 편집하는 방법에 대한 자세한 내용은 [데이터 연결 관리](../setup/manage-data-connection.md#scheduling) 안내서를 참조하십시오.
* 이제 연결 내에서 선택한 각 사용 사례에 대해 공동 작업자 간의 크레딧 분할이 설정됩니다. 각 사용 사례에 대해 서로 다른 크레딧 소비 규칙을 설정하여 크레딧이 사용되는 방식을 보다 효과적으로 제어할 수 있습니다. 크레딧 분할 기능에 대해 자세히 알아보려면 [연결 설정](../connect/establishing-connections.md#connection-settings) 안내서를 읽어 보십시오. 크레딧 사용 방법에 대한 자세한 내용은 [크레딧 활동 유형](../setup/my-activity.md#types-of-activities) 안내서를 참조하십시오. <br> ![크레딧 분할 기능을 표시하는 연결 설정 화면입니다.](/help/assets/release-notes/2025/credit-split.png){zoomable="yes"}
* 이제 게시자는 광고주로부터 연결 설정을 수락하기 전에 광고주 이름과 ID를 설정할 수 있습니다. 게시자는 광고주의 이름 및 ID와 다를 수 있는 내부 시스템에 맞는 이름 및 ID를 설정할 수 있습니다. 광고주 이름 및 ID 추가에 대한 자세한 내용은 [연결 설정](../connect/establishing-connections.md#connection-settings.md) 안내서를 참조하십시오. <br> ![게시자 설정 광고주 이름 및 ID를 표시하는 연결 설정 화면입니다.](/help/assets/release-notes/2025/add-advertiser-names-modal.png){zoomable="yes"}

## 2025년 4월 {#april-2025}

* 새 **[!UICONTROL 입력 처리됨]** 열이 신용 소비 활동 테이블에 추가되었습니다. 이 열에는 각 활동에 대해 처리된 총 입력 수(예: ID 또는 행)가 표시됩니다. [자세히 보기](/help/guide/setup/my-activity.md#inputs-processed). <br> ![내 활동 보기에서 처리된 입력 열이 강조 표시되었습니다.](/help/assets/release-notes/2025/inputs-processed-column.png){zoomable="yes"}
* 새 연락처 이메일 옵션이 계정 만들기에 추가되었습니다. 이렇게 하면 파트너 공동 작업자가 연결 프로세스 중에 필요에 따라 연락할 수 있습니다. [자세히 보기](../setup/onboard-organization.md).

## 2025년 3월 {#march-2025}

* 이제 [대상을 Real-Time CDP Collaboration으로 가져오기](/help/guide/setup/onboard-audiences.md)할 때 **1일에서 6일마다**&#x200B;의 대상 새로 고침 빈도를 설정하여 [대상 관리 크레딧 활동](/help/guide/setup/my-activity.md#types-of-activities)을 보다 효율적으로 관리할 수 있습니다. [자세히 보기](/help/guide/setup/onboard-audiences.md#schedule). <br> ![대상자 멤버십을 업데이트하기 위한 다른 빈도 간격을 보여 주는 예약 화면입니다.](/help/assets/setup/add-manage-audiences/audience-scheduling-frequency.png "대상자 멤버십을 업데이트하기 위한 다른 빈도 간격을 보여 주는 예약 화면"){width="250" align="center" zoomable="yes"}
* 이제 공동 작업자와 연결을 설정할 때 사전 정의된 **사용 사례**&#x200B;에서 선택할 수 있습니다. 선택한 사용 사례에 따라 사용 가능한 프로젝트 섹션과 제품 기능이 결정됩니다. [자세히 보기](/help/guide/collaborate/manage-projects.md#project-use-cases).
   * *Campaign 측정*&#x200B;은(는) **측정** 프로젝트 섹션을 사용하도록 설정합니다.
   * *대상 검색*&#x200B;에서 **검색** 프로젝트 섹션을 사용하도록 설정합니다.
   * *대상 활성화*&#x200B;를 통해 **활성화** 프로젝트 섹션 <br>을(를) 사용할 수 있습니다.
* 이제 더 이상 함께 작업하지 않으려는 공동 작업자와의 연결을 삭제할 수 있습니다. [자세히 보기](/help/guide/connect/establishing-connections.md#delete-connections).


## 2025년 2월 - 미국 고객에 대한 일반 가용성 {#february-2025-ga}

광고주와 게시자가 서드파티 쿠키 없이 고부가가치 대상을 검색, 활성화 및 측정할 수 있도록 특별히 제작된 Real-Time CDP Collaboration은 현재 미국에서 일반적으로 사용할 수 있습니다.

### 시작

1. **액세스 설정**: 시스템 관리자는 사용자에 대한 액세스 권한을 구성합니다. [자세히 보기](/help/guide/permissions/manage-user-access.md#RTCDP-collaboration-access).
2. **데이터 원본 연결**: Real-Time CDP Collaboration에서 사용할 대상을 가져옵니다. [자세히 보기](/help/guide/setup/onboard-audiences.md).
3. **파트너 연결 설정**: 신뢰할 수 있는 브랜드 또는 게시자와 공동 작업을 시작합니다. [자세히 보기](/help/guide/connect/establishing-connections.md).
4. **검색 및 활성화**: 프로젝트를 만들어 소중한 대상 세그먼트를 식별하고 캠페인에서 활성화합니다. [자세히 보기](/help/guide/collaborate/manage-projects.md).

### 가용성

* Real-Time CDP Collaboration은 현재 미국 고객만 사용할 수 있습니다.
* Real-Time CDP Prime 및 Ultimate 고객에게 자동으로 제공됩니다

자세한 내용은 다음을 참조하십시오.

* [Real-Time CDP Collaboration 개요](/help/guide/home.md)
* [전체 워크플로](/help/guide/end-to-end-workflow.md)
* [권한 개요](/help/guide/permissions/overview.md)
