---
title: ID 크로스워크
description: 다양한 소스에서 ID 횡단보도를 가져오는 방법 및 ID 횡단보도를 관리하는 방법을 포함하여 Real-Time CDP Collaboration의 ID 횡단보도에 대해 모두 알아봅니다
audience: admin, publisher, advertiser
badgelimitedavailability: label="제한 공개" type="Informative" url="https://helpx.adobe.com/kr/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
hidefromtoc: true
hide: true
exl-id: a51f112d-3da7-4482-a24a-6d9f269d28d1
source-git-commit: dd1386f9371cb40285315d11e07b139d3115e147
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 22%

---

# ID 크로스워크

{{limited-availability-release-note}}

다양한 소스에서 ID 횡단보도를 가져오는 방법 및 ID 횡단보도를 관리하는 방법을 포함하여 Real-Time CDP Collaboration의 ID 횡단보도에 대해 모두 알아봅니다.

ID 횡단보기는 여러 데이터 세트 및 플랫폼에서 고객 ID를 안전하고 개인정보 보호 규정을 준수하는 방식으로 연결할 수 있습니다. Real-Time CDP Collaboration은 해시된 식별자를 활용하여 사용자가 개인 식별 정보(PII)를 노출하지 않고 ID를 동기화하고 조정할 수 있도록 합니다. 이를 통해 통합 뷰를 통해 더 나은 공동 작업 및 타겟팅 마케팅 노력을 위한 고객을 파악할 수 있습니다.

<!--
In Real-Time CDP Collaboration, use identity crosswalks alongside your audiences by [TODO] insert material here. 
-->


첫 번째 단계로 ID 횡단보도를 Real-Time CDP Collaboration으로 가져와야 합니다. ID 횡단보도를 Real-Time CDP Collaboration으로 가져오려면 아래 섹션을 참조하십시오.

>[!NOTE]
>
>Real-Time CDP Collaboration 베타 릴리스에서는 Real-Time CDP의 데이터 세트에서 ID 횡단보도를 가져올 수 있습니다. 추가 옵션은 후속 릴리스에서 사용할 수 있습니다.

## ID 횡단보도를 Real-Time CDP Collaboration으로 가져오기 {#import-crosswalk}

**[!UICONTROL 설정]** > **[!UICONTROL ID 횡단보도]** 탭으로 이동하고 더하기 **+** 기호를 선택한 다음 **[!UICONTROL ID 횡단보도]**&#x200B;를 선택합니다.

![ID 횡단보도를 추가하기 위해 화면으로 이동하는 방법에 대한 기록](/help/assets/setup/identity-crosswalks/import-identity-crosswalk.gif)

### 크로스워크 소스 선택

ID 횡단보도를 가져올 소스를 선택하십시오. Real-Time CDP Collaboration의 첫 번째 릴리스에서는 Experience Platform이 횡단보도 가져오기에 대한 유일한 지원 소스입니다.

>[!TIP]
>
>Platform에서는 Experience Platform에서 가져오는 횡단보도를 *데이터 세트*&#x200B;라고 합니다.

횡단보도의 소스로 Experience Platform을 선택한 후 ID 횡단보도를 가져올 [Experience Platform 샌드박스](https://experienceleague.adobe.com/ko/docs/experience-platform/sandbox/home)를 선택하십시오.

![횡단보도 원본을 선택하는 방법에 대한 기록](/help/assets/setup/identity-crosswalks/select-crosswalk-source.gif)

### 크로스워크 선택

횡단보도의 소스로 Experience Platform을 선택한 후,

### 세부 정보 입력

제품으로 가져오는 ID 횡단보도의 이름과 설명을 입력합니다.

### 조인 키 선택 {#select-join-key}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_crosswalk_join_key"
>title="조인 키"
>abstract="조인 키는 서로 다른 데이터 세트에서 레코드를 일치시키고 연결하는 데 사용되는 고유 식별자입니다. 이를 통해 다양한 소스의 데이터를 동일한 개인이나 단체와 정확하게 연결할 수 있습니다. 선택된 크로스워크의 모든 열 머리글은 조인 키 역할을 할 수 있습니다."

조인 키는 서로 다른 데이터 세트에서 레코드를 일치시키고 연결하는 데 사용되는 고유 식별자입니다. 이를 통해 다양한 소스의 데이터를 동일한 개인이나 단체와 정확하게 연결할 수 있습니다. 적절한 조인 키를 선택하면 데이터를 효과적으로 병합하고 조정할 수 있으므로 캠페인의 정확성과 완성도를 높일 수 있습니다.

선택된 크로스워크의 모든 열 머리글은 조인 키 역할을 할 수 있습니다.

횡단보도 테이블에 대해 원하는 조인 키를 선택하고 **[!UICONTROL 다음]**&#x200B;을(를) 선택하여 다음 단계로 진행합니다.

### 검토

이전 화면에서 선택 항목을 검토합니다. 선택 내용이 만족스러우면 **[!UICONTROL 다음]**&#x200B;을(를) 선택하여 워크플로우를 완료합니다.

## 다음 단계

ID 횡단보도를 Real-Time CDP으로 가져오는 방법을 학습한 후 지금까지 Real-Time CDP Collaboration에 추가한 모든 ID 횡단보도를 볼 수 있습니다. 이제 대상자를 Real-Time CDP Collaboration으로 가져올 때 가져온 ID 횡단보도를 사용할 수도 있습니다.
