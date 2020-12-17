---
title: Adobe Analytics 계측 키트를 사용하여 뷰어 계측
seo-title: Adobe Analytics 계측 키트를 사용하여 뷰어 계측
description: 널
seo-description: Adobe Analytics Instrumentation Kit를 사용하여 뷰어를 계수하는 방법을 알아봅니다.
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: a2824244-1755-42de-a167-42af117cf038
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 38%

---


# Adobe Analytics 계측 키트를 사용하여 뷰어 계측{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Adobe Analytics 계측 키트를 사용하여 HTML5 뷰어를 Adobe Analytics과 통합할 수 있습니다.

사전 정의된 Dynamic Media Classic HTML5 뷰어 사전 설정을 사용하는 경우 데이터를 Adobe Analytics으로 전송하는 데 필요한 모든 구현 코드가 이미 포함되어 있으므로 추가 계측을 수행할 필요가 없습니다.

## Dynamic Media Classic {#set-up-adobe-analytics-tracking-from-scene-publishing-system}에서 Adobe Analytics 추적 설정

모든 HTML5 뷰어의 경우 HTML 컨테이너에 일반적으로 &lt;head> 요소에 다음 JavaScript를 추가합니다.

```as3
<!-- ***** Site Catalyst Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

`Company` 은 Dynamic Media Classic 회사 이름으로 설정됩니다. `&preset` 회사 사전 설정 이름이 아닐 경우 선택 사항입니다 `companypreset`. 이러한 경우 `companypreset-1, companypreset-2` 등이 될 수 있습니다. 숫자가 클수록 사전 설정의 최신 인스턴스입니다. 올바른 회사 사전 설정 값 이름을 확인하려면 **URL 복사** 를 클릭한 다음 `preset=` 매개 변수를 확인하여 회사 사전 설정 이름을 찾습니다.

이제 Adobe Analytics 추적 코드에 뷰어 이벤트를 전송하는 함수를 추가합니다.

`s7ComponentEvent()` 함수를 컨테이너 HTML(또는 JSP, ASPX 또는 기타)에 추가합니다.

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

함수 이름은 대/소문자를 구분합니다. `s7componentEvent`에 전달되는 유일한 매개 변수는 마지막 매개 변수입니다.`eventData`. `s7track()` 은 위에 포함된 s_code.jsp에 정의됩니다. `s7track` 각 이벤트당 모든 추적을 처리합니다. Adobe Analytics로 전송되는 데이터를 추가로 사용자 지정하려면 이 영역에서 수행합니다.

## HREF 및 ITEM 이벤트 활성화 {#enabling-href-and-item-events}

이미지 맵 편집을 통해 뷰어에서 HREF(롤오버) 및 ITEM(마우스 클릭/터치) 이벤트를 활성화할 수 있습니다. 뷰어 컨텐츠와 연결된 이미지 맵 내에서 HREF 및 ITEM의 식별자를 정의합니다. 이미지 맵 내의 HREF 값에 `&rolloverKey=` 매개 변수를 추가합니다.
