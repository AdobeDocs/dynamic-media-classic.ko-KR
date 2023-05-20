---
title: PSD 파일 작업
description: Adobe Dynamic Media Classic에서 PSD 파일로 작업하는 방법을 알아봅니다.
uuid: 5836b660-6bca-46e7-ab39-1a31d1e0cff2
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4086e3db-5aca-41a0-8f15-302afbf67ddb
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: e3b8c4b9-e9c4-4d7f-84de-2efb456755a1
source-git-commit: dc1ec666b208cec8fffe836d64ed501f6ccf4e7b
workflow-type: tm+mt
source-wordcount: '1003'
ht-degree: 25%

---

# PSD 파일 작업{#working-with-psd-files}

<!--   USED TO BE AN OPTION UNDER COLOR PROFILE OPTIONS * **Convert To sRGB (default)** - Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on web pages. -->

PSD(Photoshop 문서 파일)는 Adobe Dynamic Media Classic에서 템플릿을 만드는 데 가장 많이 사용됩니다. PSD 파일을 업로드할 때 파일에서 Adobe Dynamic Media Classic 템플릿을 자동으로 만들 수 있습니다(업로드 화면에서 템플릿 만들기 옵션 선택).

Adobe Dynamic Media Classic은 파일을 사용하여 템플릿을 만드는 경우 레이어가 있는 PSD 파일에서 여러 이미지를 만듭니다. 각 레이어에 대해 하나의 이미지가 만들어집니다.

## PSD 업로드 선택 사항 {#psd-upload-options}

PSD 파일을 업로드하는 옵션은 업로드 작업 옵션 대화 상자의 Photoshop 옵션 아래에 있습니다. 파일을 자르고, 해당 색상 프로필을 선택하고, 파일을 사용하여 템플릿을 만들고, 앵커를 선택할 수 있습니다.

PSD 파일을 업로드할 때 사용할 수 있는 선택 사항은 다음과 같습니다.

* **자르기 옵션** - 아래에 위치: **[!UICONTROL 자르기 옵션]**. 선택 **[!UICONTROL 트림]** PSD 파일의 가장자리에서 공백을 자동으로 자르려면 다음을 선택합니다. **[!UICONTROL 수동]** PSD 파일의 측면을 자르려면 다음을 수행합니다.

   * **[!UICONTROL 트림]** - 다음을 선택합니다. **[!UICONTROL 다음을 기준으로 트림]** 메뉴 및 선택 **[!UICONTROL 색상]** 또는 **[!UICONTROL 투명도]**.
   다음을 선택하면 **[!UICONTROL 색상]** [모퉁이] 옵션을 선택하고 자르려는 공백 색상을 가장 잘 나타내는 색상으로 PSD의 모퉁이를 선택합니다.

   슬라이더를 드래그하여 0에서 1까지의 공차를 지정합니다. 색상을 기반으로 트림하려는 경우 PDF 모서리에서 선택한 색상과 정확하게 일치하는 경우에만 픽셀을 자르려면 0을 지정합니다. 값이 1에 가까워질수록 색상 차이를 더 많이 허용합니다. 투명도를 기준으로 트리밍하려면 픽셀이 투명한 경우에만 자르도록 0을 지정합니다. 1에 가까운 숫자를 지정하면 더 많은 투명도가 허용됩니다.

   * **[!UICONTROL 수동]** - 이미지의 어느 한 면 또는 각 면에서 자를 픽셀 수를 입력합니다. 이미지를 잘라내는 정도는 이미지 파일의 ppi(인치당 픽셀 수) 설정에 따라 달라집니다. 예를 들어, 이미지에 150ppi가 표시되고 [위쪽], [오른쪽], [아래쪽] 및 [왼쪽] 텍스트 상자에 75를 입력하면 0.5입니다. 이미지의 각 면에서 잘립니다.


* **색상 프로파일 옵션** - 아래에 위치: **[!UICONTROL 색상 프로파일 옵션]**.

   * **[!UICONTROL 기본 색상 유지]**

   * **[!UICONTROL 원래 색상 공간 유지]** - 이미지의 원래 색상 공간을 유지합니다.

   * **[!UICONTROL 사용자 정의 시작]** > **[!UICONTROL 종료]** - [변환] 및 [색상 공간으로 변환]을 선택할 수 있는 메뉴를 엽니다. 표준 Photoshop 색상 공간 또는 Adobe Dynamic Media Classic에 업로드한 색상 공간을 선택할 수 있습니다. [ICC 프로필](/help/icc-profiles.md)을 참조하십시오.

* **PHOTOSHOP 선택 사항**

   * **[!UICONTROL 레이어 유지]** - PSD의 레이어(있는 경우)를 개별 에셋으로 분할합니다. 자산 레이어의 PSD 연결은 유지됩니다. 세부 사항 보기의 PSD 파일을 열고 레이어 패널을 선택하여 해당 파일을 볼 수 있습니다. PSD 파일에서 레이어 보기 및 편집을 참조하십시오.

   * **[!UICONTROL 템플릿 만들기]** - PSD 파일의 레이어로 템플릿을 만듭니다.

   * **[!UICONTROL 텍스트 추출]** - 사용자가 뷰어에서 텍스트를 검색할 수 있도록 텍스트를 추출합니다.

   * **[!UICONTROL 레이어를 배경 크기로 확장]** - 리핑된 이미지 레이어의 크기를 배경 레이어의 크기로 확장합니다.

   * **[!UICONTROL 레이어 이름 지정]** - PSD 파일의 레이어가 별도의 이미지로 업로드됩니다. Adobe Dynamic Media Classic에서 이러한 이미지의 이름을 지정하려면 다음 옵션 중에서 선택합니다.

      * **[!UICONTROL 레이어 이름]** - PSD 파일에서 해당 레이어 이름 뒤에 이미지 이름을 지정합니다. 예를 들어 원본 PSD 파일에서 이름이 Price Tag인 레이어는 이미지 이름도 Price Tag가 됩니다. 그러나 PSD 파일의 레이어 이름이 기본 Photoshop 레이어 이름(배경, 레이어 1, 레이어 2 등)이면 PSD 파일에서 해당 레이어 번호의 이름을 따서 이미지 이름이 지정됩니다. <!-- not their default layer names -->

      * **[!UICONTROL Photoshop 및 레이어 번호]** - 원래 레이어 이름을 무시하고 PSD 파일에서 레이어 번호 뒤에 이미지 이름을 지정합니다. Photoshop 파일 이름 뒤에 레이어 번호가 붙어 이미지의 이름이 지정됩니다. 예를 들어, 라는 파일의 두 번째 레이어는 `Spring Ad.psd` 이(가) 이름이 지정됨 `Spring Ad_2` Photoshop에 기본값이 아닌 이름이 있더라도.

      * **[!UICONTROL Photoshop 및 레이어 이름]** - PSD 파일 뒤에 레이어 이름 또는 레이어 번호를 붙여서 이미지 이름을 지정합니다. 레이어 번호는 PSD 파일의 레이어 이름이 Photoshop 기본 레이어 이름인 경우 사용됩니다. 예를 들어 `Price Tag` PSD 파일 내 `SpringAd` 이(가) 이름이 지정됨 `Spring Ad_Price Tag`. 기본 이름이 레이어 2인 레이어가 호출됩니다. `Spring Ad_2`.
   * **[!UICONTROL 앵커]** - PSD 파일에서 생성된 레이어 컴포지션에서 생성된 템플릿에서 이미지가 고정되는 방식을 지정합니다. 기본 앵커는 가운데입니다. 가운데 앵커를 통해 대체 이미지의 종횡비에 상관없이 같은 공간을 대체 이미지로 가장 알맞게 채울 수 있도록 합니다. 템플릿 참조 및 매개 변수 대체 사용 시 해당 이미지를 다른 종횡비의 이미지로 대체할 때 효과적으로 같은 공간을 점유합니다. 템플릿의 지정된 공간을 채울 대체 이미지가 애플리케이션에 필요한 경우 다른 설정으로 변경합니다.


## PSD 파일의 레이어 보기 및 편집 {#viewing-and-editing-layers-in-a-psd-file}

PSD을 업로드할 때 레이어 유지 옵션을 선택한 경우 Adobe Dynamic Media Classic에서 개별 레이어를 에셋으로 리핑했습니다. [상세 보기]의 [찾아보기] 패널에서 파일을 열어 PSD 파일에 속하는 에셋 레이어를 보고 편집할 수 있습니다.

>[!NOTE]
>
>Adobe Dynamic Media Classic은 중첩 레이어 그룹에서 최대 5개 수준을 지원합니다.

1. 찾아보기 패널에서 전체 PSD 파일을 두 번 클릭합니다. 파일이 세부 사항 보기로 열립니다.

   >[!NOTE]
   >
   >PSD 레이어 중 하나가 아니라 전체 자산을 열어야 합니다.

1. 선택 **[!UICONTROL 레이어]**. 모든 레이어가 [레이어] 패널에 개별 이미지로 표시됩니다.
1. 레이어를 두 번 클릭하고 다음 중 하나를 수행합니다.

   * 레이어에 이미지 맵을 만들려면 다음을 선택합니다. **[!UICONTROL 이미지 맵]** 아이콘. (참조: [이미지 맵 만들기](creating-image-maps.md#creating_image_maps).)
   * 레이어에 확대/축소 대상을 만들려면 다음을 선택합니다. **[!UICONTROL 확대/축소 Target]** 아이콘. (참조: [유도된 확대/축소에 대한 확대/축소 대상 만들기](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).)
   * 레이어를 자르려면 를 선택합니다 **[!UICONTROL 자르기]** 아이콘. (참조: [이미지 자르기](cropping-image.md#cropping_an_image).)
   * 레이어를 선명하게 하려면 를 선택합니다 **[!UICONTROL 선명하게]**. (참조: [이미지 선명하게 하기](sharpening-image.md#sharpening_an_image).)
   * 레이어를 조정하려면 를 선택합니다 **[!UICONTROL 조정]**. (참조: [이미지 조정](adjusting-image.md#adjusting_an_image).)

1. 선택 **[!UICONTROL 저장]** 또는 **[!UICONTROL 다른 이름으로 저장]**.
1. 다른 레이어를 보거나 편집하려면 레이어 미리 보기 하단의 화살표를 선택합니다.
1. 레이어 세부 사항 보기를 종료하려면 **[!UICONTROL 격자 보기]** 아이콘.
