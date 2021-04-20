---
title: Adobe Analytics 비디오 보고서 활성화
description: Adobe Analytics 비디오 보고서를 활성화하는 방법을 알아봅니다.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
translation-type: tm+mt
source-git-commit: 3def4a02eda8dc36f2811b3d4f0e870fff1994e4
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 16%

---


# Adobe Analytics 비디오 보고서 활성화{#enabling-adobe-analytics-video-reports}

Dynamic Media Classic에서 Adobe Analytics을 구성할 때 Adobe Analytics 하트비트 기반 비디오 보고를 사용하면 4개의 비디오 뷰어 이벤트(재생, 일시 중지, 중지, 마일스톤)를 더 이상 활성화할 수 없습니다. 비디오 하트비트는 즉시 사용 가능한 Dynamic Media Classic HTML5 비디오 및 혼합 미디어 뷰어에서 작동합니다. 비디오 플레이어는 Adobe Analytics 비디오 보고서 내에서 보기 위한 추적 데이터를 생성합니다.

* 스트리밍 미디어 및 &#39;하트비트 측정&#39;에 대한 소개는 [스트리밍 미디어용 Adobe Analytics 정보](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html#about-adobe-analytics-for-streaming-media)를 참조하십시오.

* Adobe Analytics 비디오 보고서와 Dynamic Media Classic의 통합은 솔루션 변수를 지원하지만 사용자 지정 변수는 지원하지 않습니다.

   솔루션 변수 및 사용자 지정 변수에 대한 자세한 내용은 [오디오 및 비디오 매개 변수](https://experienceleague.adobe.com/docs/media-analytics/using/metrics-and-metadata/audio-video-parameters.html#metrics-and-metadata)를 참조하십시오.

* 즉시 사용 가능한 1분 단위의 세그먼트가 지원됩니다. 그러나 시간 증분을 기반으로 고객이 정의한 중대한 이벤트, % 중대한 이벤트 또는 오프셋 중대한 이벤트와 같은 사용자 지정 세그먼트 보고는 지원되지 않습니다.

   스트리밍 미디어 요구 사항 및 설정에 대한 자세한 내용은 Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html)에서 [스트리밍 미디어 측정을 참조하십시오.

* 사용자 지정 및 솔루션 변수에 대한 자세한 내용은 [미디어 보고서 지원](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports)을 참조하십시오.

>[!NOTE]
>
>Adobe Analytics의 라이센스 솔루션에 비디오 하트비트가 포함되어 있지 않으면 이 장에 설명된 절차를 계속 사용하여 Adobe Analytics 변수를 Dynamic Media Classic 뷰어 이벤트 및 변수에 할당해야 합니다.

