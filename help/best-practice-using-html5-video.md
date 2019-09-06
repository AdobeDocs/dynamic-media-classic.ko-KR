---
title: '"우수 사례: HTML5 비디오 뷰어 사용"'
seo-title: '"우수 사례: HTML5 비디오 뷰어 사용"'
description: 널
seo-description: HTML 5 비디오 뷰어 사용에 대한 우수 사례에 대해 알아봅니다.
uuid: 3 c 8924 dc -7 bea -4 c 25-b 77 b -005 f 57 b 71 b 64
contentOwner: 관리
content-type: 참조
products: sg_ Experiencemanager/dynamic-media-scene -7
geptopics: sg_ scenesevenondemand_ pk/categories/video
discoiquuid: 4 B 11 CAB 7-88 CF -42 DD -8554-2 EEA 530753 BB
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# 우수 사례: HTML5 비디오 뷰어 사용{#best-practice-using-the-html-video-viewer}

Dynamic Media Classic HTML 5 비디오 뷰어 사전 설정은 강력한 비디오 플레이어입니다. 플레이어의 디자인 측면에서 표준 웹 개발 도구를 사용하여 모든 비디오 플레이어의 기능을 만들 수 있습니다. 예를 들어 HTML5 및 CSS를 사용하여 단추, 컨트롤 및 사용자 지정 포스터 이미지 배경을 디자인하면 사용자 지정된 모습으로 고객 범위를 넓힐 수 있습니다.

뷰어의 재생 측면에서 브라우저의 비디오 기능을 자동으로 검색합니다. 그런 다음 HLS (Adaptive Video Streaming) 를 사용하여 비디오를 제공합니다. 또는 해당 배달 방법이 없으면 HTML 5 점진적 대신 사용됩니다.

HTML5 및 CSS를 사용하여 재생 구성 요소를 디자인하고 포함 재생을 제공하며 브라우저의 기능에 따라 응용 및 점진적 스트리밍을 사용하는 기능을 단일 플레이어에 결합하여 리치 미디어 컨텐츠의 범위를 데스크톱 및 모바일 사용자로 확장하고 스트리밍된 비디오 환경을 보장할 수 있습니다.

Adobe 뷰어 [참조](https://marketing.adobe.com/resources/help/en_US/s7/viewers_ref/c_html5_viewers_about.html) 안내서의 HTML 5 뷰어 정보를 참조하십시오.

## Dynamic Media Classic Video Viewer를 사용하여 데스크톱 컴퓨터 및 모바일 장치에서 비디오 재생 {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

데스크톱 및 모바일 응용 비디오 스트리밍의 경우, 비트 속도 전환에 사용되는 비디오는 응용 비디오 집합의 모든 MP 4 비디오를 기반으로 합니다.

HLS 또는 점진적 비디오를 사용하여 비디오 재생을 수행할 수 있습니다. HLS (HTTP Live Streaming) 는 네트워크 대역폭 용량에 따라 재생을 자동으로 조정하는 적응형 비디오 스트리밍을 위한 Apple 표준입니다. 또한 비디오의 나머지 부분이 다운로드될 때까지 기다릴 필요 없이 비디오의 모든 부분에 "검색" 할 수 있습니다 ( [HTTP Live 스트리밍](#UnresolvedLink-https://developer.apple.com/streaming/)참조). 비디오를 다운로드하여 사용자의 데스크탑 화면 또는 모바일 디바이스에 저장하여 점진적 비디오를 제공할 수 있습니다.

다음 표에서는 Dynamic Media Classic 비디오 뷰어를 사용하는 데스크톱 컴퓨터 및 모바일 장치에서 장치의 장치, 브라우저 및 재생 방법에 대해 설명합니다.

| 장치 | 브라우저 | 비디오 재생 모드 |
|--- |--- |--- |
| Deskop | Internet Explorer 9 및 10 | 점진적 다운로드. |
| 데스크톱 | Internet Explorer 11 + | HLS 비디오 스트리밍. |
| 데스크톱 | Firefox 23-44 | 점진적 다운로드. |
| 데스크톱 | Firefox 45 이상 | HLS 비디오 스트리밍. |
| 데스크톱 | Chrome | HLS 비디오 스트리밍. |
| 데스크톱 | Safari (Mac) | HLS 비디오 스트리밍. |
| 모바일 | Chrome (Android 6 또는 이전 버전) | 점진적 다운로드. |
| 모바일 | Chrome (Android 7 이상) | HLS 비디오 스트리밍. |
| 모바일 | Android (기본 브라우저) | 점진적 다운로드. |
| 모바일 | Safari (iOS) | HLS 비디오 스트리밍. |
| 모바일 | Chrome (iOS) | HLS 비디오 스트리밍. |
| 모바일 | Blackberry | HLS 비디오 스트리밍. |
