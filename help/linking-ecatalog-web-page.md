---
title: eCatalog를 웹 페이지에 연결
description: eCatalog 를 웹 페이지에 연결하는 방법을 알아봅니다.
uuid: 90098a90-180b-477a-8533-24a52a93200b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 140640f2-3ca4-4b6c-a240-5f01be87fa9c
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: aee72576-1e3e-401c-953d-cc2be27f7dfd
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 85%

---

# eCatalog를 웹 페이지에 연결{#linking-an-ecatalog-to-a-web-page}

웹 사이트 및 응용 프로그램은 URL 문자열 또는 포함된 코드를 통해 eCatalogs를 포함한 Dynamic Media Image Server 컨텐츠에 액세스합니다. 이러한 URL 문자열은 게시 프로세스 중에 활성화됩니다. 웹 페이지 및 애플리케이션에 eCatalog에 대한 URL 문자열 또는 포함 코드를 배치하려면 Dynamic Media Classic에서 복사합니다.

>[!NOTE]
>
>자산을 게시하기 전에는 URL이 활성화되지 않습니다.

## eCatalog URL 복사 {#copying-an-ecatalog-url}

1. [자산 찾아보기] 패널의 [표시] 드롭다운 목록에서 [**[!UICONTROL 카탈로그]**]를 클릭합니다.
1. 왼쪽의 [자산 라이브러리] 패널에서 임베드 코드를 복사하려는 eCatalog가 들어 있는 자산 폴더를 탐색합니다.
1. [자산 찾아보기] 패널 위의 도구 모음 오른쪽에서 다음 중 하나를 수행합니다.

   * **[!UICONTROL [그리드 보기]]**&#x200B;를 클릭합니다. [자산 찾아보기] 패널에서 단일 자산을 두 번 클릭하여 [세부 사항 보기]에서 엽니다. 오른쪽의 [URL 및 임베드 코드] 패널에서 원하는 뷰어의 오른쪽에 있는 **[!UICONTROL [URL 복사]]**&#x200B;를 클릭합니다.
   * **[!UICONTROL [그리드 보기]]**&#x200B;를 클릭합니다. [자산 찾아보기] 패널에서 단일 자산을 선택하고 썸네일 이미지 아래에서 **[!UICONTROL [미리 보기]]** > **[!UICONTROL [뷰어 목록]]**&#x200B;을 클릭합니다.

      [뷰어 목록] 페이지에 있는 테이블의 [작업] 열에서 **[!UICONTROL [URL 복사]]**&#x200B;를 클릭합니다.

   * **[!UICONTROL [목록 보기]]**&#x200B;를 클릭합니다. [자산 찾아보기] 패널에서 단일 자산을 선택하고 썸네일 이미지 오른쪽에서 **[!UICONTROL [미리 보기]]** > **[!UICONTROL [뷰어 목록]]**&#x200B;을 클릭합니다.

      [뷰어 목록] 페이지에 있는 테이블의 [작업] 열에서 **[!UICONTROL [URL 복사]]**&#x200B;를 클릭합니다.

   * **[!UICONTROL [그리드 보기]]**, **[!UICONTROL [목록 보기]]** 또는 **[!UICONTROL [세부 사항 보기]]**&#x200B;를 클릭합니다. 동일한 도구 모음에서 **[!UICONTROL [미리 보기]]** > **[!UICONTROL [뷰어 목록]]**&#x200B;을 클릭합니다.

      [뷰어 목록] 페이지에 있는 테이블의 [작업] 열에서 **[URL 복사]**&#x200B;를 클릭합니다.

## 웹 페이지에 eCatalog URL 추가 {#adding-ecatalog-urls-to-your-web-page}

eCatalog를 배포하는 가장 일반적인 방법은 웹 페이지에 eCatalog 썸네일 표지 페이지 형태로 링크를 배치하는 것입니다. IT 팀과 협력하여 eCatalog가 간결한 가운데 맞춤 팝업 창에서 시작되도록 합니다. IT 팀에 브라우저의 도구 모음과 주소 표시줄이 표시되지 않도록 요청합니다.

자세한 내용 및 코드 샘플은 Adobe 뷰어 참조 안내서](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/ecatalog/c-html5-20-ecatalog-viewer-about.html#section-e1c3106f5b3e445d9b95be337c2f94e2)에서 [HTML5 eCatalog 뷰어 포함 을 참조하십시오.

## eCatalog 뷰어의 임베드 코드 복사 {#copying-the-embed-code-of-an-ecatalog-viewer}

임베드 코드 기능을 사용하면 선택한 eCatalog의 뷰어 코드를 검토할 수 있습니다. 또한 뷰어 배포를 위해 코드를 클립보드로 복사하여 웹 페이지에 붙여넣을 수도 있습니다. 코드 편집은 [임베드 코드] 대화 상자에서 허용되지 않습니다.

**eCatalog 뷰어의 임베드 코드를 복사하려면:**

1. [자산 찾아보기] 패널의 [표시] 드롭다운 목록에서 [**[!UICONTROL 카탈로그]**]를 클릭합니다.
1. 왼쪽의 [자산 라이브러리] 패널에서 임베드 코드를 복사하려는 eCatalog가 들어 있는 자산 폴더를 탐색합니다.
1. [자산 찾아보기] 패널 위의 도구 모음 오른쪽에서 다음 중 하나를 수행합니다.

   * **[!UICONTROL [그리드 보기]]**&#x200B;를 클릭합니다. [자산 찾아보기] 패널에서 단일 자산을 두 번 클릭하여 [세부 사항 보기]에서 엽니다. 오른쪽의 [URL] 패널에서 **[!UICONTROL [임베드 코드]]**&#x200B;를 클릭합니다.
   * **[!UICONTROL [그리드 보기]]**&#x200B;를 클릭합니다. [자산 찾아보기] 패널에서 단일 자산을 선택하고 썸네일 이미지 아래에서 **[!UICONTROL [미리 보기]]** > **[!UICONTROL [뷰어 목록]]**&#x200B;을 클릭합니다.

      [뷰어 목록] 페이지에 있는 테이블의 [작업] 열에서 **[!UICONTROL [임베드 코드]]**&#x200B;를 클릭합니다.

   * **[!UICONTROL [목록 보기]]**&#x200B;를 클릭합니다. [자산 찾아보기] 패널에서 단일 자산을 선택하고 썸네일 이미지 오른쪽에서 **[!UICONTROL [미리 보기]]** > **[!UICONTROL [뷰어 목록]]**&#x200B;을 클릭합니다.

      [뷰어 목록] 페이지에 있는 테이블의 [작업] 열에서 **[!UICONTROL [임베드 코드]]**&#x200B;를 클릭합니다.

   * **[!UICONTROL [그리드 보기]]**, **[!UICONTROL [목록 보기]]** 또는 **[!UICONTROL [세부 사항 보기]]**&#x200B;를 클릭합니다. 동일한 도구 모음에서 **[!UICONTROL [미리 보기]]** > **[!UICONTROL [뷰어 목록]]**&#x200B;을 클릭합니다.

      [뷰어 목록] 페이지에 있는 테이블의 [작업] 열에서 **[!UICONTROL [임베드 코드]]**&#x200B;를 클릭합니다.

1. [임베드 코드] 대화 상자에서 **[!UICONTROL [클립보드에 복사]]**&#x200B;를 클릭합니다.

   코드 편집은 [임베드 코드] 대화 상자에서 허용되지 않습니다.

1. **[!UICONTROL [닫기]]**&#x200B;를 클릭합니다.
