---
title: Adobe Analytics Instrumentation Kit을 사용하여 뷰어 계기
description: Adobe Dynamic Media Classic에서 Adobe Analytics Instrumentation Kit을 사용하여 뷰어를 구현하는 방법을 알아봅니다.
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: a2824244-1755-42de-a167-42af117cf038
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 20%

---

# Adobe Analytics Instrumentation Kit을 사용하여 뷰어 계기{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Adobe Analytics 계측 키트 를 사용하여 HTML5 뷰어를 Adobe Analytics과 통합할 수 있습니다.

사전 정의된 Adobe Dynamic Media Classic HTML5 뷰어 사전 설정을 사용하는 경우 Adobe Analytics에 데이터를 보내기 위한 모든 구현 코드가 이미 포함되어 있습니다. 추가 계측은 필요하지 않습니다.

## Adobe Dynamic Media Classic에서 Adobe Analytics 추적 설정 {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

모든 HTML5 뷰어의 경우, 일반적으로 &lt;head> 요소와 같은 HTML 컨테이너에 다음 JavaScript를 추가합니다.

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Adobe Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

여기서 `Adobe Dynamic Media Classic Company ID`은 Adobe Dynamic Media Classic 회사 이름으로 설정됩니다. 그리고 회사 사전 설정 이름이 `companypreset`이 아닌 한 `&preset`은 선택 사항입니다. 이러한 경우 `companypreset-1, companypreset-2` 등이 될 수 있습니다. 숫자가 클수록 사전 설정의 최신 인스턴스입니다. 올바른 회사 사전 설정 값 이름을 확인하려면 **[!UICONTROL URL 복사]** 를 선택한 다음 `preset=`매개 변수를 확인하여 회사 사전 설정 이름을 찾으십시오.

계속하십시오. 이제 뷰어 이벤트를 Adobe Analytics 추적 코드에 전송하는 함수를 추가합니다.

`s7ComponentEvent()` 함수를 컨테이너 HTML(또는 JSP, ASPX 또는 기타)에 추가합니다.

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

함수 이름은 대/소문자를 구분합니다. `s7componentEvent`에 전달되는 유일한 매개 변수는 마지막 매개 변수입니다. `eventData`. 여기서 `s7track()`은 위에 포함된 s_code.jsp에서 정의됩니다. 및 `s7track` 은 각 이벤트마다 모든 추적을 처리합니다. Adobe Analytics로 전송되는 데이터를 추가로 사용자 지정하려면 이 영역에서 수행합니다.

## HREF 및 ITEM 이벤트 활성화 {#enabling-href-and-item-events}

이미지 맵 편집을 통해 뷰어에서 HREF(롤오버) 및 ITEM(마우스 클릭/터치) 이벤트를 활성화할 수 있습니다. 뷰어 컨텐츠와 연결된 이미지 맵 내에서 HREF 및 ITEM의 식별자를 정의합니다. 이미지 맵 내의 HREF 값에 `&rolloverKey=` 매개 변수를 추가합니다.
