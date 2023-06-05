---
title: 웹 페이지에 확대/축소 뷰어 연결
description: Adobe Dynamic Media Classic에서 Zoom 뷰어를 웹 페이지에 연결하는 방법에 대해 알아봅니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: 2073d95b-1600-481f-8038-d29e8acacf7d
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '685'
ht-degree: 34%

---

# 웹 페이지에 확대/축소 뷰어 연결{#linking-zoom-viewers-to-your-web-pages}

웹 사이트 및 애플리케이션은 URL 문자열 또는 포함된 코드를 통해 기본 이미지 및 관련 확대/축소 대상, 확대/축소 뷰어 사전 설정 등 Dynamic Media Image Server 콘텐츠에 액세스합니다. 이러한 URL 문자열은 게시 프로세스 중에 활성화됩니다. 이러한 URL 문자열 또는 포함된 코드를 웹 페이지 및 애플리케이션에 배치하려면 Adobe Dynamic Media Classic에서 해당 문자열을 복사합니다.

>[!NOTE]
>
>자산을 게시하기 전에는 URL이 활성화되지 않습니다.

## 확대/축소 뷰어 URL 복사 {#copying-a-zoom-viewer-url}

1. 왼쪽의 [자산 라이브러리] 패널에서 URL을 복사하려는 확대/축소 뷰어가 들어 있는 자산 폴더를 탐색합니다.
1. [자산 찾아보기] 패널 위의 도구 모음 오른쪽에서 다음 중 하나를 수행합니다.

   * 선택 **[!UICONTROL 격자 보기]** 또는 **[!UICONTROL 목록 보기]**. [자산 찾아보기] 패널에서 단일 자산을 두 번 클릭하여 [세부 사항 보기]에서 엽니다. 오른쪽의 URL 및 포함 코드 패널에서 을 선택합니다. **[!UICONTROL URL 복사]** 원하는 뷰어의 오른쪽에 있습니다.
   * 선택 **[!UICONTROL 격자 보기]**. 에셋 찾아보기 패널에서 단일 에셋을 선택한 다음 썸네일 이미지 아래에서 **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**.

      뷰어 목록 페이지의 테이블에 있는 작업 열에서 을 선택합니다. **[!UICONTROL URL 복사]**.

   * 선택 **[!UICONTROL 목록 보기]**. 에셋 찾아보기 패널에서 단일 에셋을 선택한 다음 썸네일 이미지의 오른쪽으로 이동합니다. **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**.

      뷰어 목록 페이지의 테이블에 있는 작업 열에서 을 선택합니다. **[!UICONTROL URL 복사]**.

   * 선택 **[!UICONTROL 격자 보기]**, **[!UICONTROL 목록 보기]**, 또는 **[!UICONTROL 세부 사항 보기]**. 동일한 도구 모음에서 다음 위치로 이동합니다. **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**.

      뷰어 목록 페이지의 테이블에 있는 작업 열에서 을 선택합니다. **[!UICONTROL URL 복사]**.

## 웹 페이지에 확대/축소 뷰어 URL 추가 {#adding-zoom-viewer-urls-to-your-web-page}

일반적으로 방문자는 먼저 확대/축소 아이콘을 선택하여 웹 사이트에서 이미지를 확대/축소합니다(종종 아이콘에 확대경의 이미지가 표시됨). 이 아이콘을 선택하면 팝업 창에서 이미지를 표시하는 동적 웹 페이지(ASP 또는 JSP)가 시작됩니다. 방문자는 실제로 이 팝업 창에서 이미지를 확대/축소합니다.

자세한 내용 및 코드 샘플은 [Adobe 뷰어 참조 안내서의 HTML 5 기본 확대/축소 뷰어 포함](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/basic-zoom/c-html5-20-basic-zoom-viewer-about.html#section-e1c3106f5b3e445d9b95be337c2f94e2).

## 확대/축소 뷰어의 포함 복사본 복사 {#copying-the-embed-copy-of-a-zoom-viewer}

임베드 코드 기능을 사용하면 선택한 확대/축소 뷰어의 뷰어 코드를 검토할 수 있습니다. 또한 뷰어 배포를 위해 코드를 클립보드로 복사하여 웹 페이지에 붙여넣을 수도 있습니다. 코드 편집은 [임베드 코드] 대화 상자에서 허용되지 않습니다.

**확대/축소 뷰어의 임베드 코드를 복사하려면:**

1. 왼쪽의 [자산 라이브러리] 패널에서 임베드 코드를 복사하려는 확대/축소 뷰어가 들어 있는 자산 폴더를 탐색합니다.
1. [자산 찾아보기] 패널 위의 도구 모음 오른쪽에서 다음 중 하나를 수행합니다.

   * 선택 **[!UICONTROL 격자 보기]**. [자산 찾아보기] 패널에서 단일 자산을 두 번 클릭하여 [세부 사항 보기]에서 엽니다. 오른쪽의 URL 및 포함 코드 패널에서 을 선택합니다. **[!UICONTROL 포함 코드]** 원하는 뷰어의 오른쪽에 있습니다.
   * 선택 **[!UICONTROL 격자 보기]**. 에셋 찾아보기 패널에서 단일 에셋을 선택한 다음 썸네일 이미지 아래에서 **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**.

      뷰어 목록 페이지의 테이블에 있는 작업 열에서 을 선택합니다. **[!UICONTROL 포함 코드]**.

   * 선택 **[!UICONTROL 목록 보기]**. 에셋 찾아보기 패널에서 단일 에셋을 선택한 다음 썸네일 이미지의 오른쪽으로 이동합니다. **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**.

      뷰어 목록 페이지의 테이블에 있는 작업 열에서 을 선택합니다. **[!UICONTROL 포함 코드]**.

   * 선택 **[!UICONTROL 격자 보기]**, **[!UICONTROL 목록 보기]**, 또는 **[!UICONTROL 세부 사항 보기]**. 동일한 도구 모음에서 다음 위치로 이동합니다. **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**.

      뷰어 목록 페이지의 테이블에 있는 작업 열에서 을 선택합니다. **[!UICONTROL 포함 코드]**.

1. 포함 코드 대화 상자에서 **[!UICONTROL 클립보드에 복사]**.

   코드 편집은 [임베드 코드] 대화 상자에서 허용되지 않습니다.

1. 선택 **[!UICONTROL 닫기]**.
