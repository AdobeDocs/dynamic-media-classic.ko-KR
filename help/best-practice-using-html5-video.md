---
title: '"우수 사례: HTML5 비디오 뷰어 사용"'
seo-title: '"우수 사례: HTML5 비디오 뷰어 사용"'
description: 널
seo-description: HTML5 비디오 뷰어 사용에 대한 우수 사례에 대해 알아봅니다.
uuid: 3c8924dc-7bea-4c25-b77b-005f57b71b64
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 4b11cab7-88cf-42dd-8554-2eea530753bb
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 30%

---


# 우수 사례: HTML5 비디오 뷰어 사용{#best-practice-using-the-html-video-viewer}

Dynamic Media Classic HTML5 비디오 뷰어 사전 설정은 강력한 비디오 플레이어입니다. 플레이어의 디자인 측면에서는 표준 웹 개발 도구를 사용하여 모든 비디오 플레이어의 기능을 만들 수 있습니다. 예를 들어 HTML5 및 CSS를 사용하여 단추, 컨트롤 및 사용자 지정 포스터 이미지 배경을 디자인하면 사용자 지정된 모습으로 고객 범위를 넓힐 수 있습니다.

뷰어의 재생 측면에서 브라우저의 비디오 기능을 자동으로 검색합니다. 그런 다음 HLS(응용 비디오 스트리밍)를 사용하여 비디오를 제공합니다. 또는 배달 방법이 없으면 HTML5 점진적 기능이 대신 사용됩니다.

HTML5 및 CSS를 사용하여 재생 구성 요소를 디자인하고 포함 재생을 제공하며 브라우저의 기능에 따라 응용 및 점진적 스트리밍을 사용하는 기능을 단일 플레이어에 결합하여 리치 미디어 컨텐츠의 범위를 데스크톱 및 모바일 사용자로 확장하고 스트리밍된 비디오 환경을 보장할 수 있습니다.

Adobe 뷰어 [참조 안내서에서](https://docs.adobe.com/content/help/en/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html) HTML5 뷰어 정보를 참조하십시오.

## Dynamic Media Classic 비디오 뷰어를 사용하여 데스크탑 컴퓨터 및 모바일 장치에서 비디오 재생 {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

데스크탑 및 모바일 적응형 비디오 스트리밍의 경우 비트 전송률 전환에 사용되는 비디오는 적응형 비디오 세트의 모든 MP4 비디오를 기반으로 합니다.

HLS 또는 점진적 비디오를 사용하여 비디오를 재생할 수 있습니다. HLS(HTTP Live Streaming)는 네트워크 대역폭 용량에 따라 재생을 자동으로 조정하는 응용 비디오 스트리밍을 위한 Apple 표준입니다. 또한 고객이 나머지 비디오의 다운로드를 기다릴 필요 없이 비디오의 모든 부분을 &quot;검색&quot;할 수 있습니다. HTTP [Live 스트리밍을 참조하십시오](https://developer.apple.com/streaming/). 점진적 비디오는 비디오를 로컬로 다운로드 및 저장하여 사용자의 데스크탑 화면 또는 모바일 디바이스에 전달됩니다.

다음 표에서는 Dynamic Media Classic 비디오 뷰어를 사용하는 데스크톱 컴퓨터와 모바일 장치에서 비디오의 장치, 브라우저 및 재생 방법에 대해 설명합니다.

| 장치 | 브라우저 | 비디오 재생 모드 |
|--- |--- |--- |
| 데스크탑 | Internet Explorer 9 및 10 | 점진적 다운로드 |
| 데스크톱 | Internet Explorer 11+ | HLS 비디오 스트리밍 |
| 데스크톱 | Firefox 23-44 | 점진적 다운로드 |
| 데스크톱 | Firefox 45 이상 | HLS 비디오 스트리밍 |
| 데스크톱 | 크롬 | HLS 비디오 스트리밍 |
| 데스크톱 | Safari(Mac) | HLS 비디오 스트리밍 |
| 모바일 | Chrome(Android 6 또는 이전 버전) | 점진적 다운로드 |
| 모바일 | Chrome(Android 7 이상) | HLS 비디오 스트리밍 |
| 모바일 | Android(기본 브라우저) | 점진적 다운로드 |
| 모바일 | Safari(iOS) | HLS 비디오 스트리밍 |
| 모바일 | Chrome(iOS) | HLS 비디오 스트리밍 |
| 모바일 | Blackberry | HLS 비디오 스트리밍 |
