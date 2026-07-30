---
title: 대상자 개요
description: 소스 위치를 포함하여 Real-Time CDP Collaboration의 대상에 대해 알아봅니다.
audience: admin, publisher
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/kr/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
topic_v2:
  - id: b5520579-b31f-4df7-9281-f0d9f91e2edc
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: f7cd44177d60bfd3d3db384f7b1a250ace4c3633
workflow-type: tm+mt
source-wordcount: 707
ht-degree: 5%

---


# 대상자 개요

{{limited-availability-release-note}}

Adobe Real-Time CDP Collaboration에서 대상은 Collaboration으로 가져오는 사용자 또는 고객 그룹입니다. 소싱 후 대상을 사용하여 공동 작업자와 중복을 발견하고 대상을 활성화하며 캠페인 성과를 측정할 수 있습니다. 대상 데이터가 이미 있는 위치에 따라 Adobe Experience Platform, 클라우드 스토리지 및 공유 시스템, 파일 업로드 워크플로 등 다양한 소스 유형에서 대상을 소스 할 수 있습니다.

## 대상자를 통해 수행할 수 있는 작업 {#audiences-in-collaboration}

대상자를 Collaboration으로 가져온 후에는 지원되는 공동 작업 워크플로우에서 사용할 수 있습니다.

Collaboration의 대상 을 사용하여 다음을 수행할 수 있습니다.

* 대상과 공동 작업자 대상 비교
* 중복 및 기회 파악
* 대상자 활성화
* 결과 및 캠페인 성과 측정
* 대상 가시성 및 관련 설정 관리

## 대상이 Collaboration에 맞는 방법 {#conceptual-diagram}

>[!NOTE]
>
> 다음 다이어그램은 소스 대상이 Collaboration에 어떻게 적합하고 프로젝트에서 어떻게 사용되는지에 대한 높은 수준의 보기를 제공합니다.

```text
Source → Data connection → Audience → Project
                                         │
                          ┌──────────────┼──────────────┐
                          ▼              ▼              ▼
                      Discover       Activate       Measure
                                         │
                                         ▼
                                    Destination
```

## 핵심 개념 {#core-concepts}

다음 개념에서는 대상 소싱 및 공동 작업 워크플로우와 관련된 주요 객체를 설명합니다.

**Source**\
대상 데이터가 생성되는 시스템 또는 위치(예: Adobe Experience Platform, 클라우드 저장소 위치 또는 파일 업로드).

**데이터 연결**\
Collaboration이 소스에서 대상 데이터에 액세스하는 데 사용하는 구성된 연결입니다. 데이터 연결에는 인증, 필드 매핑 및 예약과 같은 소스별 구성 세부 사항이 포함됩니다.

**대상자**\
Collaboration에 소스가 제공되고 프로젝트에서 사용할 수 있는 사용자 또는 고객 그룹입니다.

**Connection**\
조직과 다른 조직 간의 협업 관계.

**프로젝트**\
공동 작업자가 검색, 활성화 및 측정과 같은 지원되는 사용 사례에 대해 대상을 함께 사용하는 작업 영역입니다.

**대상**\
활성화된 대상자가 전송되는 외부 플랫폼 또는 시스템입니다.

**일치 키**
Collaboration이 데이터 세트 및 공동 작업자 간에 레코드를 일치시키는 데 사용하는 식별자입니다. 일치 키는 대상 중복, 활성화 및 측정과 같은 워크플로를 지원합니다.

## 대상 라이프사이클 {#audience-lifecycle}

Collaboration에서는 데이터 연결을 통해 대상을 소싱하고 **[!UICONTROL 설정]**&#x200B;에서 관리하며 지원되는 사용 사례를 위해 프로젝트에서 사용합니다.

1. **Source 대상**: 데이터 연결을 통해 대상 데이터를 Collaboration으로 가져옵니다.
2. **대상자 관리**: 대상자 세부 정보, 가시성 및 관련 설정을 검토하고 관리합니다.
3. **프로젝트에서 대상 사용**: **검색**, **활성화** 및 **측정**&#x200B;을(를) 포함하여 지원되는 사용 사례에 대해 프로젝트에서 소스 대상을 사용합니다.

모든 대상자가 모든 사용 사례에서 사용되는 것은 아닙니다. 예를 들어 대상자를 활성화하지 않고 **Discover**&#x200B;에 대해 소싱하여 사용하거나 대상으로 보내지 않고 **Measure** 워크플로우에서 사용할 수 있습니다.

대상자 소싱 및 관리에 대한 자세한 내용은 [Source 및 대상자 관리](./onboard-audiences.md)를 참조하십시오. 데이터 연결 관리에 대한 자세한 내용은 [데이터 연결 관리](./manage-data-connection.md)를 참조하십시오.

## 대상자 위치 {#supported-sources}

Collaboration은 여러 대상 소스 유형을 지원합니다. 선택하는 소스는 설정 흐름, 사전 요구 사항, 인증 요구 사항, 데이터 형식, 필드 매핑, 새로 고침 동작 및 대상을 Collaboration으로 가져오기 위한 사용 가능한 구성 옵션을 결정합니다.

* Adobe Experience Platform
* Amazon S3, Google 클라우드 스토리지 및 Azure 스토리지를 포함한 클라우드 스토리지
* Snowflake 및 Databricks Delta Share를 포함한 데이터 공유 서비스
* Adobe Audience Manager
* CSV 파일 업로드

지원되는 원본 목록과 원본별 설정 단계는 [원본 개요](./source-overview.md#available-sources)를 참조하세요.

## 대상자 구성 {#match-keys}

RTCDP Collaboration의 대상은 일치 키로 구성됩니다. 계정 구성에 따라 지원되는 일치 키에는 **사람 ID**, **장치 ID** 및 **파트너 ID**&#x200B;가 포함될 수 있습니다. 일치 키는 **대상 겹치기**, **활성화** 및 **측정**&#x200B;과 같은 워크플로를 지원합니다.

자세한 내용은 [일치 키 설정](../setup/onboard-account.md#set-up-match-keys) 및 [데이터 연결 관리](../setup/manage-data-connection.md#match-keys)를 참조하세요.

## 프로젝트에서 대상 사용 {#audiences-in-projects}

프로젝트는 다른 조직과 공동 작업하기 위한 컨텍스트를 제공합니다. 프로젝트 내에서 지원되는 공동 작업 사용 사례에 대상을 사용할 수 있습니다.

* **검색**: 대상을 비교하고 중복 인사이트를 검토합니다. [대상 겹치기 검색](../collaborate/discover.md)을 참조하십시오.
* **활성화**: 선택한 대상자를 캠페인에 사용할 수 있도록 활성화합니다. 활성화 작업은 프로젝트 작업 영역의 [!UICONTROL 활성화] 탭에서 시작되며 연결의 구성된 대상으로 대상자를 보냅니다. [대상자 활성화](../collaborate/activate.md)를 참조하십시오.
* **측정값**: 프로젝트와 연결된 캠페인 게재 및 전환 보고서를 검토합니다. [성능 측정](../collaborate/measure.md)을 참조하세요.

프로젝트 만들기 및 관리에 대한 자세한 내용은 [프로젝트 만들기 및 관리](../collaborate/manage-projects.md)를 참조하십시오. 대상 구성에 대한 자세한 내용은 [대상 개요](../destinations/overview.md)를 참조하십시오.

## 다음 단계 {#next-steps}

* [사용 가능한 대상 소스 검토](./source-overview.md)
* [Source 및 대상자 관리](./onboard-audiences.md)
* [프로젝트 만들기 및 관리](../collaborate/manage-projects.md)
* [대상자 중복 검색](../collaborate/discover.md)
* [대상자 활성화](../collaborate/activate.md)
* [성능 측정](../collaborate/measure.md)
* [대상 개요](../destinations/overview.md)
