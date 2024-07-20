---
title: 웹 페이지에 회전 집합 연결
description: Adobe Dynamic Media Classic에서 스핀 세트를 웹 페이지에 연결하는 방법을 알아봅니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: af75547e-20e8-44c2-b165-01532d6e21d0
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 23%

---

# 웹 페이지에 회전 집합 연결{#linking-a-spin-set-to-a-web-page}

웹 사이트 및 애플리케이션은 URL 문자열 또는 포함된 코드를 통해 스핀 세트를 포함한 Dynamic Media 이미지 서버 콘텐츠에 액세스합니다. 이러한 URL 문자열은 게시 프로세스 중에 활성화됩니다. 스핀 세트의 URL 문자열 또는 포함 코드를 웹 페이지 및 애플리케이션에 배치하려면 Adobe Dynamic Media Classic에서 복사하십시오.

>[!NOTE]
>
>자산을 게시하기 전에는 URL이 활성화되지 않습니다.

## 회전 집합 URL 복사 {#copying-a-spin-set-url}

1. [자산 찾아보기] 패널의 [표시] 드롭다운 목록에서 **[!UICONTROL 회전 집합]**&#x200B;을 선택합니다.
1. 왼쪽의 에셋 라이브러리 패널에서 포함 코드를 복사할 회전 세트가 포함된 에셋 폴더로 이동합니다.
1. [자산 찾아보기] 패널 위의 도구 모음 오른쪽에서 다음 중 하나를 수행합니다.

   * **[!UICONTROL 눈금 보기]**&#x200B;를 선택합니다. [자산 찾아보기] 패널에서 단일 자산을 두 번 클릭하여 [세부 사항 보기]에서 엽니다. 오른쪽의 URL 및 포함 코드 패널에서 원하는 뷰어의 오른쪽에 있는 **[!UICONTROL URL 복사]**&#x200B;를 선택합니다.
   * **[!UICONTROL 눈금 보기]**&#x200B;를 선택합니다. [에셋 찾아보기] 패널에서 단일 에셋을 선택한 다음 썸네일 이미지 아래에서 **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**(으)로 이동합니다.

     뷰어 목록 페이지의 표에 있는 작업 열에서 **[!UICONTROL URL 복사]**&#x200B;를 선택합니다.

   * **[!UICONTROL 목록 보기]**&#x200B;를 선택합니다. [에셋 찾아보기] 패널에서 단일 에셋을 선택한 다음 썸네일 이미지의 오른쪽에 있는 **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**(으)로 이동합니다.

     뷰어 목록 페이지의 표에 있는 작업 열에서 **[!UICONTROL URL 복사]**&#x200B;를 선택합니다.

   * **[!UICONTROL 눈금 보기]**, **[!UICONTROL 목록 보기]** 또는 **[!UICONTROL 자세히 보기]**&#x200B;를 선택하십시오. 같은 도구 모음에서 **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**(으)로 이동합니다.

     뷰어 목록 페이지의 표에 있는 작업 열에서 **[!UICONTROL URL 복사]**&#x200B;를 선택합니다.

## 웹 페이지에 회전 집합 URL 추가 {#adding-spin-set-urls-to-your-web-page}

회전 집합은 모든 확대/축소 뷰어와 마찬가지로 [확대/축소] 창에서 회전 집합을 표시하는 동적 페이지(ASP 또는 JSP)를 통해 배포됩니다. Adobe Dynamic Media Classic 플랫폼에 대한 URL 호출은 확대/축소 뷰어에서 동일한 프로토콜을 따릅니다. 그러나 뷰어 사전 설정 이름은 관리자가 기본 회전 집합 뷰어 사전 설정으로 정의한 사전 설정에 따라 달라집니다. 예를 들어 라이브가 아닌 다음 URL 구문 예에는 `viewer.jsp`이라는 사전 설정 이름이 포함되어 있으며 SKU 매개 변수는 이제 회전 집합 이름입니다.

```as3
https://sample.scene7.com/s7ondemand/spin/viewer.jsp?company=S7Web&sku=backpack_spin
```

이 URL 구문 예(링크가 라이브가 아님)에서 SKU 번호(`sku=backpack_spin`)를 확인합니다. `sku=` 뒤에 있는 문자열이 회전 집합 이름( `backpack spin`)입니다.

## 회전 집합 뷰어의 포함 코드 복사 {#copying-the-embed-code-of-a-spin-set-viewer}

임베드 코드 기능을 사용하면 선택한 회전 집합의 뷰어 코드를 검토할 수 있습니다. 또한 코드를 클립보드에 복사하여 뷰어의 배포를 위해 웹 페이지에 붙여넣을 수 있습니다. 코드 편집은 [임베드 코드] 대화 상자에서 허용되지 않습니다.

**회전 집합 뷰어의 포함 코드를 복사하려면:**

1. [자산 찾아보기] 패널의 [표시] 드롭다운 목록에서 **[!UICONTROL 회전 집합]**&#x200B;을 선택합니다.
1. 왼쪽의 에셋 라이브러리 패널에서 포함 코드를 복사할 회전 세트가 포함된 에셋 폴더로 이동합니다.
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
