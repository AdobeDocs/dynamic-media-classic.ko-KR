---
title: 비디오에 장 마커 추가
description: Dynamic Media Classic에서 비디오에 장 마커를 추가하는 방법을 알아봅니다.
uuid: 4e1e6daf-afc6-49d9-ac90-183fe2a903b2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 8bc5e552-2abb-41f0-89d2-bdf3ae5d96c2
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: a9250841-2dba-4fdc-8a6e-91b2fecef72f
source-git-commit: 1d30c98b76ebe78ff60bae87bd112de7a577182d
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 40%

---

# 비디오에 장 마커 추가 {#adding-chapter-markers-to-video}

단일 비디오나 적응형 비디오 집합에 장 마커를 추가하여 장편 비디오를 더 쉽게 보거나 탐색할 수 있습니다. 사용자가 비디오를 재생하면 비디오 타임라인에서 장 마커(비디오 스크러버라고도 함)를 선택할 수 있습니다. 이렇게 하면 관심 영역으로 손쉽게 이동하거나 새로운 컨텐츠, 데모, 자습서 등으로 바로 이동할 수 있습니다.

>[!NOTE]
>
>사용하는 비디오 플레이어가 장 마커 사용을 지원해야 합니다.

`Universal_HTML5_Video` 뷰어에 대한 장 탐색 큐 포인트와 장 제목 팝업 텍스트를 구성하려면 [비디오 뷰어 사전 설정 추가 또는 편집](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset) 을 참조하십시오(HTML5).

또한 [뷰어 사전 설정 추가 및 편집](application-setup.md#adding_and_editing_viewer_presets)을 참조하십시오.

캡션을 만들 때와 마찬가지 방법으로 비디오에 대해 장 목록을 만듭니다. 즉, WebVTT 파일을 만듭니다. 그러나, 이 파일은 사용 중일 수 있는 모든 WebVTT 캡션 파일과는 구별되어야 합니다. 캡션과 장을 하나의 WebVTT 파일로 결합해서는 안 됩니다.

다음을 샘플을 장치 탐색으로 WebVTT 파일을 만드는 데 사용하는 형식의 예로 사용할 수 있습니다.

```as3
WEBVTT 
Chapter 1 
00:00.000 --> 01:04.364 
The bicycle store behind it all. 
Chapter 2 
01:04.364 --> 02:00.944 
Creative Cloud. 
Chapter 3 
02:00.944 --> 03:02.937 
Ease of management for a working solution. 
Chapter 4 
03:02.937 --> 03:35.000 
Cost-efficient access to rapidly evolving technology.
```

위의 예에서 `Chapter 1`은 큐 식별자이며, 선택 사항입니다. `00:00:000 --> 01:04:364`의 큐 시간은 장의 시작 시간과 종료 시간을 00:00:000 형식으로 지정합니다. 마지막 세 개의 숫자는 밀리초이며, 원하는 경우 000으로 둘 수 있습니다. `The bicycle store behind it all`의 장 제목은 장 내용에 대한 실제 설명입니다. 큐 식별자, 시작 큐 시간 및 장 제목이 비디오 타임라인의 시각적 큐 포인트 위에 마우스 포인터를 두면 비디오 플레이어의 팝업에 모두 나타납니다.

HTML5 비디오 뷰어를 사용하고 있으므로, 사용자가 만드는 장 파일이 WebVTT(Web Video Text Tracks) 표준을 준수하도록 해야 합니다. 장 파일 이름 확장명은 .VTT입니다. WebVTT 캡션 표준에 대한 자세한 내용을 알 수 있습니다.

[WebVTT 를 참조하십시오. 웹 비디오 텍스트가 ](https://w3c.github.io/webvtt/) 형식을 추적합니다.

**비디오에 장 마커 추가:**

1. Dynamic Media Classic 외부의 간단한 텍스트 편집기를 사용하여 비디오 장 파일을 만듭니다.

   >[!NOTE]
   >
   >WebVTT 표준에서는 영어 이외의 언어로 비디오 장을 전역 지원하려면 지원할 각 언어에 대해 별도의 .vtt 파일과 호출을 만들어야 합니다.

1. VTT 파일을 UTF8 인코딩으로 저장하면 장 제목 텍스트에서 문자 변환과 관련된 문제가 발생하지 않습니다.

   일반적으로 장 VTT 파일의 이름은 비디오 파일과 동일하게 지정하고 여기에 `chapters`를 추가합니다. 그렇게 하면 기존 웹 컨텐츠 관리 시스템을 사용하여 비디오 URL의 생성을 자동화하는 데 도움이 될 수 있습니다.

1. Dynamic Media Classic에서 WebVTT 장 파일을 업로드합니다.

   [파일 업로드](uploading-files.md#uploading_files)를 참조하십시오.

1. 왼쪽의 [자산 라이브러리] 패널에서 업로드한 장 파일과 연결하려는 비디오 파일이 들어 있는 자산 폴더를 탐색합니다.
1. 자산 찾아보기 패널에서 단일 비디오 자산을 선택한 다음 자산의 축소판 이미지 아래에서 **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**&#x200B;을 선택합니다.
1. [뷰어 목록] 표에서 **Univeral_HTML5_Video**&#x200B;라는 HTML5 뷰어를 찾고 다음 중 하나를 수행합니다.

   * 팝업 비디오 뷰어 환경의 경우 이름의 맨 오른쪽에 있는 **[!UICONTROL URL 복사]**&#x200B;를 선택합니다.

      비디오의 복사한 URL을 다음 구문과 함께 추가하므로 복사한 URL과 캡션 파일에 연결할 수 있습니다.

      `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * 포함된 비디오 뷰어 환경의 경우 이름의 맨 오른쪽에 있는 **[!UICONTROL 포함 코드]**&#x200B;를 선택합니다.

      포함 코드 대화 상자에서 **[!UICONTROL 클립보드에 복사]**&#x200B;를 선택합니다.

      HTML5 `Universal_HTML5_Video` 뷰어의 경우 복사된 포함 코드를 다음과 같이 추가합니다.

      `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*”`
