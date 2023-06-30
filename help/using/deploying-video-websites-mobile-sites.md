---
title: 웹 사이트 및 모바일 사이트에 비디오 배포
description: Adobe Dynamic Media Classic에서 웹 사이트 및 모바일 사이트에 비디오를 배포하는 방법에 대해 알아봅니다.
uuid: 22bb4402-c0ab-4df0-89b9-99707d111927
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 0d006314-c4cc-4f6c-a51c-6075bb445e39
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 3df22d48-edb5-4927-aefb-104b53f81f1a
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '1706'
ht-degree: 34%

---

# 웹 사이트 및 모바일 사이트에 비디오 배포{#deploying-video-to-your-websites-and-mobile-sites}

웹 사이트, 모바일 사이트 및 데스크탑 애플리케이션은 URL 문자열 또는 포함된 코드를 사용하여 비디오를 비롯한 Adobe Dynamic Media Classic 서버 콘텐츠에 액세스합니다. Adobe Dynamic Media Classic은 게시 프로세스 중에 이러한 URL 문자열을 활성화합니다. 웹 페이지, 모바일 페이지 및 데스크탑 애플리케이션에 비디오에 대한 URL 문자열 또는 포함 코드를 배치하려면 Adobe Dynamic Media Classic에서 복사하십시오.

>[!NOTE]
>
>자산을 게시하기 전까지는 URL이나 포함 코드가 활성화되지 않습니다.

## 비디오 게시 {#publishing-video}

비디오를 게시하면 Adobe Dynamic Media Classic 서버가 비디오를 웹 사이트, 모바일 사이트 또는 애플리케이션에 전달할 수 있습니다.

비디오를 게시하는 데 사용할 수 있는 방법에는 두 가지가 있습니다.

* **업로드 시 자동으로 즉시 비디오 게시** - 비디오 업로드 프로세스의 일부로 Adobe Dynamic Media Classic은 비디오를 업로드하고 인코딩할 때 자동으로 게시할 수 있습니다. 즉시 게시하는 이 기능은 비디오를 나중에 별도로 게시할 필요가 없음을 의미합니다.

* **비디오를 업로드 후 수동으로 게시** - 비디오를 즉시 게시하지 않으려는 경우 수동으로 언제든지 비디오를 게시할 수 있습니다.

비디오를 게시하면 Adobe Dynamic Media Classic에서 HTML 페이지 또는 애플리케이션 코드에 대한 URL 문자열을 활성화합니다.

**비디오를 게시하려면:**

1. 다음 중 하나를 수행하십시오.

   * 업로드 시 비디오를 자동으로 즉시 게시하려면 업로드 페이지에서 을(를) 선택합니다. **[!UICONTROL 업로드 후 게시]**. 완료했으면 더 이상 수행할 단계가 없습니다.
   * 업로드 후 비디오를 수동으로 게시하려면 찾아보기 패널에서 비디오를 선택한 다음 전역 탐색 모음에서 를 선택합니다. **게시**.

## 모바일 사이트 또는 웹 사이트에 비디오 URL 연결 {#linking-a-video-url-to-a-mobile-site-or-a-website}

비디오를 게시한 후에는 웹 사이트, 모바일 사이트 또는 데스크톱 애플리케이션에서 사용할 URL을 얻을 수 있습니다. 웹 페이지 상단의 팝업 또는 모달 창에서 비디오를 표시하려는 경우 이 비디오 URL을 사용하십시오.

고객이 링크를 선택하면 장치, 대역폭 및 화면 크기가 자동으로 감지됩니다. 데스크톱에 사전 정의된 뷰어나 스마트폰과 태블릿용 모바일 장치의 기본 비디오 플레이어에서 재생하기 위해 해당 비디오가 표시됩니다.

참조: [웹 페이지에 비디오 뷰어 포함](deploying-video-websites-mobile-sites.md#embedding_the_video_viewer_on_a_web_page).

**비디오 URL을 모바일 사이트 또는 웹 사이트에 연결하려면:**

1. 에셋 찾아보기 패널의 **[!UICONTROL 표시]** 드롭다운 목록에서 다음을 선택합니다. **[!UICONTROL 비디오]** 또는 **[!UICONTROL 응용 비디오 집합]**.
1. 왼쪽의 [자산 라이브러리] 패널에서 연결하려는 비디오 또는 적응형 비디오 집합이 들어 있는 자산 폴더로 이동합니다.
1. [자산 찾아보기] 패널 위의 도구 모음 오른쪽에서 다음 중 하나를 수행합니다.

   * 선택 **[!UICONTROL 격자 보기]** 또는 **[!UICONTROL 목록 보기]**. [자산 찾아보기] 패널에서 단일 자산의 비디오 썸네일을 두 번 클릭하여 [세부 사항 보기]에서 엽니다. 오른쪽의 URL 및 포함 코드 패널에서 HTTP 스트리밍 아래에 있는 **[!UICONTROL URL 복사]** 원하는 뷰어의 오른쪽에 있습니다. 가장 좋은 방법은 와 연결된 URL을 복사하는 것입니다. `Universal_HTML5_Video` 뷰어.
   * 선택 **[!UICONTROL 격자 보기]**. 에셋 찾아보기 패널에서 단일 에셋을 선택한 다음 썸네일 이미지 아래에서 **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**.

     뷰어 목록 페이지의 테이블에 있는 작업 열에서 을 선택합니다. **[!UICONTROL URL 복사]**. 가장 좋은 방법은 와 연결된 URL을 복사하는 것입니다. `Universal_HTML5_Video` 뷰어.

   * 선택 **[!UICONTROL 목록 보기]**. 에셋 찾아보기 패널에서 단일 에셋을 선택한 다음 썸네일 이미지의 오른쪽으로 이동합니다. **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**.

     뷰어 목록 페이지의 테이블에 있는 작업 열에서 을 선택합니다. **[!UICONTROL URL 복사]**. 가장 좋은 방법은 와 연결된 URL을 복사하는 것입니다. `Universal_HTML5_Video` 뷰어.

   * 선택 **[!UICONTROL 격자 보기]**, **[!UICONTROL 목록 보기]**, 또는 **[!UICONTROL 세부 사항 보기]**. 동일한 도구 모음에서 다음 위치로 이동합니다. **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**.

     뷰어 목록 페이지의 테이블에 있는 작업 열에서 을 선택합니다. **[!UICONTROL URL 복사]**. 가장 좋은 방법은 와 연결된 URL을 복사하는 것입니다. `Universal_HTML5_Video` 뷰어.

1. 웹 사이트와 모바일 사이트에 HTML5 비디오 URL 링크를 붙여 넣습니다.

## 웹 페이지에 비디오 뷰어 포함 {#embedding-the-video-viewer-on-a-web-page}

웹 페이지에 포함된 비디오를 재생하려면 포함 코드 기능을 사용합니다. 포함 코드를 웹 페이지에 붙여 넣을 수 있도록 클립보드로 복사합니다. 코드 편집은 [임베드 코드] 대화 상자에서 허용되지 않습니다.

참조: [모바일 사이트 또는 웹 사이트에 비디오 URL 연결](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

**웹 페이지에 비디오 뷰어를 포함하려면:**

1. 에셋 찾아보기 패널의 표시 드롭다운 목록에서 다음을 선택합니다. **[!UICONTROL 비디오]** 또는 **[!UICONTROL 응용 비디오 집합]**.
1. 왼쪽의 [자산 라이브러리] 패널에서 포함 코드를 복사하려는 비디오나 적응형 비디오 집합이 들어 있는 자산 폴더로 이동합니다.
1. [자산 찾아보기] 패널 위의 도구 모음 오른쪽에서 다음 중 하나를 수행합니다.

   * 선택 **[!UICONTROL 격자 보기]** 또는 **[!UICONTROL 목록 보기]**. [자산 찾아보기] 패널에서 단일 자산의 비디오 썸네일을 두 번 클릭하여 [세부 사항 보기]에서 엽니다. 오른쪽의 URL 및 포함 코드 패널에서 HTTP 스트리밍 아래에 있는 **[!UICONTROL 포함 코드]** 원하는 뷰어의 오른쪽에 있습니다. 를 모범 사례로 선택합니다. **[!UICONTROL 포함 코드]** 와(과) 연결된 `Universal_HTML5_Video` 뷰어.
   * 선택 **[!UICONTROL 격자 보기]**. [에셋 찾아보기] 패널에서 단일 에셋을 선택한 다음 비디오 썸네일 이미지 아래에서 을 선택합니다 **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**.

     뷰어 목록 페이지의 테이블에 있는 작업 열에서 을 선택합니다. **[!UICONTROL 포함 코드]**. 를 모범 사례로 선택합니다. **[!UICONTROL 포함 코드]** 와(과) 연결된 `Universal_HTML5_Video` 뷰어.

   * 선택 **[!UICONTROL 목록 보기]**. 에셋 찾아보기 패널에서 단일 에셋을 선택한 다음 썸네일 이미지의 오른쪽으로 이동합니다. **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**.

     뷰어 목록 페이지의 테이블에 있는 작업 열에서 을 선택합니다. **[!UICONTROL 포함 코드]**. 를 모범 사례로 선택합니다. **[!UICONTROL 포함 코드]** 와(과) 연결된 `Universal_HTML5_Video` 뷰어.

   * 선택 **[!UICONTROL 격자 보기]**, **[!UICONTROL 목록 보기]**, 또는 **[!UICONTROL 세부 사항 보기]**. 동일한 도구 모음에서 다음 위치로 이동합니다. **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**.

     뷰어 목록 페이지의 테이블에 있는 작업 열에서 을 선택합니다. **[!UICONTROL 포함 코드]**. 를 모범 사례로 선택합니다. **[!UICONTROL 포함 코드]** 와(과) 연결된 `Universal_HTML5_Video` 뷰어.

1. 포함 코드 대화 상자에서 **[!UICONTROL 클립보드에 복사]**.

   코드 편집은 [임베드 코드] 대화 상자에서 허용되지 않습니다.

1. 선택 **[!UICONTROL 닫기]**.
1. 웹 페이지에 포함 코드를 붙여 넣습니다.

### MP4 비디오 자산에 HTML5 비디오를 사용하기 위한 포함 코드 구현 {#implementing-embed-code-for-using-html-video-with-mp-video-assets}

Adobe Dynamic Media Classic HTML5 비디오 플레이어를 사용하지 않고 대신 기본 HTML5를 사용하려는 경우 `<video>` mp4 비디오 자산과 함께 태그를 지정하면 다음 포함 코드 샘플을 사용할 수 있습니다.

```as3
<video poster="S7 video thumbnail URL" controls> 
        <source src="S7 OGG video asset URL (no player)" type='video/ogg; codecs="theora, vorbis"'/> 
        <source src="S7 MP4 mobile progressive video asset URL (no player)" type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'/> 
        <p>This is fallback content</p> 
</video>
```

* 바꾸기 `"S7 video thumbnail URL"` 를 사용하여 비디오를 재생하기 전에 사용자에게 표시되는 비디오의 썸네일 이미지인 비디오의 썸네일 URL을 변경할 수 있습니다.

  다음을 참조하십시오 [비디오 썸네일 URL 얻기](deploying-video-websites-mobile-sites.md#obtaining_video_thumbnail_urls).

* 바꾸기 `"S7 OGG video asset URL (no player)"` OGG 비디오에 대한 비디오의 점진적 URL이 포함된 비디오

  다음을 참조하십시오 [모바일 사이트 또는 웹 사이트에 비디오 URL 연결](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

* 바꾸기 `"S7 MP4 mobile progressive video asset URL (no player)"` 비디오의 모바일 점진적 URL과 함께 사용하십시오.

  다음을 참조하십시오 [모바일 사이트 또는 웹 사이트에 비디오 URL 연결](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

## 타사 비디오 플레이어를 사용하여 비디오 배포 {#deploying-video-using-a-third-party-video-player}

Dynamic Media Classic 비디오 뷰어 대신 서드파티 비디오 플레이어 또는 사용자 지정 빌드 비디오 플레이어를 사용하는 경우 HLS 다중 비트 전송률 비디오 스트리밍 또는 점진적 다운로드에 작동하는 직접 비디오 URL을 가져옵니다.

**타사 비디오 플레이어를 사용하여 비디오를 배포하려면:**

1. Adobe Dynamic Media Classic의 전역 탐색 바에서 **[!UICONTROL 설정]** > **[!UICONTROL 응용 프로그램 설정]** > **[!UICONTROL 일반 설정]**.
1. 사용할 URL 유형에 따라 다음 작업 중 하나를 수행하십시오.

* 다이렉트 HLS 스트리밍 비디오 URL(다중 비트율)을 생성하려면

  다음에서 **[!UICONTROL 응용 프로그램 일반 설정]** 페이지, **[!UICONTROL 서버]** 그룹, **[!UICONTROL 게시된 서버 이름]** 텍스트 필드에서 직접 URL을 구성합니다. 다음 구문을 사용합니다. `server/is/content/company/folder/filename.m3u8`

  예를 들어 게시된 서버 이름이 이라고 가정합니다. `https://s7d9.scene7.com/.` 2단계의 구문을 사용하면 직접 URL은 다음과 같이 표시될 수 있습니다.
  `https://s7d9.scene7.com/is/content/GeoRetail/AdobeRIA-AVS.m3u8`

* 직접 HLS 스트리밍 비디오 URL을 생성하려면(단일 비트 전송률)

  다음에서 **[!UICONTROL 응용 프로그램 일반 설정]** 페이지, **[!UICONTROL 서버]** 그룹, **[!UICONTROL HLS 스트리밍 서버 이름]** 텍스트 필드에서 다음 구문을 사용하여 직접 URL을 구성합니다.

  `server/company/folder/filename.ext.m3u8`

  예를 들어 HLS 스트리밍 서버 이름이 이라고 가정합니다. `https://s7mbrstream.scene7.com/hls-vod/`. 2단계의 구문을 사용하면 직접 URL은 다음과 같이 표시될 수 있습니다.
  `https://s7mbrstream.scene7.com/hls-vod/GeoRetail/MBR/ToyStory3\_Teaser1\_High\_iPad\_768x432\_1296K.mp4.m3u8`

* 직접 점진적 비디오 URL을 생성하려면

  **[!UICONTROL [애플리케이션 일반 설정]]** 페이지에 있는 **[!UICONTROL [서버]]** 그룹의 **[!UICONTROL [점진적 비디오 서버 이름]]** 텍스트 필드에서 다음 구문을 사용하여 직접 eVideo URL을 구성합니다.

  `server/company/folder/filename`

  예를 들어 점진적 비디오 서버 이름이 이라고 가정합니다. `https://s7d9.scene7.com/is/content/`. 2단계의 구문을 사용하면 직접 URL은 다음과 같이 표시될 수 있습니다.
  `https://s7d9.scene7.com/e2/GeoRetail/SourceVideo/outdoors.mp4`

## 비디오 축소판 작업 {#working-with-video-thumbnails}

Adobe Dynamic Media Classic은 인코딩된 비디오 및 사전 인코딩된 비디오에 대한 썸네일을 생성합니다. 이미지 자산 등의 비디오 썸네일을 사용할 수 있습니다. 또한 Adobe Dynamic Media Classic에서 생성하는 비디오 썸네일의 URL을 가져올 수 있습니다. 그런 다음 이러한 URL을 Adobe Dynamic Media Classic 외부에 배포할 수 있습니다. 예를 들어 웹 사이트의 검색 결과, 관련 비디오 목록 및 비디오 재생 목록에 썸네일을 배포할 수 있습니다.

썸네일은 비디오의 첫 번째 이기종 프레임(모두 검정 프레임 또는 모두 흰색 프레임 등이 아님)에 따라 생성됩니다.

### 비디오 썸네일 URL 얻기 {#obtaining-video-thumbnail-urls}

Adobe Dynamic Media Classic은 업로드 프로세스 중에 비디오 썸네일을 자동으로 생성합니다. 축소판은 [목록 보기] 및 [격자 보기]의 [찾아보기] 패널에 나타납니다.

비디오 썸네일의 URL을 생성하려면 게시 작업을 수행합니다.

다음을 참조하십시오 [비디오 게시](deploying-video-websites-mobile-sites.md#publishing_video).

게시 후에 [세부 사항 보기]의 [URL] 및 [포함 코드] 패널에서 비디오 썸네일 URL을 얻을 수 있습니다. 선택 **[!UICONTROL URL 복사]** 비디오 썸네일 오른쪽에 있으므로 해당 URL을 복사할 수 있습니다.

### 비디오 뷰어의 포스터 프레임 수정 {#modifying-poster-frames-in-video-viewers}

*포스터 프레임*&#x200B;은 비디오가 재생되기 전에 비디오 뷰어에 표시되는 초기 프레임입니다. Adobe Dynamic Media Classic은 비디오 썸네일을 포스터 프레임으로 사용합니다.

포스터 프레임에 이미지 수정자를 적용할 수 있습니다. 예를 들어 포스터 프레임을 자르거나 투명하게 만들 수 있습니다. 포스터 프레임을 수정하려면 비디오 뷰어 구성 화면을 열고 [포스터 이미지 수정자] 섹션에 수정자를 입력합니다.

다음을 참조하십시오 [비디오 뷰어 사전 설정 추가 또는 편집](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

다음을 참조하십시오 [이미지 제공 안내서](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-is-home.html?lang=en#image-serving-api).

비디오 썸네일 URL에 수정자를 추가하여 비디오 썸네일을 수정할 수도 있습니다.

>[!MORELIKETHIS]
>
>* [파일 게시](publishing-files.md#publishing_files)