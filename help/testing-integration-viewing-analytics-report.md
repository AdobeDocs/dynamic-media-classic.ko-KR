---
title: ' 보고서를 보고 Adobe Analytics 통합 테스트'
description: Adobe Analytics 보고서를 보고 Dynamic Media Classic에서 통합을 테스트하는 방법을 알아봅니다.
uuid: 937375e0-6dea-4baa-a2b0-4f3e461c9ee2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 1ddc89ff-d2e9-42eb-a442-aa6b9871c991
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 6186fcf0-99b4-447d-ae94-b4124dcb405b
source-git-commit: 8bc49ae3704f0551c70d68a0ddd63725bdcc645c
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 15%

---

#  보고서를 보고 Adobe Analytics 통합 테스트{#testing-the-integration-by-viewing-an-adobe-analytics-report}

Adobe Analytics에서 필요한 변수를 만들고 Dynamic Media Classic 이벤트에 연결하며 필요한 구현 단계를 완료하면 설정을 테스트할 수 있습니다. Adobe Analytics 자체 내에서 데이터가 캡처되고 있는지 테스트하고 확인할 수 있습니다. 여기에서 설정이 작동하는 경우, 추가 단계가 필요하지 않습니다. 위의 단계를 수행하고 Dynamic Media Classic 이벤트 데이터를 하나 이상의 사용자 지정 트래픽 변수에 연결했다고 가정할 경우 이 워크플로우에 따라 Adobe Analytics 내에서 데이터를 테스트하십시오.

**Adobe Analytics 보고서를 보고 통합을 테스트하려면**

1. 계정에서 Dynamic Media Classic Adobe 뷰어를 시작합니다. 특히 가져오려는 지표를 브로드캐스트하고 이 뷰어와 상호 작용하여 일부 이벤트 데이터를 만듭니다.

   예를 들어, 이미지 세트에서 자주 사용하는 대체 보기를 측정하려면 이미지 세트를 미리 보고 다른 축소판 이미지를 클릭합니다.

1. Adobe Analytics 내에서 **[!UICONTROL 사용자 지정 트래픽]** > **[!UICONTROL 사용자 지정 트래픽 1-10]** > [속성 이름]으로 이동하여 메뉴 선택 항목에서 트래픽 prop 이름을 선택합니다.

   예를 들어, 샘플 계정에서 **[!UICONTROL LoadAsset]** prop에 액세스하려면 적절한 메뉴 선택이 **[!UICONTROL 사용자 지정 트래픽]** > **[!UICONTROL 사용자 지정 트래픽 1-10]** > **[!UICONTROL LoadAsset]**&#x200B;입니다. 사용자 지정 prop이 10개 이상 있는 경우, 다른 메뉴 선택 사항도 표시됩니다.

1. Adobe Analytics에 의해 생성된 차트를 봅니다. 이 차트는 일반적으로 단일 지표에 대한 데이터입니다. 이 데이터가 연결된 자산도 확인하려면 이 이벤트의 자산 데이터를 가져옵니다. 예를 들어 50%만 시청하는 비디오나 한 세트의 이미지가 인기 있는 이미지를 파악하는 것이 종종 유용합니다.

>[!NOTE]
>
>모든 Adobe Dynamic Media Classic 뷰어 데이터는 Adobe Analytics의 사용자 지정 트래픽 보고서 또는 사용자 지정 전환 보고서에 표시되고 보고됩니다.

자세한 내용은 [Analytics Tutorials](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/overview.html)을 참조하십시오.