---
title: 감사 로그
description: Real-Time CDP Collaboration에서 감사 로그 기능을 사용하여 사용자 활동 및 변경 사항을 추적하는 방법에 대해 알아봅니다.
audience: admin
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/kr/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 3af1ac47-dc3d-4f19-a6b9-9e4e835977c0
TQID: https://experienceleague.adobe.com/zb09-bUpxJ2VPDknETHeayMuLpNRCaQ2VTnV9QnTRgE
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 3ce7e66b31332836fd6cc6137c94622436505cc9
workflow-type: tm+mt
source-wordcount: 950
ht-degree: 2%

---

# 감사 로그

{{limited-availability-release-note}}

시스템에서 수행되는 활동의 투명성과 가시성을 높이기 위해 Adobe Experience Platform에서 감사 로그 형태로 다양한 서비스 및 기능에 대한 사용자 활동을 감사할 수 있습니다. 이러한 로그는 Adobe Real-Time CDP Collaboration의 문제 해결에 도움이 될 수 있는 감사 추적을 형성하며, 기업이 기업 데이터 관리 정책 및 규제 요구 사항을 효과적으로 준수하는 데 도움이 됩니다.

기본적으로 감사 로그는 *누가*&#x200B;이(가) *무엇을* 작업하고 *언제*&#x200B;했는지 알려 줍니다. 로그에 기록된 각 작업에는 작업 유형, 날짜 및 시간, 작업을 수행한 사용자의 이메일 ID 및 작업 유형과 관련된 추가 속성을 나타내는 메타데이터가 포함됩니다.

Collaboration의 감사 로그 기능을 사용하여 플랫폼 내에서 사용자 활동 및 변경 사항을 추적합니다. 이 기능은 Experience Platform 감사 서비스와 통합되며, 이 기능에 대한 UI는 Experience Platform에 있습니다.

![감사 로그 기능의 높은 수준 개요 화면](/help/assets/setup/audit-logs/audit-logs-overview.png)

감사 로그에 대한 자세한 내용은 [Experience Platform 감사 로그 설명서](https://experienceleague.adobe.com/ko/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview){target="_blank"}를 참조하세요.

## 감사 로그 액세스

아래 섹션에 설명된 대로 두 가지 방법으로 감사 로그에 액세스할 수 있습니다. 두 옵션 모두 Collaboration 내에서 수행된 다양한 활동을 캡처하는 감사 로그 목록을 표시합니다.

### Collaboration 사용자 인터페이스에서 감사 로그 액세스

1. Collaboration의 **[!UICONTROL 설정]** 작업 영역에서 **[!UICONTROL 내 활동]** 탭으로 이동합니다.
2. 페이지 상단의 텍스트에서 Experience Platform 링크를 선택합니다.

![Collaboration의 [내 활동] 탭에서 감사 로그에 액세스합니다.](/help/assets/setup/audit-logs/access-from-collaboration-ui.png)

### Experience Platform 사용자 인터페이스에서 직접 감사 로그 액세스

1. [Experience Platform](https://platform.adobe.com/)&#x200B;(으)로 이동하고 왼쪽 메뉴에서 **[!UICONTROL 감사]** 섹션을 선택합니다. 감사 로그를 볼 수 없는 경우 조직의 시스템 관리자에게 연락하여 필요한 권한을 얻으십시오.

![Experience Platform에서 감사 로그에 액세스합니다.](/help/assets/setup/audit-logs/access-from-experience-platform-ui.png)

## 감사 로그 보기 및 사용

To view the audit logs:

1. Navigate to the **[!UICONTROL Audits]** section in Experience Platform.
2. Use the [filters](#filter-audit-logs) to narrow down the logs based on your criteria.
3. Select a log entry to view detailed information, including the timestamp, request ID, resource details, and action status.

![Detailed Audit Log](/help/assets/setup/audit-logs/filters-and-detailed-view.png)

### Captured activities

Audit logs capture detailed information about user activities, including:

* **Timestamp**: The exact date and time of the action performed in a month/day/year hour:minute AM/PM format.
* **Asset name**: The name of the resource on which the action was performed.
* **Category**: The type of resource the action was performed on.
* **Action**: The specific action performed, such as create or delete.
* **User**: The email address of the user who performed the action.

These logs create a comprehensive trail of all activities within your Collaboration instance, which is useful for data governance and regulatory compliance. Read more about [managing audit logs in the UI](https://experienceleague.adobe.com/ko/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview#managing-audit-logs-in-the-ui).

### Filter audit logs {#filter-audit-logs}

The audit logs UI provides several filters to help you search for specific logs:

* **Category**: The type of resource the action was performed on, such as Collaboration Instance or Collaboration Connection Invite.
* **Action**: The type of action performed. Available actions depend on the category selected. For example, actions for Collaboration Instance include create, update, and delete.
* **Request ID**: A unique identifier for the request.
* **User**: The email address of the user who performed the action.
* **Status**: The status of the action, such as allow or deny.
* **Date Range**: The range of dates for which you want to view logs.

Read more about [filtering audit logs](https://experienceleague.adobe.com/ko/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview#filter-audit-logs).

## 이점

감사 로그는 Collaboration을 사용하는 조직에 여러 가지 이점을 제공합니다.

* **데이터 거버넌스**: 감사 로그를 사용하여 플랫폼 내의 모든 활동을 추적하고 감사할 수 있도록 합니다.
* **규정 준수**: 이 기능은 규정 요구 사항을 충족하는 일련의 사용자 활동을 제공합니다.
* **문제 해결**: 감사 로그는 사용자 작업의 세부 로그를 제공하여 문제를 식별하고 해결하는 데 도움이 됩니다.

## 범주 및 작업 참조

아래 표는 Real-Time CDP Collaboration에 대한 모든 범주 및 작업에 대한 참조를 제공합니다.

![Real-Time CDP Collaboration 감사 로그에 강조 표시된 사용 가능한 범주.](/help/assets/setup/audit-logs/available-categories.png)

| 카테고리 | 작업 | 설명 |
|-------------------------------|------------------------------------------|-------------|
| **[!UICONTROL Collaboration 인스턴스]** | 만들기, 업데이트, 삭제 | 계정 만들기, 업데이트 및 삭제를 포함하여 계정을 관리합니다. 자세한 내용은 [계정 구성](/help/guide/setup/onboard-account.md) 안내서를 참조하십시오. |
| **[!UICONTROL Collaboration 연결 초대]** | 만들기, 업데이트, 삭제, 승인, 거부 | 초대 생성, 업데이트, 삭제, 승인 및 거부를 포함하여 연결 초대를 관리합니다. 자세한 내용은 [연결 설정](/help/guide/connect/establishing-connections.md) 안내서를 참조하십시오. |
| **[!UICONTROL Collaboration 연결]** | 만들기, 업데이트, 삭제, 승인, 거부, 승인 요청 | 연결 만들기, 업데이트, 삭제, 승인, 거부 및 승인 요청을 포함하여 연결을 관리합니다. |
| **[!UICONTROL Collaboration 데이터 연결]** | 만들기, 업데이트, 삭제 | 데이터 연결 만들기, 업데이트 및 삭제를 포함하여 대상을 소스 및 관리하는 위치의 데이터 연결을 관리합니다. 자세한 내용은 [데이터 연결 관리](/help/guide/setup/manage-data-connection.md) 안내서를 참조하십시오. |
| **[!UICONTROL Collaboration 데이터 엔터티]** | 만들기, 업데이트, 삭제 | 데이터 엔티티 만들기, 업데이트 및 삭제를 포함하여 Collaboration의 데이터 엔티티를 관리합니다. Data entities in this context refers to audiences. For more information, read the [sourcing and managing audiences](/help/guide/setup/onboard-audiences.md) guide. |
| **[!UICONTROL Collaboration Project]** | 만들기, 업데이트, 삭제 | Manage projects within Collaboration, including creating, updating, and deleting projects. For more information, read the [managing projects](/help/guide/collaborate/manage-projects.md) guide. |
| **[!UICONTROL Collaboration Module]** | 만들기, 업데이트, 삭제 | Manage different modules within projects, including creating, updating, and deleting various modules in the UI. For example, the ability to [activate audiences](/help/guide/collaborate/activate.md). |

{style="table-layout:auto"}

By leveraging the audit logs functionality, you can maintain a clear and detailed record of all activities within Collaboration, ensuring transparency and accountability.
