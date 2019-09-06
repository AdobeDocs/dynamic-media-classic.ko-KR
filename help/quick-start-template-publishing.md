---
title: '" 빠른 시작: 템플릿 게시 "'
seo-title: '" 빠른 시작: 템플릿 게시 "'
description: 널
seo-description: 빠르게 시작하는 데 도움이 되는 템플릿 게시 소개 및 빠른 시작을 소개합니다.
uuid: 101 B 6211-2421-4565-8635-944315 A 5 C 512
contentOwner: 관리
content-type: 참조
products: sg_ Experiencemanager/dynamic-media-scene -7
geptopics: sg_ scenesevenondemand_ pk/categories/template-publishing
discoiquuid: 03671 fc 1-ce 3 b -4 fae-ad 1 f -53 c 99 abcabde
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Quick Start: Template publishing{#quick-start-template-publishing}

Adobe Dynamic Media Classic Web-to-Print를 사용하면 고객, 클라이언트 및 교직원이 손쉽게 원하는 대로 구성하고 개인화할 수 있는 전문적으로 브랜드화된 인쇄 컨텐츠를 제작할 수 있습니다. 게시 프로세스 전체에서 회사 컨텐츠와 브랜드 ID를 유지할 수 있습니다. 최종 사용자는 인쇄물 컨텐츠를 사용자 지정할 수 있지만 사용자 지정이 허용된 컨텐츠 부분에서만 가능합니다. 제공할 수 있는 사용자 지정 인쇄물 제품의 예로 개인 설정 편지지, 명함, 포스터, 인사말 카드, 레이블, 수표, 선물, 의류, 달력, 스크랩북, 사진 앨범 등이 있습니다. 회사는 여러 지역, 프랜차이즈, 매장 및 지점에 맞게 사용자 지정할 수 있는 홍보물에서 공통 브랜드 ID를 유지할 수 있습니다.

먼저 Adobe Illustrator에서 템플릿을 디자인합니다. 템플릿은 상수 항목과 변수 항목(사용자 지정할 수 있는 변수 구성 요소)을 신중하게 정의합니다. 예를 들어 Illustrator 파일의 텍스트를 매개 변수화하면 최종 사용자가 고유한 텍스트를 입력할 수 있습니다. 마찬가지로, 변수 구성 요소로 매개 변수화한 후 배경색을 다른 배경색으로 바꿀 수 있습니다.

Dynamic Media Classic는 기본 사용 사례와 고급 사용 사례에 대한 두 가지 템플릿 게시 워크플로우를 제공합니다. 기본적인 사용 사례는 Adobe Illustrator에서 디자인을 만들고, Dynamic Media Classic에 업로드하고, SPS에서 매개 변수를 사용하여 변수 요소를 정의하는 것입니다. 고급 사용 사례에는 보다 포괄적인 가변성 정의가 필요합니다. 고급 사용 사례는 Adobe Illustrator에서 변수 요소를 만들고, 파일을 Dynamic Media Classic에 업로드하고, URL 호출을 사용하여 XML 수준에서 해당 요소를 직접 조작하는 것입니다. *`*DOM manipulation*`*&#x200B;이 시나리오가 호출됩니다.

>[!NOTE]
>
>For more information about Dynamic Media Classic web-to-print workflows, template creation, parameterization, DOM manipulation, and more, see the Web-to-Print Workflow Guide here: [www.adobe.com/go/learn_s7_webtoprint_en](https://www.adobe.com/go/learn_s7_webtoprint_en) . zip 파일을 로컬 하드 드라이브에 다운로드하고 해당 컨텐츠를 추출합니다 (Dynamic Media Classic Web-to-printworkflow 자습서 문서 및 자습서 에셋).

**빠른 시작**

이 빠른 시작에서는 Illustrator 파일을 사용하여 사용자 지정 가능한 고품질 인쇄 제품을 만드는 기본 워크플로우에 대해 설명합니다.

**1. 템플릿 게시에 사용할 Illustrator 파일 디자인**

Illustrator에서 템플릿을 디자인합니다. 고급 DOM 조작 방법을 사용하여 템플릿을 사용자 지정하려는 경우 Illustrator에서 변수 요소의 s7:elementID를 정의합니다.

[Illustrator에서 초기 템플릿 만들기](create-initial-template-illustrator.md#create_the_initial_template_in_illustrator) 및 [DOM 조작](dom-manipulation.md#dom_manipulation)을 참조하십시오.

**2. Convert your template to Dynamic Media Classic FXG and upload it to Scene7 Publishing System**

Adobe Creative Cloud 사용자는 W2P(Web to Print)용 Adobe Illustrator 플러그인을 사용할 수 있습니다. 이 플러그인은 템플릿을 Dynamic Media Classic FXG로 변환합니다. 템플릿에 글꼴이 포함되어 있는 경우 FXG 파일을 업로드하기 전에 해당 글꼴 파일을 Scene7 Publishing System에 업로드해야 합니다.

[템플릿 게시에 사용할 파일 업로드](upload-files-template-publishing.md#upload_files_for_template_publishing)를 참조하십시오.

**3. Dynamic Media Classic에서 매개 변수 보기, 정의 또는 다듬기**

[템플릿 게시 미리 보기] 및 [작성] 화면에서 매개 변수를 통해 변수 요소를 정의 및 구체화하고, 결과를 미리 보고 테스트할 수 있습니다. 이 화면에서 다음 작업을 수행할 수 있습니다.

* 매개 변수를 만들고 수정합니다.
* 매개 변수 속성과 특성의 기본값을 지정합니다.
* [URL 복사]를 클릭하여 미리 보기 URL을 클립보드로 복사하고 브라우저 창에서 결과를 미리 봅니다.

Dynamic Media Classic에서 템플릿 [매개 변수화를 참조하십시오](parameterizing-template-scene7.md#parameterizing_a_template_in_scene7).

**4. FXG 템플릿 게시**

매개 변수 및 특성 정의와 테스트를 마쳤으면 파일을 게시합니다. FXG 템플릿을 게시하면 다이내믹 미디어 이미지 서버에 배치되고 URL 이 활성화됩니다.

FXG 템플릿과 관련된 모든 이미지 및 글꼴을 게시해야 합니다.

[FXG 템플릿 게시](dom-manipulation.md#publish_fxg_templates)를 참조하십시오.

**5. URL 얻기**

이제 최종 사용자가 변수 컨텐츠를 개인 설정할 수 있도록 URL을 통해 웹 사이트에 템플릿을 포함할 준비가 되었습니다.

[FXG 템플릿을 웹 페이지에 연결](linking-fxg-template-web-page.md#linking_an_fxg_template_to_a_web_page)을 참조하십시오.
