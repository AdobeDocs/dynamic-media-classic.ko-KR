---
title: "빠른 시작: 템플릿 기본"
description: Adobe Dynamic Media Classic에서 빠르게 시작하고 실행할 수 있는 템플릿 기본 사항에 대한 소개 및 빠른 시작
uuid: 16d78cbb-f762-4263-aea9-5712eb933693
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: dd0fbb39-3f6a-496b-a9b6-63b11dcb823a
feature: Dynamic Media Classic
role: User
exl-id: bf695fee-821c-4396-829a-d57ccf475b0c
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 28%

---

# 빠른 시작: 템플릿 기본{#quick-start-template-basics}

템플릿 기본 사항은 Adobe Photoshop과 같은 이미지 편집 애플리케이션에서 계층화된 파일과 같이 동적으로 생성되고 주소 지정 가능한 계층화된 이미지 파일입니다. 레이어가 포함된 정적 파일(예: PSD 파일)과 달리 템플릿에는 매개 변수가 포함될 수 있습니다. 매개 변수를 통해 이미지의 각기 다른 측면을 다루고 사용자 지정할 수 있습니다.

한 템플릿에 이미지 레이어와 텍스트 레이어를 원하는 개수만큼 포함할 수 있습니다. 계층화된 PSD 파일과 같이 레이어가 포함된 정적 파일을 템플릿으로 변환하고 Adobe Dynamic Media Classic에서 템플릿을 만들 수 있습니다. Adobe Dynamic Media Classic에 업로드한 글꼴을 사용하여 템플릿에 텍스트 레이어를 만들 수 있습니다. 템플릿에 텍스트를 추가한 후 정렬, 글꼴, 글꼴 크기 및 색상을 변경하여 텍스트 서식을 지정할 수 있습니다.

매개변수 페이지를 사용하여 템플릿의 모든 측면을 대응 가능 매개변수로 변환할 수 있습니다. 이 과정에서 템플릿에 사용할 계층화된 이미지나 사용할 텍스트 값을 변경할 수 있습니다. 매개 변수는 URL 문자열과 함께 전달되므로 임의 매개 변수를 변경하여 이미지 서버에서 생성된 응답 이미지를 동적으로 사용자 지정할 수 있습니다.

참조: [템플릿 기본 사항](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) 교육 비디오입니다.

이 빠른 시작은 템플릿 기본 사항을 빠르게 시작하고 실행할 수 있도록 설계되었습니다.

## 1. 파일 업로드

먼저 템플릿에 사용할 PSD 파일이나 이미지 파일을 업로드합니다. Adobe Dynamic Media Classic은 PSD 외에도 다양한 이미지 파일 형식을 지원하지만 투명도를 위해 무손실 TIFF 및 PNG 이미지를 템플릿에 사용하는 것이 좋습니다.

PSD 파일을 사용하여 템플릿을 작성하는 경우 다음을 선택합니다 **[!UICONTROL 템플릿 만들기]** 다음에 있음 **[!UICONTROL 업로드 작업 옵션]** PSD 파일을 업로드할 때의 대화 상자입니다. 다음 항목도 선택 **[!UICONTROL 레이어 이름 지정]** 옵션을 사용하면 Adobe Dynamic Media Classic에서 PSD 레이어를 Adobe Dynamic Media Classic에 업로드할 때 이름을 지정하는 방법을 알 수 있습니다.

이미지 파일을 사용하는 경우에는 업로드할 때 이미지를 자르고 이미지의 클립 경로에서 표시를 만들 수도 있습니다.

전역 탐색 모음에서 를 선택합니다. **[!UICONTROL 업로드]** 컴퓨터에서 Adobe Dynamic Media Classic의 폴더로 PSD 파일 또는 기타 이미지 파일을 업로드합니다. 다음을 참조하십시오 [템플릿 파일 업로드](uploading-template-files.md#uploading_template_files).

## 2. 템플릿 만들기

PSD 파일에서 템플릿을 만들려면 다음을 선택합니다 **[!UICONTROL 템플릿 만들기]** 파일을 업로드할 때 이미지에서 템플릿을 만들려면 전역 탐색 모음에서 다음 위치로 이동합니다. **[!UICONTROL 빌드]** > **[!UICONTROL 템플릿 기본 사항]**, 캔버스의 너비 및 높이 측정값을 입력합니다. 페이지의 오른쪽 상단 모서리 근처에서 다음 중 하나를 선택합니다 **[!UICONTROL 디자이너]** 또는 **[!UICONTROL 개발자]**&#x200B;을 클릭하고 이미지를 템플릿 페이지로 드래그합니다. 이미지를 선택할 수도 있습니다 *다음 이전* (으)로 이동 **[!UICONTROL 빌드]** > **[!UICONTROL 템플릿 기본 사항]**. 템플릿 페이지는 다음 작업을 위한 도구를 제공합니다.

* 이미지 레이어 추가 레이어를 추가하려면 이미지를 템플릿 페이지로 드래그합니다.
* 텍스트 레이어 추가. 다음 항목 선택 **[!UICONTROL 텍스트 도구]** 아이콘. 포인터를 끌어 텍스트 레이어의 상자를 만든 다음 텍스트 페이지의 도구로 텍스트 서식을 지정합니다.
* 레이어 크기 및 위치 변경
* 레이어 순서 변경
* 이미지 및 텍스트 레이어에 그림자 및 후광 효과 적용

다음을 참조하십시오 [템플릿 만들기](creating-template.md#creating_a_template).

## 3. 템플릿 매개 변수 만들기

다음 단계에서는 레이어 속성을 매개 변수화하여 URL 문자열에 포함할 레이어 속성을 결정합니다. 매개 변수를 통해 템플릿을 최대한 유연하게 사용할 수 있습니다. 레이어 속성을 매개 변수로 만든 후 동적으로 변경할 수 있습니다.

레이어를 매개 변수화하려면 템플릿 페이지에서 템플릿을 연 다음 를 선택합니다 **[!UICONTROL 매개 변수]** 레이어 이름 옆에 있습니다. 매개변수 페이지에서 추가할 각 매개변수 옆의 옵션을 선택합니다. 다음을 참조하십시오 [템플릿 매개 변수 만들기](creating-template-parameters.md#creating_template_parameters).

## 4. 템플릿 게시

템플릿을 게시하면 템플릿이 Dynamic Media 이미지 서버에 배치되어 웹 사이트 또는 애플리케이션에 동적으로 전달될 수 있습니다. 또한 게시를 수행하면 Dynamic Media 이미지 서버에서 웹 사이트 또는 애플리케이션으로 템플릿을 호출하는 URL이 활성화됩니다.

템플릿과 관련된 모든 이미지를 게시해야 합니다.

템플릿을 게시하려면 게시로 표시하고 전역 탐색 모음에서 을 선택합니다. **[!UICONTROL 게시]**. 그런 다음 을 선택합니다 **[!UICONTROL 게시 제출]**. 다음을 참조하십시오 [템플릿 게시](publishing-templates.md#publishing_templates).

## 5. 웹 페이지에 템플릿 연결

Dynamic Media Classic은 템플릿에 대한 URL을 생성하고, 템플릿을 Dynamic Media 이미지 서버에 게시할 때 URL을 활성화합니다. 템플릿 미리 보기 페이지에서 이러한 URL 문자열을 복사할 수 있습니다.

찾아보기 패널에서 템플릿을 선택한 다음 을 선택합니다 **[!UICONTROL 미리 보기]** 템플릿 미리 보기 페이지를 엽니다. 템플릿을 게재할 이미지 사전 설정을 선택한 다음 을 선택합니다 **[!UICONTROL URL 복사]**. 미리보기 페이지에서 URL을 복사한 후에는 웹 사이트나 애플리케이션에서 사용할 수 있습니다. [템플릿을 웹 페이지에 연결](linking-template-web-page.md#linking_a_template_to_a_web_page)을 참조하십시오.
