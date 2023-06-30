---
title: Adobe Analytics 계측 키트를 사용하여 뷰어 계측
description: Adobe Dynamic Media Classic의 Adobe Analytics Instrumentation Kit를 사용하여 뷰어를 계측하는 방법에 대해 알아봅니다.
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: a2824244-1755-42de-a167-42af117cf038
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
topic: Integrations, Development
level: Experienced
source-git-commit: 5d8b7cb8b4616a998346675d7324b568634698fb
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 20%

---

# Adobe Analytics 계측 키트를 사용하여 뷰어 계측{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Adobe Analytics Instrumentation Kit를 사용하여 HTML5 뷰어와 Adobe Analytics을 통합할 수 있습니다.

사전 정의된 Adobe Dynamic Media Classic HTML5 뷰어 사전 설정을 사용하는 경우, Adobe Analytics으로 데이터를 전송하기 위한 모든 구현 코드가 이미 포함되어 있으므로 추가적인 계측이 필요하지 않습니다.

## Adobe Dynamic Media Classic에서 Adobe Analytics 추적 설정 {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

모든 HTML 5 뷰어에 대해 다음 JavaScript를 HTML 컨테이너에 추가합니다(일반적으로 &lt;head> 요소:

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Adobe Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

위치 `Adobe Dynamic Media Classic Company ID` Adobe Dynamic Media Classic 회사 이름으로 설정되어 있습니다. 및 `&preset` 회사 사전 설정 이름이 이 아닌 경우 선택 사항입니다. `companypreset`. 이러한 경우 다음과 같을 수 있습니다. `companypreset-1, companypreset-2`등. 숫자가 클수록 사전 설정의 최신 인스턴스입니다. 올바른 회사 사전 설정 값 이름을 결정하려면 다음을 선택합니다. **[!UICONTROL URL 복사]** 을(를) 찾은 다음 `preset=`매개 변수를 사용하여 회사 사전 설정 이름을 찾을 수 있습니다.

계속해서 이제 Adobe Analytics 추적 코드에 뷰어 이벤트를 전송하는 함수를 추가합니다.

추가 `s7ComponentEvent()` 컨테이너 HTML(또는 JSP, ASPX 또는 기타)에 대한 함수:

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

함수 이름은 대소문자를 구분합니다. 에 전달된 유일한 매개 변수 `s7componentEvent`필수 은(는) 마지막 입니다. `eventData`. 위치 `s7track()` 는 위에 포함된 s_code.jsp에 정의되어 있습니다. 및 `s7track` 는 각 이벤트당 모든 추적을 처리합니다. Adobe Analytics로 전송되는 데이터를 추가로 사용자 지정하려면 이 영역에서 수행합니다.

## HREF 및 항목 이벤트 활성화 {#enabling-href-and-item-events}

이미지 맵 편집을 통해 뷰어에서 HREF(롤오버) 및 ITEM(마우스 클릭/터치) 이벤트를 활성화할 수 있습니다. 뷰어 컨텐츠와 연결된 이미지 맵 내에서 HREF 및 ITEM의 식별자를 정의합니다. 추가 `&rolloverKey=` 매개 변수를 이미지 맵 내의 HREF 값에 추가합니다.
