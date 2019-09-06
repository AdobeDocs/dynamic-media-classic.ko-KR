---
title: 비디오에 캡션 추가
seo-title: 비디오에 캡션 추가
description: 널
seo-description: 비디오에 캡션을 추가하는 방법 학습
uuid: 4 CC 64469-4369-44 A 9-83 DB -63 BAD 51 ABA 8 A
contentOwner: 관리
content-type: 참조
products: sg_ Experiencemanager/dynamic-media-scene -7
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# 비디오에 캡션 추가{#adding-captions-to-video}

단일 비디오나 적응형 비디오 집합에 캡션을 추가하여 비디오 사용을 세계 시장으로 확장할 수 있습니다. 캡션을 추가하면 여러 가지 각 언어로 오디오를 다시 녹음하기 위해 오디오를 더빙하거나 원어민이 투입될 필요가 없어집니다. 비디오는 녹음된 언어로 재생됩니다. 외국어 자막이 표시되기 때문에 다른 언어를 사용하는 사람들도 오디오를 이해할 수 있게 됩니다.

또한 캡션을 사용하면 귀가 들리지 않거나 난청인 사람들을 위한 청각 장애용 캡션을 통해 액세스 가능성이 더 커집니다.

>[!NOTE]
>
>사용하는 비디오 플레이어가 캡션 표시를 지원해야 합니다.

캡션 효과를 구성하고, 다음 뷰어들의 메뉴 텍스트를 포함하여 캡션 메뉴 자체를 편집하려면 [비디오 뷰어 사전 설정 추가 또는 편집](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset)을 참조하십시오.

* `Universal_HTML5_Video` 뷰어.
* `Universal_HTML5_MixedMedia_dark` 뷰어.
* `Universal_HTML5_MixedMedia_light` 뷰어.

[뷰어 사전 설정 추가 및 편집](application-setup.md#adding_and_editing_viewer_presets)을 참조하십시오.

Dynamic Media Classic 에는 캡션 파일을 JSON (JavaScript Object Notation) 포맷으로 변환하는 기능이 있습니다. 이 변환은 JSON 텍스트를 숨겨져 있지만 완전한 비디오의 스크립트로서 웹 페이지에 포함할 수 있음을 의미합니다. 이렇게 되면 검색 엔진이 컨텐츠를 탐색하고 색인화하여 비디오를 더 쉽게 검색할 수 있도록 하고, 고객에게 비디오 컨텐츠에 대한 추가적인 세부 정보를 제공할 수 있습니다.

See [Serving static (non-image) contents](https://marketing.adobe.com/resources/help/en_US/s7/is_ir_api/is_api/c_serving_static_nonimage_contents.html) in the *Adobe Image Serving API Help* for more information about using the JSON function in a URL.

**비디오에 캡션을 추가하려면**

1. 사용하고 있는 뷰어 유형에 따라 Scene7 Publishing System의 외부 타사 애플리케이션을 사용하여 캡션 비디오 캡션 파일을 만들 수 있습니다.

   | 뷰어 유형 | 캡션 파일 |
   |--- |--- |
   | HTML5 | HTML5 비디오 뷰어를 사용하는 경우, 사용자가 만드는 캡션 파일이 WebVTT(Web Video Text Tracks) 표준을 준수하도록 해야 합니다. 캡션 파일 이름 확장자는 .vtt입니다. WebVTT 캡션 표준에 대한 자세한 내용을 알 수 있습니다.<br><br>[Webvtt를 참조하십시오](https://dev.w3.org/html5/webvtt/). 웹 비디오 텍스트 트랙 형식. <br><br>Scene7 Publishing System 외부에서 캡션 파일을 작성하는 데 사용할 수 있는 도구 및 서비스에는 무료와 유료 제품이 모두 있습니다. 예를 들어 스타일이 없는 간단한 비디오 캡션 파일을 만들려면 다음과 같은 무료 온라인 캡션 작성 및 편집 도구를 사용할 수 있습니다. <br><br>[Webvtt 캡션 제작](https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html) <br><br>최상의 결과를 얻을 수 있도록 Internet Explorer 9 이상, Google Chrome 또는 Safari의 도구를 사용합니다. <br><br>도구의 [비디오 파일 <b>입력</b> ] 필드에 비디오 파일의 URL를 붙여넣은 다음 [불러오기] 를 클릭합니다 <b></b>. <br><br>예를 들어, 비디오 파일에 대해 Dynamic Media Classic URL를 사용하는 경우 SPS에서 개별 비디오 자산 (응용 비디오 집합이 아니거나 마스터 비디오가 아님) 를 두 번 클릭하여 [세부 사항 보기] 에서 엽니다. [세부 사항 보기]의 오른쪽 패널에서 URL 및 포함 코드를 확장합니다. 그런 다음 [모바일] 그룹 아래의 [모바일(점진적)] 오른쪽에 있는 URL 복사를 클릭합니다. This process gives you the URL to the video file itself which you can then paste into the <b>Enter URL of video file</b> field. 그러면 Internet Explorer, Chrome 또는 Safari가 비디오를 기본적으로 재생할 수 있습니다. 이제 사이트에서 제공하는 화면의 지침에 따라 WebVTT 파일을 작성하고 저장합니다. 끝나면, 캡션 파일 컨텐츠를 복사하여 일반 텍스트 편집기에 붙여 넣고 .vtt 파일 이름 확장자로 저장합니다. <br><br><b>참고:</b> 영어 이외의 언어로 된 비디오 캡션을 전체적으로 지원하려면 Webvtt 표준을 통해 지원하려는 각 언어에 대해 별도의. vtt 파일과 호출을 만들어야 합니다. <br><br>일반적으로 캡션 VTT 파일의 이름은 비디오 파일과 동일하게 지정하고 여기에 captions를 추가합니다. 그렇게 하면 기존 웹 컨텐츠 관리 시스템을 사용하여 비디오 URL의 생성을 자동화하는 데 도움이 될 수 있습니다. |

1. Scene7 Publishing System에서 WebVTT, DFXP 또는 SMPTE XML 캡션 파일을 업로드합니다.

   [파일 업로드](uploading-files.md#uploading_files)를 참조하십시오.

1. 왼쪽의 [자산 라이브러리] 패널에서 업로드한 캡션 파일과 연결하려는 비디오 파일이 들어 있는 자산 폴더를 탐색합니다.
1. [자산 찾아보기] 패널에서 단일 비디오 자산을 선택하고 자산의 썸네일 이미지 아래에서 **[미리 보기]** &gt; **[뷰어 목록]**&#x200B;을 클릭합니다.
1. In the Viewer List table, find the HTML5 viewer named **Univeral_HTML5_Video**, **Universal_HTML5_MixedMedia_dark**, or **Universal_HTML5_MixedMedia_light**, then do one of the following:

   * 팝업 비디오 뷰어 환경의 경우 이름의 오른쪽 끝에 있는 **[URL 복사]**&#x200B;를 클릭합니다.

      복사한 비디오 URL을 다음 구문에 추가하여 복사한 캡션 파일 URL과 연결합니다.

      `&caption=<full Copy URL path to the caption file .vtt>,1`

      Note the `,1` at the end of the caption URL path. 경로에서 .vtt 파일 이름 확장자 바로 뒤에 나오는 이것은 각각 `1` 또는 `0`으로 설정하여 비디오 플레이어 막대에 있는 폐쇄 캡션 단추를 활성화 또는 비활성화하는 옵션입니다.

   * 임베드된 비디오 뷰어 환경의 경우 이름의 오른쪽 끝에 있는 **[임베드 코드]**&#x200B;를 클릭합니다.

      [임베드 코드] 대화 상자에서 **[클립보드에 복사]**&#x200B;를 클릭합니다.

      For the HTML5 `Universal_HTML5_Video`, `Universal_HTML5_MixedMedia_dark`, or `Universal_HTML5_MixedMedia_light` viewers, append the copied embed code with the following:

      `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1”`

      Note the `,1` at the end of the URL path. URL 경로에서 .vtt 파일 이름 확장자 바로 뒤에 나오는 이것은 각각 `1` 또는 `0`으로 설정하여 비디오 플레이어 막대에 있는 캡션 단추를 활성화 또는 비활성화하는 옵션입니다.

