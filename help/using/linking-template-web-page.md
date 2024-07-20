---
title: 웹 페이지에 템플릿 연결
description: Adobe Dynamic Media Classic에서 웹 페이지에 템플릿을 연결하는 방법을 알아봅니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: 6305c287-360f-48c2-b456-58be0791c7af
topic: Administration, Content Management, Development
level: Experienced
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 16%

---

# 웹 페이지에 템플릿 연결{#linking-a-template-to-a-web-page}

웹 사이트 및 애플리케이션은 URL 문자열을 통해 Dynamic Media Image Server 콘텐츠에 액세스합니다. 템플릿을 게시하면 Adobe Dynamic Media Classic이 Dynamic Media 이미지 서버에서 템플릿을 참조하는 URL 문자열을 활성화합니다. 테스트를 위해 이 URL을 웹 브라우저에 붙여넣을 수 있습니다.

웹 페이지 및 애플리케이션에 URL 문자열을 배치하려면 Adobe Dynamic Media Classic에서 해당 문자열을 복사합니다. 이미지 사전 설정으로 생성된 템플릿 URL 문자열을 가져오려면 미리 보기 화면 또는 찾아보기 패널(자세히 보기)로 이동합니다. 이미지 사전 설정을 선택한 다음 [URL 복사] 단추를 선택합니다.

>[!NOTE]
>
>자산을 게시하기 전에는 URL이 활성화되지 않습니다.

## 템플릿 URL 얻기 {#obtaining-a-template-url}

[템플릿 미리 보기] 화면에서 이미지 사전 설정에 의해 생성된 템플릿 URL 문자열을 얻을 수 있습니다. URL을 복사하면 필요한 경우 붙여 넣을 수 있도록 클립보드에 저장됩니다. [템플릿 미리 보기] 페이지에서 이미지 사전 설정으로 생성된 템플릿 URL 문자열을 가져오려면 다음을 수행합니다.

1. 템플릿의 롤오버 **[!UICONTROL 미리 보기]** 단추를 선택하거나 **[!UICONTROL 파일]** > **[!UICONTROL 미리 보기]**(으)로 이동합니다.
1. [사전 설정] 메뉴를 사용하여 템플릿 이미지를 전달할 이미지 사전 설정을 선택합니다. 미리보기 페이지에는 템플릿이 서버에서 전달될 때의 모양이 표시됩니다.
1. URL을 클립보드에 복사하려면 **[!UICONTROL URL 복사]**&#x200B;를 선택하십시오.

## 웹 페이지에 템플릿 URL 추가 {#adding-template-urls-to-your-web-page}

웹 페이지에 템플릿을 추가하려면 웹 페이지 개발 팀에 문의하여 HTML 웹 페이지 코드의 `<IMG>` 태그를 수정하십시오. Adobe Dynamic Media Classic URL 문자열을 사용하여 Dynamic Media 이미지 서버에 요청합니다. 상거래 엔진 또는 동적 웹 페이지 코드는 템플릿의 이미지 사전 설정에서 정의한 서식 지정 사양과 함께 템플릿 이미지를 삽입합니다.

>[!MORELIKETHIS]
>
>* [웹 페이지에 동적 이미지 추가](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)
