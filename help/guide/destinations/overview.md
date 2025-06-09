---
title: 표시 개요
description: Real-Time CDP Collaboration의 대상에 대해 알아봅니다.
audience: admin, publisher
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/kr/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
source-git-commit: f19aff1b7d10a446dd209721e7a6fdf537c9d63e
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 5%

---

# 대상 개요

{{limited-availability-release-note}}

대상은 타깃팅된 대상을 외부 플랫폼으로 전송하는 데 사용되는 통합입니다. 이러한 통합을 통해 다양한 마케팅 채널 및 플랫폼에서 캠페인 및 고객 참여에 사용할 대상을 활성화할 수 있습니다.

현재 대상은 Real-Time CDP Collaboration의 게시자만 사용할 수 있습니다. 게시자는 캠페인에서 사용할 대상을 외부 플랫폼(예: Adobe Experience Platform)으로 보내도록 대상을 구성할 수 있습니다. 그러면 광고주는 [프로젝트 내의 대상을 활성화](../collaborate/activate.md)할 수 있으며 게시자의 구성된 대상으로 전송됩니다.

>[!IMPORTANT]
>
>현재, 광고주가 프로젝트 내에서 대상을 활성화하면 자동으로 게시자의 구성된 대상으로 전송됩니다. 게시자는 **해야** 대상 *이전*&#x200B;을(를) 구성해야 합니다. 구성된 대상이 없으면 대상자가 사용자에게 전송되고 프로젝트 내의 **[!UICONTROL 활성화]** 탭에 표시되지만 활성화되지는 않습니다.

## 대상 구성 {#configure-destinations}

대상을 구성하려면 **[!UICONTROL 설정]**(으)로 이동한 다음 **[!UICONTROL 내 대상]** 탭을 선택합니다. 여기에서 사용 가능한 모든 대상을 볼 수 있습니다.

>[!NOTE]
>
> 현재 Adobe Experience Platform만 Real-Time CDP Collaboration 내에서 셀프서비스 대상으로 사용할 수 있습니다. Amazon S3 또는 Snowflake과 같은 대상을 구성하는 데 관심이 있는 경우 Adobe 담당자에게 문의하십시오.

![사용 가능한 대상을 표시하는 설정 작업 영역의 내 대상 탭입니다.](/help/assets/destinations/overview/my-destinations-overview.png)

대상 구성을 시작하려면 선택한 대상 내에서 **[!UICONTROL 설정]** 옵션을 선택하십시오. 특정 대상을 구성하는 방법에 대한 자세한 내용은 [사용 가능한 대상](#available-destinations) 표의 안내서를 참조하십시오.

![Adobe Experience Platform 지정에 대해 [설정] 옵션이 강조 표시된 [내 대상] 작업 영역입니다.](/help/assets/destinations/overview/my-destinations-set-up.png)

### 사용 가능한 대상 {#available-destinations}

Real-Time CDP Collaboration에서 구성할 수 있는 대상은 다음과 같습니다. 해당 대상에 대한 구성 가이드를 보려면 아래 표에서 대상 이름을 선택하십시오. 현재 사용할 수 없는 대상을 구성하는 데 관심이 있는 경우 Adobe 담당자에게 문의하십시오.

| 대상 | 가용성 |
| --- | --- |
| [Adobe Experience Platform](./experience-platform.md) | 사용 가능 |
| Amazon S3 | 곧 출시 예정 |
| Snowflake | 곧 출시 예정 |
| Google 클라우드 스토리지 | 곧 출시 예정 |
| Azure Blob 스토리지 | 곧 출시 예정 |

## 다음 단계

대상을 구성하고 나면 프로젝트 내에서 [타깃팅된 대상 활성화](../collaborate/activate.md)를 시작할 수 있습니다.
