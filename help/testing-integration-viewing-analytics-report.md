---
title: Adobe Analytics 보고서를 보고 통합 테스트
seo-title: Adobe Analytics 보고서를 보고 통합 테스트
description: 널
seo-description: Adobe Analytics 보고서를 보고 통합을 테스트하는 방법을 알아봅니다.
uuid: 937375 e 0-6 dea -4 baa-a 2 b 0-4 f 3 e 461 c 9 ee 2
contentOwner: 관리
content-type: 참조
products: sg_ Experiencemanager/dynamic-media-scene -7
geptopics: sg_ Scenesevenondemand_ PK/categories/adobe_ analytics_ instrumentation_ kit
discoiquuid: 1 DDC 89 FF-D 2 E 9-42 EB-A 442-AA 6 B 9871 C 991
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Adobe Analytics 보고서를 보고 통합 테스트{#testing-the-integration-by-viewing-an-adobe-analytics-report}

Adobe Analytics에서 필요한 변수를 만들어 Dynamic Media Classic 이벤트에 연결하고 필요한 구현 단계를 완료한 후 설정을 테스트해야 합니다. Adobe Analytics 자체 내에서 데이터가 캡처되고 있는지 테스트하고 확인할 수 있습니다. 여기에서 설정이 작동하는 경우, 추가 단계가 필요하지 않습니다. 위 단계를 따른 경우를 가정하고 Dynamic Media Classic 이벤트 데이터를 하나 이상의 사용자 지정 트래픽 변수에 연결한 경우를 가정할 경우, 이 워크플로에 따라 Adobe Analytics 내에서 데이터를 테스트하십시오.

**Adobe Analytics 보고서를 보고 통합을 테스트하려면**

1. 계정, 특히 캡처할 지표를 브로드캐스트하는 계정 중에서 Dynamic Media Classic 뷰어를 실행하고 해당 뷰어를 사용하여 일부 이벤트 데이터를 만듭니다.

   예를 들어 이미지 집합에서 가장 인기 있는 대체 보기를 측정하려는 경우 이미지 집합을 미리 보고 다른 썸네일 이미지를 클릭합니다.

1. Inside Adobe Analytics, go to Custom Traffic &gt; Custom Traffic 1-10 &gt; [Name of prop], selecting your traffic prop name from the menu choices.

   예를 들어, 샘플 계정으로 LoadAsset Prop에 액세스하려는 경우 적절한 메뉴 선택 항목은 [사용자 지정 트래픽] &gt; [사용자 지정 트래픽 1-10] &gt; [LoadAsset]입니다. 11개 이상의 사용자 지정 Prop이 있는 경우 메뉴 선택 항목도 추가로 표시될 수 있습니다.

1. Adobe Analytics에 의해 생성된 차트를 봅니다. 일반적으로 단일 지표에 대한 데이터일 뿐입니다. 이 데이터가 어떤 자산이 연관되어 있는지 알고 싶을 경우 (예: 50%만 시청하거나 세트의 이미지가 가장 인기 있는 자산) 이 이벤트의 자산 데이터도 캡처해야 합니다.

>[!NOTE]
>
>모든 Dynamic Media Classic 뷰어 데이터는 Adobe Analytics의 사용자 지정 트래픽 보고서나 사용자 지정 전환 보고서에 표시되고 보고됩니다.

자세한 내용은 [www.adobe.com/go/learn_sc7_sitecatalystguide_en](https://www.adobe.com/go/learn_sc7_sitecatalystguide_en)를 참조하십시오.
