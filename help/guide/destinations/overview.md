---
title: 표시 개요
description: Real-Time CDP Collaboration의 대상에 대해 알아봅니다.
audience: admin, publisher
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 5cbbf5c4-4caa-40da-97be-690d95c1201c
source-git-commit: 4ef7f8c7c27935f0e5b3620da63e7129f2714b37
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 6%

---

# 대상 개요

{{limited-availability-release-note}}

대상은 타깃팅된 대상을 외부 플랫폼으로 전송하는 데 사용되는 통합입니다. 이러한 통합을 통해 다양한 마케팅 채널 및 플랫폼에서 캠페인 및 고객 참여에 사용할 대상을 활성화할 수 있습니다.

공동 작업자는 캠페인에서 사용할 대상을 Adobe Experience Platform과 같은 외부 플랫폼으로 보내도록 대상을 구성할 수 있습니다. 그런 다음 공동 작업자는 [프로젝트 내의 대상을 활성화](../collaborate/activate.md)할 수 있으며, 이러한 대상은 연결의 구성된 대상으로 전송됩니다. 연결에 구성된 대상 활성화 설정 [에 따라 공동 작업자가 활성화할 수 있습니다](/help/guide/connect/establishing-connections.md#configure-connection-settings).

>[!IMPORTANT]
>
>현재 공동 작업자가 프로젝트 내에서 대상을 활성화하면 연결의 구성된 대상으로 자동으로 전송됩니다. **반드시** 대상을 구성해야 공동 작업자가 프로젝트 내의 대상을 활성화할 수 있습니다.

## 대상 구성 {#configure-destinations}

대상을 구성하려면 **[!UICONTROL 설정]**(으)로 이동한 다음 **[!UICONTROL 내 대상]** 탭을 선택합니다. 여기에서 사용 가능한 모든 대상을 볼 수 있습니다.

>[!NOTE]
>
> 현재 Adobe Experience Platform만 Collaboration 내에서 셀프서비스 대상으로 사용할 수 있습니다. Amazon S3 또는 Snowflake과 같은 대상을 구성하는 데 관심이 있는 경우 Adobe 담당자에게 문의하십시오.

![사용 가능한 대상을 표시하는 설정 작업 영역의 내 대상 탭입니다.](/help/assets/destinations/overview/my-destinations-overview.png)

대상 구성을 시작하려면 선택한 대상 내에서 **[!UICONTROL 설정]** 옵션을 선택하십시오. 특정 대상을 구성하는 방법에 대한 자세한 내용은 [사용 가능한 대상](#available-destinations) 표의 안내서를 참조하십시오.

![Adobe Experience Platform 지정에 대해 [설정] 옵션이 강조 표시된 [내 대상] 작업 영역입니다.](/help/assets/destinations/overview/my-destinations-set-up.png)

### 사용 가능한 대상 {#available-destinations}

Collaboration에서 구성할 수 있는 대상은 다음과 같습니다. 해당 대상에 대한 구성 가이드를 보려면 아래 표에서 대상 이름을 선택하십시오. 현재 사용할 수 없는 대상을 구성하는 데 관심이 있는 경우 Adobe 담당자에게 문의하십시오.

| 대상 | 가용성 |
| --- | --- |
| [Adobe Experience Platform](./experience-platform.md) | 사용 가능 |
| Amazon S3 | 곧 출시 예정 |
| Snowflake | 곧 출시 예정 |
| Google 클라우드 스토리지 | 곧 출시 예정 |
| Azure Blob 스토리지 | 곧 출시 예정 |

## 다음 단계

대상을 구성하고 나면 프로젝트 내에서 [타깃팅된 대상 활성화](../collaborate/activate.md)를 시작할 수 있습니다.
