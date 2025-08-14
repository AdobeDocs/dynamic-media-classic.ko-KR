---
title: '빠른 시작: 템플릿 기본'
description: Adobe Dynamic Media Classic에서 빠르게 시작하고 실행할 수 있는 템플릿 기본 사항에 대한 소개 및 빠른 시작
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: bf695fee-821c-4396-829a-d57ccf475b0c
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 17%

---

# 빠른 시작: 템플릿 기본{#quick-start-template-basics}

템플릿 기본 사항은 Adobe Photoshop과 같은 이미지 편집 애플리케이션에서 계층화된 파일과 같이 동적으로 생성되고 주소 지정 가능한 계층화된 이미지 파일입니다. 레이어가 포함된 정적 파일(예: PSD 파일)과 달리 템플릿에는 매개 변수가 포함될 수 있습니다. 매개 변수를 통해 이미지의 각기 다른 측면을 다루고 사용자 지정할 수 있습니다.

한 템플릿에 이미지 레이어와 텍스트 레이어를 원하는 개수만큼 포함할 수 있습니다. 계층화된 PSD 파일과 같이 레이어가 포함된 정적 파일을 템플릿으로 변환하고 Adobe Dynamic Media Classic에서 템플릿을 만들 수 있습니다. Adobe Dynamic Media Classic에 업로드한 글꼴을 사용하여 템플릿에 텍스트 레이어를 만들 수 있습니다. 서식 파일에 텍스트를 추가한 후 정렬, 글꼴, 글꼴 크기 및 색상을 변경하여 서식 지정할 수 있습니다.

매개변수 페이지를 사용하여 템플릿의 모든 측면을 대응 가능 매개변수로 변환할 수 있습니다. 이렇게 하면 사용할 계층화된 이미지 또는 템플릿에서 사용할 텍스트 값을 변경할 수 있습니다. 매개 변수가 URL 문자열과 함께 전달되므로 이미지 서버에서 생성된 응답 이미지를 동적으로 사용자 지정할 수 있습니다.

[템플릿 기본 사항](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) 교육 비디오도 참조하세요.

이 빠른 시작은 템플릿 기본 사항을 빠르게 시작하고 실행할 수 있도록 설계되었습니다.

## &#x200B;1. 파일 업로드

먼저 템플릿에 사용할 PSD 파일이나 이미지 파일을 업로드합니다. Adobe Dynamic Media Classic은 PSD 외에도 다양한 이미지 파일 형식을 지원하지만 투명성을 위해 무손실 TIFF 및 PNG 이미지를 템플릿에 사용하는 것이 좋습니다.

PSD 파일을 사용하여 템플릿을 만드는 경우 PSD 파일을 업로드할 때 **[!UICONTROL 업로드 작업 옵션]** 대화 상자에서 **[!UICONTROL 템플릿 만들기]**&#x200B;를 선택합니다. 또한 **[!UICONTROL 레이어 이름 지정]** 옵션을 선택하면 Adobe Dynamic Media Classic에서 PSD 레이어를 Adobe Dynamic Media Classic에 업로드할 때 레이어 이름을 지정할 수 있습니다.

이미지 파일을 사용하는 경우 이미지를 자를 수 있으며, 이미지를 업로드할 때 이미지의 클리핑 패스에서 마스크를 만들 수도 있습니다.

전역 탐색 모음에서 **[!UICONTROL 업로드]**&#x200B;를 선택하여 컴퓨터의 PSD 파일 또는 기타 이미지 파일을 Adobe Dynamic Media Classic의 폴더로 업로드합니다. [템플릿 파일 업로드](uploading-template-files.md#uploading_template_files)를 참조하십시오.

## &#x200B;2. 템플릿 만들기

PSD 파일에서 템플릿을 만들려면 파일을 업로드할 때 **[!UICONTROL 템플릿 만들기]**&#x200B;를 선택합니다. 이미지에서 템플릿을 만들려면 전역 탐색 모음에서 **[!UICONTROL 빌드]** > **[!UICONTROL 템플릿 기본 사항]**(으)로 이동하여 캔버스의 너비와 높이 측정값을 입력하십시오. 페이지의 오른쪽 상단 모서리에서 **[!UICONTROL Designer]** 또는 **[!UICONTROL 개발자]**&#x200B;를 선택하고 이미지를 템플릿 페이지로 끕니다. *빌드* > **[!UICONTROL 템플릿 기본 사항]**(으)로 이동하여 **[!UICONTROL 이전]** 이미지를 선택할 수도 있습니다. 템플릿 페이지는 다음 작업을 위한 도구를 제공합니다.

* 이미지 레이어 추가 레이어를 추가하려면 이미지를 템플릿 페이지로 드래그합니다.
* 텍스트 레이어 추가. **[!UICONTROL 텍스트 도구]** 아이콘을 선택합니다. 포인터를 끌어 텍스트 레이어의 상자를 만든 다음 텍스트 페이지의 도구를 사용하여 텍스트 서식을 지정합니다.
* 레이어 크기 및 위치 변경
* 레이어 순서 변경
* 이미지 및 텍스트 레이어에 그림자 및 후광 효과 적용

[템플릿 만들기](creating-template.md#creating_a_template)를 참조하십시오.

## &#x200B;3. 템플릿 매개 변수 만들기

다음 단계에서는 레이어 속성을 매개 변수화하여 URL 문자열에 포함할 레이어 속성을 결정합니다. 매개 변수를 통해 템플릿을 최대한 유연하게 사용할 수 있습니다. 레이어 속성을 매개 변수로 만든 후 동적으로 변경할 수 있습니다.

레이어를 매개 변수화하려면 템플릿 페이지에서 템플릿을 연 다음 레이어 이름 옆에 있는 **[!UICONTROL 매개 변수]**&#x200B;을 선택합니다. 매개변수 페이지에서 추가할 각 매개변수 옆의 옵션을 선택합니다. [템플릿 매개 변수 만들기](creating-template-parameters.md#creating_template_parameters)를 참조하십시오.

## &#x200B;4. 템플릿 게시

템플릿을 게시하면 템플릿이 Dynamic Media 이미지 서버에 배치되어 웹 사이트 또는 애플리케이션에 동적으로 전달될 수 있습니다. 또한 게시를 수행하면 Dynamic Media 이미지 서버에서 웹 사이트 또는 애플리케이션으로 템플릿을 호출하는 URL이 활성화됩니다.

템플릿과 관련된 모든 이미지를 게시해야 합니다.

템플릿을 게시하려면 게시용으로 표시하고 전역 탐색 모음에서 **[!UICONTROL 게시]**&#x200B;를 선택합니다. 그런 다음 **[!UICONTROL 게시 제출]**&#x200B;을 선택합니다. [템플릿 게시](publishing-templates.md#publishing_templates)를 참조하십시오.

## &#x200B;5. 웹 페이지에 템플릿 연결

Dynamic Media Classic은 템플릿에 대한 URL을 생성하고, 템플릿을 Dynamic Media 이미지 서버에 게시할 때 URL을 활성화합니다. 템플릿 미리 보기 페이지에서 이러한 URL 문자열을 복사할 수 있습니다.

[찾아보기] 패널에서 템플릿을 선택한 다음 **[!UICONTROL 미리 보기]**&#x200B;를 선택하여 [템플릿 미리 보기] 페이지를 엽니다. 템플릿을 전달할 이미지 사전 설정을 선택한 다음 **[!UICONTROL URL 복사]** 단추를 클릭합니다. 미리보기 페이지에서 URL을 복사한 후에는 웹 사이트나 애플리케이션에서 사용할 수 있습니다. [웹 페이지에 템플릿 연결](linking-template-web-page.md#linking_a_template_to_a_web_page)을 참조하십시오.
