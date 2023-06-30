---
title: 이미지 맵 만들기
description: Adobe Dynamic Media Classic에서 이미지 맵을 만드는 방법을 알아봅니다.
uuid: 0dcc4956-006e-4a74-9d6a-6d4bb23790ce
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4eddf983-38cb-4f00-b3be-85c20bdd6f69
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: deafbd03-06bc-4d7e-87a1-5620ebcac426
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '2430'
ht-degree: 49%

---

# 이미지 맵 만들기 {#creating-image-maps}

이미지 맵은 이미지, eCatalog 페이지 또는 회전 집합 이미지의 영역으로, 텍스트가 있는 롤오버 패널을 표시합니다. 사용자가 이미지 맵을 선택하면 특정 종류의 작업이 트리거됩니다. 예를 들어 사용자가 제품에 대한 자세한 정보를 확인할 수 있도록 웹 페이지가 시작됩니다. 이미지 맵 위로 포인터를 이동하면 윤곽선이 나타납니다.

Adobe Dynamic Media Classic에서 이미지 맵을 만드는 기능 외에도 Adobe Acrobat 또는 Adobe InDesign에서 카탈로그를 디자인할 때 이미지 맵을 만들 수도 있습니다.

이미지 맵을 만들 때 다음 작업 중 하나를 수행할 수 있습니다.

* 롤오버 텍스트를 입력합니다.
* 웹 페이지를 시작하기 위한 JavaScript 및 URL을 입력합니다.
* 이미지 맵에 사용할 URL 템플릿을 만듭니다.
* 이미지 맵을 다른 이미지, eCatalog 페이지 또는 회전 집합에 복사합니다.
* 이미지 맵을 CSV 또는 XML로 내보냅니다.
* 탭으로 구분된 파일 또는 XML 파일에서 이미지 메타데이터를 가져옵니다.
* World Wide Web Consortium의 결정에 따라 기타 작업을 정의합니다.
* 이미지 맵을 미리 봅니다.

## 이미지 맵 그리기 및 조정 {#drawing-and-adjusting-an-image-map}

1. 다음 중 하나를 수행하십시오.

   * 그리드 보기 또는 목록 보기에서 이미지로 작업하는 경우 편집 드롭다운 목록에서 를 선택합니다 **[!UICONTROL 이미지 맵]**. 또는 세부 사항 보기에서 연 다음 를 선택합니다 **[!UICONTROL 이미지 맵]** 이미지 위로 이동합니다.
   * [격자 보기] 또는 [목록 보기]에서 회전 집합을 사용하여 작업하는 경우 다음을 선택합니다 **[!UICONTROL 편집]**. 또는 세부 사항 보기에서 연 다음 를 선택합니다 **[!UICONTROL 편집]**. 이미지 자산을 선택한 다음 을 선택합니다. **[!UICONTROL 이미지 맵]**.
   * eCatalog로 작업하는 경우 표 형태 보기, 목록 보기, 세부 사항 보기에서 다음을 선택합니다. **[!UICONTROL 편집]**. 다음 항목 선택 **[!UICONTROL 페이지 매핑]** 탭.

   ![이미지 맵 이미지](assets/ma_image_map.png)

1. 사각형 또는 다각형(다변형) 이미지 맵을 그립니다.

   * **사각형 맵** - [사각형 이미지 맵] 도구를 선택하고 페이지로 드래그하여 사각형을 만듭니다. 사각형 맵에 점을 추가하려면(따라서 다각형 맵으로 변경) Ctrl 키를 누른 다음 삽입 도구를 원하는 위치에 놓고 선택합니다.

   * **다각형 맵** - [다각형 이미지 맵] 도구를 선택하고 둘러싸려는 이미지 영역의 주변에 있는 점을 선택합니다. 다각형 밀도 슬라이더를 사용하여 다각형의 점 밀도를 변경합니다. 다른 맵을 선택할 경우 원본 밀도가 저장됩니다. 다각형에서 점을 추가, 삭제 또는 이동하면 원본 밀도가 손실되고 슬라이더가 최대값으로 재설정됩니다.

1. 원하는 경우 [이미지 맵] 목록에 이미지 맵 이름을 입력합니다. 이미지 맵을 그리면 Adobe Dynamic Media Classic에서 이미지 맵에 이름을 지정합니다.

   이 이름을 만들려면 Adobe Dynamic Media Classic은 작업 중인 이미지 또는 eCatalog 페이지의 이름에 일련 번호를 추가합니다. 선택한 이름을 입력할 수 있습니다.

1. 사용자가 이미지 맵을 선택할 때 새 웹 페이지를 열려면 이미지 맵 목록에 URL을 입력합니다.

   [JavaScript 및 URL 입력](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls)을 참조하십시오.

1. 사용자가 포인터를 이미지 맵 위로 이동할 때 롤오버 텍스트를 표시하려면 [이미지 맵] 목록에 텍스트를 입력합니다. 이미지 맵 목록에서 **[!UICONTROL 표시]** 메뉴 및 선택 **[!UICONTROL 롤오버 텍스트]**. 그런 다음 사용자에게 화면에 표시할 텍스트를 입력합니다. 워드 프로세서에서 텍스트를 작성하고 [롤오버 텍스트] 필드에 복사할 수 있습니다.

1. 사용자가 마우스를 이미지 맵 위로 이동할 때 다른 작업 효과를 발생시키려면 작업을 정의합니다. 다음에서 **[!UICONTROL 표시]** 드롭다운 목록에서 다음을 선택합니다. **[!UICONTROL 기타 작업]**. 작업의 특성을 입력합니다. (다음으로 이동 **[!UICONTROL 표시]** > **[!UICONTROL 모두]** 이미지 맵에 대한 롤오버 텍스트 및 작업을 만들려면)

   다음을 참조하십시오 [이미지 맵에 대한 다른 작업 정의](creating-image-maps.md#defining_other_actions_for_image_maps).

1. 다음 중 하나를 수행합니다(선택 사항).

   * 이미지 맵을 미리 보려면 다음을 선택합니다 **[!UICONTROL 미리 보기]**.
   * 이미지 맵 또는 다각형 꼭지점을 삭제하려면 이미지에서 모양을 선택한 다음 를 선택합니다 **[!UICONTROL 삭제]**. 또는 eCatalog의 경우 Order Pages 탭에서 을 선택합니다. **[!UICONTROL 맵 지우기]** 모든 페이지에서 이미지 맵을 제거합니다.
   * 이미지, 회전 집합의 이미지 또는 eCatalog 페이지에서 이미지 맵을 일시적으로 제거하려면 삭제하지 않고 [이미지 맵] 목록에서 해당 [켜짐] 선택 사항을 선택 취소합니다.

1. 선택 **[!UICONTROL 저장]**.

### 이미지 맵의 위치, 모양 및 크기 조정 {#adjusting-the-position-shape-and-size-of-image-maps}

이미지 맵의 위치, 모양 및 크기를 변경하려면 [이미지 맵] 단추 를 선택합니다. 그런 다음 **[!UICONTROL 패닝]** 도구를 사용한 다음 지침을 따릅니다.

* **위치 변경** - 포인터를 이미지 맵의 테두리 근처로 이동하지 않고 옆으로 이동합니다. 십자형 화살표 아이콘이 표시되면 맵을 새 위치로 드래그합니다.

* **크기 및 모양 변경** - 이미지 맵의 모양과 크기를 변경하는 방법은 사각형 또는 다각형 이미지 맵으로 작업하고 있는지 여부에 따라 달라집니다.

>[!TIP]
>
>화면 하단에 있는 [크기] 슬라이더를 끌어 보기를 변경하고 이미지 맵 보기를 향상시킬 수 있습니다.

* **사각형 이미지 맵** - 이미지 맵의 한 쪽이나 모서리 위로 포인터를 이동합니다. 양면 화살표 아이콘이 표시되면 끌기를 시작합니다. Shift 키를 누른 상태로 끌어 크기를 변경하지만 종횡비(모양)는 유지합니다.

* **다각형 이미지 맵** - 사각형 선택 핸들을 드래그합니다. 선택 핸들을 만들려면 이미지 맵의 테두리를 선택하고 드래그를 시작합니다.

### 겹치는 이미지 맵 처리 {#handling-overlapping-image-maps}

이미지나 eCatalog 페이지에 이미지 맵이 여러 개 포함되어 있고 맵이 겹치는 경우 맵이 겹치는 방식을 결정할 수 있습니다. 이렇게 하려면 [이미지 맵] 목록에서 맵 순서를 변경합니다. 맵 이름을 목록에서 위나 아래로 드래그합니다. 목록에서 이름이 표시되는 위치에 따라 해당 이미지 맵이 다른 이미지 맵과 겹치는지 여부가 결정됩니다.

### 이미지 맵 데이터 가져오기 {#importing-image-map-data}

각 페이지에서 이미지 맵 데이터를 입력하는 대신 이미지, 회전 집합 또는 eCatalog의 데이터를 [맵 요약] 화면으로 가져올 수 있습니다. 탭으로 구분된 파일이나 XML DTD 형태로 이미지 맵 데이터를 가져옵니다. 파일의 필드는 [맵 요약] 화면에 표시된 순서대로 정렬되어야 합니다(이름, 목차 레이블, 맵, URL, 롤오버 텍스트, 다른 작업 및 검색 문자열). 이미지 맵 데이터를 가져오면 각 이미지 맵을 만들 때 [이미지 맵] 목록에 데이터를 입력하지 않아도 됩니다.

**이미지 맵 데이터를 가져오려면:**

1. 이미지 맵 편집기 페이지(이미지 또는 회전 집합의 이미지) 또는 eCatalog 편집 화면의 [맵 페이지] 탭으로 이동합니다.
1. 선택 **[!UICONTROL 메타데이터 가져오기]**.
1. 메타데이터 업로드 대화 상자에서 이미지 또는 이미지 맵 을 선택하여 원하는 에셋 속성 유형에서 메타데이터를 업로드합니다.
1. [파일 생성] 드롭다운 목록에서 만들려는 파일 유형을 선택합니다.
1. (선택 사항) 선택 **[!UICONTROL 생성]** 만들려는 파일 형식을 기반으로 결과 데이터를 미리 봅니다. 선택 **[!UICONTROL 닫기]** 메타데이터 업로드 대화 상자로 돌아갑니다.
1. 업로드할 파일을 찾습니다. [파일 이름] 텍스트 필드에 생성된 파일의 이름을 지정합니다.
1. (선택 사항) [작업 이름] 필드에 메타데이터 업로드 작업의 이름을 지정합니다.
1. 선택 **[!UICONTROL 업로드]**.

### 이미지 맵 복사 {#copying-image-maps}

이미지나 eCatalog 페이지의 이미지 맵을 다른 이미지나 eCatalog 페이지에 복사할 수 있습니다. 사용 **[!UICONTROL 이미지 맵 복사]** 먼저 제작을 시작하십시오. 이미지 맵을 복사하여 레이아웃이나 매핑 구조를 공유하는 이미지나 페이지에 다시 만들 수도 있습니다.

예를 들어 eCatalog의 이미지 맵 복사는 동일한 eCatalog의 외국어 버전 간에 모든 이미지 맵을 복사하는 편리한 방법입니다. 최상의 결과를 내려면 페이지 수와 이미지가 동일한 eCatalog 간에 복사하십시오. 복사하는 eCatalog에 이미 이미지 맵이 포함되어 있는 경우 복사가 수행될 때 해당 이미지 맵이 삭제됩니다.

**이미지 맵을 복사하려면:**

1. 이미지 맵 편집기 페이지(이미지 또는 회전 집합의 이미지) 또는 eCatalog 편집 화면의 [맵 페이지] 탭으로 이동합니다.
1. 선택 **[!UICONTROL 다음 위치에 맵 복사]**.
1. 이미지에서 이미지 맵을 복사하는지, 아니면 eCatalog에서 이미지 맵을 복사하는지에 따라 다음 중 하나를 수행합니다.

   * (이미지) [이미지 선택] 화면에서 이미지 맵을 복사할 타겟 이미지를 선택합니다.
   * (eCatalog) [자산 선택] 화면에서 이미지 맵을 복사할 타겟 이미지 또는 eCatalog 페이지를 선택합니다.

1. 선택 **[!UICONTROL 선택]**.

## 템플릿을 사용하여 JavaScript 및 URL 입력 {#using-a-template-to-enter-javascript-and-urls}

보다 쉽고 효율적으로 이미지 맵 URL을 입력하기 위해 URL 템플릿(Href 템플릿이라고도 함)을 정의할 수 있습니다. 대부분의 이미지 맵 URL이 고정된 일반 형식을 공유하는 경우 URL 템플릿을 정의합니다. 고정된 URL 부분을 URL 템플릿으로 입력하면 이미지 맵을 만들 때마다 URL의 이 부분을 입력할 필요가 없습니다. URL 템플릿에 JavaScript 명령, 경로 이름 및 매개 변수를 포함할 수도 있습니다. 기본적으로 URL 템플릿에는 이라는 자체 Adobe Dynamic Media Classic JavaScript 핸들러가 포함되어 있습니다. `loadProduct` 그러면 새 창에서 이미지가 열립니다.

>[!NOTE]
>
>JavaScript 코드를 이미지 맵의 HREF 속성에 추가하면 해당 코드가 클라이언트의 컴퓨터에서 실행됩니다. 따라서 JavaScript 코드가 안전한지 확인하십시오.

### URL 템플릿 정보 {#about-url-templates}

URL 템플릿은 [이미지 맵] 목록의 URL 열 내용을 템플릿의 이중 달러 기호(&#39;$$&#39;)로 대체하는 방식으로 작동합니다.

```as3
Javascript:loadProduct(‘$$’);void(0);
```

이미지 맵 간에 변경되지 않는 모든 값은 URL 템플릿에 배치합니다. 변경되는 값만 [이미지 맵] 목록의 URL 열에 추가합니다. 예:

* URL 템플릿 - `javascript:loadProduct(‘https://www.examplesitehere.com/$$’);void(0);`
* URL 값 - `product.htm`
* 실제 URL 생성됨 - `javascript:loadProduct(‘https://www.examplesitehere.com/product.html);void(0);`

기본적으로 URL 템플릿에는 이라는 자체 Adobe Dynamic Media Classic JavaScript 핸들러가 포함되어 있습니다. `loadProduct` 그러면 URL 대상이 있는 새 창이 열립니다. 그러나 모든 JavaScript 코드를 사용하여 이 JavaScript 핸들러를 바꾸거나 다음 Adobe Dynamic Media Classic 핸들러 중 하나를 사용할 수 있습니다.

* `loadProductCW` - URL 열에 지정된 URL 타겟을 현재 창에 표시합니다. 이 핸들러는 주로 웹 사이트 내의 페이지에 통합된 eCatalog에 사용됩니다.

* `loadProductPW` - 상위 창(현재 창을 연 페이지)의 URL 열에 지정된 URL 대상을 표시합니다. 현재 창은 열려 있지만 상위 창이 URL 타겟을 표시하도록 변경됩니다.

  >[!NOTE]
  >
  >핸들러 `loadProductPW`는 DHTML 및 HTML5 뷰어를 지원하지 않습니다.

### URL 템플릿 만들기 {#creating-a-url-template}

1. [맵 편집기] 화면(이미지 또는 회전 집합) 또는 eCatalog 화면((eCatalog)의 [맵 페이지] 탭에서 [URL 템플릿] 옵션 옆에 있는 [편집]을 선택합니다. [맵 템플릿 편집] 대화 상자가 열립니다.
1. JavaScript 코드와 전체 URL(변수 부분이 달러 기호로 대체됨)을 입력합니다. [$$]). 마우스 오른쪽 단추를 클릭하고 을 선택하여 코드를 붙여넣을 수 있습니다. **[!UICONTROL 붙여넣기]**.
1. 선택 **[!UICONTROL 저장]**.

### URL 템플릿 처리 {#handling-url-templates}

[맵 편집기] 페이지(이미지와 회전 집합) 및 eCatalog 화면(eCatalog)의 [맵 페이지] 탭에서는 URL 템플릿을 처리하는 다음 명령을 제공합니다.

* **URL 템플릿 옵션** - URL 템플릿 옵션을 선택하여 이미지 또는 eCatalog 페이지의 모든 이미지 맵에 URL 템플릿을 적용합니다.

* **템플릿 옵션** - 개별 이미지 맵에서 URL 템플릿을 사용하지 않으려면 URL 이미지 맵 목록에서 템플릿 옵션을 선택 취소합니다.

## 이미지 맵에 대한 다른 작업 정의 {#defining-other-actions-for-image-maps}

다음을 선택할 수 있습니다. **[!UICONTROL 표시]** 메뉴 및 선택 **[!UICONTROL 기타 작업]** 롤오버 텍스트 및 웹 페이지 시작 이외의 작업을 트리거합니다. 사용자가 포인터를 이미지 맵 위로 이동할 때 작업을 시작할 수 있습니다. 이러한 작업은 World Wide Web Consortium HTML 사양에서 클라이언트측 이미지 맵에 대해 정의된 특성입니다. 그러한 보고서는 아래와 같습니다.

* **`accesskey`** - 사용자가 키보드에서 지정된 키를 누를 때 작업을 트리거합니다.

* **`onfocus`** - 커서, 누르기 또는 액세스 키 누름에 의해 이미지 맵에 포커스가 있을 때 이벤트를 트리거합니다. 예를 들어 이미지 맵에 포커스가 있을 때 웹 페이지를 시작하고 이미지 맵이 포커스를 잃을 때 웹 페이지를 닫을 수 있습니다.

* **`onblur`** - 커서 또는 누르기에 의해 이미지 맵이 포커스를 잃을 때 이벤트를 트리거합니다.

**이미지 맵의 다른 작업을 정의하려면:**

1. eCatalog 화면의 맵 편집기 화면(이미지 및 스핀 세트)이나 맵 페이지 탭(eCatalogs)에서 **[!UICONTROL 표시]** 메뉴 및 선택 **[!UICONTROL 기타 작업]**.
1. World Wide Web Consortium HTML 사양에 지정된 구문을 사용하여 [이미지 맵] 목록의 [다른 작업] 열에 지원되는 특성을 추가합니다.
1. 선택 **[!UICONTROL 저장]**.

다음 항목 선택 **[!UICONTROL 표시]** 메뉴 및 선택 **[!UICONTROL 모두]** 이미지 맵에 롤오버 텍스트 및 작업을 사용하려는 경우

## Adobe Acrobat 또는 Adobe InDesign에서 이미지 맵 만들기 {#creating-image-maps-in-adobe-acrobat-or-adobe-indesign}

Adobe Acrobat 또는 Adobe InDesign에서 eCatalog를 디자인하는 동안 이미지 맵을 만들 수 있습니다.

Adobe Acrobat 또는 Adobe InDesign에서 이미지 맵을 표시할 위치에 하이퍼링크 참조를 만들고 이미지 맵의 URL 위치를 지정합니다. PDF 파일을 Adobe Dynamic Media Classic에 업로드할 때 링크 추출 옵션을 선택하면 링크가 이미지 맵으로 자동 변환됩니다.

자세한 내용은 Adobe InDesign 도움말 또는 Adobe Acrobat 도움말을 참조하십시오.

### Adobe InDesign에서 이미지 맵 만들기 {#to-create-image-maps-in-adobe-indesign}

1. Adobe InDesign에서 **[!UICONTROL Windows®]** > **[!UICONTROL 인터랙티브한]** > **[!UICONTROL 하이퍼링크]**.
1. [하이퍼링크] 패널에서 이미지 맵으로 만들 텍스트, 프레임 또는 그래픽을 선택합니다.
1. 선택 **[!UICONTROL 새 하이퍼링크]** 을 클릭합니다.
1. 새 하이퍼링크 대화 상자의 **[!UICONTROL 링크 대상]** 메뉴, 선택 **[!UICONTROL URL]**.
1. URL 상자에 제품 ID를 입력하거나 붙여 넣습니다.
1. 선택 **[!UICONTROL 확인]**. (Adobe Dynamic Media Classic은 이미지 맵 URL 템플릿을 사용하여 URL을 완료합니다.)

   >[!NOTE]
   >
   >Adobe InDesign에서는 모양 옵션을 설정할 필요가 없습니다. Adobe Dynamic Media Classic에서 모양을 지정할 수 있습니다.

1. 만들려는 모든 이미지 맵에 대해 2-6 단계를 반복합니다.
1. 파일을 PDF로 내보냅니다.
1. Adobe Dynamic Media Classic에 PDF을 업로드합니다.
1. 위치 **[!UICONTROL PDF 옵션]**, 선택 **[!UICONTROL 링크 추출]**.

### Adobe Acrobat에서 이미지 맵 만들기 {#to-create-image-maps-in-adobe-acrobat}

1. Adobe Acrobat에서 **[!UICONTROL 도구]** > **[!UICONTROL 고급 편집]** > **[!UICONTROL 링크 도구]**.
1. 마우스를 끌어 이미지 맵을 만듭니다.
1. Create Link 상자에서 **[!UICONTROL 사용자 지정 링크]**, 및 선택 **[!UICONTROL 다음]**.

>[!NOTE]
>
>Adobe Acrobat에서는 모양 옵션을 설정할 필요가 없습니다. Adobe Dynamic Media Classic에서 모양을 지정할 수 있습니다.

1. Link Properties 상자에서 **[!UICONTROL 작업]**.
1. 선택 **[!UICONTROL 웹 링크 열기]** 작업 선택 메뉴에서 을(를) 선택한 다음 **[!UICONTROL 추가]**.
1. URL 편집 상자에 이미지 맵의 제품 ID를 입력하고 다음을 선택합니다. **[!UICONTROL 확인]**. (Adobe Dynamic Media Classic은 이미지 맵 URL 템플릿을 사용하여 URL을 완료합니다.)
1. 만들려는 모든 이미지 맵에 대해 1-7 단계를 반복합니다.
1. 파일을 저장합니다.
1. Adobe Dynamic Media Classic에 PDF을 업로드하고 PDF 옵션에서 링크 추출 을 선택합니다.
