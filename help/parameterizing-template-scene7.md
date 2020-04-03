---
title: Dynamic Media Classic에서 템플릿 매개 변수화
seo-title: Dynamic Media Classic에서 템플릿 매개 변수화
description: 널
seo-description: Dynamic Media Classic에서 템플릿을 매개 변수화하는 방법 알아보기
uuid: 27c8c8b4-47f3-4270-a6db-d304648ba357
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template-publishing
discoiquuid: df1a9ff5-a5ba-4480-ba0d-a19bc665f907
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Dynamic Media Classic에서 템플릿 매개 변수화{#parameterizing-a-template-in-scene}

Dynamic Media Classic FXG로 저장한 Illustrator 템플릿을 Scene7 Publishing System에 업로드한 후 변수 요소를 정의할 수 있습니다. 이렇게 하려면 [템플릿 게시 작성] 및 [미리 보기] 화면에서 변수 요소를 매개 변수화합니다. Dynamic Media Classic에서는 레이어 및 해당 속성에 텍스트 및 개체 매개 변수를 정의하는 도구를 제공합니다. 한 템플릿의 여러 버전을 만들 수도 있습니다.

FXG 템플릿을 매개 변수화하면 템플릿의 텍스트, 이미지 및 그래픽 가변성을 사용자 지정할 수 있습니다. 예를 들어 최종 사용자가 웹 사용자 인터페이스를 통해 텍스트를 수정할 수 있도록 한 줄의 텍스트를 매개 변수화할 수 있습니다. 최종 사용자가 필드에 개인 설정된 텍스트를 채울 수 있도록 빈 텍스트 필드를 변수로 정의할 수 있습니다. Dynamic Media Classic Template Publishing Build 화면에서 디자인 요소의 특성과 속성을 매개 변수화할 수도 있습니다.

>[!NOTE]
>
>DOM 조작을 사용하려는 경우에는 Dynamic Media Classic에서 템플릿을 매개 변수화할 필요가 없습니다.

## FXG 템플릿에서 매개 변수 정의 {#defining-parameters-in-fxg-templates}

Dynamic Media Classic에서 다음 단계에 따라 FXG 템플릿의 매개 변수를 정의합니다.

1. [찾아보기] 창에서 FXG 파일을 선택합니다.
1. Click **Build** and choose **Template Publishing**, or click the file’s **Edit** button.

   [템플릿 게시] 화면이 열립니다.

1. LRCo\FXG\Welcome_Summit_10 (FXG 파일)을 선택하고 [ **작성** ] > [템플릿 **게시]를 클릭합니다**.</p>

   ![](assets/wp_fxg_edit.png)

1. [템플릿 게시] 화면의 [레이어] 패널에서 매개 변수화하려는 요소가 포함된 레이어를 선택합니다.

   >[!NOTE]
   >
   >눈 아이콘을 클릭하여 켰다가 꺼서 원하는 개체를 선택했는지 확인합니다.

1. [속성] 패널에서 [이름] 열(텍스트 매개 변수화) 또는 [매개 변수] 열(개체 매개 변수화)에서 매개 변수를 클릭합니다.

   * **텍스트텍스트**&#x200B;필드를 클릭합니다(속성 목록 아래쪽으로 스크롤하여 찾기). [매개 변수] 대화 상자가 나타납니다. Select the text that you want to parameterize and click **Add**. 텍스트의 각기 다른 부분을 선택하고 각 부분에 대한 매개 변수를 추가하면 동일한 텍스트 속성에서 여러 매개 변수를 만들 수 있습니다. To change the name of the parameter, click it, enter a new name, and click **Close**.

   * **개체매개**&#x200B;변수 열에서 상자를 클릭합니다. [매개 변수 편집] 대화 상자가 나타납니다. Enter a name and click **OK**.
   한 번에 여러 특성을 동일한 값으로 사용자 지정하려면 각 특성에 동일한 매개 변수 이름을 사용합니다. 예를 들어 템플릿에 사각형과 별이 있는 경우 각 항목의 SolidColor 색상 특성에 대한 [매개 변수] 이름으로 `newcolor`를 입력할 수 있습니다. `newcolor` 값을 변경할 때마다 사각형과 별이 모두 새 색상으로 바뀝니다.

1. [값] 또는 [데이터] 필드에 특성의 기본값을 지정합니다. 선택한 개체의 모든 속성을 설정하여 원하는 모양을 정확하게 지정합니다.
1. (선택 사항) 매개 변수화하려는 모든 개체 또는 레이어에 대해 3-5 단계를 반복합니다.
1. **저장** 또는 **다른 이름으로 저장**&#x200B;을 클릭합니다.
1. Click **Preview** to open the FXG Preview window and see the parameters you created with their default values.

## FXG 템플릿에서 개체나 레이어 표시 또는 숨기기 {#show-or-hide-an-object-or-layer-in-the-fxg-template}

숨겨진 개체와 레이어는 미리 보기나 출력에 표시되지 않지만 파일에서 삭제되지는 않습니다. 필요한 경우 다시 표시할 수 있습니다. 가시성은 변수로 만들 수 있는 특성입니다. 눈 아이콘을 클릭하여 켜거나 끄면 개체 또는 레이어 가시성의 기본값이 설정됩니다.

1. [개체] 패널에서 개체 또는 레이어 이름 옆에 있는 눈 아이콘을 클릭하면 파일에서 숨겨집니다.
1. 다시 클릭하면 개체가 표시됩니다.

## 한 템플릿의 여러 버전 만들기 {#create-different-versions-of-a-template}

특성을 편집하여 각기 다른 사용자에 맞게 템플릿의 여러 버전을 만들 수 있습니다.

[템플릿 게시] 화면에서 [다른 이름으로 저장]을 클릭하여 원본 FXG 템플릿을 덮어쓰지 않고 파일을 새 FXG 템플릿으로 저장합니다.

## 스트로크 텍스트 사용 {#using-stroked-text}

스트로크 텍스트는 특성을 매개 변수화할 수 있는 방법을 보여 주는 한 예입니다. Dynamic Media Classic에서는 다음과 같은 획 텍스트 기능을 지원합니다.

* 스트로크 너비
* 대시 기호로 된 스트로크 패턴
* 다양한 연결 스타일
* 다양한 끝 스타일
* 스트로크 중복 인쇄
* 스팟 색상 지원을 비롯하여 스트로크에 대한 별도의 색상 처리

다음 표에서는 스트로크 텍스트를 지원하는 특성에 대해 설명합니다.

| 속성 | 설명 |
|--- |--- |
| s7:fill `<Boolean>`(S7FXG Only) | 텍스트에 채우기를 사용할지 여부를 지정합니다. 기본값은 true입니다. |
| s7:stroke `<Boolean>` (S7FXG Only) | 텍스트에 스트로크를 사용할지 여부를 지정합니다. 기본값은 false입니다. |
| s7:weight `<number>` (S7FXG Only) | 텍스트의 스트로크 너비(포인트)를 지정합니다. 기본값은 1포인트입니다. |
| s7:joints `<string>` (miter, round, bevel) (S7FXG Only) | 스트로크의 연결 유형을 지정합니다. 기본값은 round입니다. |
| s7:caps `<string>` (none, round, square) (S7FXG Only) | 스트로크의 끝 모양 유형을 지정합니다. 기본값은 round입니다. |
| s7:miterLimit `<number>` (S7FXG Only) | 연결이 스트로크의 마이터 연결일 때 마이터 제한을 지정합니다. 기본값은 4입니다. |
| s7:strokeOverprint `<Boolean>` (S7FXG Only) | 스트로크에 중복 인쇄를 사용할지 여부를 지정합니다. 기본값은 false입니다. |
| s7:strokeColorName (S7FXG에만 해당) | 스트로크의 색상 이름을 정의한다는 점을 제외하고 s7:colorName과 같습니다. |
| s7:strokeColorValue (S7FXG에만 해당) | 스트로크의 색상 값을 정의한다는 점을 제외하고 s7:colorValue와 같습니다. |
| s7:strokeColorspace (S7FXG에만 해당) | 스트로크의 색상 공간을 정의한다는 점을 제외하고 s7:colorspace와 같습니다. |
| flm:dashPattern `<array>` (S7FXG Only) | 기본적으로 대시 및 간격 패턴은 없습니다. 이 특성은 스트로크의 대시/간격 패턴을 정의합니다. 첫 번째 값은 스트로크의 대시입니다. 두 번째 값은 대시 사이의 간격입니다. 대시 및 간격으로 대체 값을 지정하여 여러 값의 배열을 동일한 방식으로 확장할 수 있습니다. |

## 뒤틀린 텍스트 사용 {#using-warped-text}

뒤틀린 텍스트를 사용하면 물결 무늬, 플래그, 늘이기 등의 효과로 텍스트 모양을 수정할 수 있습니다.

뒤틀린 텍스트는 서식 있는 텍스트 개체에 지원됩니다. 텍스트는 세로 또는 가로 방향일 수 있으며 점 텍스트, 영역 텍스트 및 경로 유형 텍스트일 수 있습니다. 뒤틀린 텍스트를 적용하려면 먼저 전체 텍스트 개체를 선택해야 합니다.

Adobe Illustrator에서 뒤틀린 텍스트를 만들 수 있습니다.

텍스트를 뒤틀 때 다음 특성을 설정할 수 있습니다.

* 스타일
* 방향
* 벤드
* 가로 왜곡
* 세로 왜곡

각 특성에 값 집합이 포함됩니다.

| 속성 | 값 | 기본값 |
|--- |--- |--- |
| Styles7:warpStyle | nonearcarcLowerarcUpperarchbulgeshellLowershellUpperflagwavefishrisefishEyeinflatesqueezetwist | 없음 |
| Directions7:warpDirection | horizontalvertical | 가로 |
| Bends7:warpBend | -1에서 1 사이 | 0.5 |
| 가로 왜곡7:비틀기 가로 왜곡 | -1에서 1 사이 | 0 |
| 세로 왜곡7:비틀기 세로 왜곡 | -1에서 1 사이 | 0 |

>[!NOTE]
>
>For `inflate` and `fishEye`, changing the `s7:warpDirection` flag between horizontal and vertical does not have any effect on the output.

뒤틀린 텍스트를 만들고 사용하는 방법에 대한 자세한 내용은 Adobe Illustrator 설명서를 참조하십시오.

>[!MORELIKETHIS]
>
>* [Illustrator에서 초기 템플릿 만들기](create-initial-template-illustrator.md#create_the_initial_template_in_illustrator)
>* [Upload files for Template Publishing](upload-files-template-publishing.md#upload_files_for_template-publishing)

