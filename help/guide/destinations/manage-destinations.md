---
title: 클라우드 스토리지 대상 구성 및 관리
description: Real-Time CDP Collaboration에서 클라우드 스토리지 대상을 구성, 보기 및 삭제하는 방법을 알아봅니다.
audience: admin, publisher
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/kr/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
topic_v2:
  - id: b5520579-b31f-4df7-9281-f0d9f91e2edc
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 60124235569ca9b17b3bb1cef502d57d39e82e1f
workflow-type: tm+mt
source-wordcount: 885
ht-degree: 2%

---

# 클라우드 스토리지 대상 구성 및 관리

**[!UICONTROL 활성화]** 작업 영역에서 클라우드 저장소 대상을 구성, 보기 및 삭제하려면 이 안내서를 사용하십시오. 대상을 구성하려면 **[!UICONTROL 카탈로그]** 탭을 사용하고, 대상을 관리하려면 **[!UICONTROL 대상]** 탭을 사용하고, 대상에 활성화된 대상을 검토하려면 **[!UICONTROL 활성화된 대상]** 탭을 사용하십시오.

대상을 구성한 후 대상을 활성화하면 사용할 수 있습니다. 지원되는 대상의 전체 목록을 보려면 [사용 가능한 대상](./overview.md#available-destinations) 표를 참조하십시오.

>[!NOTE]
>
> 이 안내서에서는 **[!DNL Amazon S3]** 대상을 예로 사용합니다. 안내식 구성 워크플로우는 지원되는 클라우드 스토리지 대상 유형에서 공유되지만 인증 방법, 필수 필드 및 커넥터 기능은 다를 수 있습니다. 대상을 구성하기 전에 해당 Adobe Experience Platform 대상 설명서에 연결된 [클라우드 저장소 대상 요구 사항](./cloud-storage-destination-requirements.md)을 검토하십시오.
>
> Adobe Experience Platform에는 Real-Time CDP Collaboration에 별도의 구성 워크플로가 있습니다. 이를 구성하려면 [대상으로 Adobe Experience Platform 구성](./experience-platform.md)을 참조하십시오.

## 사전 요구 사항 {#prerequisites}

대상을 구성하기 전에 다음을 확인하십시오.

* **[!UICONTROL 활성화]** 작업 영역에 액세스할 수 있습니다.
* 클라우드 스토리지 공급자에 필요한 연결 정보가 있습니다.
* 계정을 만들어야 하는 경우 필요한 자격 증명 또는 권한이 있습니다.
* 클라우드 저장소 대상에 대한 [요구 사항](./cloud-storage-destination-requirements.md)을 검토했습니다.

## 대상 구성 {#configure-destination}

대상을 구성할 때는 클라우드 스토리지 계정을 Real-Time CDP Collaboration에 연결하고 대상 데이터를 내보내는 방법을 정의합니다.

**[!UICONTROL 활성화]** > **[!UICONTROL 카탈로그]**(으)로 이동합니다.

**[!UICONTROL 카탈로그]** 탭에 사용 가능한 대상 공급자가 표시됩니다. 각 대상은 카드로 표시됩니다. 대상에 따라 카드에 구성된 계정과 추가 정보 보기 작업이 표시될 수 있습니다.

![대상 공급자 카드를 표시하는 카탈로그 탭입니다.](/help/assets/destinations/manage-destinations/destination-provider-catalog.png)

구성할 대상 공급자를 찾은 다음 **[!UICONTROL 설정]**&#x200B;을 선택합니다.

대상 구성 안내 설정이 열리고 **[!UICONTROL 인증]**, **[!UICONTROL 대상 만들기]**, **[!UICONTROL 필드 매핑]** 및 **[!UICONTROL 검토]**&#x200B;의 네 가지 단계를 안내합니다.

### 인증 {#authenticate}

**[!UICONTROL 인증]** 단계에서는 Real-Time CDP Collaboration과 대상 계정 간의 연결을 설정합니다.

기존 계정을 사용할 수 있는 경우 계정 선택기에서 선택합니다. 계정을 만들려면 **[!UICONTROL 새 계정]**&#x200B;을 선택하세요.

인증 방법을 선택하고 필요한 계정 정보를 제공합니다. 사용 가능한 인증 방법 및 필드는 선택한 대상 공급자에 따라 다릅니다. 커넥터별 요구 사항은 [클라우드 저장소 대상 요구 사항](./cloud-storage-destination-requirements.md)을 참조하십시오.

**[!UICONTROL Amazon S3에 연결]**&#x200B;을 선택합니다. 다른 대상 공급자의 경우 단추에 해당 공급자 이름이 표시됩니다.

계정의 유효성을 검사한 후 **[!UICONTROL 다음]**&#x200B;을(를) 선택하십시오.

![계정 선택 및 새 계정 만들기를 표시하는 인증 단계입니다.](/help/assets/destinations/manage-destinations/authenticate-destination-account.png)

### 대상 만들기 {#create-destination}

**[!UICONTROL 대상 만들기]** 단계는 대상 내보내기 파일이 전달되는 위치와 방법을 정의합니다.

대상 이름을 입력하고 필요한 저장소 및 내보내기 설정을 완료합니다. 사용 가능한 필드는 선택한 대상 공급자에 따라 다릅니다. 정의 및 커넥터별 요구 사항은 [클라우드 저장소 대상 요구 사항](./cloud-storage-destination-requirements.md)에서 연결된 대상 설명서를 참조하십시오.

모든 필수 필드를 완료한 후 **[!UICONTROL 다음]**&#x200B;을(를) 선택하십시오. 안내가 있는 설정이 필드 매핑 단계로 진행합니다.

![대상 구성 필드를 표시하는 대상 만들기 단계입니다.](/help/assets/destinations/manage-destinations/configure-new-destination.png)

### 필드 매핑 {#map-fields}

**[!UICONTROL 필드 매핑]** 단계에서는 대상 일치 키가 대상에서 예상한 ID 필드에 매핑되는 방식을 정의합니다.

표준 Real-Time CDP 대상 워크플로우와 달리 Real-Time CDP Collaboration은 대상이 만들어지는 동안 이러한 매핑을 구성합니다. 대상 일치 키는 소스 필드로 표시됩니다. 각 소스 필드를 해당 대상 ID에 매핑하여 대상에서 내보낸 식별자를 인식하고 해당 식별자를 의도한 사용자와 연결할 수 있도록 합니다.

다른 일치 키 매핑을 추가하려면 **[!UICONTROL 필드 추가]**&#x200B;를 선택하고 매핑을 제거하려면 삭제 아이콘을 선택하십시오. 필요한 모든 매핑을 검토하고 구성합니다.

매핑이 완료되면 **[!UICONTROL 다음]**&#x200B;을 선택합니다. 안내가 있는 설정이 검토 단계로 진행합니다.

![활성화 일치 키 매핑 구성을 표시하는 맵 필드 단계입니다.](/help/assets/destinations/manage-destinations/map-destination-fields.png)

### 검토 {#review-destination}

**[!UICONTROL 검토]** 단계에서는 대상 구성을 만들기 전에 요약합니다.

대상 설정을 검토합니다. 변경하려면 연필 아이콘 ![연필 아이콘](../../assets/icons/edit.png)을 선택하세요. 적용 가능한 섹션의 경우 구성을 업데이트하십시오.

구성이 올바르면 **[!UICONTROL 완료]**&#x200B;를 선택합니다. 대상이 만들어지고 대상 활성화에 사용할 수 있습니다.

![완료 전에 대상 구성 요약을 표시하는 검토 단계입니다.](/help/assets/destinations/manage-destinations/review-destination-configuration.png)

## 구성된 대상 보기 {#view-configured-destinations}

대상을 구성하면 대상 인벤토리에 표시됩니다. 인벤토리에서 상태와 이에 활성화된 대상을 검토할 수 있습니다.

**[!UICONTROL 활성화]** > **[!UICONTROL 대상]**(으)로 이동합니다. **[!UICONTROL 대상]** 탭에는 구성된 대상 테이블이 표시됩니다.

![구성된 대상을 표시하는 대상 탭입니다.](/help/assets/destinations/manage-destinations/configured-destinations-list.png)

## 대상 삭제 {#delete-destination}

대상 활성화에 더 이상 필요하지 않은 대상을 삭제합니다. 대상을 삭제하면 대상 인벤토리에서 대상이 제거되고 나중에 대상이 활성화되지 않습니다.

>[!IMPORTANT]
>
>대상을 삭제해도 이전에 대상으로 내보낸 대상 데이터는 제거되지 않습니다. 이전에 내보낸 데이터를 대상 데이터 저장소에서 직접 제거합니다.

**[!UICONTROL 활성화]** > **[!UICONTROL 대상]**(으)로 이동합니다.

제거할 대상을 찾고 **[!UICONTROL 작업]** 열에서 줄임표 아이콘을 선택한 다음 **[!UICONTROL 삭제]**&#x200B;를 선택합니다.

![줄임표 아이콘과 삭제 작업이 강조 표시된 활성화 작업 영역의 대상 탭입니다.](/help/assets/destinations/manage-destinations/delete-configured-destination.png)

확인 대화 상자가 나타납니다. 제거할 대상을 검토한 다음 **[!UICONTROL 삭제]**&#x200B;를 선택하여 확인하십시오.

대상이 대상 인벤토리에서 제거되어 더 이상 대상 활성화에 사용할 수 없습니다.

## 다음 단계 {#next-steps}

대상을 구성하고 나면 프로젝트 내에서 [대상 활성화](../collaborate/activate.md)를 시작할 수 있습니다.
