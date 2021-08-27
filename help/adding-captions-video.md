---
title: '비디오에 캡션 추가 '
description: Adobe Dynamic Media Classic에서 비디오에 캡션을 추가하는 방법을 알아봅니다.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 66a1ab20-6036-4c3d-bb66-dd06d917c7f2
source-git-commit: ad5270545be502d3aaabba574353787622ab0445
workflow-type: tm+mt
source-wordcount: '904'
ht-degree: 32%

---

# 비디오에 캡션 추가 {#adding-captions-to-video}

단일 비디오나 적응형 비디오 집합에 캡션을 추가하여 비디오 사용을 세계 시장으로 확장할 수 있습니다. 캡션을 추가하면 여러 가지 각 언어로 오디오를 다시 녹음하기 위해 오디오를 더빙하거나 원어민이 투입될 필요가 없어집니다. 비디오는 녹음된 언어로 재생됩니다. 외국어 자막이 표시되기 때문에 다른 언어를 사용하는 사람들도 오디오를 이해할 수 있게 됩니다.

또한 캡션을 사용하면 귀가 들리지 않거나 난청인 사람들을 위한 청각 장애용 캡션을 통해 액세스 가능성이 더 커집니다.

>[!NOTE]
>
>사용하는 비디오 플레이어가 캡션 표시를 지원해야 합니다.

다음 뷰어의 메뉴 텍스트를 포함하여 [캡션 효과]를 구성하고 [캡션 메뉴 자체]를 편집하려면 다음을 수행합니다.

* `Universal_HTML5_Video` 뷰어
* `Universal_HTML5_MixedMedia_dark` 뷰어
* `Universal_HTML5_MixedMedia_light` 뷰어

[비디오 뷰어 사전 설정 추가 또는 편집](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset)을 참조하십시오.

또한 [뷰어 사전 설정 추가 및 편집](application-setup.md#adding_and_editing_viewer_presets)을 참조하십시오.

Adobe Dynamic Media Classic에서는 캡션 파일을 JSON(JavaScript 개체 표기법) 형식으로 변환할 수 있습니다. 이 변환은 JSON 텍스트를 숨겨져 있지만 완전한 비디오의 스크립트로서 웹 페이지에 포함할 수 있음을 의미합니다. 그런 다음 검색 엔진은 컨텐츠를 크롤링하고 색인화하여 비디오를 보다 손쉽게 검색할 수 있게 만들고 고객에게 비디오 컨텐츠에 대한 자세한 정보를 제공할 수 있습니다.

URL에서 JSON 함수를 사용하는 방법에 대한 자세한 내용은 *Adobe 이미지 제공 API 도움말*&#x200B;의 [정적(비이미지) 콘텐츠 제공](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents.html?lang=en#image-serving-api)을 참조하십시오.

**비디오에 캡션을 추가하려면:**

1. Dynamic Media Classic의 외부 타사 응용 프로그램을 사용하여 사용 중인 뷰어 유형에 따라 비디오 캡션 파일을 만듭니다.

   | 뷰어 유형 | 캡션 파일 |
   |--- |--- |
   | HTML5 | HTML5 비디오 뷰어를 사용하는 경우, 사용자가 만드는 캡션 파일이 WebVTT(Web Video Text Tracks) 표준을 준수하도록 해야 합니다. 캡션 파일 이름 확장자는 .vtt입니다. WebVTT 캡션 표준에 대한 자세한 내용을 알 수 있습니다.<br><br>[WebVTT](https://w3c.github.io/webvtt/) 를 참조하십시오. 웹 비디오 텍스트 트랙 형식입니다. <br><br>Adobe Dynamic Media Classic 외부에서 캡션 파일을 작성하는 데 사용할 수 있는 도구와 서비스에 대해 무료 및 유료 서비스가 모두 있습니다. 예를 들어 스타일이 없는 간단한 비디오 캡션 파일을 만들려면 다음과 같은 무료 온라인 캡션 작성 및 편집 도구를 사용할 수 있습니다. <br><br>[WebVTT 캡션 작성기](https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html) <br><br>최상의 결과를 얻으려면 Internet Explorer 9 이상, Google Chrome 또는 Safari에서 도구를 사용하십시오. <br><br>도구의 비디오  <b>파일 URL </b> 입력 필드에서 비디오 파일의 URL을 붙여 넣은 다음  <b>로드</b>를 선택합니다. <br><br>예를 들어 비디오 파일에 Dynamic Media Classic URL을 사용하는 경우 개별 비디오 자산(응용 비디오 세트 또는 기본 비디오가 아님)을 두 번 클릭하여 세부 사항 보기에서 엽니다. [세부 사항 보기]의 오른쪽 패널에서 URL 및 포함 코드를 확장합니다. 그런 다음 모바일 그룹 오른쪽의 모바일(점진적) 아래에서 <b>URL 복사</b>를 선택합니다. 이 프로세스에서는 비디오 파일 자체에 대한 URL을 제공하여 <b>비디오 파일의 URL 입력</b> 필드에 붙여넣을 수 있습니다. 그러면 Internet Explorer, Chrome 또는 Safari가 비디오를 기본적으로 재생할 수 있습니다. 이제 사이트에서 제공하는 화면의 지침에 따라 WebVTT 파일을 작성하고 저장합니다. 완료되면 캡션 파일 내용을 복사하여 일반 텍스트 편집기에 붙여넣은 다음 VTT 파일 확장자로 저장합니다. <br><br><b>참고:</b> 영어 이외의 언어로 비디오 캡션을 전역 지원하려면 WebVTT 표준을 사용하려면 지원할 각 언어에 대해 별도의 .vtt 파일 및 호출을 만들어야 합니다. <br><br>일반적으로 캡션 VTT 파일의 이름은 비디오 파일과 동일하게 지정하고 여기에 captions를 추가합니다. 그렇게 하면 기존 웹 컨텐츠 관리 시스템을 사용하여 비디오 URL의 생성을 자동화하는 데 도움이 될 수 있습니다. |

1. Dynamic Media Classic Adobe에서 WebVTT, DFXP 또는 SMPTE XML 캡션 파일을 업로드합니다.

   [파일 업로드](uploading-files.md#uploading_files)를 참조하십시오.

1. 왼쪽의 [자산 라이브러리] 패널에서 업로드한 캡션 파일과 연결하려는 비디오 파일이 들어 있는 자산 폴더를 탐색합니다.
1. 자산 찾아보기 패널에서 단일 비디오 자산을 선택한 다음 자산의 축소판 이미지 아래에서 **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**&#x200B;을 선택합니다.
1. 뷰어 목록 테이블에서 **Universal_HTML5_Video**, **Universal_HTML5_MixedMedia_dark** 또는 **Universal_HTML5_MixedMedia_light**&#x200B;라는 HTML5 뷰어를 찾은 다음 중 하나를 수행합니다.

   * 팝업 비디오 뷰어 환경의 경우 이름의 맨 오른쪽에 있는 **[!UICONTROL URL 복사]**&#x200B;를 선택합니다.

      비디오의 복사한 URL을 다음 구문과 함께 추가하므로 복사한 URL과 캡션 파일에 연결할 수 있습니다.

      `&caption=<full Copy URL path to the caption file .vtt>,1`

      캡션 URL 경로의 끝에 `,1`을 참고하십시오. 경로에서 VTT 파일 이름 확장자 바로 다음에, 각각 `1` 또는 `0` 로 설정하여 비디오 플레이어 모음에서 닫힌 캡션 단추를 활성화 또는 비활성화할 수 있습니다.

   * 포함된 비디오 뷰어 환경의 경우 이름의 맨 오른쪽에 있는 **[!UICONTROL 포함 코드]**&#x200B;를 선택합니다.

      포함 코드 대화 상자에서 **[!UICONTROL 클립보드에 복사]**&#x200B;를 선택합니다.

      HTML5 `Universal_HTML5_Video`, `Universal_HTML5_MixedMedia_dark` 또는 `Universal_HTML5_MixedMedia_light` 뷰어의 경우 복사된 포함 코드를 다음과 같이 추가합니다.

      `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1”`

      URL 경로의 끝에 `,1`을(를) 참고하십시오. URL 경로에서 VTT 파일 이름 확장명 직후, 각각 `1` 또는 `0` 로 설정하여 비디오 플레이어 모음에서 캡션 단추를 활성화하거나 비활성화할 수 있습니다.
