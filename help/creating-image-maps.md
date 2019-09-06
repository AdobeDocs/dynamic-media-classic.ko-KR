---
title: 이미지 맵 만들기
seo-title: 이미지 맵 만들기
description: 널
seo-description: 이미지 맵을 만드는 방법을 살펴봅니다.
uuid: 0 DCC 4956-006 E -4 A 74-9 D 6 A -6 D 4 BB 23790 CE
contentOwner: 관리
content-type: 참조
products: sg_ Experiencemanager/dynamic-media-scene -7
geptopics: sg_ scenesevenondemand_ pk/categories/master_ files
discoiquuid: 4 EDDF 983-38 CB -4 F 00-B 3 BE -85 C 20 BDD 6 F 69
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# 이미지 맵 만들기{#creating-image-maps}

이미지 맵은 이미지, eCatalog 페이지 또는 회전 집합 이미지의 영역으로, 텍스트가 있는 롤오버 패널을 표시합니다. 사용자가 이미지 맵을 클릭하면 일종의 작업이 트리거됩니다. 예를 들어 사용자가 제품에 대한 자세한 정보를 확인할 수 있도록 웹 페이지가 시작됩니다. 이미지 맵에 주의하도록 사용자가 포인터를 이미지 위로 이동할 때 이미지 맵 주위에 윤곽이 나타납니다.

Dynamic Media Classic에서 이미지 맵을 만드는 기능 외에 Adobe Acrobat 또는 Adobe InDesign에서 카탈로그를 디자인할 때 이미지 맵을 만들 수도 있습니다.

이미지 맵을 만들 때 다음 중 원하는 작업을 수행할 수 있습니다.

* 롤오버 텍스트를 입력합니다.
* 웹 페이지를 시작하기 위한 JavaScript 및 URL을 입력합니다.
* 이미지 맵에 사용할 URL 템플릿을 만듭니다.
* 이미지 맵을 다른 이미지, eCatalog 페이지 또는 회전 집합에 복사합니다.
* 이미지 맵을 CSV 또는 XML로 내보냅니다.
* 탭으로 구분된 파일이나 XML 파일에서 이미지 메타데이터를 가져옵니다.
* World Wide Web Consortium의 결정에 따라 기타 작업을 정의합니다.
* 이미지 맵을 미리 봅니다.

## 이미지 맵 그리기 및 조정 {#drawing-and-adjusting-an-image-map}

1. 다음 중 하나를 수행하십시오.

   * If you are working with an image in the Grid View or List View, in the Edit drop-down list click **Image Map**. Or, open it in Detail View, and then click **Image Map** above the image.
   * If you are working with a SpinSet in the Grid View or List View, click **Edit**. Or, open it in Detail View, and then click **Edit**. Select an image asset, and then click **Image Map**.
   * If you are working with an eCatalog, in the Grid View, List View, Detail View, click **Edit**. **맵 페이지** 탭을 클릭합니다.
   ![](assets/ma_image_map.png)

1. 사각형 또는 다각형(다변형) 이미지 맵을 그립니다.

   **사각형 맵** 사각형 이미지 맵을 선택하고 페이지에서 드래그하여 사각형을 만듭니다. 사각형 맵에 점을 추가하여 다각형 맵으로 변경하려면 Ctrl 키를 누르고 원하는 위치에 삽입 도구를 놓은 다음 클릭합니다.

   **다각형 맵** 다각형 이미지 맵 도구를 선택하고 묶으려는 이미지 영역 경계의 점을 클릭합니다. 다각형 밀도 슬라이더를 사용하여 다각형의 점 밀도를 변경합니다. 다른 맵을 선택할 경우 원본 밀도가 저장됩니다. 다각형에서 점을 추가, 삭제 또는 이동하면 원본 밀도가 손실되고 슬라이더가 최대값으로 재설정됩니다.

1. 원하는 경우 [이미지 맵] 목록에 이미지 맵 이름을 입력합니다. 이미지 맵을 그리면 Dynamic Media Classic에서 해당 맵을 지정합니다.

   이름을 만들기 위해 Dynamic Media Classic는 작업 중인 이미지 또는 ecatalog 페이지의 이름에 순차적 번호를 추가합니다. 선택한 이름을 입력할 수 있습니다.

1. 사용자가 [이미지 맵]을 클릭할 때 새 웹 페이지를 열려면 [이미지 맵] 목록에 URL을 입력합니다.

   [JavaScript 및 URL 입력](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls)을 참조하십시오.

1. 사용자가 포인터를 이미지 맵 위로 이동할 때 롤오버 텍스트를 표시하려면 [이미지 맵] 목록에 텍스트를 입력합니다. [이미지 맵] 목록에서 [표시] 메뉴를 선택한 다음 [롤오버 텍스트]를 선택합니다. 화면에서 사용자에게 표시할 텍스트를 입력합니다. 워드 프로세서에서 텍스트를 작성하고 [롤오버 텍스트] 필드에 복사할 수 있습니다.
1. 사용자가 마우스를 이미지 맵 위로 이동할 때 다른 작업 효과를 발생시키려면 작업을 정의합니다. [표시] 드롭다운 목록에서 [다른 작업]을 클릭합니다. 작업의 특성을 입력합니다. 이미지 맵의 작업과 롤오버 텍스트를 만들려면 [표시] &gt; [두 가지 모두]를 클릭합니다.

   [이미지 맵의 다른 작업 정의](creating-image-maps.md#defining_other_actions_for_image_maps)를 참조하십시오.

1. 다음 중 하나를 수행합니다(선택 사항).

   * [미리 보기]를 클릭하여 이미지 맵을 미리 봅니다.
   * 이미지 맵이나 다각형 꼭지점을 삭제하려면 이미지에서 모양을 선택하고 [삭제]를 클릭합니다. 또는 eCatalog의 경우 [주문 페이지] 탭에서 [맵 지우기]를 클릭하여 모든 페이지에서 이미지 맵을 제거합니다.
   * 이미지, 회전 집합의 이미지 또는 eCatalog 페이지에서 이미지 맵을 일시적으로 제거하려면 삭제하지 않고 [이미지 맵] 목록에서 해당 [켜짐] 선택 사항을 선택 취소합니다.

1. [저장]를 클릭합니다.

### 이미지 맵의 위치, 모양 및 크기 조정 {#adjusting-the-position-shape-and-size-of-image-maps}

이미지 맵의 위치, 모양 및 크기를 변경하려면 [이미지 맵] 단추 를 선택합니다. 그런 다음 패닝 툴을 선택하고 다음 지침을 따르십시오.

**위치** 변경 포인터를 이미지 맵의 테두리 위가 아닌 근처로 이동합니다. 십자형 화살표 아이콘이 표시되면 맵을 새 위치로 드래그합니다.

**크기를 변경하고 이미지 맵의 모양과 크기를** 변경하는 방법은 사각형 또는 다각형 이미지 맵을 사용한 작업 여부에 따라 달라집니다.

***팁**: 화면 하단에 있는 크기 슬라이더를 드래그하여 뷰를 변경하고 이미지 맵을 보다 잘 볼 수 있습니다.*

**사각형 이미지 맵** 포인터를 이미지 맵의 측면 또는 모서리 위로 이동합니다. 양면 화살표 아이콘이 표시되면 끌기를 시작합니다. Shift 키를 누른 상태로 끌어 크기를 변경하지만 종횡비(모양)는 유지합니다.

**다각형 이미지 맵정사각형** 선택 핸들을 드래그합니다. 선택 핸들을 만들려면 이미지 맵의 테두리를 클릭하고 끌기를 시작합니다.

### 겹치는 이미지 맵 처리 {#handling-overlapping-image-maps}

이미지나 eCatalog 페이지에 이미지 맵이 여러 개 포함되어 있고 맵이 겹치는 경우 맵이 겹치는 방식을 결정할 수 있습니다. 이렇게 하려면 [이미지 맵] 목록에서 맵 순서를 변경합니다. 맵 이름을 목록에서 위나 아래로 드래그합니다. 목록에서 이름이 표시되는 위치에 따라 해당 이미지 맵이 다른 이미지 맵과 겹치는지 여부가 결정됩니다.

### 이미지 맵 데이터 가져오기 {#importing-image-map-data}

각 페이지에서 이미지 맵 데이터를 입력하는 대신 이미지, 회전 집합 또는 eCatalog의 데이터를 [맵 요약] 화면으로 가져올 수 있습니다. 탭으로 구분된 파일이나 XML DTD 형태로 이미지 맵 데이터를 가져옵니다. 파일의 필드는 [맵 요약] 화면에 표시된 순서대로 정렬되어야 합니다(이름, 목차 레이블, 맵, URL, 롤오버 텍스트, 다른 작업 및 검색 문자열). 이미지 맵 데이터를 가져오면 각 이미지 맵을 만들 때 [이미지 맵] 목록에 데이터를 입력하지 않아도 됩니다.

**이미지 맵 데이터를 가져오려면**

1. 이미지 맵 편집기 페이지(이미지 또는 회전 집합의 이미지) 또는 eCatalog 편집 화면의 [맵 페이지] 탭으로 이동합니다.
1. [메타데이터 가져오기]를 클릭합니다.
1. [메타데이터 업로드] 대화 상자에서 [이미지] 또는 [이미지 맵]을 클릭하여 원하는 자산 속성 유형의 메타데이터를 업로드합니다.
1. [파일 생성] 드롭다운 목록에서 만들려는 파일 유형을 선택합니다.
1. (선택 사항) [생성]을 클릭하여 만들려는 파일 유형을 기준으로 결과 데이터를 미리 봅니다. [닫기]를 클릭하여 [메타데이터 업로드] 대화 상자로 돌아갑니다.
1. 업로드할 파일을 찾습니다. [파일 이름] 텍스트 필드에 생성된 파일의 이름을 지정합니다.
1. (선택 사항) [작업 이름] 필드에 메타데이터 업로드 작업의 이름을 지정합니다.
1. [업로드]를 클릭합니다.

### 이미지 맵 복사 {#copying-image-maps}

이미지나 eCatalog 페이지의 이미지 맵을 다른 이미지나 eCatalog 페이지에 복사할 수 있습니다. 이미지 맵을 빨리 만들려면 [이미지 맵 복사]를 사용합니다. 이미지 맵을 복사하여 동일한 레이아웃이나 매핑 구조를 공유하는 이미지 또는 페이지에 다시 만들 수도 있습니다.

예를 들어 eCatalog의 이미지 맵 복사는 동일한 eCatalog의 외국어 버전 간에 모든 이미지 맵을 복사하는 편리한 방법입니다. 최상의 결과를 내려면 페이지 수와 이미지가 동일한 eCatalog 간에 복사하십시오. 복사하는 타겟 eCatalog에 이미지 맵이 이미 포함되어 있으면 복사 시 해당 이미지 맵이 삭제됩니다.

**이미지 맵을 복사하려면**

1. 이미지 맵 편집기 페이지(이미지 또는 회전 집합의 이미지) 또는 eCatalog 편집 화면의 [맵 페이지] 탭으로 이동합니다.
1. [다음 위치에 [맵 복사]를 클릭합니다.
1. 이미지에서 이미지 맵을 복사하는지, 아니면 eCatalog에서 이미지 맵을 복사하는지에 따라 다음 중 하나를 수행합니다.

   * (이미지) [이미지 선택] 화면에서 이미지 맵을 복사할 타겟 이미지를 선택합니다.
   * (eCatalog) [자산 선택] 화면에서 이미지 맵을 복사할 타겟 이미지 또는 eCatalog 페이지를 선택합니다.

1. [선택]을 클릭합니다.

## 템플릿을 사용하여 JavaScript 및 URL 입력 {#using-a-template-to-enter-javascript-and-urls}

보다 쉽고 효율적으로 이미지 맵 URL을 입력하기 위해 URL 템플릿(Href 템플릿이라고도 함)을 정의할 수 있습니다. 대부분의 이미지 맵 URL이 고정된 일반 형식을 공유하는 경우 URL 템플릿을 정의합니다. 고정된 URL 부분을 URL 템플릿으로 입력하면 이미지 맵을 만들 때마다 URL의 이 부분을 입력할 필요가 없습니다. URL 템플릿에 JavaScript 명령, 경로 이름 및 매개 변수를 포함할 수도 있습니다. By default, the URL template contains a proprietary Dynamic Media Classic JavaScript handler called `loadProduct` that opens the image in a new window.

>[!NOTE]
>
>이미지 맵의 HREF 속성에 Javascript 코드를 추가하면 Javascript 코드가 클라이언트 컴퓨터에서 실행됩니다. 따라서 Javascript 코드가 안전한지 확인하십시오.

### URL 템플릿 정보 {#about-url-templates}

URL 템플릿은 [이미지 맵] 목록의 URL 열 내용을 템플릿의 이중 달러 기호('$$')로 대체하는 방식으로 작동합니다.

```as3
Javascript:loadProduct(‘$$’);void(0);
```

이미지 맵 간에 변경되지 않는 모든 값을 URL 템플릿에 배치합니다. 변경되는 값만 [이미지 맵] 목록의 URL 열에 추가합니다. 예:

* URL 템플릿: j `avascript:loadProduct(‘https://www.examplesitehere.com/$$’);void(0);`
* URL 값: `product.htm`
* 생성된 실제 URL: `javascript:loadProduct(‘https://www.examplesitehere.com/product.html);void(0);`

By default, the URL template includes a proprietary Dynamic Media Classic JavaScript handler called `loadProduct` that opens a new window with the URL destination. 그러나 JavaScript 코드를 사용하여 이 JavaScript 핸들러를 바꾸거나 다음 Dynamic Media Classic 핸들러 중 하나를 사용할 수 있습니다.

* `loadProductCW`

   URL 열에 지정된 URL 타겟을 현재 창에 표시합니다. 이 핸들러는 주로 웹 사이트 내의 페이지에 통합된 eCatalog에 사용됩니다.

* `loadProductPW`

   : URL 열에 지정된 URL 타겟을 상위 창(현재 창을 연 페이지)에 표시합니다. 현재 창은 열려 있지만 상위 창이 URL 타겟을 표시하도록 변경됩니다.

   *****참고: 핸들러는`loadProductPW`DHTML 및 HTML 5 뷰어를 지원하지 않습니다.*

### URL 템플릿 만들기 {#creating-a-url-template}

URL 템플릿을 만들려면:

1. [맵 편집기] 화면(이미지 또는 회전 집합) 또는 eCatalog 화면((eCatalog)의 [맵 페이지] 탭에서 [URL 템플릿] 옵션 옆에 있는 [편집]을 선택합니다. [맵 템플릿 편집] 대화 상자가 열립니다.
1. Enter the JavaScript code and the complete URL (with the variable portion replaced by dollar signs [$$]). 마우스 오른쪽 단추를 클릭하고 [붙여넣기]를 선택하여 코드를 붙여 넣을 수 있습니다.
1. [저장] 단추를 선택합니다.

### URL 템플릿 처리 {#handling-url-templates}

[맵 편집기] 페이지(이미지와 회전 집합) 및 eCatalog 화면(eCatalog)의 [맵 페이지] 탭에서는 URL 템플릿을 처리하는 다음 명령을 제공합니다.

**URL 템플릿 옵션** URL 템플릿을 선택하여 이미지 또는 ecatalog 페이지의 모든 이미지 맵에 URL 템플릿을 적용합니다.

**템플릿 선택** 개별 이미지 맵이 URL 템플릿을 사용하지 않게 하려면 URL 이미지 맵 목록에서 템플릿 옵션을 선택 취소합니다.

## 이미지 맵의 다른 작업 정의 {#defining-other-actions-for-image-maps}

[표시] 메뉴를 선택한 다음 [다른 작업]을 선택하여 롤오버 텍스트와 웹 페이지 시작 이외의 작업을 트리거할 수 있습니다. 사용자가 포인터를 이미지 맵 위로 이동할 때 작업을 시작할 수 있습니다. 이러한 작업은 World Wide Web Consortium HTML 사양에서 클라이언트측 이미지 맵에 대해 정의된 특성입니다. 그러한 보고서는 아래와 같습니다.

**Accesskey** 는 사용자가 키보드의 지정된 키를 누를 때 동작을 트리거합니다.

**Onfocus** 는 이미지 맵이 포커스를 받거나 탭하거나 액세스 키를 눌러 포커스를 받을 때 이벤트를 트리거합니다. 예를 들어 이미지 맵에 포커스가 있을 때 웹 페이지를 시작하고 이미지 맵이 포커스를 잃을 때 웹 페이지를 닫을 수 있습니다.

**Onblur** 는 이미지 맵이 커서 또는 탭 방식으로 포커스를 잃으면 이벤트를 트리거합니다.

**이미지 맵의 다른 작업을 정의하려면**

1. [맵 편집기] 화면(이미지 및 회전 집합) 또는 eCatalog 화면(eCatalog) [맵 페이지] 탭에서 [표시] 메뉴를 선택한 다음 [다른 작업]을 선택합니다.
1. World Wide Web Consortium HTML 사양에 지정된 구문을 사용하여 [이미지 맵] 목록의 [다른 작업] 열에 지원되는 특성을 추가합니다.
1. **[저장]**&#x200B;을 클릭합니다.

이미지 맵에 롤오버 텍스트와 작업을 모두 사용하려는 경우 [표시] 메뉴를 선택한 다음 [두 가지 모두]를 선택합니다.

## Adobe Acrobat 또는 Adobe InDesign에서 이미지 맵 만들기 {#creating-image-maps-in-adobe-acrobat-or-adobe-indesign}

Adobe Acrobat 또는 Adobe InDesign에서 eCatalog를 디자인하는 동안 이미지 맵을 만들 수 있습니다.

Acrobat 또는 InDesign에서 이미지 맵을 표시할 하이퍼링크 참조를 만들고 이미지 맵의 URL 위치를 지정합니다. PDF 파일을 Dynamic Media Classic에 업로드할 때 링크 추출 옵션을 선택하면 자동으로 링크가 이미지 맵으로 변환됩니다.

자세한 내용은 InDesign 도움말이나 Acrobat 도움말을 참조하십시오.

### Adobe InDesign에서 이미지 맵 만들기 {#to-create-image-maps-in-adobe-indesign}

1. InDesign에서 [창] &gt; [대화형] &gt; [하이퍼링크]를 클릭하여 [하이퍼링크] 패널을 엽니다.
1. 이미지 맵으로 만들려는 텍스트, 프레임 또는 그래픽을 선택합니다.
1. [하이퍼링크] 패널의 패널 메뉴에서 [새 하이퍼링크]를 클릭합니다.
1. [새 하이퍼링크] 대화 상자의 [다음으로 링크] 메뉴에서 [URL]을 선택합니다.
1. [URL] 상자에 제품 ID를 입력하거나 붙여 넣고 [확인]을 클릭합니다. (Dynamic Media Classic는 이미지 맵 URL 템플릿을 사용하여 URL를 완료합니다.)

   >[!NOTE]
   >
   >InDesign에서 모양 선택 사항을 설정할 필요는 없습니다. Dynamic Media Classic에서 모양을 지정할 수 있습니다.

1. 만들려는 모든 이미지 맵에 대해 2-5 단계를 반복합니다.
1. 파일을 PDF로 내보냅니다.
1. PDF를 Dynamic Media Classic에 업로드하고 PDF 옵션에서 링크 추출을 선택합니다.

### Adobe Acrobat에서 이미지 맵 만들기 {#to-create-image-maps-in-adobe-acrobat}

1. Acrobat에서 [도구] &gt; [고급 편집] &gt; [링크 도구]를 선택합니다.
1. 마우스를 끌어 이미지 맵을 만듭니다. [링크 만들기] 상자가 열립니다.
1. [사용자 지정 링크]를 선택하고 [다음]을 클릭합니다.

   *****참고: Acrobat에서 모양 옵션을 설정할 필요는 없습니다. Dynamic Media Classic에서 모양을 지정할 수 있습니다.*

1. [링크 속성] 상자에서 [작업]을 클릭합니다.
1. [작업 선택] 메뉴에서 [웹 링크 열기]를 선택하고 [추가]를 클릭합니다.
1. [URL 편집] 상자에 이미지 맵의 제품 ID를 입력하고 [확인]을 클릭합니다. (Dynamic Media Classic는 이미지 맵 URL 템플릿을 사용하여 URL를 완료합니다.)
1. 만들려는 모든 이미지 맵에 대해 1-7 단계를 반복합니다.
1. 파일을 저장합니다.
1. PDF를 Dynamic Media Classic에 업로드하고 PDF 옵션에서 링크 추출을 선택합니다.
