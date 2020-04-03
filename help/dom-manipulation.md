---
title: DOM 조작
seo-title: DOM 조작
description: 널
seo-description: DOM 조작에 대한 자세한 내용을 살펴보십시오.
uuid: 275cd49d-2a55-41f9-80b0-e147d0cd2907
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template-publishing
discoiquuid: 890ca93e-3146-4347-864b-bd5e94037038
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# DOM 조작{#dom-manipulation}

DOM(문서 개체 모델) 조작은 해당 XML 코드를 직접 조작하여 디자인 파일을 편집하는 기술입니다. DOM 조작을 통해 컨텐츠 및 변경을 비롯하여 변수 디자인 요소를 보다 강력하게 제어할 수 있습니다. 필요에 따라 새 요소를 만들 수도 있습니다.

Dynamic Media Classic에서는 템플릿이 게시된 후 URL 명령을 통해 Dynamic Media Classic FXG 템플릿의 DOM을 조작할 수 있습니다. FXG 템플릿의 디자인 요소는 URL을 통해 명령을 전달하여 조작됩니다. 이렇게 하면 특성을 동적으로 조작하고 그래픽에 추가할 수 있습니다.

DOM 조작을 사용하려면 Illustrator 파일에 s7:elementID를 만든 후 Dynamic Media Classic FXG 파일로 변환한 다음 SPS에 업로드합니다.

>[!NOTE]
>
>DOM 조작 명령을 사용하는 경우 전달되는 모든 값을 URL로 인코딩해야 합니다.

>[!NOTE]
>
>Illustrator Plug-in for Web-to-Print (for converting Illustrator files) converts to FXG 2.0. For information about this specification, see [www.adobe.com/go/learn_s7_fxg2_en](https://www.adobe.com/go/learn_s7_fxg2_en).

## Illustrator 파일에서 s7:elementID 만들기 {#creating-s-elementids-in-illustrator-files}

Illustrator에서 만든 디자인에 DOM 조작을 사용하려면 Illustrator 디자인에 s7:elementID를 만듭니다. s7:elementID를 만들면 템플릿이 게시된 후 URL 명령을 사용하여 디자인 요소를 수정할 수 있습니다.

### 텍스트의 DOM 조작을 위해 s7:elementID 만들기 {#creating-s-elementids-for-dom-manipulation-of-text}

텍스트 개체의 DOM 조작을 만들려면 Illustrator에서 [레이어] 패널을 엽니다. 변수 텍스트가 포함된 텍스트 레이어에서 s7:elementID를 사용하여 레이어 이름을 지정합니다. To do so, enter the letters `id` (for identification), a colon ( `:`), and a name. 다음은 s7:elementID 텍스트 레이어 이름의 예입니다.

`id:BirthdayBoyName`

`id:DateofBirth`

`id:EnterFirstNameHer`

### 개체의 DOM 조작을 위해 s7:elementID 만들기 {#creating-s-elementids-for-dom-manipulation-of-objects}

최종 사용자가 개체 특성을 변경할 수 있게 하려는 경우 개체의 s7:elementID를 만듭니다. 개체는 전체 텍스트 프레임, 그래픽 및 이미지를 구성할 수 있습니다. 배경색은 개체 요소 ID의 예입니다. 세션이 변경되면 최종 사용자가 세션에 적합한 포스터를 만들기 위해 포스터의 배경색을 바꿀 수 있습니다.

Illustrator에서 개체의 s7:elementID를 만들려면 먼저 개체에 대한 별도 레이어를 만듭니다.

Illustrator에서 개체의 s7:elementID를 만들려면 다음 단계를 수행합니다.

1. 객체를 선택합니다.
1. 창 **>** 레이어를 **클릭합니다**.
1. 레이어 패널에서 개체 레이어의 이름을 s7:elementID로 지정합니다. To do so, enter the letters `id` (for identification), a colon ( `:`), and description to identify the element. 다음은 s7:elementID 개체 레이어 이름의 예입니다.

   `id:BackgroundColor`

   `id:RotationPercentage`

   `id:JacketJPG`

## FXG 템플릿 게시 {#publish-fxg-templates}

FXG 템플릿을 게시하면 웹 사이트 및 애플리케이션에서 사용할 수 있는 Dynamic Media Classic 서버에 배치됩니다. 게시 프로세스에서 Scene7 Publishing System이 웹 사이트 또는 애플리케이션에 필요한 URL을 활성화합니다.

>[!NOTE]
>
>FXG 템플릿을 사용하려면 글꼴과 이미지를 포함하여 템플릿을 만드는 데 사용된 모든 컨텐츠를 게시합니다. 필수 파일을 모두 포함하지 않으면 게시할 때 오류 메시지가 나타납니다.

### FXG 템플릿을 게시로 표시 {#mark-fxg-templates-for-publish}

Dynamic Media 이미지 서버에 배치하려면 템플릿과 모든 지원 파일을 게시로 표시해야 합니다.

1. 찾아보기 패널에서 사용되는 그래픽, 이미지 및 글꼴과 함께 FXG 템플릿을 선택합니다.
1. 게시로 **표시를 클릭합니다**.

### FXG 템플릿 게시 {#publish-your-fxg-template}

1. 글로벌 탐색 막대에서 **[게시]**&#x200B;를 클릭합니다.
1. [시기] 선택 사항을 선택하고 선택적으로 게시 작업의 이름을 입력합니다.
1. Click **Start Publish**.

### 텍스트 오버플로우 표시기 표시 {#text-overflow-indicator-display}

*텍스트 오버플로우 표시기*&#x200B;는 텍스트가 텍스트 프레임(또는 스레드 텍스트인 경우 마지막 텍스트 프레임)에서 지정된 공간을 초과하는 경우를 보여 줍니다. 이 표시기는 위에 더하기 기호가 있는 빨간색 상자입니다. SPS의 텍스트 오버플로우 표시기는 항상 활성화됩니다.

텍스트 오버플로우 표시기는 `markOverflowingTextFrame` 수정자를 사용하여 제어합니다. 다음과 같이 수정자를 사용합니다.

| 수정자/값 | 설명 |
|--- |--- |
| markOverflowingTextFrame=0,1 | 값이 1이면 텍스트 오버플로우 표시기가 나타납니다. 기본값은 0입니다. 기본값은 0이지만 SPS의 텍스트 오버플로우 표시기는 항상 활성화됩니다. markOverflowingTextFrame 수정자는 대/소문자를 구분합니다. |

>[!MORELIKETHIS]
>
>* [가변성 정의: 매개 변수화 및 DOM 조작](defining-variability-parameterization-versus-dom.md#defining_variability_parameterization_versus_dom_manipulation)
>* [Publishing](publishing-files.md#publishing_files)

