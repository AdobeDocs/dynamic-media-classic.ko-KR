---
title: PDF 작업
description: Adobe Dynamic Media Classic에서 PDF를 사용하여 작업하는 방법을 알아봅니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
topic: Integrations, Development
level: Experienced
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 25%

---

# PDF 작업{#working-with-pdfs}

PDF(Portable Document Format) 파일은 Adobe Dynamic Media Classic에서 eCatalogs를 만드는 데 가장 많이 사용됩니다. PDF 파일, Adobe Dynamic Media Classic을 업로드할 때 페이지가 기본적으로 래스터화 또는 rip되어 리치 미디어를 빌드하는 데 사용할 수 있습니다.

페이지 추출을 위해 PDF을 업로드할 때 Adobe은 다음 제한을 적용합니다.

| 제한 유형 | 제한 적용됨 | 2022년 12월 31일 제한 변경 |
| --- | --- | --- |
| 추출을 위해 고려할 PDF의 최대 페이지 수 | 5000(새 업로드용) | 100(모든 PDF의 경우) |

[Dynamic Media 제한 사항](/help/using/limitations.md)도 참조하세요.

## PDF 업로드 선택 사항 {#pdf-upload-options}

PDF 파일을 업로드할 때 다양한 방법으로 형식을 지정할 수 있습니다. 페이지를 자르고, 검색어를 추출하고, 인치당 픽셀 수 해상도를 입력하고, 색상 공간을 선택합니다. PDF 파일에는 종종 트림 여백, 자르기 표시, 등록 표시 및 기타 프린터 표시가 들어 있습니다. PDF 파일을 업로드할 때 페이지 측면에서 이러한 표시를 자를 수 있습니다.

PDF 파일을 업로드하는 옵션은 PDF 옵션 아래의 업로드 페이지에 있습니다.

### 처리 옵션

**[!UICONTROL 래스터화]**: (기본값) PDF 파일의 페이지를 분리하고 벡터 그래픽을 비트맵 이미지로 변환합니다. eCatalog를 만들려면 이 옵션을 선택합니다.

**[!UICONTROL 검색 단어 추출]**: 파일의 키워드를 eCatalog 뷰어에서 검색할 수 있도록 PDF 파일에서 단어를 추출합니다.

**[!UICONTROL 링크 추출]**: PDF 파일에서 링크를 추출하여 eCatalog 뷰어에서 사용되는 이미지 맵으로 변환합니다.

**[!UICONTROL 여러 페이지로 된 PDF을 사용하여 eCatalog 자동 생성]**: PDF 파일에서 eCatalog를 자동으로 만듭니다. eCatalog 이름은 업로드한 PDF 파일을 따서 지정됩니다. 이 선택 사항은 업로드할 때 PDF 파일을 래스터화한 경우에만 사용할 수 있습니다.

### 해상도

해상도 설정을 결정합니다. PDF 파일에서 인치당 표시되는 픽셀 수를 결정하는 설정입니다. 초기값은 150입니다.

### 색상 공간 옵션

[색상 공간] 메뉴를 선택한 다음 PDF 파일의 색상 공간을 선택합니다. 대부분의 PDF 파일은 [RGB] 및 [CMYK] 색상 이미지를 모두 포함합니다. 온라인 보기에서는 RGB 색상 공간이 선호됩니다.

* **[!UICONTROL 자동으로 감지]**: PDF 파일의 색상 공간을 유지합니다.

* **[!UICONTROL RGB 강제 적용]**: RGB 색상 공간으로 변환합니다.

* **[!UICONTROL CMYK로 강제 적용]**: CMYK 색상 공간으로 변환합니다.

* **[!UICONTROL 회색 음영으로 강제 적용]**: 회색 음영 색 공간으로 변환합니다.

### 색상 프로파일 옵션

* **[!UICONTROL sRGB로 변환]**: sRGB(표준 빨강 녹색 파랑)로 변환됩니다. sRGB는 웹 페이지에 이미지를 표시하는 데 권장되는 색상 공간입니다.

* **[!UICONTROL 원래 색 공간 유지]**: 원래 색 공간을 유지합니다.

* **[!UICONTROL 사용자 지정 변환]** > **[!UICONTROL 변환]**: 색상 공간으로 변환할 수 있도록 메뉴를 엽니다. 표준 Photoshop 색상 공간 또는 Adobe Dynamic Media Classic에 업로드한 색상 공간을 선택할 수 있습니다.

[ICC 프로필](/help/using/icc-profiles.md#icc_profiles)을 참조하십시오.

## PDF 파일에서 공백 자르기 {#cropping-white-space-from-a-pdf-file}

PDF 파일을 업로드할 때 자동으로 공백 픽셀을 자를 수 있습니다.

1. [자르기] 메뉴를 선택하고 [트림]을 선택합니다.
1. 다음 선택 사항을 지정합니다.

   * **[!UICONTROL 다음을 기준으로 트림]**: 색상 또는 투명도를 기준으로 자를지 여부를 선택합니다.

      * **[!UICONTROL 색상]**: 색상 옵션을 선택합니다. 그런 다음 **[!UICONTROL 모서리]** 메뉴를 선택하고 자르려는 공백 색상을 가장 잘 나타내는 색상으로 PDF 모서리를 선택합니다.

      * **[!UICONTROL 투명도]**: 투명도 옵션을 선택합니다.

   * **[!UICONTROL 허용 한도]**: 슬라이더를 드래그하여 0에서 1까지의 허용 한도를 지정하십시오.

   * **[!UICONTROL 색상을 기준으로 트리밍]**: PDF 모서리에서 선택한 색상과 정확히 일치하는 경우에만 픽셀을 자르도록 0을 지정합니다. 값이 1에 가까워질수록 색상 차이를 더 많이 허용합니다.

   * **[!UICONTROL 투명도를 기준으로 트리밍]**: 픽셀이 투명한 경우에만 자르도록 0을 지정합니다. 1에 가까운 숫자를 사용하면 투명도가 더 높아집니다.

## PDF 페이지 양쪽에서 자르기 {#cropping-from-the-sides-of-pdf-pages}

PDF 파일을 업로드할 때 페이지 양쪽에서 프린터 표시를 수동으로 제거할 수 있습니다.

1. 자르기 메뉴에서 **[!UICONTROL 수동]**&#x200B;을 선택합니다.
1. [위쪽], [오른쪽], [아래쪽] 및 [왼쪽] 텍스트 상자에 픽셀 설정을 입력하여 페이지 위쪽, 아래쪽 및 측면에서 자릅니다.

잘리는 페이지 양은 PDF 파일에 대해 입력한 [해상도 PX/인치] 설정에 따라 달라집니다. 예를 들어 해상도 PX/인치(Resolution PX/Inch) 설정으로 150(기본값)을 입력한다고 가정합니다. 그런 다음 페이지 양쪽에서 75픽셀을 자릅니다. 이 경우 0.5인치 이(가) 잘립니다. 인치당 150픽셀에서는 75픽셀이 0.5인치입니다.
