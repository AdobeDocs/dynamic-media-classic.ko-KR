---
title: 이미지 집합을 웹 페이지에 연결
description: 이미지 세트를 웹 페이지에 연결하는 방법을 알아봅니다.
uuid: 8153a228-b2ec-4bc2-8996-266113a83df5
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: 40f4abab-9059-4d92-a761-f6d573b42e00
feature: Dynamic Media Classic,뷰어,이미지 세트
role: User
exl-id: df4e5218-2a66-413c-b247-b2a16d884041
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 89%

---

# 이미지 집합을 웹 페이지에 연결{#linking-an-image-set-to-a-web-page}

이미지 집합을 게시하면 웹 사이트 또는 애플리케이션에 사용할 해당 URL 또는 임베드 코드를 복사할 수 있습니다. 필요한 경우 URL을 배포하거나 임베드 코드를 붙여넣어 사용자가 웹 사이트 또는 애플리케이션에서 이미지 집합을 볼 수 있도록 합니다.

>[!NOTE]
>
>자산을 게시하기 전에는 URL이 활성화되지 않습니다.

## 이미지 집합 URL 복사 {#copying-an-image-set-url}

1. [자산 찾아보기] 패널의 [표시] 드롭다운 목록에서 **[!UICONTROL [이미지 집합]]**&#x200B;을 클릭합니다.
1. 왼쪽의 [자산 라이브러리] 패널에서 임베드 코드를 복사하려는 이미지 집합이 들어 있는 자산 폴더를 탐색합니다.
1. [자산 찾아보기] 패널 위의 도구 모음 오른쪽에서 다음 중 하나를 수행합니다.

   * **[!UICONTROL [그리드 보기]]**&#x200B;를 클릭합니다. [자산 찾아보기] 패널에서 단일 자산을 두 번 클릭하여 [세부 사항 보기]에서 엽니다. 오른쪽의 [URL 및 임베드 코드] 패널에서 원하는 뷰어의 오른쪽에 있는 **[!UICONTROL [URL 복사]]**&#x200B;를 클릭합니다.
   * **[!UICONTROL [그리드 보기]]**&#x200B;를 클릭합니다. [자산 찾아보기] 패널에서 단일 자산을 선택하고 썸네일 이미지 아래에서 **[!UICONTROL [미리 보기]]** > **[!UICONTROL [뷰어 목록]]**&#x200B;을 클릭합니다.

      [뷰어 목록] 페이지에 있는 테이블의 [작업] 열에서 **[!UICONTROL [URL 복사]]**&#x200B;를 클릭합니다.

   * **[!UICONTROL [목록 보기]]**&#x200B;를 클릭합니다. [자산 찾아보기] 패널에서 단일 자산을 선택하고 썸네일 이미지 오른쪽에서 **[!UICONTROL [미리 보기]]** > **[!UICONTROL [뷰어 목록]]**&#x200B;을 클릭합니다.

      [뷰어 목록] 페이지에 있는 테이블의 [작업] 열에서 **[!UICONTROL [URL 복사]]**&#x200B;를 클릭합니다.

   * **[!UICONTROL [그리드 보기]]**, **[!UICONTROL [목록 보기]]** 또는 **[!UICONTROL [세부 사항 보기]]**&#x200B;를 클릭합니다. 동일한 도구 모음에서 **[!UICONTROL [미리 보기]]** > **[!UICONTROL [뷰어 목록]]**&#x200B;을 클릭합니다.

      [뷰어 목록] 페이지에 있는 테이블의 [작업] 열에서 **[!UICONTROL [URL 복사]]**&#x200B;를 클릭합니다.

## 웹 페이지에 이미지 집합 URL 추가 {#adding-image-set-urls-to-your-web-page}

이미지 집합을 배포하는 가장 일반적인 방법은 탐색 아이콘을 통해 웹 페이지에 링크를 배치하는 것입니다. 클릭하면 팝업 확대/축소 창에 이미지 세트를 표시하는 JSP(동적 페이지)가 시작됩니다. 확대/축소 링크는 실제 확대/축소 기능이 포함된 팝업 창을 엽니다.

자세한 내용 및 코드 샘플은 Adobe 뷰어 참조 안내서](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/zoom/c-html5-20-zoom-viewer-about.html#section-e1c3106f5b3e445d9b95be337c2f94e2)에서 [HTML5 확대/축소 뷰어 포함 을 참조하십시오.

## 이미지 집합 뷰어의 임베드 코드 복사 {#copying-the-embed-code-of-an-image-set-viewer}

임베드 코드 기능을 사용하면 선택한 이미지 집합의 뷰어 코드를 검토할 수 있습니다. 또한 뷰어 배포를 위해 코드를 클립보드로 복사하여 웹 페이지에 붙여넣을 수도 있습니다. 코드 편집은 [임베드 코드] 대화 상자에서 허용되지 않습니다.

**이미지 집합 뷰어의 임베드 코드를 복사하려면:**

1. [자산 찾아보기] 패널의 [표시] 드롭다운 목록에서 **[!UICONTROL [이미지 집합]]**&#x200B;을 클릭합니다.
1. 왼쪽의 [자산 라이브러리] 패널에서 임베드 코드를 복사하려는 이미지 집합이 들어 있는 자산 폴더를 탐색합니다.
1. [자산 찾아보기] 패널 위의 도구 모음 오른쪽에서 다음 중 하나를 수행합니다.

   * **[!UICONTROL [그리드 보기]]**&#x200B;를 클릭합니다. [자산 찾아보기] 패널에서 단일 자산을 두 번 클릭하여 [세부 사항 보기]에서 엽니다. 오른쪽의 [URL] 패널에서 **[!UICONTROL [임베드 코드]]**&#x200B;를 클릭합니다.
   * **[!UICONTROL [그리드 보기]]**&#x200B;를 클릭합니다. [자산 찾아보기] 패널에서 단일 자산을 선택하고 썸네일 이미지 아래에서 **[!UICONTROL [미리 보기]]** > **[!UICONTROL [뷰어 목록]]**&#x200B;을 클릭합니다.

      [뷰어 목록] 페이지에 있는 테이블의 [작업] 열에서 **[!UICONTROL [임베드 코드]]**&#x200B;를 클릭합니다.

   * **[!UICONTROL [목록 보기]]**&#x200B;를 클릭합니다. [자산 찾아보기] 패널에서 단일 자산을 선택하고 썸네일 이미지 오른쪽에서 **[!UICONTROL [미리 보기]]** > **[!UICONTROL [뷰어 목록]]**&#x200B;을 클릭합니다.

      [뷰어 목록] 페이지에 있는 테이블의 [작업] 열에서 **[!UICONTROL [임베드 코드]]**&#x200B;를 클릭합니다.

   * **[!UICONTROL [그리드 보기]]**, **[목록 보기]** 또는 **[세부 사항 보기]**&#x200B;를 클릭합니다. 동일한 도구 모음에서 **[!UICONTROL [미리 보기]]** > **[!UICONTROL [뷰어 목록]]**&#x200B;을 클릭합니다.

      [뷰어 목록] 페이지에 있는 테이블의 [작업] 열에서 **[!UICONTROL [임베드 코드]]**&#x200B;를 클릭합니다.

1. [임베드 코드] 대화 상자에서 **[!UICONTROL [클립보드에 복사]]**&#x200B;를 클릭합니다.

   코드 편집은 [임베드 코드] 대화 상자에서 허용되지 않습니다.

1. **[!UICONTROL [닫기]]**&#x200B;를 클릭합니다.

>[!MORELIKETHIS]
>
>* [게시](publishing-files.md#publishing_files)

