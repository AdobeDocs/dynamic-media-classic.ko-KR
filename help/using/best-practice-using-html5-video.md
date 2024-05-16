---
title: HTML5 비디오 뷰어 사용에 대한 우수 사례
description: HTML5 비디오 뷰어 사용에 대한 모범 사례에 대해 알아봅니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: ce49e4ce-8dc0-41e1-865a-249f23757553
topic: Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 10%

---

# HTML5 비디오 뷰어 사용에 대한 우수 사례{#best-practice-using-the-html-video-viewer}

Adobe Dynamic Media Classic HTML5 비디오 뷰어 사전 설정은 강력한 비디오 플레이어입니다. 플레이어의 디자인 측면에서는 표준 웹 개발 도구를 사용하여 비디오 플레이어의 전체 기능을 만들 수 있습니다. 예를 들어 HTML5 및 CSS를 사용하여 단추, 컨트롤 및 사용자 지정 포스터 이미지 배경을 디자인하면 사용자 지정된 모습으로 고객 범위를 넓힐 수 있습니다.

뷰어의 재생 측에서는 브라우저의 비디오 기능을 자동으로 감지합니다. 그런 다음 적응형 비디오 스트리밍이라고도 하는 HLS(HTTP 라이브 스트리밍)를 사용하여 비디오를 제공합니다. 또는 해당 전달 방법이 없으면 대신 HTML5 progressive가 사용됩니다.

단일 플레이어로 결합하여 다음과 같은 기능을 제공합니다.

* HTML5 및 CSS를 사용하여 디자인된 재생 구성 요소
* 포함된 재생
* 브라우저의 기능을 기반으로 하는 적응형 및 점진적 스트리밍 사용

리치 미디어 콘텐츠의 범위를 데스크탑 및 모바일 사용자까지 확장할 수 있습니다. 또한 간소화된 비디오 환경을 보장합니다.

참조: [HTML5 뷰어 정보](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers#viewers-for-aem-assets-only) ( Adobe 뷰어 참조 안내서)를 참조하십시오.

참조: [뷰어 사전 설정](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) 교육 비디오입니다.

## Adobe Dynamic Media Classic 비디오 뷰어를 사용하여 데스크탑 컴퓨터 및 모바일 장치에서 비디오 재생 {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

데스크탑 및 모바일 응용 비디오 스트리밍의 경우, 비트 전송률 전환에 사용되는 비디오는 응용 비디오 세트의 모든 MP4 비디오를 기반으로 합니다.

비디오 재생은 HLS 또는 점진적 비디오를 사용하여 발생합니다. HLS(HTTP 라이브 스트리밍)는 네트워크 대역폭 용량에 따라 자동으로 재생을 조정하는 적응형 비디오 스트리밍을 위한 Apple 표준입니다. 또한 고객이 나머지 비디오가 다운로드될 때까지 기다릴 필요 없이 비디오의 어느 지점으로든 &quot;검색&quot;할 수 있습니다. 참조: [HTTP 라이브 스트리밍](https://developer.apple.com/streaming/). 점진적 비디오는 사용자의 데스크탑 스크린 또는 모바일 디바이스에 비디오를 다운로드하고 로컬로 저장함으로써 전달된다.

다음 표에서는 Adobe Dynamic Media Classic 비디오 뷰어를 사용하는 데스크탑 컴퓨터 및 모바일 장치에서 비디오의 장치, 브라우저 및 재생 방법에 대해 설명합니다.

| 장치 | 브라우저 | 비디오 재생 모드 |
|--- |--- |--- |
| 데스크톱 | Internet Explorer 9 및 10 | 점진적 다운로드. |
| 데스크톱 | Internet Explorer 11+ | HLS 비디오 스트리밍. |
| 데스크톱 | Firefox 23-44 | 점진적 다운로드. |
| 데스크톱 | Firefox 45 이상 | HLS 비디오 스트리밍. |
| 데스크톱 | 크롬 | HLS 비디오 스트리밍. |
| 데스크톱 | Safari(Mac) | HLS 비디오 스트리밍. |
| 모바일 | Chrome(Android™ 6 이하) | 점진적 다운로드. |
| 모바일 | Chrome(Android™ 7 이상) | HLS 비디오 스트리밍. |
| 모바일 | Android™ (기본 브라우저) | 점진적 다운로드. |
| 모바일 | Safari(iOS) | HLS 비디오 스트리밍. |
| 모바일 | Chrome(iOS) | HLS 비디오 스트리밍. |
| 모바일 | 블랙베리® | HLS 비디오 스트리밍. |
