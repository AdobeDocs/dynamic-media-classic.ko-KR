---
title: 이미지 맵 만들기
description: Adobe Dynamic Media Classic에서 이미지 맵을 만드는 방법을 알아봅니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: deafbd03-06bc-4d7e-87a1-5620ebcac426
topic: Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '2444'
ht-degree: 30%

---

# 이미지 맵 만들기 {#creating-image-maps}

이미지 맵은 이미지, eCatalog 페이지 또는 텍스트가 있는 롤오버 패널을 표시하는 SpinSet의 이미지입니다. 사용자가 이미지 맵을 선택하면 특정 종류의 작업이 트리거됩니다. 예를 들어 사용자가 제품에 대해 자세히 알 수 있도록 웹 페이지가 시작됩니다. 이미지 맵 위로 포인터를 이동하면 윤곽선이 나타납니다.

Adobe Dynamic Media Classic에서 이미지 맵을 만드는 기능 외에도 Adobe Acrobat 또는 Adobe InDesign에서 카탈로그를 디자인할 때 이미지 맵을 만들 수도 있습니다.

이미지 맵을 만들 때 다음 작업 중 하나를 수행할 수 있습니다.

* 롤오버 텍스트를 입력합니다.
* 웹 페이지를 시작하기 위한 JavaScript 및 URL을 입력합니다.
* 이미지 맵에 사용할 URL 템플릿을 만듭니다.
* 이미지 맵을 다른 이미지, eCatalog 페이지 또는 회전 집합에 복사합니다.
* 이미지 맵을 CSV 또는 XML로 내보냅니다.
* 탭으로 구분된 파일 또는 XML 파일에서 이미지 메타데이터를 가져옵니다.
* World Wide Web 컨소시엄에서 결정한 다른 작업을 정의합니다.
* 이미지 맵을 미리 봅니다.

## 이미지 맵 그리기 및 조정 {#drawing-and-adjusting-an-image-map}

1. 다음 중 하나를 수행하십시오.

   * 눈금 보기 또는 목록 보기에서 이미지로 작업하는 경우 편집 드롭다운 목록에서 **[!UICONTROL 이미지 맵]**&#x200B;을(를) 선택합니다. 또는 세부 사항 보기에서 연 다음 이미지 위에서 **[!UICONTROL 이미지 맵]**&#x200B;을 선택합니다.
   * 눈금 보기 또는 목록 보기에서 회전 집합을 사용하여 작업하는 경우 **[!UICONTROL 편집]**&#x200B;을(를) 선택합니다. 또는 세부 사항 보기에서 연 다음 **[!UICONTROL 편집]**&#x200B;을 선택합니다. 이미지 자산을 선택한 다음 **[!UICONTROL 이미지 맵]**&#x200B;을 선택합니다.
   * 전자 카탈로그로 작업하는 경우 표 보기, 목록 보기, 세부 정보 보기에서 **[!UICONTROL 편집]**&#x200B;을 선택합니다. **[!UICONTROL 페이지 매핑]** 탭을 선택합니다.

   ![이미지 맵 그림](assets/ma_image_map.png)

1. 사각형 또는 다각형(다변형) 이미지 맵을 그립니다.

   * **사각형 맵**: 사각형 이미지 맵 도구를 선택하고 페이지에서 드래그하여 사각형을 만듭니다. 사각형 맵에 점을 추가하려면(따라서 다각형 맵으로 변경) Ctrl 키를 누른 다음 삽입 도구를 원하는 위치에 놓고 선택합니다.

   * **다각형 맵**: [다각형 이미지 맵] 도구를 선택하고 묶을 이미지 영역의 주변에 있는 점을 선택합니다. 다각형 밀도 슬라이더를 사용하여 다각형의 점 밀도를 변경합니다. 다른 맵을 선택할 경우 원본 밀도가 저장됩니다. 다각형에서 점을 추가, 삭제 또는 이동하면 원래 밀도가 손실됩니다. 슬라이더가 최대값으로 재설정됩니다.

1. 원하는 경우 [이미지 맵] 목록에 이미지 맵 이름을 입력합니다. 이미지 맵을 그리면 Adobe Dynamic Media Classic에서 이미지 맵에 이름을 지정합니다.

   이 이름을 만들려면 Adobe Dynamic Media Classic은 작업 중인 이미지 또는 eCatalog 페이지의 이름에 일련 번호를 추가합니다. 선택한 이름을 입력할 수 있습니다.

1. 사용자가 이미지 맵을 선택할 때 새 웹 페이지를 열려면 이미지 맵 목록에 URL을 입력합니다.

   JavaScript 및 URL을 입력하려면 [을(를) 참조하십시오](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. 사용자가 포인터를 이미지 맵 위로 이동할 때 롤오버 텍스트를 표시하려면 [이미지 맵] 목록에 텍스트를 입력합니다. 이미지 맵 목록에서 **[!UICONTROL 표시]** 메뉴를 선택하고 **[!UICONTROL 롤오버 텍스트]**&#x200B;를 선택합니다. 그런 다음 사용자에게 화면에 표시할 텍스트를 입력합니다. 워드 프로세서에서 텍스트를 작성하고 [롤오버 텍스트] 필드에 복사할 수 있습니다.

1. 사용자가 마우스를 이미지 맵 위로 이동할 때 다른 작업 효과를 발생시키려면 작업을 정의합니다. **[!UICONTROL 표시]** 드롭다운 목록에서 **[!UICONTROL 기타 작업]**&#x200B;을 선택합니다. 작업의 특성을 입력합니다. **[!UICONTROL 표시]** > **[!UICONTROL 모두]**(으)로 이동하여 이미지 맵에 대한 롤오버 텍스트 및 작업을 만듭니다.

   [이미지 맵에 대한 다른 작업 정의](creating-image-maps.md#defining_other_actions_for_image_maps)를 참조하십시오.

1. 다음 중 하나를 수행합니다(선택 사항).

   * 이미지 맵을 미리 보려면 **[!UICONTROL 미리 보기]**&#x200B;를 선택하십시오.
   * 이미지 맵 또는 다각형 꼭지점을 삭제하려면 이미지에서 모양을 선택한 다음 **[!UICONTROL 삭제]**&#x200B;를 선택합니다. 또는 eCatalog의 경우 [페이지 순서] 탭에서 **[!UICONTROL 맵 지우기]**&#x200B;를 선택하여 모든 페이지에서 이미지 맵을 제거합니다.
   * 을(를) 제거하려면 다음 작업을 수행하십시오.
      * 이미지의 이미지 맵
      * 스핀 세트의 이미지
      * 또는 eCatalog 페이지

     일시적으로, 삭제하지 않고 이미지 맵 목록에서 해당 [켜기] 옵션을 선택 해제합니다.

1. **[!UICONTROL 저장]**&#x200B;을 선택합니다.

### 이미지 맵의 위치, 모양 및 크기 조정 {#adjusting-the-position-shape-and-size-of-image-maps}

이미지 맵의 위치, 모양 및 크기를 변경하려면 [이미지 맵] 단추를 선택합니다. 그런 다음 **[!UICONTROL Pan]** 도구를 선택하고 다음 지침을 따릅니다.

* **위치 변경**: 포인터를 이미지 맵의 테두리 근처로 이동하지 않습니다. 십자형 화살표 아이콘이 표시되면 맵을 새 위치로 드래그합니다.

* **크기 및 모양 변경**: 이미지 맵의 모양과 크기를 변경하는 방법은 사각형 또는 다각형 이미지 맵으로 작업하고 있는지 여부에 따라 달라집니다.

>[!TIP]
>
>화면 하단에 있는 [크기] 슬라이더를 끌어 보기를 변경하고 이미지 맵 보기를 향상시킬 수 있습니다.

* **사각형 이미지 맵**: 포인터를 이미지 맵의 한 쪽이나 모서리 위로 이동합니다. 양면 화살표 아이콘이 표시되면 끌기를 시작합니다. Shift 키를 누른 채 드래그하여 크기를 변경하고 종횡비(모양)를 유지합니다.

* **다각형 이미지 맵**: 사각형 선택 핸들을 드래그합니다. 선택 핸들을 만들려면 이미지 맵의 테두리를 선택하고 드래그를 시작합니다.

### 겹치는 이미지 맵 처리 {#handling-overlapping-image-maps}

이미지 또는 eCatalog 페이지에 둘 이상의 이미지 맵이 포함되어 있고 맵이 겹치는 경우 맵이 겹치는 방식을 결정할 수 있습니다. 이렇게 하려면 [이미지 맵] 목록에서 맵 순서를 변경합니다. 맵 이름을 목록에서 위나 아래로 드래그합니다. 목록에서 이름이 표시되는 위치에 따라 해당 이미지 맵이 다른 이미지 맵과 겹치는지 여부가 결정됩니다.

### 이미지 맵 데이터 가져오기 {#importing-image-map-data}

각 페이지에서 이미지 맵 데이터를 입력하는 대신 이미지, 회전 집합 또는 eCatalog의 데이터를 [맵 요약] 화면으로 가져올 수 있습니다. 탭으로 구분된 파일이나 XML DTD 형태로 이미지 맵 데이터를 가져옵니다. 파일의 필드는 [맵 요약] 화면에 표시된 순서대로 정렬되어야 합니다(이름, 목차 레이블, 맵, URL, 롤오버 텍스트, 다른 작업 및 검색 문자열). 이미지 맵 데이터를 가져오면 각 이미지 맵을 만들 때 이미지 맵 목록에 데이터를 입력하는 문제를 줄일 수 있습니다.

**이미지 맵 데이터를 가져오려면:**

1. 이미지 맵 편집기 페이지(이미지 또는 회전 집합의 이미지) 또는 eCatalog 편집 화면의 [맵 페이지] 탭으로 이동합니다.
1. **[!UICONTROL 메타데이터 가져오기]**&#x200B;를 선택합니다.
1. 메타데이터 업로드 대화 상자에서 이미지 또는 이미지 맵 을 선택하여 원하는 에셋 속성 유형에서 메타데이터를 업로드합니다.
1. `Generate File` 드롭다운 목록에서 만들려는 파일 형식을 선택합니다.
1. (선택 사항) 만들려는 파일 형식을 기반으로 결과 데이터를 미리 보려면 **[!UICONTROL 생성]**&#x200B;을 선택합니다. 메타데이터 업로드 대화 상자로 돌아가려면 **[!UICONTROL 닫기]**&#x200B;를 선택합니다.
1. 업로드할 파일을 찾습니다. [파일 이름] 텍스트 필드에 생성된 파일의 이름을 지정합니다.
1. (선택 사항) [작업 이름] 필드에 메타데이터 업로드 작업의 이름을 지정합니다.
1. **[!UICONTROL 업로드]**&#x200B;를 선택합니다.

### 이미지 맵 복사 {#copying-image-maps}

이미지나 eCatalog 페이지의 이미지 맵을 다른 이미지나 eCatalog 페이지에 복사할 수 있습니다. **[!UICONTROL 이미지 맵 복사]**&#x200B;를 사용하여 이미지 맵 만들기를 시작하십시오. 이미지 맵을 복사하여 레이아웃이나 매핑 구조를 공유하는 이미지나 페이지에 다시 만들 수도 있습니다.

예를 들어 eCatalog에서 이미지 맵을 복사하면 동일한 eCatalog의 외국어 버전 간에 모든 이미지 맵을 편리하게 복사할 수 있습니다. 최상의 결과를 얻으려면 페이지 수가 동일한 eCatalogs와 이미지가 동일한 간에 복사하는 것이 가장 좋습니다. 복사하는 eCatalog에 이미 이미지 맵이 포함되어 있는 경우 복사가 수행될 때 해당 이미지 맵이 삭제됩니다.

**이미지 맵을 복사하려면:**

1. 이미지 맵 편집기 페이지(이미지 또는 회전 집합의 이미지) 또는 eCatalog 편집 화면의 [맵 페이지] 탭으로 이동합니다.
1. **[!UICONTROL 지도 복사]**&#x200B;를 선택합니다.
1. 이미지에서 이미지 맵을 복사하는지, 아니면 eCatalog에서 이미지 맵을 복사하는지에 따라 다음 중 하나를 수행합니다.

   * (이미지) [이미지 선택] 화면에서 이미지 맵을 복사할 타겟 이미지를 선택합니다.
   * (eCatalog) [자산 선택] 화면에서 이미지 맵을 복사할 타겟 이미지 또는 eCatalog 페이지를 선택합니다.

1. **[!UICONTROL 선택]**&#x200B;을 선택하세요.

## 템플릿을 사용하여 JavaScript 및 URL 입력 {#using-a-template-to-enter-javascript-and-urls}

보다 쉽고 효율적으로 이미지 맵 URL을 입력하기 위해 URL 템플릿(Href 템플릿이라고도 함)을 정의할 수 있습니다. 대부분의 이미지 맵 URL이 고정된 일반 형식을 공유하는 경우 URL 템플릿을 정의합니다. 고정된 URL 부분을 URL 템플릿으로 입력하면 이미지 맵을 만들 때마다 URL의 이 부분을 입력할 필요가 없습니다. URL 템플릿에는 JavaScript 명령, 경로 이름 및 매개 변수도 포함될 수 있습니다. 기본적으로 URL 템플릿에는 새 창에서 이미지를 여는 `loadProduct`이라는 고유한 Adobe Dynamic Media Classic JavaScript 처리기가 포함되어 있습니다.

>[!NOTE]
>
>JavaScript 코드를 이미지 맵의 HREF 특성에 추가하면 이 코드는 클라이언트의 컴퓨터에서 실행됩니다. 따라서 JavaScript 코드가 안전한지 확인하십시오.

### URL 템플릿 정보 {#about-url-templates}

URL 템플릿은 이미지 맵 목록의 URL 열 콘텐츠를 대체하여 작동합니다. 템플릿에서 이중 달러 기호(&#39;$$&#39;)로 대체합니다.

```as3
Javascript:loadProduct('$$');void(0);
```

이미지 맵 간에 변경되지 않는 모든 값은 URL 템플릿에 배치합니다. 변경되는 값만 [이미지 맵] 목록의 URL 열에 추가합니다. 예:

* URL 템플릿: `javascript:loadProduct('https://www.examplesitehere.com/$$');void(0);`
* URL 값: `product.htm`
* 실제 URL 생성됨: `javascript:loadProduct('https://www.examplesitehere.com/product.html);void(0);`

기본적으로 URL 템플릿에는 URL 대상이 있는 새 창을 여는 `loadProduct`이라는 고유한 Adobe Dynamic Media Classic JavaScript 처리기가 포함되어 있습니다. 그러나 모든 JavaScript 코드를 사용하여 이 JavaScript 핸들러를 교체하거나 다음 Adobe Dynamic Media Classic 핸들러 중 하나를 사용할 수 있습니다.

* `loadProductCW`: 현재 창의 URL 열에 지정된 URL 대상을 표시합니다. 이 핸들러는 주로 웹 사이트 내의 페이지에 통합된 eCatalog에 사용됩니다.

* `loadProductPW`: 부모 창(현재 창을 연 페이지)의 URL 열에 지정된 URL 대상을 표시합니다. 현재 창은 열려 있지만 상위 창이 URL 타겟을 표시하도록 변경됩니다.

  >[!NOTE]
  >
  >`loadProductPW` 처리기는 DHTML 및 HTML5 뷰어를 지원하지 않습니다.

### URL 템플릿 만들기 {#creating-a-url-template}

1. 맵 편집기 화면(이미지 또는 스핀 세트) 또는 eCatalog 화면의 맵 페이지 탭(eCatalogs)에서 URL 템플릿 옵션 옆에 있는 편집을 선택합니다. [맵 템플릿 편집] 대화 상자가 열립니다.
1. JavaScript 코드와 전체 URL을 입력합니다(변수 부분이 달러 기호 [$$]&#x200B;(으)로 대체됨). 마우스 오른쪽 단추를 클릭하고 **[!UICONTROL 붙여넣기]**&#x200B;를 선택하여 코드를 붙여넣을 수 있습니다.
1. **[!UICONTROL 저장]**&#x200B;을 선택합니다.

### URL 템플릿 처리 {#handling-url-templates}

[맵 편집기] 페이지(이미지와 회전 집합) 및 eCatalog 화면(eCatalog)의 [맵 페이지] 탭에서는 URL 템플릿을 처리하는 다음 명령을 제공합니다.

* **URL 템플릿 옵션**: URL 템플릿 옵션을 선택하여 이미지 또는 eCatalog 페이지의 모든 이미지 맵에 URL 템플릿을 적용합니다.

* **템플릿 옵션**: 개별 이미지 맵에서 URL 템플릿을 사용하지 않으려면 URL 이미지 맵 목록에서 템플릿 옵션을 선택 취소합니다.

## 이미지 맵에 대한 다른 작업 정의 {#defining-other-actions-for-image-maps}

**[!UICONTROL 표시]** 메뉴를 선택하고 **[!UICONTROL 기타 작업]**&#x200B;을 선택하여 롤오버 텍스트 및 웹 페이지 시작 이외의 작업을 트리거할 수 있습니다. 사용자가 포인터를 이미지 맵 위로 이동할 때 작업을 시작할 수 있습니다. 이러한 작업은 World Wide Web Consortium HTML 사양에서 클라이언트측 이미지 맵에 대해 정의된 특성입니다. 그러한 보고서는 아래와 같습니다.

* **`accesskey`**: 사용자가 키보드에서 지정된 키를 누르면 작업을 트리거합니다.

* **`onfocus`**: 이미지 맵에서 커서, 탭 또는 액세스 키를 눌러 포커스를 받을 때 이벤트를 트리거합니다. 예를 들어 이미지 맵에서 포커스를 받으면 웹 페이지를 시작하고 이미지 맵에서 포커스를 잃으면 웹 페이지를 닫을 수 있습니다.

* **`onblur`**: 이미지 맵에서 커서나 탭 표시로 포커스가 손실되면 이벤트를 트리거합니다.

**이미지 맵에 대한 다른 작업을 정의하려면**

1. 맵 편집기 화면(이미지 및 스핀 세트)이나 eCatalog 화면(eCatalogs)의 맵 페이지 탭에서 **[!UICONTROL 표시]** 메뉴를 선택하고 **[!UICONTROL 기타 작업]**&#x200B;을 선택합니다.
1. World Wide Web Consortium HTML 사양에 지정된 구문을 사용하여 [이미지 맵] 목록의 [다른 작업] 열에 지원되는 특성을 추가합니다.
1. **[!UICONTROL 저장]**&#x200B;을 선택합니다.

이미지 맵에 롤오버 텍스트와 작업을 포함하려면 **[!UICONTROL 표시]** 메뉴를 선택하고 **[!UICONTROL 모두]**&#x200B;를 선택합니다.

## Adobe Acrobat 또는 Adobe InDesign에서 이미지 맵 만들기 {#creating-image-maps-in-adobe-acrobat-or-adobe-indesign}

Adobe Acrobat 또는 Adobe InDesign에서 eCatalog를 디자인하는 동안 이미지 맵을 만들 수 있습니다.

Adobe Acrobat 또는 Adobe InDesign에서 이미지 맵을 표시할 위치에 하이퍼링크 참조를 만들고 이미지 맵의 URL 위치를 지정합니다. PDF 파일을 Adobe Dynamic Media Classic에 업로드할 때 링크 추출 옵션을 선택하면 링크가 이미지 맵으로 자동 변환됩니다.

자세한 내용은 Adobe InDesign 도움말 또는 Adobe Acrobat 도움말을 참조하십시오.

### Adobe InDesign에서 이미지 맵 만들기 {#to-create-image-maps-in-adobe-indesign}

1. Adobe InDesign에서 **[!UICONTROL Windows®]** > **[!UICONTROL 대화형]** > **[!UICONTROL 하이퍼링크]**&#x200B;로 이동합니다.
1. [하이퍼링크] 패널에서 이미지 맵으로 만들 텍스트, 프레임 또는 그래픽을 선택합니다.
1. 패널 메뉴에서 **[!UICONTROL 새 하이퍼링크]**&#x200B;를 선택합니다.
1. 새 하이퍼링크 대화 상자의 **[!UICONTROL 연결 대상]** 메뉴에서 **[!UICONTROL URL]**&#x200B;을(를) 선택합니다.
1. URL 상자에 제품 ID를 입력하거나 붙여 넣습니다.
1. **[!UICONTROL 확인]**&#x200B;을 선택합니다. (Adobe Dynamic Media Classic은 이미지 맵 URL 템플릿을 사용하여 URL을 완료합니다.)

   >[!NOTE]
   >
   >Adobe InDesign에서는 모양 옵션을 설정할 필요가 없습니다. Adobe Dynamic Media Classic에서 모양을 지정할 수 있습니다.

1. 만들려는 모든 이미지 맵에 대해 2단계부터 6단계까지 반복합니다.
1. 파일을 PDF로 내보냅니다.
1. PDF을 Adobe Dynamic Media Classic에 업로드합니다.
1. **[!UICONTROL PDF 옵션]**&#x200B;에서 **[!UICONTROL 링크 추출]**&#x200B;을 선택합니다.

### Adobe Acrobat에서 이미지 맵 만들기 {#to-create-image-maps-in-adobe-acrobat}

1. Adobe Acrobat에서 **[!UICONTROL 도구]** > **[!UICONTROL 고급 편집]** > **[!UICONTROL 도구 연결]**(으)로 이동합니다.
1. 드래그하여 이미지 맵을 만듭니다.
1. 링크 만들기 상자에서 **[!UICONTROL 사용자 지정 링크]**&#x200B;를 선택하고 **[!UICONTROL 다음]**&#x200B;을 선택합니다.

>[!NOTE]
>
>Adobe Acrobat에서는 모양 옵션을 설정할 필요가 없습니다. Adobe Dynamic Media Classic에서 모양을 지정할 수 있습니다.

1. 링크 속성 상자에서 **[!UICONTROL 작업]**&#x200B;을 선택합니다.
1. 동작 선택 메뉴에서 **[!UICONTROL 웹 링크 열기]**&#x200B;를 선택한 다음 **[!UICONTROL 추가]**&#x200B;를 선택합니다.
1. URL 편집 상자에 이미지 맵의 제품 ID를 입력하고 **[!UICONTROL 확인]**&#x200B;을 선택합니다. (Adobe Dynamic Media Classic은 이미지 맵 URL 템플릿을 사용하여 URL을 완료합니다.)
1. 만들려는 모든 이미지 맵에 대해 1-7 단계를 반복합니다.
1. 파일을 저장합니다.
1. PDF을 Adobe Dynamic Media Classic에 업로드하고 PDF 옵션에서 링크 추출 을 선택합니다.
