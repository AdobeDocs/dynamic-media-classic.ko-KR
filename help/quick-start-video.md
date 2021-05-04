---
title: '"빠른 시작: 비디오"'
description: Dynamic Media Classic 비디오를 빠르게 시작하고 실행하는 데 도움이 되는 소개 및 빠른 시작을 참조하십시오.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,뷰어,비디오
role: Business Practitioner
exl-id: 1157400c-b33a-422e-848c-258660ddc748
translation-type: tm+mt
source-git-commit: 1beb30b9eda4487dcd549034906079dee0b3149a
workflow-type: tm+mt
source-wordcount: '1425'
ht-degree: 43%

---

# 빠른 시작: 비디오{#quick-start-video}

Adobe Dynamic Media Classic Video는 데스크탑, iOS, Android™, BlackBerry® 및 Windows® 모바일 디바이스를 비롯한 다양한 화면에서 스트리밍할 수 있는 고품질 적응형 비디오를 손쉽게 퍼블리싱할 수 있는 엔드 투 엔드 솔루션입니다. 적응형 비디오 집합은 다른 비트 전송률 및 형식으로 인코딩된 동일한 비디오의 여러 버전(예: 400kbps, 800kbps 및 1000kbps)을 그룹화합니다. 데스크톱 컴퓨터나 모바일 장치가 사용 가능한 대역폭을 검색합니다.

예를 들어 iOS 모바일 장치에서는 3G, 4G 또는 Wi-Fi와 같은 대역폭을 검색합니다. 그런 다음 적응형 비디오 집합 내의 다양한 비디오 비트 전송률 중에서 적합한 인코딩된 비디오를 자동으로 선택합니다. 이 비디오는 데스크톱, 모바일 장치 또는 태블릿으로 스트리밍됩니다.

또한 데스크톱이나 모바일 장치에서 네트워크 상태가 변경될 경우 비디오 품질이 자동으로 동적으로 전환됩니다. 또한 고객이 데스크탑의 전체 화면 모드로 전환하면 응용 비디오 세트가 더 나은 해상도를 사용하여 응답하여 고객의 보기 환경을 개선합니다. 응용 비디오 세트를 사용하면 여러 화면 및 장치에서 Dynamic Media Classic 비디오를 재생하는 고객에게 최상의 재생 방법을 제공합니다.

재생하는 동안 재생하거나 선택할 인코딩된 비디오를 결정하기 위해 비디오 플레이어가 사용하는 논리는 다음 알고리즘을 기준으로 합니다.

1. 비디오 플레이어는 플레이어 자체에서 &quot;초기 비트 전송률&quot;에 설정된 값에 가장 가까운 비트 전송률을 기반으로 초기 비디오 조각을 로드합니다.
1. 다음 기준을 사용하여 대역폭 속도 변경 사항을 기반으로 비디오 플레이어를 전환합니다.

   1. 플레이어는 낮은 대역폭 스트림을 선택하거나 예상 대역폭과 동일한 높은 대역폭 스트림을 선택합니다.
   1. 플레이어는 사용 가능한 대역폭의 80%만 고려합니다. 그러나, 만일 그것이 전환되고 있다면, 과대 중복을 피하고 즉시 다시 돌아와야 하는 것을 피하기 위해서는 단지 70%만이 더 보수적이다.

알고리즘에 대한 기술 정보는 [https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp)에서 알고리즘의 로직을 참조하십시오.

단일 비디오 및 응용 비디오 세트를 관리하기 위해 Dynamic Media Classic에서는 다음을 지원합니다.

* 지원되는 많은 비디오 형식 및 오디오 형식에서 비디오를 업로드하고 여러 화면에서 재생할 수 있도록 비디오를 MP4 H.264 형식으로 인코딩. 사전 정의된 Dynamic Media Classic 응용 비디오 사전 설정, 단일 비디오 인코딩 사전 설정을 사용하거나 자체 인코딩을 사용자 정의하여 비디오의 품질과 크기를 제어할 수 있습니다.

   응용 비디오 세트가 생성되면 MP4 비디오가 포함됩니다.

   >[!NOTE]
   >
   >/기본 소스 비디오 및 기타 소스 형식 비디오는 응용 비디오 집합에 추가된 *이(가) 아닙니다.*

* Universal_HTML5_Video, Universal_HTML5_MixedMedia_dark 및 Universal_HTML5_MixedMedia_light 뷰어의 비디오 캡션 및 Universal_HTML5_Video, Universal_HTML5_MixedMedia_dark 및 Universal_HTML5_MixedMixed의 비디오 장 탐색 media_light 뷰어.

   [비디오에 캡션 추가](adding-captions-video.md)를 참조하십시오.

   [비디오에 장 마커 추가](adding-chapter-markers-video.md)를 참조하십시오.

* 비디오 자산의 효율적인 관리를 위해 전체 메타데이터 지원을 사용하여 비디오를 구성하고 찾고 검색합니다.
* iPhone, iPad, Android™, BlackBerry® 및 Windows® 폰을 비롯한 웹과 데스크탑, 모바일 장치에 응용 비디오 세트를 제공합니다.

   적응형 비디오 스트리밍은 다양한 iOS 플랫폼에서 지원됩니다.

   [Adobe 뷰어 참조 안내서](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources.html)에서 최신 지원을 참조하십시오.

   Dynamic Media Classic에서는 MP4 H.264 비디오에 대한 모바일 비디오 재생을 지원합니다. 다음 웹 사이트에서 이 비디오 형식을 지원하는 BlackBerry® 장치를 찾을 수 있습니다.

   BlackBerry®](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482)에서 지원되는 비디오 형식을 참조하십시오.[

   다음 위치에서 이 비디오 형식을 지원하는 Windows® 장치를 찾을 수 있습니다.

   Windows® Phone](https://docs.microsoft.com/en-us/)에서 지원되는 비디오 형식을 참조하십시오.[

* 다음을 포함한 Dynamic Media Classic 뷰어 사전 설정을 사용하여 비디오를 재생합니다.

   * 단일 비디오 뷰어
   * 비디오 및 이미지 컨텐츠를 결합하는 혼합 미디어 뷰어

* 브랜드 요구에 맞는 비디오 플레이어를 구성합니다.
* 간단한 URL이나 포함 코드를 사용하여 웹 사이트, 모바일 사이트 또는 모바일 애플리케이션에 비디오를 통합합니다.

**빠른 시작**

다음 단계별 작업 과정 설명은 Dynamic Media Classic의 응용 비디오 세트를 빠르게 시작하고 실행하는 데 도움이 되도록 설계되었습니다. 각 단계 뒤에는 자세한 정보를 확인할 수 있는 항목 제목의 상호 참조가 있습니다.

## 1. 비디오 업로드 및 인코딩

다음 2가지 시나리오 중 하나를 사용하여 적응형 비디오 집합을 업로드하고 생성하십시오.

* **사전 인코딩된 비디오**  업로드 - 비디오가 Dynamic Media Classic 외부에서 이미 인코딩된 경우 전역 탐색 막대에서 [업로드]를 클릭하여 MP4 비디오 파일 **** 을 찾아 Dynamic Media Classic에 바로 업로드합니다. **[!UICONTROL 작성]** > **[!UICONTROL 적응형 비디오 집합]**&#x200B;을 클릭합니다. 비디오 파일을 찾습니다. 원하는 비디오 파일을 [적응형 비디오 집합] 테이블로 끌어서 놓고 집합을 저장합니다.
* **마스터 소스 비디오**  업로드 - 비디오가 인코딩되지 않은 경우 전역 탐색 막대에서 [업로드]를 클릭하여 마스터 비디오 소스 파일(MP4 아님)을 업로드하고 Dynamic Media **** 에서 자동으로 MP4 파일로 인코딩하도록 합니다. **[!UICONTROL 업로드 작업 옵션]** 대화 상자의 **[!UICONTROL EVideo 옵션]**&#x200B;에서 **[!UICONTROL 적응형 비디오]**&#x200B;를 선택합니다.

   이 기본 옵션을 이용하면 16:9이든, 4:3이든 업로드한 비디오 크기에 맞게 올바른 인코딩 사전 설정을 비디오에 자동으로 적용하는 적응형 비디오 집합을 만들 수 있습니다. 업로드 작업을 제출하면 올바른 종횡비의 비디오 인코딩 3개를 포함하는 적응형 비디오 집합이 자동으로 만들어집니다.

   또는 동일한 **[!UICONTROL 작업 옵션]** 대화 상자의 **[!UICONTROL EVideo 옵션]**&#x200B;에서 **[!UICONTROL 단일 인코딩 사전 설정]**&#x200B;을 확장합니다.**데스크톱**, **모바일(iPhone, iPad, Android™)** 및 **태블릿(iPad, Android™)**&#x200B;에서 원하는 개별 비디오 인코딩 사전 설정을 선택하여 MP4 파일을 만듭니다.

* 또는 **[!UICONTROL 재처리]** 기능을 사용하여 마스터 비디오를 다시 처리할 수도 있습니다. 새로 인코딩된 비디오가 기존 적응형 비디오 집합에 추가됩니다.

[비디오 업로드 및 인코딩](uploading-encoding-videos.md#uploading_and_encoding_videos)을 참조하십시오.

**선택 사항입니다**

Dynamic Media Classic에서는 사전 정의된 다양한 비디오 인코딩 사전 설정을 제공합니다. 이러한 사전 정의된 사전 설정은 오늘날 사용되는 가장 일반적인 비디오 인코딩 설정을 반영하며 대상 페이지에서 재생되도록 최적화되어 있습니다.

그러나 추가적인 사용자 지정이 필요한 경우, 관리자는 비디오 사전 설정을 만들어 비디오의 크기 및 재생 환경을 최종 사용자에 맞게 사용자 지정할 수 있습니다. 관리자는 **[!UICONTROL 설정]** > **[!UICONTROL 애플리케이션 설정]** > **[!UICONTROL 비디오 사전 설정]** > **[!UICONTROL 단일 인코딩 사전 설정]**&#x200B;에서 사용할 수 있는 비디오 사전 설정 페이지에서 비디오 사전 설정을 추가하고 관리할 수 있습니다. [비디오 사전 설정] 페이지에서는 비디오 사전 설정을 추가, 편집, 삭제 및 활성화하는 선택 사항을 제공합니다.

[비디오 인코딩 사전 설정으로 작업](uploading-encoding-videos.md#working_with_video_encoding_presets)을 참조하십시오.

## 2. 비디오 뷰어에서 비디오 미리 보기

**[!UICONTROL 비디오가 데스크톱, 웹 사이트 또는 모바일 장치에서 최종 사용자에게 어떻게 재생되는지 확인하려면 [찾아보기] 패널에서 [비디오]를 선택하고 [미리 보기]를 클릭합니다]**.

[비디오 뷰어에서 비디오 미리 보기](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer)를 참조하십시오.

[미리 보기] 페이지에서 비디오를 재생할 수 있습니다. 다른 비디오 뷰어를 선택하여 비디오가 다른 플레이어에서 어떻게 표시되는지 확인할 수도 있습니다. 데스크톱, 태블릿 및 모바일 장치에서 여러 화면을 재생할 때 HTML5 비디오 플레이어를 사용하는 것이 좋습니다.

**선택 사항입니다**

뷰어 사전 설정 사용자 정의 - Dynamic Media Classic에서는 비디오를 전달하기 위한 사전 정의된 뷰어 사전 설정을 제공합니다. 이러한 사전 설정은 뷰어의 모양과 재생 컨트롤 작동 방식을 결정합니다. 관리자는 뷰어 사전 설정 페이지에서 뷰어 사전 설정을 추가하고 관리하여 비디오 뷰어를 사용자 지정할 수 있습니다. 이 페이지를 열려면 Dynamic Media Classic의 오른쪽 위 모서리에서 **[!UICONTROL 설정]** > **[!UICONTROL 뷰어 사전 설정]**&#x200B;을 클릭합니다. [뷰어 사전 설정] 페이지에서는 뷰어 사전 설정을 추가, 편집, 삭제 및 활성화하는 명령을 제공합니다.

[비디오 뷰어 사전 설정으로 작업](previewing-videos-video-viewer.md#working_with_video_viewer_presets)을 참조하십시오.

## 3. 웹 사이트 및 모바일 사이트에 비디오 배포

비디오를 웹 사이트에 통합하려면, 다음 중 하나를 수행하면 됩니다.

* 비디오를 자체 팝업 또는 모달 창에 표시합니다. 이 경우 **[!UICONTROL URL 복사]** 기능을 사용합니다.

   비디오의 URL을 얻으려면 격자 보기나 목록 보기의 [찾아보기 패널]에서 선택합니다. **[!UICONTROL 미리 보기]**&#x200B;를 클릭한 다음 `Universal_HTML5_Viewer` 오른쪽에 있는 **[!UICONTROL URL 복사]**&#x200B;를 클릭합니다.

   **[!UICONTROL URL 복사]**&#x200B;를 클릭하면 URL이 클립보드로 복사됩니다. 이 코드를 웹 사이트, 모바일 사이트 또는 애플리케이션의 HTML에 배치합니다.

   >[!NOTE]
   >
   >URL은 비디오 또는 적응형 비디오 집합을 게시한 후에만 활성화됩니다.

* 웹 페이지에 포함된 비디오를 표시합니다. 이 경우 **[!UICONTROL 포함 코드]** 기능을 사용합니다.

   비디오의 포함 코드를 구하려면, 격자 보기나 목록 보기의 [찾아보기 패널]에서 비디오를 선택합니다. **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**&#x200B;을 클릭합니다. 테이블의 작업 열에서 `Universal_HTML5_Video` 오른쪽에 있는 **[!UICONTROL 포함 코드]**&#x200B;를 클릭합니다. 코드 편집은 허용되지 않습니다.

   **[!UICONTROL 닫기]**&#x200B;를 클릭하고 포함 코드를 웹 페이지에 붙여 넣습니다.

   >[!NOTE]
   >
   >포함 코드는 비디오 또는 적응형 비디오 집합을 게시한 후에만 활성화됩니다.

[웹 사이트 및 모바일 사이트에 비디오 배포](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites)를 참조하십시오.

>[!MORELIKETHIS]
>
>* [비디오 인코딩 우수 사례](uploading-encoding-videos.md#best_practices_for_video_encoding)

