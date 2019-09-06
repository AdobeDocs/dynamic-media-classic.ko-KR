---
title: Adobe Analytics 비디오 보고서 활성화
seo-title: Adobe Analytics 비디오 보고서 활성화
description: 널
seo-description: Adobe Analytics 비디오 보고서를 활성화하는 방법을 알아봅니다.
uuid: 078594 B 2-7 D 53-4714-8128-FF 3 B 5 C 3 A 5 E 36
contentOwner: 관리
content-type: 참조
products: sg_ Experiencemanager/dynamic-media-scene -7
geptopics: sg_ Scenesevenondemand_ PK/categories/adobe_ analytics_ instrumentation_ kit
discoiquuid: 18644 a 53-92 DA -40 AB-B 961-318 D 8332 C 54 D
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Adobe Analytics 비디오 보고서 활성화{#enabling-adobe-analytics-video-reports}

Adobe Analytics 하트비트 기반 비디오 보고를 사용하는 경우 Dynamic Media Classic에서 Adobe Analytics를 구성할 때 4 개의 비디오 뷰어 이벤트 (재생, 일시 중지, 중지, 이정표) 를 더 이상 활성화할 필요가 없습니다. 비디오 하트비트는 기본 Dynamic Media Classic HTML 5 비디오 및 mixedmedia 뷰어와 함께 사용할 수 있습니다. 비디오 플레이어는 Adobe Analytics 비디오 보고서 내에서 보기 위한 추적 데이터를 생성합니다.

* Adobe Analytics 비디오 보고서와 Dynamic Media Classic의 통합은 솔루션 변수를 지원하지만 사용자 지정 변수는 지원하지 않습니다.

   See [Configure Analytics Video Reporting](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/video_analytics_config.html) for more information about solution variables and custom variables.

* 1분 간격으로 증분되는 기본 세그먼트가 지원됩니다. 그러나 시간 증분을 기반으로 고객이 정의한 중대한 이벤트, % 중대한 이벤트 또는 오프셋 중대한 이벤트와 같은 사용자 지정 세그먼트 보고는 지원되지 않습니다.

For more information about Video Heartbeat requirements and setup, see [Measuring Video in Adobe Analytics using Video Heartbeat](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/).

>[!NOTE]
>
>Adobe Analytics의 라이센스 솔루션에 비디오 하트비트가 포함되어 있지 않은 경우 이 장에 설명된 단계를 계속 수행하여 Dynamic Media Classic 뷰어 이벤트 및 변수에 Adobe Analytics 변수를 할당해야 합니다.

