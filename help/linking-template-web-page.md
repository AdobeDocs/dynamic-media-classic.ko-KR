---
title: 템플릿을 웹 페이지에 연결
seo-title: 템플릿을 웹 페이지에 연결
description: 널
seo-description: 템플릿을 웹 페이지에 연결하는 방법을 알아봅니다.
uuid: F 111 EF 06-4 AFC -454 C -86 CE -5 D 640236 D 40 B
contentOwner: 관리
content-type: 참조
products: sg_ Experiencemanager/dynamic-media-scene -7
geptopics: sg_ Scenesevenondemand_ pk/categories/template_ basics
discoiquuid: 989 dba 07-448 a -45 b 1-b 157-af 50 abb 5359 a
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# 템플릿을 웹 페이지에 연결{#linking-a-template-to-a-web-page}

웹 사이트와 애플리케이션은 URL 문자열을 통해 다이내믹 미디어 이미지 서버 컨텐츠에 액세스합니다. 템플릿을 게시하면 Dynamic Media Classic에서 다이내믹 미디어 이미지 서버의 템플릿을 참조하는 URL 문자열을 활성화합니다. 테스트를 위해 이 URL을 웹 브라우저에 붙여 넣을 수 있습니다.

웹 페이지와 애플리케이션에 URL 문자열을 배치하려면 Scene7 Publishing System에서 복사합니다. 이미지 사전 설정을 사용하여 생성된 템플릿 URL 문자열을 얻으려면 [미리 보기] 화면이나 찾아보기 패널([세부 사항 보기])로 이동합니다. 이미지 사전 설정을 선택한 다음 [URL 복사] 단추를 선택합니다.

>[!NOTE]
>
>자산을 게시하기 전에는 URL이 활성화되지 않습니다.

## 템플릿 URL 얻기 {#obtaining-a-template-url}

[템플릿 미리 보기] 화면에서 이미지 사전 설정에 의해 생성된 템플릿 URL 문자열을 얻을 수 있습니다. URL을 복사하면 필요한 경우 붙여 넣을 수 있도록 클립보드에 저장됩니다. [템플릿 미리 보기] 화면에서 이미지 사전 설정을 사용하여 생성된 템플릿 URL 문자열을 얻으려면 다음 단계를 수행합니다.

1. 템플릿의 롤오버 [미리 보기] 단추를 클릭하거나 [파일] &gt; [미리 보기]를 선택합니다. [미리 보기] 화면이 열립니다.
1. 사전 설정 메뉴를 사용하여 템플릿 이미지를 제공하는 데 사용할 이미지 사전 설정을 선택합니다. 서버에서 템플릿이 제공될 때의 템플릿 모양이 [미리 보기] 화면에 표시됩니다.
1. [URL 복사] 단추를 클릭하여 URL을 클립보드로 복사합니다.

## 웹 페이지에 템플릿 URL 추가 {#adding-template-urls-to-your-web-page}

To add a template to your web page, consult with your web page development team to modify the `<IMG>` tag in your HTML web page code using the Dynamic Media Classic URL string to make a request to Dynamic Media Image Servers. 상거래 엔진이나 동적 웹 페이지 코드는 템플릿에 대해 선택한 이미지 사전 설정에 정의된 크기 및 형식 지정 사양에 따라 템플릿 이미지를 삽입합니다.

>[!MORELIKETHIS]
>
>* [웹 페이지에 동적 이미지 추가](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)
