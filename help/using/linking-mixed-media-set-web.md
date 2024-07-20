---
title: 웹 페이지에 혼합 미디어 집합 연결
description: Adobe Dynamic Media Classic에서 혼합 미디어 세트를 웹 페이지에 연결하는 방법을 알아봅니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/mixed_media_sets
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: 76a7530c-0cc7-4a7f-bc31-2950c4946871
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 22%

---

# 웹 페이지에 혼합 미디어 집합 연결{#linking-a-mixed-media-set-to-a-web-page}

혼합 미디어 세트를 게시한 후 웹 사이트 또는 애플리케이션에서 사용할 관련 URL을 가져올 수 있습니다. 그런 다음 필요에 따라 URL을 배포하여 사용자가 웹 사이트 또는 애플리케이션에서 혼합 미디어 세트를 볼 수 있도록 할 수 있습니다.

## 혼합 미디어 집합 URL 얻기 {#obtain-a-mixed-media-set-url}

1. [자산 찾아보기] 패널의 [표시] 드롭다운 목록에서 **[!UICONTROL 미디어 집합]**&#x200B;을 선택합니다.
1. 왼쪽의 에셋 라이브러리 패널에서 포함 코드를 복사할 미디어 세트가 포함된 에셋 폴더로 이동합니다.
1. [자산 찾아보기] 패널 위의 도구 모음 오른쪽에서 다음 중 하나를 수행합니다.

   * **[!UICONTROL [그리드 보기]]**&#x200B;를 클릭합니다. [자산 찾아보기] 패널에서 단일 자산을 두 번 클릭하여 [세부 사항 보기]에서 엽니다. 오른쪽의 URL 및 포함 코드 패널에서 원하는 뷰어의 오른쪽에 있는 **[!UICONTROL URL 복사]**&#x200B;를 선택합니다.
   * **[!UICONTROL [그리드 보기]]**&#x200B;를 클릭합니다. [에셋 찾아보기] 패널에서 단일 에셋을 선택한 다음 썸네일 이미지 아래에서 **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**(으)로 이동합니다.

     뷰어 목록 페이지의 표에 있는 작업 열에서 **[!UICONTROL URL 복사]**&#x200B;를 선택합니다.

   * **[!UICONTROL [목록 보기]]**&#x200B;를 클릭합니다. [에셋 찾아보기] 패널에서 단일 에셋을 선택한 다음 썸네일 이미지의 오른쪽에 있는 **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**(으)로 이동합니다.

     뷰어 목록 페이지의 표에 있는 작업 열에서 **[!UICONTROL URL 복사]**&#x200B;를 선택합니다.

   * **[!UICONTROL [그리드 보기]]**, **[!UICONTROL [목록 보기]]** 또는 **[!UICONTROL [세부 사항 보기]]**&#x200B;를 클릭합니다. 같은 도구 모음에서 **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**(으)로 이동합니다.

     뷰어 목록 페이지의 표에 있는 작업 열에서 **[!UICONTROL URL 복사]**&#x200B;를 선택합니다.

## 웹 페이지에 혼합 미디어 집합 URL 추가 {#add-mixed-media-set-urls-to-your-web-page}

혼합 미디어 세트를 배포하는 가장 일반적인 방법은 웹 페이지에 링크(탐색 아이콘 사용)를 배치하는 것입니다. 선택하면 링크가 혼합 미디어 집합 뷰어에 혼합 미디어 집합을 표시하는 동적 페이지(ASP 또는 JSP)를 시작합니다.

## 혼합 미디어 집합 뷰어의 포함 코드 복사 {#copying-the-embed-code-of-a-mixed-media-set-viewer}

임베드 코드 기능을 사용하면 선택한 혼합 미디어 집합의 뷰어 코드를 검토할 수 있습니다. 또한 코드를 클립보드에 복사하여 뷰어의 배포를 위해 웹 페이지에 붙여넣을 수 있습니다. 코드 편집은 [임베드 코드] 대화 상자에서 허용되지 않습니다.

**혼합 미디어 집합 뷰어의 포함 코드를 복사하려면:**

1. [자산 찾아보기] 패널의 [표시] 드롭다운 목록에서 **[!UICONTROL 혼합 미디어 집합]**&#x200B;을 선택합니다.
1. 왼쪽의 에셋 라이브러리 패널에서 포함 코드를 복사할 혼합 미디어 세트가 포함된 에셋 폴더로 이동합니다.
1. [자산 찾아보기] 패널 위의 도구 모음 오른쪽에서 다음 중 하나를 수행합니다.

   * **[!UICONTROL [그리드 보기]]**&#x200B;를 클릭합니다. [자산 찾아보기] 패널에서 단일 자산을 두 번 클릭하여 [세부 사항 보기]에서 엽니다. 오른쪽의 URL 및 포함 코드 패널에서 원하는 뷰어의 오른쪽에 있는 **[!UICONTROL 포함 코드]**&#x200B;를 선택합니다.
   * **[!UICONTROL [그리드 보기]]**&#x200B;를 클릭합니다. [에셋 찾아보기] 패널에서 단일 에셋을 선택한 다음 썸네일 이미지 아래에서 **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**(으)로 이동합니다.

     뷰어 목록 페이지의 표에 있는 작업 열에서 **[!UICONTROL 포함 코드]**&#x200B;를 선택합니다.

   * **[!UICONTROL [목록 보기]]**&#x200B;를 클릭합니다. [에셋 찾아보기] 패널에서 단일 에셋을 선택한 다음 썸네일 이미지의 오른쪽에 있는 **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**(으)로 이동합니다.

     뷰어 목록 페이지의 표에 있는 작업 열에서 **[!UICONTROL 포함 코드]**&#x200B;를 선택합니다.

   * **[!UICONTROL [그리드 보기]]**, **[!UICONTROL [목록 보기]]** 또는 **[!UICONTROL [세부 사항 보기]]**&#x200B;를 클릭합니다. 같은 도구 모음에서 **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**(으)로 이동합니다.

     뷰어 목록 페이지의 표에 있는 작업 열에서 **[!UICONTROL 포함 코드]**&#x200B;를 선택합니다.

1. 포함 코드 대화 상자에서 **[!UICONTROL 클립보드에 복사]**&#x200B;를 선택합니다.

   코드 편집은 [임베드 코드] 대화 상자에서 허용되지 않습니다.

1. **[!UICONTROL [닫기]]**&#x200B;를 클릭합니다.

>[!MORELIKETHIS]
>
>* [Publish](publishing-files.md#publishing_files)
