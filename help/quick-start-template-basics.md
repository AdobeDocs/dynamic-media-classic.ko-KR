---
title: '"빠른 시작: 템플릿 기본"'
description: 템플릿을 빠르게 시작하고 실행하는 데 도움이 되는 소개 및 빠른 시작 템플릿 기본 사항.
uuid: 16d78cbb-f762-4263-aea9-5712eb933693
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: dd0fbb39-3f6a-496b-a9b6-63b11dcb823a
feature: Dynamic Media Classic
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '789'
ht-degree: 71%

---


# Quick Start: Template Basics{#quick-start-template-basics}

Template Basics는 Adobe Photoshop과 같은 이미지 편집 응용 프로그램에서 레이어가 있는 파일과 같은 레이어가 있는 이미지 파일을 동적으로 만들고 주소 지정이 가능한 레이어가 있는 이미지 파일입니다. 레이어가 포함된 정적 파일(예: PSD 파일)과 달리 템플릿에는 매개 변수가 포함될 수 있습니다. 매개 변수를 통해 이미지의 각기 다른 측면을 다루고 사용자 지정할 수 있습니다.

한 템플릿에 이미지 레이어와 텍스트 레이어를 원하는 개수만큼 포함할 수 있습니다. 레이어가 포함된 정적 파일(예: 레이어로 구성된 PSD 파일)을 템플릿으로 변환할 수 있고 Dynamic Media Classic에서 템플릿을 만들 수 있습니다. Dynamic Media Classic에 업로드한 글꼴을 사용하여 템플릿에 텍스트 레이어를 만들 수 있습니다. 템플릿에 텍스트를 추가한 후 정렬, 글꼴, 글꼴 크기 및 색상을 변경하여 텍스트 서식을 지정할 수 있습니다.

[매개 변수] 화면을 사용하여 템플릿의 임의 측면을 주소 부여 가능한 매개 변수로 전환할 수 있습니다. 이 과정에서 템플릿에 사용할 계층화된 이미지나 사용할 텍스트 값을 변경할 수 있습니다. 매개 변수는 URL 문자열과 함께 전달되므로 임의 매개 변수를 변경하여 이미지 서버에서 생성된 응답 이미지를 동적으로 사용자 지정할 수 있습니다.

**빠른 시작**

이 빠른 시작은 템플릿 기본을 빨리 시작하고 실행하는 데 도움이 됩니다.

**1. 파일 업로드**

먼저 템플릿에 사용할 PSD 파일이나 이미지 파일을 업로드합니다. Dynamic Media Classic에서는 PSD 외에도 많은 이미지 파일 형식을 지원하지만 투명도를 위해 허용되는 손실 없는 TIFF 및 PNG 이미지가 템플릿에 권장됩니다.

PSD 파일을 사용하여 템플릿을 작성하는 경우 PSD 파일을 업로드할 때 [업로드 작업 선택 사항] 대화 상자에서 [템플릿 만들기] 선택 사항을 선택합니다. 또한 레이어 이름 지정 옵션을 선택하여 Dynamic Media Classic에 PSD 레이어를 업로드할 때 PSD 레이어의 이름을 지정하는 방법을 Dynamic Media Classic에 알려 줍니다.

이미지 파일을 사용하는 경우에는 업로드할 때 이미지를 자르고 이미지의 클립 경로에서 표시를 만들 수도 있습니다.

전역 탐색 막대에서 [업로드] 단추를 선택하여 컴퓨터에서 Dynamic Media Classic의 폴더로 PSD 파일이나 다른 이미지 파일을 업로드합니다. [템플릿 파일 업로드](uploading-template-files.md#uploading_template_files)를 참조하십시오.

**2. 템플릿 만들기**

PSD 파일에서 템플릿을 만들려면 파일을 업로드할 때 [템플릿 만들기] 선택 사항을 선택합니다. 이미지에서 템플릿을 만들려면 [작성] > [템플릿 기본]을 선택하고 캔버스의 너비 및 높이 측정값을 입력한 다음 [디자이너] 또는 [개발자]를 선택하고 이미지를 [템플릿] 화면으로 드래그합니다. [작성] > [템플릿 기본]을 선택하기 전에 이미지를 선택할 수도 있습니다. [템플릿] 화면에서는 다음 작업을 위한 도구를 제공합니다.

* 이미지 레이어 추가 레이어를 추가하려면 이미지를 [템플릿] 화면으로 드래그합니다.
* 텍스트 레이어 추가. [텍스트] 도구 를 선택하고 텍스트 레이어 상자를 끌어서 그린 다음 [텍스트] 화면의 도구를 사용하여 텍스트 서식을 지정합니다.
* 레이어 크기 및 위치 변경
* 레이어 순서 변경
* 이미지 및 텍스트 레이어에 그림자 및 후광 효과 적용

[ 템플릿 만들기hzw100](creating-template.md#creating_a_template)를 참조하십시오.

**3. 템플릿 매개 변수 만들기**

다음 단계에서는 레이어 속성을 매개 변수화하여 URL 문자열에 포함할 레이어 속성을 결정합니다. 매개 변수를 통해 템플릿을 최대한 유연하게 사용할 수 있습니다. 레이어 속성을 매개 변수로 만든 후 동적으로 변경할 수 있습니다.

레이어를 매개 변수화하려면 [템플릿] 화면에서 템플릿을 열고 레이어 이름 옆에 있는 [매개 변수] 단추를 선택합니다. [매개 변수] 화면에서 추가하려는 각 매개 변수 옆에 있는 선택 사항을 선택합니다. [템플릿 매개 변수 만들기](creating-template-parameters.md#creating_template_parameters)를 참조하십시오.

**4. 템플릿 게시**

템플릿을 게시하면 웹 사이트 또는 애플리케이션에 동적으로 전달할 수 있도록 Dynamic Media 이미지 서버에 템플릿이 배치됩니다. 또한 게시를 통해 Dynamic Media 이미지 서버의 템플릿을 웹 사이트 또는 응용 프로그램으로 호출하도록 URL을 활성화합니다.

템플릿과 관련된 모든 이미지를 게시해야 합니다.

템플릿을 게시하려면 게시로 표시하고 글로벌 탐색 막대에서 [게시] 단추를 선택합니다. 그런 다음 [게시 시작] 단추를 선택합니다. [템플릿 게시](publishing-templates.md#publishing_templates)를 참조하십시오.

**5. 템플릿을 웹 페이지에 연결**

Dynamic Media Classic에서는 템플릿을 Dynamic Media 이미지 서버에 게시할 때 템플릿에 대한 URL을 만들고 URL을 활성화합니다. [템플릿 미리 보기] 화면에서 이러한 URL 문자열을 복사할 수 있습니다.

찾아보기 패널에서 템플릿을 선택하고 [미리 보기] 단추를 클릭하여 [템플릿 미리 보기] 화면을 엽니다. 템플릿 제공 시 사용할 이미지 사전 설정을 선택한 다음 [URL 복사] 단추를 선택합니다. [미리 보기] 화면에서 URL을 복사한 후 웹 사이트나 애플리케이션에서 사용할 수 있습니다. [템플릿을 웹 페이지에 연결](linking-template-web-page.md#linking_a_template_to_a_web_page)을 참조하십시오.
