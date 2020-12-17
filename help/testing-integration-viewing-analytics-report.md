---
title: Adobe Analytics 보고서를 보고 통합 테스트
seo-title: Adobe Analytics 보고서를 보고 통합 테스트
description: 널
seo-description: Adobe Analytics 보고서를 보고 통합을 테스트하는 방법을 알아봅니다.
uuid: 937375e0-6dea-4baa-a2b0-4f3e461c9ee2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 1ddc89ff-d2e9-42eb-a442-aa6b9871c991
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 42%

---


# Adobe Analytics 보고서를 보고 통합 테스트{#testing-the-integration-by-viewing-an-adobe-analytics-report}

Adobe Analytics에서 필요한 변수를 만든 후 Dynamic Media Classic 이벤트에 연결하고 필요한 구현 단계를 완료한 후 설정을 테스트해야 합니다. Adobe Analytics 자체 내에서 데이터가 캡처되고 있는지 테스트하고 확인할 수 있습니다. 여기에서 설정이 작동하는 경우, 추가 단계가 필요하지 않습니다. 위의 단계를 따르고 Dynamic Media Classic 이벤트 데이터를 하나 이상의 사용자 지정 트래픽 변수에 연결했다고 가정하고, 이 워크플로에 따라 Adobe Analytics 내에서 데이터를 테스트합니다.

**Adobe Analytics 보고서를 보고 통합을 테스트하려면**

1. 캡처할 지표를 브로드캐스트하고 이 지표와 상호 작용하여 일부 이벤트 데이터를 만드는 계정, 특히 계정에서 Dynamic Media Classic 뷰어를 시작합니다.

   예를 들어 이미지 집합에서 가장 인기 있는 대체 보기를 측정하려는 경우 이미지 집합을 미리 보고 다른 썸네일 이미지를 클릭합니다.

1. Adobe Analytics 내에서 사용자 지정 트래픽 > 사용자 지정 트래픽 1-10 > [prop]의 이름으로 이동하여 메뉴 선택 사항에서 트래픽 prop 이름을 선택합니다.

   예를 들어, 샘플 계정으로 LoadAsset Prop에 액세스하려는 경우 적절한 메뉴 선택 항목은 [사용자 지정 트래픽] > [사용자 지정 트래픽 1-10] > [LoadAsset]입니다. 11개 이상의 사용자 지정 Prop이 있는 경우 메뉴 선택 항목도 추가로 표시될 수 있습니다.

1. Adobe Analytics에 의해 생성된 차트를 봅니다. 일반적으로 단일 지표에 대한 데이터일 뿐입니다. 이 데이터가 연결되어 있는 에셋과 관련하여 알고 싶은 경우(예: 50%만 시청하는 비디오나 세트의 이미지가 가장 인기 있는 항목) 이 이벤트의 에셋 데이터도 캡처해야 합니다.

>[!NOTE]
>
>모든 Dynamic Media Classic 뷰어 데이터는 Adobe Analytics의 사용자 지정 트래픽 보고서 또는 사용자 지정 전환 보고서에 표시되고 보고됩니다.

자세한 내용은 [www.adobe.com/go/learn_sc7_sitecatalystguide_en](https://www.adobe.com/go/learn_sc7_sitecatalystguide_en)을 참조하십시오.
