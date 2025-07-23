---
title: 감사 로그
description: Real-Time CDP Collaboration에서 감사 로그 기능을 사용하여 사용자 활동 및 변경 사항을 추적하는 방법에 대해 알아봅니다.
audience: admin
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 3af1ac47-dc3d-4f19-a6b9-9e4e835977c0
source-git-commit: eed99cfafd5ffad5a468741f7258c162454769b7
workflow-type: tm+mt
source-wordcount: '888'
ht-degree: 1%

---

# 감사 로그

{{limited-availability-release-note}}

시스템에서 수행되는 활동의 투명성과 가시성을 높이기 위해 Adobe Experience Platform에서 감사 로그 형태로 다양한 서비스 및 기능에 대한 사용자 활동을 감사할 수 있습니다. 이러한 로그는 Adobe Real-Time CDP Collaboration의 문제 해결에 도움이 될 수 있는 감사 추적을 형성하며, 기업이 기업 데이터 관리 정책 및 규제 요구 사항을 효과적으로 준수하는 데 도움이 됩니다.

기본적으로 감사 로그는 *누가*&#x200B;이(가) *무엇을* 작업하고 *언제*&#x200B;했는지 알려 줍니다. 로그에 기록된 각 작업에는 작업 유형, 날짜 및 시간, 작업을 수행한 사용자의 이메일 ID 및 작업 유형과 관련된 추가 속성을 나타내는 메타데이터가 포함됩니다.

Collaboration의 감사 로그 기능을 사용하여 플랫폼 내에서 사용자 활동 및 변경 사항을 추적합니다. 이 기능은 Experience Platform 감사 서비스와 통합되며, 이 기능에 대한 UI는 Experience Platform에 있습니다.

![감사 로그 기능의 높은 수준 개요 화면](/help/assets/setup/audit-logs/audit-logs-overview.png)

감사 로그에 대한 자세한 내용은 [Experience Platform 감사 로그 설명서](https://experienceleague.adobe.com/en/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview){target="_blank"}를 참조하세요.

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

감사 로그를 보려면:

1. Experience Platform의 **[!UICONTROL 감사]** 섹션으로 이동합니다.
2. [필터](#filter-audit-logs)를 사용하여 조건에 따라 로그 범위를 좁힙니다.
3. 타임스탬프, 요청 ID, 리소스 세부 정보 및 작업 상태를 포함하여 자세한 정보를 보려면 로그 항목을 선택하십시오.

![자세한 감사 로그](/help/assets/setup/audit-logs/filters-and-detailed-view.png)

### 캡처된 활동

감사 로그는 다음을 포함하여 사용자 활동에 대한 자세한 정보를 캡처합니다.

* **타임스탬프**: 수행한 작업의 정확한 날짜 및 시간(월/일/년 시간):minute 오전/오후 형식입니다.
* **자산 이름**: 작업이 수행된 리소스의 이름입니다.
* **범주**: 작업이 수행된 리소스의 유형입니다.
* **작업**: 만들기 또는 삭제와 같이 수행된 특정 작업입니다.
* **사용자**: 작업을 수행한 사용자의 전자 메일 주소입니다.

이러한 로그는 Collaboration 인스턴스 내의 모든 활동에 대한 포괄적인 추적을 생성하므로 데이터 거버넌스 및 규제 준수에 유용합니다. [UI에서 감사 로그 관리](https://experienceleague.adobe.com/en/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview#managing-audit-logs-in-the-ui)에 대해 자세히 알아보십시오.

### 감사 로그 필터링 {#filter-audit-logs}

감사 로그 UI는 특정 로그를 검색하는 데 도움이 되는 몇 가지 필터를 제공합니다.

* **범주**: Collaboration 인스턴스 또는 Collaboration 연결 초대와 같이 작업이 수행된 리소스의 유형입니다.
* **작업**: 수행된 작업의 유형입니다. 사용 가능한 작업은 선택한 범주에 따라 다릅니다. 예를 들어 Collaboration 인스턴스에 대한 작업에는 만들기, 업데이트 및 삭제가 포함됩니다.
* **요청 ID**: 요청의 고유 식별자입니다.
* **사용자**: 작업을 수행한 사용자의 전자 메일 주소입니다.
* **상태**: 허용 또는 거부와 같은 작업 상태입니다.
* **날짜 범위**: 로그를 보려는 날짜 범위입니다.

[감사 로그 필터링](https://experienceleague.adobe.com/en/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview#filter-audit-logs)에 대해 자세히 알아보세요.

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
| **[!UICONTROL Collaboration 데이터 엔터티]** | 만들기, 업데이트, 삭제 | 데이터 엔티티 만들기, 업데이트 및 삭제를 포함하여 Collaboration의 데이터 엔티티를 관리합니다. 이 컨텍스트의 데이터 엔티티는 대상자를 참조합니다. 자세한 내용은 [대상자 소싱 및 관리](/help/guide/setup/onboard-audiences.md) 안내서를 참조하십시오. |
| **[!UICONTROL Collaboration 프로젝트]** | 만들기, 업데이트, 삭제 | 프로젝트 만들기, 업데이트 및 삭제를 포함하여 Collaboration 내에서 프로젝트를 관리합니다. 자세한 내용은 [프로젝트 관리](/help/guide/collaborate/manage-projects.md) 안내서를 참조하십시오. |
| **[!UICONTROL Collaboration 모듈]** | 만들기, 업데이트, 삭제 | UI에서 다양한 모듈 생성, 업데이트 및 삭제를 포함하여 프로젝트 내에서 다양한 모듈을 관리합니다. 예를 들어, [대상을 활성화](/help/guide/collaborate/activate.md)하는 기능입니다. |

{style="table-layout:auto"}

감사 로그 기능을 활용하면 Collaboration 내의 모든 활동에 대한 명확하고 자세한 기록을 유지 관리할 수 있으므로, 투명성과 신뢰성을 보장할 수 있습니다.
