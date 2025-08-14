---
title: 웹 페이지에 견본 집합 연결
description: Adobe Dynamic Media Classic에서 웹 페이지에 견본 세트를 연결하는 방법을 알아봅니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/swatch_sets
feature: Dynamic Media Classic,Viewers
role: User
exl-id: 8bb1c744-270a-4752-b163-443708fca6c2
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 16%

---

# 웹 페이지에 견본 집합 연결{#linking-a-swatch-set-to-a-web-page}

견본 집합을 게시한 후에는 웹 사이트 또는 애플리케이션에서 연결된 URL 또는 포함 코드를 사용할 수 있습니다. 그런 다음 필요에 따라 URL 또는 포함 코드를 배포하여 사용자가 웹 사이트 또는 애플리케이션에서 견본 세트를 볼 수 있도록 할 수 있습니다.

>[!NOTE]
>
>자산을 게시하기 전에는 URL이 활성화되지 않습니다.

## 견본 집합 URL 복사 {#copying-a-swatch-set-url}

1. [자산 찾아보기] 패널의 [표시] 드롭다운 목록에서 **[!UICONTROL 견본 집합]**&#x200B;을 선택합니다.
1. 왼쪽의 에셋 라이브러리 패널에서 포함 코드를 복사할 견본 세트가 포함된 에셋 폴더로 이동합니다.
1. [자산 찾아보기] 패널 위의 도구 모음 오른쪽에서 다음 중 하나를 수행합니다.

   * **[!UICONTROL 눈금 보기]**&#x200B;를 선택합니다. [자산 찾아보기] 패널에서 단일 자산을 두 번 클릭하여 [세부 사항 보기]에서 엽니다. 오른쪽의 URL 및 포함 코드 패널에서 원하는 뷰어의 오른쪽에 있는 **[!UICONTROL URL 복사]**&#x200B;를 선택합니다.
   * **[!UICONTROL 눈금 보기]**&#x200B;를 선택합니다. [에셋 찾아보기] 패널에서 단일 에셋을 선택한 다음 썸네일 이미지 아래에서 **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**(으)로 이동합니다.

     뷰어 목록 페이지의 표에 있는 작업 열에서 **[!UICONTROL URL 복사]**&#x200B;를 선택합니다.

   * **[!UICONTROL 목록 보기]**&#x200B;를 선택합니다. [에셋 찾아보기] 패널에서 단일 에셋을 선택한 다음 썸네일 이미지의 오른쪽에 있는 **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**(으)로 이동합니다.

     뷰어 목록 페이지의 표에 있는 작업 열에서 **[!UICONTROL URL 복사]**&#x200B;를 선택합니다.

   * **[!UICONTROL 눈금 보기]**, **[!UICONTROL 목록 보기]** 또는 **[!UICONTROL 자세히 보기]**&#x200B;를 선택하십시오. 같은 도구 모음에서 **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**(으)로 이동합니다.

     뷰어 목록 페이지의 표에 있는 작업 열에서 **[!UICONTROL URL 복사]**&#x200B;를 선택합니다.

## 웹 페이지에 견본 집합 URL 추가 {#adding-swatch-set-urls-to-your-web-page}

견본 집합을 배포하는 가장 일반적인 방법은 웹 페이지에 링크(탐색 아이콘 사용)를 배치하는 것입니다. 이 옵션을 선택하면 팝업 확대/축소 창에 견본 세트를 표시하는 동적 페이지(ASP 또는 JSP)가 시작됩니다. 확대/축소 링크를 클릭하면 실제 확대/축소 기능이 포함된 팝업 창이 열립니다.

자세한 내용 및 코드 샘플은 Adobe 뷰어 참조 가이드의 [HTML5 확대/축소 뷰어 포함](https://experienceleague.adobe.com/ko/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/zoom/c-html5-20-zoom-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2)을 참조하십시오.

## 견본 집합 뷰어의 포함 코드 복사 {#copying-the-embed-code-of-a-swatch-set-viewer}

임베드 코드 기능을 사용하면 선택한 견본 집합의 뷰어 코드를 검토할 수 있습니다. 또한 코드를 클립보드에 복사하여 뷰어의 배포를 위해 웹 페이지에 붙여넣을 수 있습니다. 코드 편집은 [임베드 코드] 대화 상자에서 허용되지 않습니다.

**견본 집합 뷰어의 포함 코드를 복사하려면:**

1. [자산 찾아보기] 패널의 [표시] 드롭다운 목록에서 **[!UICONTROL 견본 집합]**&#x200B;을 선택합니다.
1. 왼쪽의 에셋 라이브러리 패널에서 포함 코드를 복사할 견본 세트가 포함된 에셋 폴더로 이동합니다.
1. [자산 찾아보기] 패널 위의 도구 모음 오른쪽에서 다음 중 하나를 수행합니다.

   * **[!UICONTROL 눈금 보기]**&#x200B;를 선택합니다. [자산 찾아보기] 패널에서 단일 자산을 두 번 클릭하여 [세부 사항 보기]에서 엽니다. 오른쪽의 URL 및 포함 코드 패널에서 원하는 뷰어의 오른쪽에 있는 **[!UICONTROL 포함 코드]**&#x200B;를 선택합니다.
   * **[!UICONTROL 눈금 보기]**&#x200B;를 선택합니다. [에셋 찾아보기] 패널에서 단일 에셋을 선택한 다음 썸네일 이미지 아래에서 **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**(으)로 이동합니다.

     뷰어 목록 페이지의 표에 있는 작업 열에서 **[!UICONTROL 포함 코드]**&#x200B;를 선택합니다.

   * **[!UICONTROL 목록 보기]**&#x200B;를 선택합니다. [에셋 찾아보기] 패널에서 단일 에셋을 선택한 다음 썸네일 이미지의 오른쪽에 있는 **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**(으)로 이동합니다.

     뷰어 목록 페이지의 표에 있는 작업 열에서 **[!UICONTROL 포함 코드]**&#x200B;를 선택합니다.

   * **[!UICONTROL 눈금 보기]**, **[!UICONTROL 목록 보기]** 또는 **[!UICONTROL 자세히 보기]**&#x200B;를 선택하십시오. 같은 도구 모음에서 **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**(으)로 이동합니다.

     뷰어 목록 페이지의 표에 있는 작업 열에서 **[!UICONTROL 포함 코드]**&#x200B;를 선택합니다.

1. 포함 코드 대화 상자에서 **[!UICONTROL 클립보드에 복사]**&#x200B;를 선택합니다.

   코드 편집은 [임베드 코드] 대화 상자에서 허용되지 않습니다.

1. **[!UICONTROL 닫기]**&#x200B;를 선택합니다.

>[!MORELIKETHIS]
>
>* [게시](publishing-files.md#publishing_files)
