---
title: Adobe Analytics 비디오 보고서 활성화
seo-title: Adobe Analytics 비디오 보고서 활성화
description: 널
seo-description: Adobe Analytics 비디오 보고서를 활성화하는 방법을 알아봅니다.
uuid: 078594b2-7d53-4714-8128-ff3b5c3a5e36
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 18644a53-92da-40ab-b961-318d8332c54d
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 26%

---


# Adobe Analytics 비디오 보고서 활성화{#enabling-adobe-analytics-video-reports}

Adobe Analytics 하트비트 기반 비디오 보고를 사용하면 Dynamic Media Classic에서 Adobe Analytics을 구성할 때 4개의 비디오 뷰어 이벤트(재생, 일시 중지, 중지, 마일스톤)를 더 이상 활성화할 필요가 없습니다. 비디오 하트비트는 즉시 사용 가능한 Dynamic Media Classic HTML5 비디오 및 혼합 미디어 뷰어에서 작동합니다. 비디오 플레이어는 Adobe Analytics 비디오 보고서 내에서 보기 위한 추적 데이터를 생성합니다.

* Adobe Analytics 비디오 보고서와 Dynamic Media Classic의 통합은 솔루션 변수를 지원하지만 사용자 지정 변수는 지원하지 않습니다.

   솔루션 변수 및 사용자 지정 변수에 대한 자세한 내용은 [분석 비디오 보고 구성](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/video_analytics_config.html)을 참조하십시오.

* 1분 간격으로 증분되는 기본 세그먼트가 지원됩니다. 그러나 시간 증분을 기반으로 고객이 정의한 중대한 이벤트, % 중대한 이벤트 또는 오프셋 중대한 이벤트와 같은 사용자 지정 세그먼트 보고는 지원되지 않습니다.

비디오 하트비트 요구 사항 및 설정에 대한 자세한 내용은 비디오 하트비트](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/)를 사용하여 Adobe Analytics에서 비디오 측정을 참조하십시오.[

>[!NOTE]
>
>Adobe Analytics의 라이센스 솔루션에 비디오 하트비트가 포함되어 있지 않으면 이 장에 설명된 절차를 계속 사용하여 Adobe Analytics 변수를 Dynamic Media Classic 뷰어 이벤트 및 변수에 할당해야 합니다.

