---
title: 비디오 뷰어에서 비디오 미리 보기
description: 비디오 뷰어에서 비디오를 미리 보는 방법에 대해 알아봅니다.
uuid: 7ab4e805-6e5d-461b-bd99-5e09b9ced950
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 6a2e6df1-9186-42e2-9b85-01f132936c72
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: b8d1a0b4-67ab-482d-a685-a087fb850143
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '881'
ht-degree: 28%

---

# 비디오 뷰어에서 비디오 미리 보기{#previewing-videos-in-a-video-viewer}

비디오 뷰어에서 비디오가 표시 및 재생되는 방식을 미리 볼 수 있습니다.

다음을 참조하십시오 [뷰어 사전 설정 추가 및 편집](application-setup.md#adding_and_editing_viewer_presets).

**비디오 뷰어에서 비디오를 미리 보려면:**

1. 왼쪽의 에셋 라이브러리 패널에서 표시 드롭다운 목록을 선택하고 **[!UICONTROL 비디오]** (단일 인코딩 비디오) 또는 **[!UICONTROL 응용 비디오 집합]**. 응용 비디오 인코딩 사전 설정을 사용하면 다중 비트 전송률이 인코딩된 비디오 세트가 생성됩니다.
1. 왼쪽의 자산 라이브러리 패널에서 자산 폴더를 탐색하여 미리 보려는 비디오를 선택합니다.
1. 다음 중 하나를 수행합니다.

   * 도구 모음의 오른쪽에 있는 에셋 창 위에서 을(를) 선택합니다 **[!UICONTROL 목록 보기]**. 에셋 창에서 에셋을 마우스로 가리킨 다음 을 선택합니다 **[!UICONTROL 미리 보기]**.
   * 도구 모음의 오른쪽에 있는 에셋 창 위에서 을(를) 선택합니다 **[!UICONTROL 격자 보기]**. 에셋 창의 에셋 썸네일 창에서 을 선택합니다. **[!UICONTROL 미리 보기]**.
   * 도구 모음의 오른쪽에 있는 에셋 창 위에서 을(를) 선택합니다 **[!UICONTROL 세부 사항 보기]**. 동일한 도구 모음에서 를 선택합니다. **[!UICONTROL 미리 보기]**.
   * [자산] 창에서 자산을 선택합니다. 도구 모음에서 다음 위치로 이동 **[!UICONTROL 파일]** > **[!UICONTROL 미리 보기]**.

1. (선택 사항) [미리 보기] 창 하단에 있는 드롭다운 목록에서 복사할 때 자산 URL에 적용할 URL 인코딩을 선택합니다.
1. 다음 항목 선택 **[!UICONTROL 미리 보기]** 링크를 클릭하여 선택한 뷰어에서 에셋을 검토할 수 있습니다.
1. 표시된 뷰어를 닫습니다.
1. 선택 **[!UICONTROL 닫기]** 자산 화면으로 돌아갑니다.

>[!NOTE]
>
>Adobe Dynamic Media Classic은 데스크탑에서 MP4 비디오를 미리 볼 수 있는 편리한 방법을 제공합니다. 이 방법을 사용할 경우 모바일 장치에서 실제로 테스트하지 않고도 데스크톱에서 모바일 컨텐츠를 미리 볼 수 있습니다. 그러나 데스크탑 미리 보기에 표시되는 내용은 모바일 장치에서 재생이 어떻게 표시되는지 사실적으로 보여 주지 않습니다. 모바일 장치에서 비디오가 어떻게 보이고 재생되는지 미리 보려면 [미리 보기] 화면으로 이동하여 다음을 선택합니다. **[!UICONTROL URL 복사]**&#x200B;을 클릭하고 모바일 장치의 웹 브라우저에 해당 URL을 입력합니다. 자세한 내용은 [웹 사이트 및 모바일 사이트에 비디오 배포](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites).

## 비디오 뷰어 사전 설정 작업 {#working-with-video-viewer-presets}

사용자는 비디오 뷰어에서 비디오를 봅니다. 비디오 뷰어의 동작 및 표시 모양과 재생 컨트롤 작동 방식은 비디오 재생을 위해 선택한 뷰어 사전 설정에 따라 달라집니다. [미리 보기] 화면에서 뷰어 사전 설정을 선택합니다. 사전 설정을 선택하면 선택한 뷰어 사전 설정으로 비디오를 재생하기 위한 URL 또는 포함 코드를 얻을 수 있습니다.

Adobe Dynamic Media Classic에는 비디오 재생을 위해 사전 정의된 많은 뷰어 사전 설정이 포함되어 있으며 관리자인 경우 사용자 지정 뷰어 사전 설정을 만들 수 있습니다. 비디오 뷰어를 구성하기 위한 설정이 12개 이상 있습니다. 크기, 색상, 비디오 및 오디오 컨트롤, 진행률 표시줄, 사용자 인터페이스 스킨 및 소셜 기능을 구성할 수 있습니다.

다음을 참조하십시오 [비디오 뷰어에서 비디오 미리 보기](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer).

참조: [비디오 사전 설정](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) 교육 비디오입니다.

### 비디오 뷰어 사전 설정 추가 또는 편집 {#adding-or-editing-a-video-viewer-preset}

뷰어 사전 설정을 사용하여 다양한 뷰어 유형 및 사전 정의된 설정을 확인할 수 있습니다. 사용자 지정된 뷰어 사전 설정을 추가 및 편집하거나 Adobe Dynamic Media Classic과 함께 제공되는 기존 뷰어 사전 설정을 편집할 수도 있습니다.

[뷰어 사전 설정]에서 뷰어 사전 설정을 활성화, 필터링 및 정렬하고 미리 볼 수 있습니다.

[뷰어 사전 설정](application-setup.md#viewer_presets)을 참조하십시오.

참조: [비디오 사전 설정](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) 교육 비디오입니다.

**비디오 뷰어 사전 설정을 추가 또는 편집하려면:**

1. Adobe Dynamic Media Classic의 오른쪽 상단 모서리 근처에서 **[!UICONTROL 설정]** > **[!UICONTROL 뷰어 사전 설정]**.

   비디오 뷰어에 대한 사전 설정만 보려면 표 바로 위에 있는 도구 모음의 열린 뷰어 드롭다운 목록에서 비디오 뷰어 를 선택합니다.

1. 비디오 표시용 뷰어 사전 설정을 추가하거나 편집합니다.

   * **추가** - 선택 **[!UICONTROL 추가]** 을 클릭합니다. 뷰어 사전 설정 추가 대화 상자의 각 드롭다운 목록에서 플랫폼과 뷰어를 선택한 다음 를 선택합니다 **[!UICONTROL 추가]**.
   참조: [뷰어 사전 설정 추가 및 편집](application-setup.md#adding_and_editing_viewer_presets).

   * **기존 뷰어 사전 설정에서 시작하여 추가** - 표에서 비디오 뷰어 사전 설정을 선택한 다음 을 선택합니다. **[!UICONTROL 편집]** 을 클릭합니다.
   비디오 뷰어를 재구성한 후 다음을 선택합니다. **[!UICONTROL 다른 이름으로 저장]** [사전 설정 이름] 텍스트 필드에 다른 이름을 사용하여 사전 설정을 저장합니다.

   * **편집** - 비디오 뷰어 사전 설정을 선택한 다음 선택 **[!UICONTROL 편집]**.



1. 뷰어 구성 페이지의 사전 설정 이름 필드에 사전 설정 이름을 입력하거나 편집합니다.
1. 원하는 나머지 선택 사항을 설정합니다.

   옵션에 대한 설명을 보려면 해당 정보 팁 아이콘을 선택합니다.

1. 다음 중 하나를 수행하십시오.

   * 선택 **[!UICONTROL 다른 이름으로 저장]** 기존 사전 설정에서 시작하여 뷰어 사전 설정을 추가한 경우.
   * 선택 **[!UICONTROL 저장]** 뷰어 사전 설정을 추가하거나 편집한 경우.

>[!MORELIKETHIS]
>
>* [비디오 인코딩 우수 사례](uploading-encoding-videos.md#best_practices_for_video_encoding)
>* [비디오 인코딩 사전 설정 작업](uploading-encoding-videos.md#working_with_video_encoding_presets)

