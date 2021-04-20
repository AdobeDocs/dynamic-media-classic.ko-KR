---
title: 템플릿을 웹 페이지에 연결
description: 템플릿을 웹 페이지에 연결하는 방법을 알아봅니다.
uuid: f111ef06-4afc-454c-86ce-5d640236d40b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 989dba07-448a-45b1-b157-af50abb5359a
feature: Dynamic Media Classic
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 68%

---


# 템플릿을 웹 페이지에 연결{#linking-a-template-to-a-web-page}

웹 사이트와 애플리케이션은 URL 문자열을 통해 Dynamic Media Image Server 컨텐츠에 액세스합니다. 템플릿을 게시하면 Dynamic Media Classic에서 Dynamic Media 이미지 서버의 템플릿을 참조하는 URL 문자열을 활성화합니다. 테스트를 위해 이 URL을 웹 브라우저에 붙여 넣을 수 있습니다.

웹 페이지 및 응용 프로그램에 URL 문자열을 배치하려면 Dynamic Media Classic에서 복사합니다. 이미지 사전 설정을 사용하여 생성된 템플릿 URL 문자열을 얻으려면 [미리 보기] 화면이나 찾아보기 패널([세부 사항 보기])로 이동합니다. 이미지 사전 설정을 선택한 다음 [URL 복사] 단추를 선택합니다.

>[!NOTE]
>
>자산을 게시하기 전에는 URL이 활성화되지 않습니다.

## 템플릿 URL 얻기 {#obtaining-a-template-url}

[템플릿 미리 보기] 화면에서 이미지 사전 설정에 의해 생성된 템플릿 URL 문자열을 얻을 수 있습니다. URL을 복사하면 필요한 경우 붙여 넣을 수 있도록 클립보드에 저장됩니다. [템플릿 미리 보기] 화면에서 이미지 사전 설정을 사용하여 생성된 템플릿 URL 문자열을 얻으려면 다음 단계를 수행합니다.

1. 템플릿의 롤오버 [미리 보기] 단추를 클릭하거나 [파일] > [미리 보기]를 선택합니다. [미리 보기] 화면이 열립니다.
1. 사전 설정 메뉴를 사용하여 템플릿 이미지를 제공하는 데 사용할 이미지 사전 설정을 선택합니다. 서버에서 템플릿이 제공될 때의 템플릿 모양이 [미리 보기] 화면에 표시됩니다.
1. [URL 복사] 단추를 클릭하여 URL을 클립보드로 복사합니다.

## 웹 페이지에 템플릿 URL 추가  {#adding-template-urls-to-your-web-page}

웹 페이지에 템플릿을 추가하려면 웹 페이지 개발 팀과 협의하여 Dynamic Media Classic URL 문자열을 사용하여 HTML 웹 페이지 코드의 `<IMG>` 태그를 수정하여 Dynamic Media 이미지 서버에 요청합니다. 상거래 엔진이나 동적 웹 페이지 코드는 템플릿에 대해 선택한 이미지 사전 설정에 정의된 크기 및 형식 지정 사양에 따라 템플릿 이미지를 삽입합니다.

>[!MORELIKETHIS]
>
>* [웹 페이지에 동적 이미지 추가](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)

