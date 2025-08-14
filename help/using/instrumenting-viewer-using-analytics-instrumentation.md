---
title: Adobe Analytics 계측 키트를 사용하여 뷰어 계측
description: Adobe Dynamic Media Classic의 Adobe Analytics Instrumentation Kit를 사용하여 뷰어를 계측하는 방법에 대해 알아봅니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
topic: Integrations, Development
level: Experienced
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 15%

---

# Adobe Analytics 계측 키트를 사용하여 뷰어 계측{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Adobe Analytics Instrumentation Kit를 사용하여 HTML5 뷰어와 Adobe Analytics을 통합할 수 있습니다.

사전 정의된 Adobe Dynamic Media Classic HTML5 뷰어 사전 설정을 사용하는 경우 Adobe Analytics으로 데이터를 전송하기 위한 모든 구현 코드가 이미 포함되어 있습니다. 추가적인 계기는 추가할 필요가 없습니다.

## Adobe Dynamic Media Classic에서 Adobe Analytics 추적 설정 {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

모든 HTML5 뷰어에 대해 일반적으로 &lt;head> 요소의 HTML 컨테이너에 다음 JavaScript을 추가합니다.

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Adobe Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

`Adobe Dynamic Media Classic Company ID`이(가) Adobe Dynamic Media Classic 회사 이름으로 설정된 경우. `&preset`은(는) 선택 사항입니다. 회사 사전 설정 이름이 `companypreset`이(가) 아닌 경우 이 이름은 선택 사항이 아닙니다. 이러한 경우 `companypreset-1, companypreset-2`이(가) 될 수 있습니다. 숫자가 클수록 사전 설정의 최신 인스턴스입니다. 올바른 회사 사전 설정 값 이름을 확인하려면 **[!UICONTROL URL 복사]**&#x200B;를 선택한 다음 `preset=`매개 변수를 확인하여 회사 사전 설정 이름을 찾으십시오.

계속해서 이제 Adobe Analytics 추적 코드에 뷰어 이벤트를 전송하는 함수를 추가합니다.

`s7ComponentEvent()` 함수를 컨테이너 HTML(또는 JSP, ASPX 또는 기타)에 추가합니다.

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

함수 이름은 대소문자를 구분합니다. 필요한 `s7componentEvent`에 전달된 유일한 매개 변수는 마지막 매개 변수입니다. `eventData`. `s7track()`이(가) 위에 포함된 s_code.jsp에 정의되어 있습니다. `s7track`은(는) 각 이벤트당 모든 추적을 처리합니다. (이 영역에서는 Adobe Analytics에 전송되는 데이터를 추가로 사용자 지정할 수 있습니다.)

## HREF 및 항목 이벤트 활성화 {#enabling-href-and-item-events}

이미지 맵 편집을 통해 뷰어에서 HREF(롤오버) 및 ITEM(마우스 클릭/터치) 이벤트를 활성화할 수 있습니다. 뷰어 컨텐츠와 연결된 이미지 맵 내에서 HREF 및 ITEM의 식별자를 정의합니다. 이미지 맵 내의 HREF 값에 `&rolloverKey=` 매개 변수를 추가합니다.
