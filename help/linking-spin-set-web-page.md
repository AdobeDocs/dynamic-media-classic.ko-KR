---
title: 회전 집합을 웹 페이지에 연결
description: 스핀 세트를 웹 페이지에 연결하는 방법을 알아봅니다.
uuid: d3c5773e-60c4-4e8b-9c48-e1e3eb8028d0
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 651b21ef-e322-4e6d-8e37-45ffd56f7a58
feature: Dynamic Media Classic,뷰어,스핀 세트
role: User
exl-id: af75547e-20e8-44c2-b165-01532d6e21d0
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '720'
ht-degree: 87%

---

# 회전 집합을 웹 페이지에 연결{#linking-a-spin-set-to-a-web-page}

웹 사이트 및 응용 프로그램은 URL 문자열 또는 포함된 코드를 통해 스핀 세트를 포함한 Dynamic Media 이미지 서버 컨텐츠에 액세스합니다. 이러한 URL 문자열은 게시 프로세스 중에 활성화됩니다. 웹 페이지 및 애플리케이션에 스핀 세트에 대한 URL 문자열 또는 포함 코드를 배치하려면 Dynamic Media Classic에서 복사합니다.

>[!NOTE]
>
>자산을 게시하기 전에는 URL이 활성화되지 않습니다.

## 회전 집합 URL 복사 {#copying-a-spin-set-url}

1. [자산 찾아보기] 패널의 [표시] 드롭다운 목록에서 **[!UICONTROL [회전 집합]]**&#x200B;을 클릭합니다.
1. 왼쪽의 [자산 라이브러리] 패널에서 임베드 코드를 복사하려는 회전 집합 뷰어가 들어 있는 자산 폴더를 탐색합니다.
1. [자산 찾아보기] 패널 위의 도구 모음 오른쪽에서 다음 중 하나를 수행합니다.

   * **[!UICONTROL [그리드 보기]]**&#x200B;를 클릭합니다. [자산 찾아보기] 패널에서 단일 자산을 두 번 클릭하여 [세부 사항 보기]에서 엽니다. 오른쪽의 [URL 및 임베드 코드] 패널에서 원하는 뷰어의 오른쪽에 있는 **[!UICONTROL [URL 복사]]**&#x200B;를 클릭합니다.
   * **[!UICONTROL [그리드 보기]]**&#x200B;를 클릭합니다. [자산 찾아보기] 패널에서 단일 자산을 선택하고 썸네일 이미지 아래에서 **[!UICONTROL [미리 보기]]** > **[!UICONTROL [뷰어 목록]]**&#x200B;을 클릭합니다.

      [뷰어 목록] 페이지에 있는 테이블의 [작업] 열에서 **[!UICONTROL [URL 복사]]**&#x200B;를 클릭합니다.

   * **[!UICONTROL [목록 보기]]**&#x200B;를 클릭합니다. [자산 찾아보기] 패널에서 단일 자산을 선택하고 썸네일 이미지 오른쪽에서 **[!UICONTROL [미리 보기]]** > **[!UICONTROL [뷰어 목록]]**&#x200B;을 클릭합니다.

      [뷰어 목록] 페이지에 있는 테이블의 [작업] 열에서 **[!UICONTROL [URL 복사]]**&#x200B;를 클릭합니다.

   * **[!UICONTROL [그리드 보기]]**, **[!UICONTROL [목록 보기]]** 또는 **[!UICONTROL [세부 사항 보기]]**&#x200B;를 클릭합니다. 동일한 도구 모음에서 **[!UICONTROL [미리 보기]]** > **[!UICONTROL [뷰어 목록]]**&#x200B;을 클릭합니다.

      [뷰어 목록] 페이지에 있는 테이블의 [작업] 열에서 **[!UICONTROL [URL 복사]]**&#x200B;를 클릭합니다.

## 웹 페이지에 회전 집합 URL 추가 {#adding-spin-set-urls-to-your-web-page}

회전 집합은 모든 확대/축소 뷰어와 마찬가지로 [확대/축소] 창에서 회전 집합을 표시하는 동적 페이지(ASP 또는 JSP)를 통해 배포됩니다. Dynamic Media Classic 플랫폼에 대한 URL 호출은 확대/축소 뷰어의 동일한 프로토콜을 따릅니다. 그러나 뷰어 사전 설정 이름은 관리자가 기본 회전 집합 뷰어 사전 설정으로 정의한 사전 설정에 따라 달라집니다. 예를 들어 다음의 작동하지 않는 URL 구문 예에는 `viewer.jsp`라는 사전 설정 이름이 포함되며 이제 SKU 매개 변수가 스핀 세트 이름입니다.

```as3
https://sample.scene7.com/s7ondemand/spin/viewer.jsp?company=S7Web&sku=backpack_spin
```

이 URL에서 구문 예에서(링크는 작동하지 않음) SKU 번호(`sku=backpack_spin`)를 확인합니다. `sku=` 뒤의 문자열은 스핀 세트 이름( `backpack spin`)입니다.

## 회전 집합 뷰어의 임베드 코드 복사 {#copying-the-embed-code-of-a-spin-set-viewer}

임베드 코드 기능을 사용하면 선택한 회전 집합의 뷰어 코드를 검토할 수 있습니다. 또한 뷰어 배포를 위해 코드를 클립보드로 복사하여 웹 페이지에 붙여넣을 수도 있습니다. 코드 편집은 [임베드 코드] 대화 상자에서 허용되지 않습니다.

**회전 집합 뷰어의 임베드 코드를 복사하려면:**

1. [자산 찾아보기] 패널의 [표시] 드롭다운 목록에서 **[!UICONTROL [회전 집합]]**&#x200B;을 클릭합니다.
1. 왼쪽의 [자산 라이브러리] 패널에서 임베드 코드를 복사하려는 회전 집합 뷰어가 들어 있는 자산 폴더를 탐색합니다.
1. [자산 찾아보기] 패널 위의 도구 모음 오른쪽에서 다음 중 하나를 수행합니다.

   * **[!UICONTROL [그리드 보기]]**&#x200B;를 클릭합니다. [자산 찾아보기] 패널에서 단일 자산을 두 번 클릭하여 [세부 사항 보기]에서 엽니다. 오른쪽의 [URL 및 임베드 코드] 패널에서 원하는 뷰어의 오른쪽에 있는 **[!UICONTROL [임베드 코드]]**&#x200B;를 클릭합니다.
   * **[!UICONTROL [그리드 보기]]**&#x200B;를 클릭합니다. [자산 찾아보기] 패널에서 단일 자산을 선택하고 썸네일 이미지 아래에서 **[!UICONTROL [미리 보기]]** > **[!UICONTROL [뷰어 목록]]**&#x200B;을 클릭합니다.

      [뷰어 목록] 페이지에 있는 테이블의 [작업] 열에서 **[!UICONTROL [임베드 코드]]**&#x200B;를 클릭합니다.

   * **[!UICONTROL [목록 보기]]**&#x200B;를 클릭합니다. [자산 찾아보기] 패널에서 단일 자산을 선택하고 썸네일 이미지 오른쪽에서 **[!UICONTROL [미리 보기]]** > **[!UICONTROL [뷰어 목록]]**&#x200B;을 클릭합니다.

      [뷰어 목록] 페이지에 있는 테이블의 [작업] 열에서 **[!UICONTROL [임베드 코드]]**&#x200B;를 클릭합니다.

   * **[!UICONTROL [그리드 보기]]**, **[!UICONTROL [목록 보기]]** 또는 **[!UICONTROL [세부 사항 보기]]**&#x200B;를 클릭합니다. 동일한 도구 모음에서 **[!UICONTROL [미리 보기]]** > **[!UICONTROL [뷰어 목록]]**&#x200B;을 클릭합니다.

      [뷰어 목록] 페이지에 있는 테이블의 [작업] 열에서 **[!UICONTROL [임베드 코드]]**&#x200B;를 클릭합니다.

1. [임베드 코드] 대화 상자에서 **[!UICONTROL [클립보드에 복사]]**&#x200B;를 클릭합니다.

   코드 편집은 [임베드 코드] 대화 상자에서 허용되지 않습니다.

1. **[!UICONTROL [닫기]]**&#x200B;를 클릭합니다.
