---
title: Adobe Analytics 계측 키트를 사용하여 뷰어 계측
seo-title: Adobe Analytics 계측 키트를 사용하여 뷰어 계측
description: 널
seo-description: Adobe Analytics Instrumentation Kit를 사용하여 뷰어를 측정하는 방법을 알아봅니다.
uuid: CF 9 A 4002-966 D -4641-9 CD 0-2 EE 8 B 5454 F 60
contentOwner: 관리
content-type: 참조
products: sg_ Experiencemanager/dynamic-media-scene -7
geptopics: sg_ Scenesevenondemand_ PK/categories/adobe_ analytics_ instrumentation_ kit
discoiquuid: A 2824244-1755-42 de-A 167-42 AF 117 CF 038
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Adobe Analytics 계측 키트를 사용하여 뷰어 계측{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Adobe Analytics Instrumentation Kit를 사용하여 HTML 5 뷰어를 Adobe Analytics와 통합할 수 있습니다.

사전 정의된 Dynamic Media Classic HTML 5 뷰어 사전 설정을 사용하는 경우 Adobe Analytics에 데이터를 보내는 데 필요한 모든 구현 코드가 이미 포함되어 있어야 합니다. —추가 작업은 필요하지 않습니다.

## Scene7 Publishing System에서 Adobe Analytics 추적 설정 {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

모든 HTML 5 뷰어에 대해 HTML 컨테이너에 다음 JavaScript를 추가합니다 (일반적으로 &lt; head &gt; 요소).

```as3
<!-- ***** Site Catalyst Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<SPS Company ID>&preset=companypreset-1"></script>
```

`Company`는 SPS 회사 이름으로 설정됩니다. `&preset` 은 회사 사전 설정 이름이 아닌 `companypreset`경우 선택 사항입니다. `companypreset-1, companypreset-2`이러한 경우, 그럴 수 있습니다. 숫자가 클수록 사전 설정의 최신 인스턴스입니다. To determine the correct company preset value name, click **Copy URL** , and then look at the `preset=`parameter to find the company preset name.

이제 Adobe Analytics 추적 코드에 뷰어 이벤트를 전송하는 함수를 추가합니다.

Add the `s7ComponentEvent()` function to the container HTML (or JSP, or ASPX or other):

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

함수 이름은 대/소문자를 구분합니다. The only parameter passed to `s7componentEvent`that is required is the last one: `eventData`. `s7track()` 에 포함된 s_ code. jsp에 정의되어 있습니다. `s7track` 각 이벤트당 추적을 모두 처리합니다. Adobe Analytics로 전송되는 데이터를 추가로 사용자 지정하려면 이 영역에서 수행합니다.

## HREF 및 ITEM 이벤트 활성화 {#enabling-href-and-item-events}

이미지 맵 편집을 통해 뷰어에서 HREF(롤오버) 및 ITEM(마우스 클릭/터치) 이벤트를 활성화할 수 있습니다. 뷰어 컨텐츠와 연결된 이미지 맵 내에서 HREF 및 ITEM의 식별자를 정의합니다. Add a `&rolloverKey=` parameter to the HREF value within the Image Map.
