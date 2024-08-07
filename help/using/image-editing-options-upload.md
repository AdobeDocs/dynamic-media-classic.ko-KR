---
title: 업로드 시 이미지 세부 조정 옵션
description: Adobe Dynamic Media Classic에서 업로드 시 사용할 수 있는 이미지 미세 조정 옵션에 대해 알아봅니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 2d9fc6d8-973f-4aaa-bc2c-b49cda2cde58
topic: Administration, Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '1200'
ht-degree: 28%

---

# 업로드 시 이미지 세부 조정 옵션{#image-editing-options-at-upload}

이미지 파일을 업로드할 때 AI, EPS 및 PSD 파일을 포함하면 [업로드 작업 선택 사항] 대화 상자에서 다음 편집 작업을 수행할 수 있습니다.

* 이미지 가장자리에서 공백을 자릅니다.
* 이미지 측면에서 수동으로 자릅니다.
* 색상 프로필을 선택합니다.
* 클립 경로에서 마스크를 만듭니다.
* 언샵 마스킹 선택 사항으로 이미지를 선명하게 합니다.
* 녹아웃 배경

이러한 옵션은 업로드 페이지의 **[!UICONTROL 이미징 편집 옵션]** 제목 아래에 있습니다.

## 이미지에서 공백 자르기

이미지에서 공백 픽셀을 자동으로 자를 수 있습니다. 업로드 작업 옵션 대화 상자에서 **[!UICONTROL 자르기 옵션]**&#x200B;을 선택합니다. **[!UICONTROL 자르기]** 드롭다운 목록에서 **[!UICONTROL 트리밍]**&#x200B;을(를) 선택합니다. 다음 선택 사항을 선택합니다.

* **[!UICONTROL 다음을 기준으로 재단]**: 이 드롭다운 목록에서 색상 또는 투명도를 기준으로 자를지 여부를 선택합니다.

   * **[!UICONTROL 색상]**: **[!UICONTROL 색상]** 옵션을 선택합니다. 그런 다음 **[!UICONTROL 모퉁이]** 드롭다운 목록에서 자르려는 공백 색상을 가장 잘 나타내는 색상으로 이미지의 모퉁이를 선택합니다.

   * **[!UICONTROL 투명도]**: 투명도 옵션을 선택합니다.

* **[!UICONTROL 허용 한도]**: 슬라이더를 드래그하여 0에서 1까지의 허용 한도를 지정하십시오.

   * **색상을 기준으로 트리밍**: 이미지의 모퉁이에서 선택한 색상과 정확히 일치하는 경우에만 픽셀을 자르도록 0을 지정합니다. 값이 1에 가까워질수록 색상 차이를 더 많이 허용합니다.

   * **투명도를 기준으로 트리밍**: 픽셀이 투명한 경우에만 자르도록 0을 지정합니다. 1에 가까운 숫자를 사용하면 투명도가 더 높아집니다.

## 이미지의 측면에서 수동으로 자르기

이미지 측면에서 수동으로 자르려면 [자르기] 메뉴를 선택한 다음 [수동]을 선택합니다. 이미지의 임의 측면이나 각 측면에서 자를 픽셀 수를 입력합니다. 이미지를 잘라내는 정도는 이미지 파일의 ppi(인치당 픽셀 수) 설정에 따라 달라집니다. 예를 들어 이미지가 150ppi를 표시한다고 가정해 보겠습니다. 그런 다음 [위쪽], [오른쪽], [아래쪽] 및 [왼쪽] 텍스트 상자에 75를 입력합니다. 이 시점에서 각 면은 0.5인치 잘립니다.

## 색상 프로파일 선택

이미지의 색상 공간을 선택하려면 색상 프로파일 옵션을 선택합니다.

* **[!UICONTROL sRGB로 변환]**: sRGB(표준 빨강 녹색 파랑)로 변환됩니다. sRGB는 웹 페이지에 이미지를 표시하는 데 권장되는 색상 공간입니다.

* **[!UICONTROL 원래 색 공간 유지]**: 원래 색 공간을 유지합니다.

* **[!UICONTROL 사용자 지정 변환]** > **[!UICONTROL 변환]**: 색상 공간으로 변환할 수 있도록 메뉴를 엽니다. 표준 Photoshop 색상 공간 또는 Adobe Dynamic Media Classic에 업로드한 색상 공간을 선택할 수 있습니다.

[ICC 프로필](icc-profiles.md#icc_profiles)을 참조하십시오.

## 클리핑 패스에서 마스크 만들기

클리핑 패스 정보를 기반으로 이미지에 대한 마스크를 만들려면 **[!UICONTROL 클리핑 패스에서 마스크 만들기]**&#x200B;를 선택합니다. 이 선택 사항은 클립 경로가 생성된 이미지 편집 애플리케이션으로 만들어진 이미지에 적용됩니다.

## [선명 취소 마스크]를 사용하여 이미지 선명

이 필터를 사용하면 최종 다운샘플링된 이미지에서 선명하게 하기 필터 효과를 미세 조정할 수 있습니다. 효과의 강도, 효과의 반경(픽셀 단위 측정) 및 무시되는 대비 임계값을 제어하는 데 도움이 됩니다.

이 효과는 Photoshop의 언샵 마스크 필터와 동일한 옵션을 사용합니다. 이름으로 예상되는 것과는 반대로 언샵 마스크는 선명하게 하는 필터입니다.

언샵 마스킹 아래에서 원하는 옵션을 설정합니다. 설정 옵션은 다음 표에 설명되어 있습니다.

| 언샵 마스크 옵션 | 설명 |
| --- | --- |
| 금액 | [양]은 가장자리 픽셀에 적용되는 대비의 양을 제어합니다.<br><br>효과의 강도로 생각하십시오. Dynamic Media Classic과 Adobe Photoshop의 [언샵 마스크] 양 값에는 차이가 있습니다. 가장 큰 차이는 Photoshop의 금액 범위가 1%에서 500%라는 점이다. 반면 Adobe Dynamic Media Classic에서는 값 범위가 0.0~5.0입니다. Adobe Dynamic Media Classic의 값 5.0은 Photoshop의 500%에 해당하는 대략적인 값이고, 값 0.9는 90%에 해당하는 값입니다. |
| 반경 | 효과의 반경을 제어합니다. <br><br>값 범위는 0-250입니다. 효과는 이미지의 모든 픽셀에서 실행되고, 모든 픽셀에서 모든 방향으로 퍼져 나갑니다. 반경은 픽셀 단위로 측정됩니다. 예를 들어 2000 × 2000 픽셀 이미지와 500 × 500 픽셀 이미지에 대해 유사한 선명하게 하기 위해 2000 × 2000 픽셀 이미지에 대해 두 픽셀의 반경을 설정합니다. 그런 다음 500×500 픽셀 이미지에 있는 한 픽셀의 반경 값을 설정합니다. 픽셀이 더 많은 이미지에는 더 큰 값이 사용됩니다. |
| 임계값 | 임계값은 언샵 마스크 필터가 적용될 때 무시되는 대비 범위입니다. 이 필터를 사용할 때 이미지에 &quot;노이즈&quot;가 삽입되지 않도록 이 효과가 중요합니다. 값 범위는 회색 음영 이미지의 밝기 단계 수인 0-255입니다. 0=검정, 128=50% 회색, 255=흰색입니다. <br><br>예를 들어, 12의 임계값은 잡음이 추가되지 않도록 피부 색조 밝기는 무시하지만 눈썹이 피부와 만나는 지점과 같이 대비되는 영역에 가장자리 대비를 추가합니다.<br><br>예를 들어 다른 사람의 얼굴 사진이 있는 경우 [언샵 마스크]는 이미지의 대비되는 부분에 영향을 줍니다. 예를 들어, 속눈썹과 피부가 만나 뚜렷한 대조 영역을 만들고 매끄러운 피부 그 자체입니다. 가장 부드러운 피부조차도 밝기 값에서 미묘한 변화가 일어납니다. 임계값을 사용하지 않는 경우, 필터는 피부 픽셀에서 이러한 미묘한 변화를 강조합니다. 결국, 선명도가 높아지면서 속눈썹의 대비가 증가하여 노이즈가 있는 원치 않는 효과가 만들어집니다.<br><br>이 문제를 방지하기 위해 필터에 부드러운 피부처럼 대비가 크게 변경되지 않는 픽셀을 무시하도록 하는 임계값이 도입되었습니다. <br><br>앞에 표시된 지퍼 그래픽에서 지퍼 옆에 있는 질감을 확인합니다. 문턱값이 너무 낮아 노이즈를 억제하지 못하기 때문에 화상 노이즈가 나타난다. |
| 모노크롬 | 이미지 밝기(강도)를 언샵 마스킹하려면 선택합니다.<br><br>각 색상 구성 요소를 개별적으로 선택 해제하려면 선택을 취소합니다. |

[이미지 선명하게 하기](sharpening-image.md#sharpening_an_image)도 참조하세요.

[Adobe Dynamic Media 및 이미지 서버에서 이미지 선명하게 하기](/help/using/assets/s7_sharpening_images.pdf)도 참조하세요.

## 녹아웃 배경

[녹아웃 배경]을 사용하면 이미지를 업로드할 때 이미지의 배경을 자동으로 제거할 수 있습니다. 이 기술은 특정 개체로 주의를 끌어 복잡한 배경에서 눈에 띄도록 하는 데 유용합니다.

| 녹아웃 배경 옵션 | 설명 |
| --- | --- |
| 녹아웃 배경 | 녹아웃 배경 기능 및 옵션을 활성화하거나 &quot;켜기&quot;하려면 선택합니다. |
| 모서리 | 필수.<br>녹아웃할 배경색을 정의하는 데 사용되는 이미지의 모퉁이입니다.<br>왼쪽 위, 왼쪽 아래, 오른쪽 위 또는 오른쪽 아래 중 하나를 선택할 수 있습니다</b>.<b> |
| 채우기 방법 | 필수. <br>설정한 모퉁이 위치에서 픽셀 투명도를 제어합니다.<br>다음 채우기 방법 중 하나를 선택할 수 있습니다.<br>· <b>Flood 채우기</b>: 지정한 모퉁이와 일치하는 모든 픽셀을 투명하게 전환하고 여기에 연결됩니다.<br>· <b>픽셀 일치</b>: 이미지의 위치에 관계없이 일치하는 모든 픽셀을 투명하게 바꿉니다. |
| 허용치 | 선택적.<br>설정한 모퉁이 위치에 따라 픽셀 색상 일치의 허용 가능한 변화 정도를 제어합니다.<br>픽셀 색상을 정확하게 일치시키려면 0.0 값을 사용하십시오. 또는 1.0 값을 사용하여 가장 큰 변형을 허용합니다. |

>[!MORELIKETHIS]
>
>* [이미지 자르기](cropping-image.md#cropping_an_image)
