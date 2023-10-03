---
title: Adobe Analytics 비디오 보고서 활성화
description: Adobe Dynamic Media Classic에서 Adobe Analytics 비디오 보고서를 활성화하는 방법을 알아봅니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
topic: Development, Integrations
level: Experienced
source-git-commit: 1b90beb99b161b76da81403f5aed9755b3a92c8b
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 5%

---

# Adobe Analytics 비디오 보고서 활성화{#enabling-adobe-analytics-video-reports}

Adobe Analytics 하트비트 기반 비디오 보고를 사용하여 Adobe Dynamic Media Classic에서 Adobe Analytics을 구성할 때 4개의 비디오 뷰어 이벤트(재생, 일시 중지, 중지, 이정표)를 더 이상 활성화하지 않아도 됩니다. 비디오 하트비트는 기본 Adobe Dynamic Media Classic HTML5 비디오 및 혼합 미디어 뷰어와 함께 작동합니다. 비디오 플레이어는 Adobe Analytics 비디오 보고서 내에서 보기 위한 추적 데이터를 생성합니다.

* 스트리밍 미디어 및 &#39;하트비트 측정&#39;에 대한 소개는 다음을 참조하십시오. [適用於串流媒體的 Adobe Analytics 정보](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

* Adobe Analytics 비디오 보고서와 Adobe Dynamic Media Classic의 통합은 솔루션 변수를 지원하지만 사용자 지정 변수는 지원하지 않습니다.

  다음을 참조하십시오 [오디오 및 비디오 매개 변수](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/variables/audio-video-parameters.html) 솔루션 변수 및 사용자 지정 변수에 대한 자세한 정보입니다.

* 1분 단위의 기본 세그먼트가 지원됩니다. 그러나 시간 증분에 따른 고객 정의 이정표, % 이정표 또는 오프셋 이정표와 같은 사용자 정의 세그먼트 보고는 지원되지 않습니다.

  스트리밍 미디어 요구 사항 및 설정에 대한 자세한 내용은 [Adobe Analytics에서 Steaming Media 측정](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

* 사용자 지정 및 솔루션 변수에 대한 자세한 내용은 을 참조하십시오. [미디어 보고서 지원](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports).

>[!NOTE]
>
>사용 허가된 Adobe Analytics 솔루션에 비디오 하트비트가 포함되지 않은 경우 이 장에 설명된 단계를 계속 사용하여 Adobe Analytics 변수를 Adobe Dynamic Media Classic 뷰어 이벤트 및 변수에 지정해야 합니다.
