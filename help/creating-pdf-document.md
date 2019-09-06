---
title: PDF 문서 만들기
seo-title: PDF 문서 만들기
description: 널
seo-description: Dynamic Media Classic에서 Web-to-Print 프로세스를 사용하여 PDF 문서를 만드는 방법을 살펴봅니다.
uuid: 274 FB 06 B -320 B -40 FA -8 B 61-C 224 D 8 ACEAA 1
contentOwner: 관리
content-type: 참조
products: sg_ Experiencemanager/dynamic-media-scene -7
geptopics: sg_ scenesevenondemand_ pk/categories/template-publishing
discoiquuid: 87 E 91 E 8 E -10 A 2-4 FBA -87 C 7-AAD 2 BD 798146
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# PDF 문서 만들기 {#creating-a-pdf-document}

W2P(Web to Print) 프로세스의 최종 단계는 사용자 지정 PDF를 생성하는 것입니다. 최종 사용자는 개발자가 만든 웹 애플리케이션을 사용하여 템플릿을 개인 설정한 후 최종 PDF 문서를 만듭니다. 이 최종 PDF는 일반적으로 전문가 등급 인쇄를 위해 인쇄 서비스 공급자에게 전송됩니다. 최종 PDF가 예상대로 인쇄되도록 하려면 올바른 작업 선택 사항 파일을 사용하고 글꼴, 프린터 표시 및 색상을 올바르게 설정합니다.

## PDF 사전 설정 지정 {#setting-up-pdf-presets}

PDF Joboptions 파일을 만들어 Dynamic Media Classic 서버에 업로드하여 PDF 호환성 수준 및 프린터 설정을 지정합니다. 예를 들어 PDF/X-4 호환 PDF 출력(PDF 인쇄 게시 워크플로에 권장됨)을 선택할 수 있습니다. 작성 소프트웨어(예: Adobe Illustrator) 또는 Acrobat에서 작업 선택 사항 파일을 만들 수 있습니다. 인쇄 작업에 적합한 작업 선택 사항 설정을 조언해 줄 수 있는 인쇄업체에 항상 확인합니다.

작업 선택 사항 파일을 만드는 방법 및 Acrobat에서 작업 선택 사항 파일을 만드는 방법에 대한 자세한 내용은 Adobe Acrobat 도움말을 참조하십시오.

Illustrator에서 작업 선택 사항 파일을 만들려면

1. [편집] &gt; [Adobe PDF 사전 설정]을 선택합니다.
1. 대화 상자에서 사용하려는 사전 설정을 선택합니다.

   다음 작업 옵션 설정은 Dynamic Media Classic에서 지원됩니다.

   | 작업 옵션 | 설명 |
   |--- |--- |
   | 일반 | <ul><li>호환성 </li><li>개체 수준 압축</li><li>썸네일 포함</li><li>빠른 웹 보기를 위해 최적화</li></ul> |
   | 이미지 | <ul><li>다운샘플링</li><li>해상도</li><li>임계값</li><li>컬러, 회색 및 모노용 압축</li></ul> |
   | 글꼴 | <ul><li>모든 글꼴 포함(글꼴이 기본적으로 포함됨)</li><li>OpenType 글꼴 포함</li><li>사용된 문자의 비율이 다음보다 적을 때 서브세트 글꼴 포함</li><li>항상 포함 목록</li><li>포함 안 함 목록</li></ul> |
   | 색상 | <ul><li>색상 전략(이미지에만 태그 지정은 모든 항목에 태그 지정으로 처리됨)</li><li>문서 렌더링 의도</li><li>4.2.5에서는 다음 작업 공간만 지원됩니다. 4.3에서는 IPS에 업로드된 모든 고객 제공 프로필을 사용할 수 있습니다.</li><li>해결 방법으로, 회사의 기본 색상 프로필을 사용하도록 전환할 아트웍의 타겟 색상 공간을 지정할 수 있습니다.</li></ul> |
   | RGB | <ul><li>e-sRGB </li><li>scRGB with encoding range [-4.0, 4.0]</li><li>Lab D50</li><li>PCS XYZ</li><li>평면 XYZ</li><li>선형 ROMM-RGB</li><li>ROMM-RGB</li><li>sYCC 8비트</li><li>e-sYCC 8비트</li></ul> |
   | 회색 | <ul><li>회색 감마 1.8</li><li>회색 감마 2.2</li><li>점 게인 10%</li><li>점 게인 15%</li><li>점 게인 20%</li><li>점 게인 25%</li><li>점 게인 30%</li><li>sGray</li></ul> |
   | 보정된 CMYK 색상 공간의 CMYK 값 유지 |  |
   | 고급 | [OPI 설명 유지]가 항상 켜져 있음 |
   | 표준 | 규격 표준 |

   >[!NOTE]
   >
   >Dynamic Media Classic는 Joboptions 파일에서 프린터 표시 설정을 무시합니다. 대신 프린터 표시는 Dynamic Media Classic URL 명령을 사용하여 구성됩니다.

1. [내보내기]를 클릭하고 이름과 위치를 지정한 다음 [저장]을 클릭합니다.
1. 작업 선택 사항 파일을 Scene7 Publishing System에 자산으로 업로드합니다.

   URL에서 참조하여 게시된 템플릿과 함께 사용합니다. 예:

   `https://yourpublishserver.scene7.com/is/agm/SiliconPublishing/PetNews?&fmt=pdf,cmyk&joboption=SPSfilenameid`

## 인쇄할 PDF 준비 {#preparing-the-pdf-for-print}

인쇄할 PDF를 마무리하기 전에 이 섹션의 지침을 따라야 합니다.

**이미지**

게시 작업의 모든 이미지가 Dynamic Media Classic 서버에 업로드되고 게시되었는지 확인합니다.

**Fonts**

게시 작업의 모든 글꼴이 Dynamic Media Classic 서버로 업로드되고 게시되었는지 확인합니다. 최종 사용자가 글꼴을 변경할 수 있게 하려는 경우 글꼴을 호스팅할 법적 권리가 있는지 확인합니다.

**이미지 해상도(인치당 픽셀 수)**

비트맵 이미지의 해상도는 생성된 인쇄용 PDF에서 Dynamic Media Classic Server에 의해 보존됩니다. 필요한 경우 Dynamic Media Classic에서 이미지 해상도를 확대합니다. 최적 결과를 얻으려면 웹에서 미리 볼 때 해상도를 기본값(일반적으로 72dpi)으로 유지합니다. 회사의 모든 이미지에 대한 기본 해상도는 [게시 설정/이미지 서버] 창의 [기본 인쇄 해상도] 섹션에서 설정됩니다. 고해상도(예: 300dpi)를 설정하면 처리 시간이 더 길어질 수 있으므로 인쇄용 PDF에만 적용해야 합니다. PDF 작업의 기본 해상도를 수동으로 재정의하려면 URL에 imageRes= 명령을 사용합니다.

**색상 관리**

문서와 이미지는 회색 음영, CMYK, 이름이 지정된 스팟 색상, RGB 또는 Lab 색상 모델을 사용할 수 있습니다. ICC 색상 프로필을 사용하여 각 항목을 보정 해제하거나 보정할 수 있습니다. 최상의 결과를 얻으려면 생성된 인쇄용 PDF에 프로필을 포함합니다. Dynamic Media Classic Server는 기본적으로 이 작업을 수행합니다. 필요한 모든 색상 프로필이 Dynamic Media Classic 플랫폼에 업로드되었는지 확인합니다. 가급적이면 디자인 애플리케이션에 설정된 색상 관리 옵션이 다이내믹 미디어 클래식 서버에 설정되어 있는지 확인하십시오.

**디자인 애플리케이션 색상 관리 설정:** 작성 애플리케이션(예: Adobe Illustrator)의 [색상 설정]에 있는 [작업 공간] 섹션에서 [RGB] 및 [CMYK] 색상 프로필을 지정합니다.

**Dynamic Media Classic 색상 관리 설정:** 일반적으로 디자인 애플리케이션의 색상 관리 설정은 Dynamic Media Classic 서버의 기본 색상 프로필과 일치해야 합니다. 이러한 설정은 [게시 설정/이미지 서버] 창에서 확인할 수 있습니다.

## 프린터 표시 제공 {#displaying-printer-marks}

다음과 같은 용도로 PDF를 만들 수 있습니다.

* 완성된 문서
* 프로덕션을 위해 프린터에 전송할 수 있는 중간 문서(예: 필름 또는 판)

중간 문서에는 도련 여백, 프린터 표시 등의 추가 프로덕션 컨텐츠가 포함될 수 있습니다. 이 컨텐츠는 일반적으로 완성된 페이지 경계 외부에 표시됩니다.

Acrobat의 "프린터 표시 추가" 화면에서 사용할 수 있는 모든 표시가 지원됩니다. 프린터 표시는 `printerMark` 매개 변수로 제어됩니다. `&printerMark=trim marks, bleed marks, registration marks, color bars, page information, style, line weight, layer embed`구문은 입니다.

* trim marks = 0|1
* bleed marks = 0|1
* registration marks = 0|1
* color bars = 0|1
* page information = 0|1
* style = Illustrator | IllustratorJ | QuarkXPress
* line weight = 0.125 | 0.25 | 0.50
* layer embed = 0|1

인쇄 프로덕션용으로 문서를 준비할 때 프린터 표시는 인쇄 서비스에서 교정지 생성을 위해 분리 필름을 정렬하고, 올바른 보정 및 잉크 밀도를 위해 필름을 측정하고, 크기에 맞게 필름을 트림하는 데 필요할 수 있습니다. 프린터 표시는 트림 상자, 도련 상자 등의 문서 상자 경계를 나타냅니다. 프로덕션 관련 컨텐츠에는 다음이 포함될 수 있습니다.

**미디어 상자** 페이지를 인쇄할 물리적 미디어의 경계. 미디어 상자 외부 컨텐츠는 무시해도 파일의 의미에 영향을 주지 않습니다.

**도련 상자** 프로덕션 환경에서 출력할 때 페이지 컨텐츠가 잘리는 영역입니다. 도련 상자에는 자르기, 접기 및 트림 장비의 물리적 제한을 수용하는 데 필요한 영역이 포함될 수 있습니다. 기본값은 페이지의 자르기 상자입니다.

**트림 상자** 트리밍 완료 후 완료된 페이지의 의도한 크기입니다. 트림 상자는 인쇄 지침, 절단선, 색상 막대 등의 프로덕션 관련 컨텐츠를 허용하기 위해 미디어 상자보다 작을 수 있습니다. 기본값은 페이지의 자르기 상자입니다.

**아트 상자** 페이지의 작성자가 의도한 대로 페이지의 의미 있는 컨텐츠 (잠재적인 공백 포함) 의 범위입니다. 기본값은 페이지의 자르기 상자입니다.

다음 표에 있는 수정자를 사용하여 Adobe Illustrator, InDesign 및 Acrobat에서 사용 가능한 프린터 표시를 복제할 수 있습니다.

| 수정자/값 | 설명 |
|--- |--- |
| bleedMargin=top,left,bottom,right | Acrobat에서 [페이지 상자 설정] 선택 사항을 사용하여 지정합니다. BleedBox를 선택한 다음 [여백 컨트롤] 선택 사항을 사용하여 여백을 지정합니다.<br><br>값은 안쪽으로 들어가는 아트웍의 원래 가장자리(미디어 상자)를 기준으로 위쪽, 왼쪽, 아래쪽 및 오른쪽 가장자리의 거리를 나타냅니다. 값 (0-1000) 는 포인트 단위입니다.<br><br>새 높이 = 원래 높이 - (위쪽 + 아래쪽)<br><br>새 너비 = 원래 너비 - (왼쪽 + 오른쪽) |
| mediaMargin=top,left,bottom,right | Acrobat에서 [페이지 상자 설정] 선택 사항을 사용하여 지정합니다. [페이지 크기 변경] 선택 사항 아래의 [사용자 지정 페이지 크기]를 수정합니다.<br><br>값은 바깥쪽으로 나가는 아트웍의 원래 가장자리(미디어 상자)를 기준으로 위쪽, 왼쪽, 아래쪽 및 오른쪽 가장자리의 거리를 나타냅니다. 값 (0-1000) 는 포인트 단위입니다.<br><br>새 높이 = top + bottom + original heightnew<br><br>width = top + bottom + original 폭<br><br>새 높이와 새 폭 값에 따라 생성된 PDF의 새 페이지 크기가 결정됩니다.<br><br>새 미디어 상자가 정의되면 트림 여백과 도련 여백의 모든 계산에서 새 미디어 상자를 아트웍 가장자리로 고려해야 합니다. |
| trimMargin=top,left,bottom,right | Acrobat에서 [페이지 상자 설정] 선택 사항을 사용하여 지정합니다. [트림 상자]를 선택한 다음 [여백 컨트롤] 선택 사항을 사용하여 여백을 지정합니다.<br><br>값은 안쪽으로 들어가는 아트웍의 원래 가장자리(미디어 상자)를 기준으로 위쪽, 왼쪽, 아래쪽 및 오른쪽 가장자리의 거리를 나타냅니다. 값 (0-1000) 는 포인트 단위입니다.<br><br>새 높이 = 원래 높이 - (위쪽 + 아래쪽)<br><br>새 너비 = 원래 너비 - (왼쪽 + 오른쪽) |
| printerMark= trim marks, bleed marks, registration marks, color bars, page information, style, line weight, layer embed | 값은 다음과 같습니다.<br><br>trim marks = 0,1 (default is 0)<br><br>bleed marks = 0,1 (default is 0)<br><br>registration marks = 0,1 (default is 0)<br><br>page information = 0,1 (default is 0)<br><br>page information = 0,1 (default is 0)<br><br>style = default, indesignj 1, indesignj 2, illustrator, illustratorj, quarkxpress (default is default)<br><br>line weight = 0.125-0.2, both values inclusive (default is 0.25)<br><br>layer embed = 0, 1, with 1 creating a new layer containing all printer marks (default is 1)<br><br>to use a new layer are used, the marks and color bars appear different and match with the corresponding styles used by Acrobat. |

프린터 표시에 대한 다음 사항에 주의하십시오.

* 프린터 표시를 지정할 때 URL 호출을 통해 도련 여백, 트림 여백 및 미디어 여백을 지정합니다. 이러한 여백을 지정하지 않고 프린터 표시를 지정하면 생성된 PDF의 보이는 영역 외부에 이러한 표시가 나타납니다. 또한 트림 표시와 도련 표시가 겹칩니다.
* Specifying the same margin values for the trim margin and bleed margin results in trim marks and bleed marks overlapping when both these flags are set to 1 in `&printerMark`.
* URL 호출을 통해 fmt=swf/image 형식을 지정할 경우 이 기능은 PDF 출력과 관련이 있으므로 프린터 표시나 여백 없이 출력됩니다.
* Specifying `&printerMark=`through the URL results in default values being used for all parameters. Specifying `&printerMark=1` results in trim marks being set to 1 and default values for other parameters. 그러나 n번째 요소를 ON으로 설정하려면 URL을 통해 모든 (n-1) 매개 변수를 지정해야 합니다.
* `&trimMargin`값을 `&bleedMargin`하나만 지정하면 `&mediaMargin` 해당 값이 원래 아트웍의 맨 위, 아래, 왼쪽 및 오른쪽 여백에 적용됩니다.
* `&trimMargin`top `&bleedMargin`값과 왼쪽 값만 지정하면 top `&mediaMargin` 값이 bottom 값에 할당되고 왼쪽 값이 right와 같아집니다.
* `&trimMargin`값을 `&bleedMargin`통해 올바른 값을 지정하지 `&mediaMargin` 않으면 왼쪽 값이 오른쪽에 지정됩니다.
* 다중 페이지 PDF의 경우 모든 페이지에 프린터 표시/여백이 적용됩니다. Acrobat에서는 사용자가 프린터 표시/여백의 페이지 범위를 선택할 수 있습니다.
* 프린터 표시/여백이 활성화된 PDF 출력은 달리 지정되지 않은 경우 Acrobat X와 정확하게 일치합니다.

URL의 &amp;joboption 수정자를 통해 PDF/X-4 호환 PDF 파일을 만들려는 경우 PDF ISO_15930-7-2008.pdf에 지정된 프린터 표시와 관련된 제한 사항에 주의해야 합니다.

* PDF 파일의 각 페이지 개체에 MediaBox가 포함되어 있습니다. PDF/X-4 준수 파일의 각 페이지 개체에는 TrimBox나 ArtBox 중 하나가 포함되며 둘 다 포함되지는 않습니다. MediaBox는 상속에 의해 포함될 수 있습니다.
* BleedBox가 있는 경우 ArtBox나 TrimBox는 BleedBox 경계 바깥쪽으로 확장되지 않습니다. CropBox가 있는 경우 ArtBox, TrimBox 또는 BleedBox는 CropBox 경계 바깥쪽으로 확장되지 않습니다.
* ArtBox, TrimBox, CropBox 또는 BleedBox는 MediaBox 경계 바깥쪽으로 확장되지 않습니다.
* 일부 산업에서는 BleedBox를 사용해야 합니다. 적절한 무역 관행을 준수해야 합니다.
* ArtBox보다 TrimBox를 사용하는 것이 좋습니다.
* TrapNet 및 PrinterMark 주석을 제외한 모든 주석은 BleedBox(또는 BleedBox가 없는 경우 TrimBox 또는 ArtBox)에서 완전히 벗어난 Rect 값을 갖습니다. 모든 PrinterMark 주석은 TrimBox나 ArtBox를 완전히 벗어난 Rect 값을 갖습니다. PDF/X-4 준수 판독기는 PDF TrapNet 주석을 제외한 주석을 완전히 무시할 수 있습니다.
* Rect의 모든 좌표가 경계 상자 외부나 가장자리에 있으며 두 사각형의 교차점이 0인 경우 Rect가 경계 상자를 완전히 벗어난 것으로 간주됩니다.
* ViewerPreferences 사전에 ViewArea, ViewClip, PrintArea 또는 PrintClip 키가 포함되어 있는 경우 각 키의 값은 MediaBox 또는(파일의 모든 페이지 개체에 BleedBox가 있는 경우) BleedBox입니다.

