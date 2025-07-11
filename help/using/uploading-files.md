---
title: 파일 업로드
description: Adobe Dynamic Media Classic에서 파일을 업로드하는 방법을 알아봅니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 8dfcfb3f-6472-4efd-bc87-d5111eee45ce
topic: Content Management
level: Intermediate
source-git-commit: 1cd516119da23f5ef4c0195273025ddd4b3fa789
workflow-type: tm+mt
source-wordcount: '3858'
ht-degree: 26%

---

# 파일 업로드{#uploading-files}

에셋 파일을 Adobe Dynamic Media Classic에 업로드하기 전에 에셋 파일의 이름이 올바른지 확인하십시오. 또한 폴더 구조가 원하는 방식으로 설정되고 구성되어 있는지 확인합니다. Adobe Dynamic Media Classic에서 제공하는 FTP 사이트나 컴퓨터 또는 네트워크에서 직접 파일을 업로드할 수 있습니다. Adobe Dynamic Media Classic에서는 파일을 업로드할 때 최적화하는 옵션을 제공합니다. Adobe Dynamic Media Classic Desktop 응용 프로그램을 설치한 경우 바탕 화면에서 직접 파일과 폴더를 끌어 업로드할 수 있습니다. [[애플리케이션 일반 설정]](application-setup.md#general_settings)을 참조하십시오.

## 업로드할 자산 및 폴더 준비 {#preparing-your-assets-and-folders-for-uploading}

Adobe Dynamic Media Classic에 에셋을 업로드하기 전에 에셋의 형식과 크기가 올바른지 확인하십시오. 에셋 이름을 지정하려면 Adobe Dynamic Media Classic 규칙도 준수해야 합니다. 폴더 구성 및 파일 구조를 설정함으로써 간편하게 파일을 찾고 작업할 수 있습니다.

### 지원되는 자산 파일 형식 {#supported-asset-file-formats}

이 표에는 Adobe Dynamic Media Classic이 지원하는 에셋 파일 형식이 나와 있습니다. 지원되는 Camera Raw 파일에 대한 자세한 내용은 [https://helpx.adobe.com/kr/camera-raw/using/supported-cameras.html](https://helpx.adobe.com/kr/camera-raw/using/supported-cameras.html)을(를) 참조하십시오.

| 자산 파일 형식 | 설명 |
| --- | --- |
| 오디오 | AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3 |
| 계단식 스타일 시트 | CSS |
| 색상 프로필 | ICC, ICM |
| 글꼴 | AFM, OTF, PFB, PFM, PhotoFont, TTC, TTF |
| FXG | FXG |
| Illustrator | AI, FXG |
| 이미지 | BMP, FPX, GIF, JPEG, JPG, PNG, PICT(Windows®만 해당), TIF, TIFF |
| InDesign | INDD, INDT |
| MS® Office | DOC, PPT, RTF, XLS |
| PDF | PDF |
| Photoshop | PSD, FXG 및 카메라 원시 |
| PostScript | EPS, PS |
| Adobe Dynamic Media Classic 이미지 작성 | VNC, VNT, VNW |
| SVG | SVG, SVGX |
| TAR | TAR |
| 비디오 | 3GP, AVI, M2P, M2T, M2TS, M2V, M4V, MOV, MP4, MPEG, MPG, MTS, OGV, TS, VOB, WMV/ASF |
| XML | XML |
| ZIP | ZIP |

TAR 및 ZIP 업로드 지원에는 파일 압축을 풀 때 선택하는 확인란이 들어 있습니다.

### Dynamic Media에서 지원되지 않는 이미지 형식 {#unsupported-image-formats-dynamic-media}

다음 목록은 Dynamic Media에서 지원되는 *지원되지 않는* 래스터 이미지 파일 형식의 하위 유형에 대해 설명합니다.

* IDAT 청크 크기가 100MB보다 큰 PNG 파일입니다.
* PSB 파일
* CMYK, RGB, 회색 음영 또는 비트맵 이외의 색상 공간이 있는 PSD 파일은 지원되지 않습니다. DuoTone, Lab 및 Indexed 색상 공간은 지원되지 않습니다.
* 비트 깊이가 16보다 큰 PSD 파일.
* 부동 소수점 데이터가 있는 TIFF 파일입니다.
* Lab 색상 공간이 있는 TIFF 파일.

### 자산 유형 {#asset-types}

Adobe Dynamic Media Classic 프로그램을 사용하여 최적의 결과를 얻으려면 권장 파일 형식과 크기를 사용하십시오. 이 표에는 자산 유형 및 자주 사용하는 자산의 권장 형식과 파일 크기가 나열되어 있습니다.

| 자산 유형 | 설명/권장 사항 |
| --- | --- |
| 오디오 | 입력 오디오 자산 형식에는 AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3가 포함됩니다. 오디오를 MP3, AAC 및 HE-AAC로 트랜스코딩할 수 있습니다. |
| 이미지(이미지 크기 조정, 확대/축소, 이미지 집합, 회전 집합) | 이미지는 가장 긴 크기에서 2000픽셀 이상이어야 합니다. 일반적인 이미지 크기는 가장 긴 크기에서 1500픽셀에서 2500픽셀 사이입니다. TIFF 및 PNG 파일을 비롯한 손실 없는 이미지 형식이 권장됩니다. JPEG 이미지를 사용하는 경우에는 최고 품질 설정을 사용합니다. GIF 애니메이션 파일은 다른 정적 콘텐츠처럼 처리됩니다. |
| eCatalog | Adobe Acrobat 또는 &quot;press-ready&quot;로 저장된 Adobe Creative Suite 애플리케이션에서 생성된 고해상도 PDF 파일을 사용합니다. PDF에는 필요한 모든 글꼴, 이미지, 마스크가 포함됩니다. 또한 필요한 모든 참조 그래픽 요소를 단일 페이지, 이중 페이지 스프레드 또는 다중 페이지 형식으로 포함합니다. 파일 이름을 영숫자 순으로 지정하여 페이지를 정렬합니다. 업로드하기 쉽도록 eCatalog에 대한 모든 PDF를 단일 폴더에 배치합니다. 업로드 시 자르기 선택 사항을 선택하여 절단선, 등록 타겟 또는 색상 막대를 비롯한 트림 영역을 PDF에서 제거할 수 있습니다. 대부분의 인쇄용 PDF 파일은 CMYK 색상 공간에 있으므로 PDF 파일에 사용된 CMYK ICC 색상 프로필을 가져오는 것이 중요합니다. |
| 템플릿 | 텍스트, 이미지 및 레이어를 포함할 수 있는 계층화된 이미지 또는 레이아웃 디자인입니다. 변수 데이터를 사용자 지정할 수 있도록 이미지 레이어, 텍스트 문자열, 특성(예: 색상 및 크기)을 매개 변수화할 수 있습니다. 템플릿에 사용하기 위한 이미지 요구 사항은 다른 이미지와 같습니다. Photoshop 또는 다른 이미지 편집 프로그램에서 그래픽을 준비합니다. 각 그래픽을 TIFF 또는 PNG 형식의 평면화된 투명 파일로 저장합니다. 이미지 해상도가 필요한 용도에 적합한지 확인합니다. 인쇄용 이미지는 300ppi입니다. |
| 비디오 | Adobe Dynamic Media Classic은 OGV 및 MP4 형식으로 저장된 비디오 파일을 지원합니다. 업로드 시 파일을 MP4 형식으로 변환할 수 있습니다. [지원되는 자산 파일 형식](#supported-static-file-formats)을 참조하십시오. |
| 글꼴 | TrueType, `Type1`(Windows®만 해당), OpenType® 글꼴 및 PhotoFonts를 업로드했습니다. |
| 이미지 | 이미지 및 계층화된 이미지 파일입니다. |
| 이미지 집합 및 견본 집합 | 뷰어에 표시할 수 있는 관련 이미지 집합입니다. |
| ICC 프로필 | 업로드된 이미지를 소스 색상 공간에서 다른 색상 공간으로 변환하는 데 사용할 수 있는 색상 프로파일. |
| 비네팅 | 이미지 작성 프로그램으로 작성된 이미지 및 관련 파일. |
| 컨텐츠 파일 | Adobe InDesign, Illustrator 또는 Photoshop 컨텐츠 파일입니다. |
| FXG 파일 | 인쇄, 웹, 이메일, 데스크톱 및 장치 출력용 사용자 지정 가능한 템플릿을 만드는 데 사용할 수 있는 해상도 독립적인 그래픽 형식 파일입니다. |
| SVG 파일 | 이미지 제공 서버가 렌더링할 수 있는 확장 가능한 벡터 그래픽 파일입니다. |
| XML 파일 | 요청의 경로와 쿼리 부분을 수정하는 데 사용되는 전처리 규칙을 정의하는 파일입니다. |
| 계단식 스타일 시트 파일 | HTML5 뷰어의 사용자 지정을 위해 CSS 스킨을 업로드합니다. |
| JavaScript 파일 | JavaScript 파일은 계정 정보를 담기 위해 뷰어 계측에 사용됩니다. Adobe Security에서는 (사이트 간 스크립팅을 방지하기 위해) 전달에 사용할 별도의 도메인이 있는 클라이언트 계정에 대해서만 이 자산 유형을 권장합니다. |

>[!NOTE]
>
>이미지 파일과 PDF를 Adobe Dynamic Media Classic에 업로드하면 시스템이 이러한 소스 파일을 P-TIFF(피라미드 TIFF) 파일로 변환합니다. 이러한 P-TIFF는 나중에 Dynamic Media 이미지 서버에 게시되는 파일입니다. Adobe Dynamic Media Classic은 Adobe Dynamic Media Classic 확대/축소 뷰어로 볼 때 빠르게 확대/축소할 수 있는 다양한 확대/축소 비율이 포함되어 있으므로 피라미드 Tiff 파일 형식을 사용합니다.

### 지원되는 정적 파일 형식 {#supported-static-file-formats}

Adobe Dynamic Media Classic은 여러 정적 파일 형식을 지원합니다. 정적 콘텐츠 는 CSS, PDF, SVG 및 XML과 같이 &quot;있는 그대로&quot; 게시된 모든 자산입니다.

다음과 같은 파일 유형을 게시할 수 있습니다.

* 애니메이션 GIF
* 오디오 파일
* CSS
* JavaScript(회사가 고유한 도메인으로 구성된 경우)
* 기본 비디오
* PDF (기존 eCatalog/PDF 워크플로우에 대한 모든 PDF를 전송하지 않도록 업로드 후 PDF을 게시용으로 표시한 경우)
* PrX 비디오
* SVG
* XML
* ZIP

Adobe Dynamic Media Classic은 정적 콘텐츠의 미리보기 URL을 생성하는 옵션을 제공하지 않습니다.

### 파일 이름 요구 사항 {#filename-requirements}

업로드 프로세스 동안 파일 이름에서 파일 이름 확장자가 제거되므로 파일에 동일한 루트 이름을 사용할 수 없습니다. Adobe Dynamic Media Classic 시스템에서 에셋 파일 이름에서 파일 이름 확장자를 뺀 값이 에셋의 에셋 ID가 됩니다. 이 때문에 동일한 이름을 가진 자산이 있으면 안 됩니다.

회사의 모든 사용자가 파일 이름 지정에 대한 다음 규칙을 이해하는지 확인합니다.

* 이름이 같은 자산 ID는 시스템에서 사용할 수 없습니다.
* 자산 ID 이름은 대소문자를 구분합니다.
* 우수 사례로, 자산 ID에 공백이 포함되지 않도록 합니다(예: black jacket.tif 및 blue jacket.jpg). Adobe Dynamic Media Classic은 자산 이름을 사용하여 URL 문자열을 구성하는 경우 자산 이름의 빈 공간을 ASCII 인코딩합니다. 이러한 ASCII 코드는 읽기 어려우며 URL 읽기가 더 어려워질 수 있습니다.
* 언어 관련 문자는 파일 이름에 허용됩니다. 그러나 다음 문자는 파일 이름에 허용되지 않습니다.

  `\ ; / ? : @ & = + $ , &#42; " &lt; > | ' { } %`

  파일 이름에 위 문자 중 하나 이상이 포함된 경우 업로드 시 해당 문자가 파일 이름에서 제거됩니다.

일반적으로 에셋 파일 이름은 항목 번호, 제품 SKU 또는 다음과 같은 다른 이름과 같을 수 있습니다.

| 항목 | 파일 이름 | 자산 ID |
| --- | --- | --- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### 폴더 구성 및 구조 {#folder-organization-and-structure}

컨텐츠를 시스템에 업로드하기 전에 Adobe Dynamic Media Classic에서 컨텐츠에 대한 폴더 및 하위 폴더를 구성하고 구조화합니다. 이렇게 미리 계획하면 다음과 같은 두 가지 주요 장점이 있습니다.

* FTP를 통해 콘텐츠를 Adobe Dynamic Media Classic에 업로드할 때 업로드 중에 폴더 구조를 복제하도록 시스템에 지시할 수 있습니다. 이렇게 하면 콘텐츠가 컴퓨터 또는 네트워크에 있는 것과 동일한 Adobe Dynamic Media Classic 폴더 및 하위 폴더에 구성됩니다. (Adobe Dynamic Media Classic에서 폴더 구조를 복제하려면 FTP를 통해 에셋을 업로드할 때 하위 폴더 포함 옵션을 선택합니다.)
* 파일을 업로드한 후 시스템 내에서 폴더를 다시 구성하는 것이 신중하게 고려된 폴더 구조로 시작하는 것보다 훨씬 더 어렵습니다.

Adobe Dynamic Media Classic에 콘텐츠를 저장하기 위해 선택하는 폴더 이름 지정 접근 방식 및 구조는 조직의 요구 사항에 따라 다릅니다. 다음은 몇 가지 샘플 폴더 구조입니다.

**SKU 기반**: 폴더의 이름은 SKU 또는 항목 번호에 따라 지정됩니다. 예를 들어 0, 20 및 30숫자 시리즈에 대해 별도의 폴더가 만들어집니다.

**브랜드 기반**: 여러 브랜드 라인을 사용하는 제조업체 및 다른 회사의 다른 브랜드를 판매하는 소매업체의 경우, 다른 브랜드의 제품 폴더로 파일을 구분하십시오.

**프로젝트 기반**: 폴더는 롤아웃/드롭 날짜 또는 프로젝트 이름에 따라 구성됩니다. 주로 eCatalog를 생성하는 클라이언트가 이 방법을 선호합니다.

**웹 사이트 폴더 계층 구조 미러링**: 이 폴더 구조는 웹 사이트의 폴더 구조를 미러링합니다. 폴더 이름에는 제품 범주 등이 있습니다.

## 파일 업로드 기본 정보 {#uploading-your-files}

FTP를 통해 데스크탑에서 개별 파일을 업로드하거나 폴더를 업로드할 수 있습니다. 100MB가 넘는 파일을 업로드하거나 전체 폴더 및 하위 폴더를 업로드하려면 **FTP를 통해** 탭을 선택합니다.

Adobe Dynamic Media Classic에서 업로드 작업이 시작 및 종료되는 시기를 확인하고 문제가 발생하면 알리는 이메일 메시지를 보냅니다.

대규모 업로드 작업 중(또는 직후에) 일부 새 항목에 &quot;이미지가 아직 최적화되지 않음&quot; 메시지가 표시될 수 있습니다. 이 메시지는 파일이 아직 완전히 처리되지 않아 Adobe Dynamic Media Classic에 추가되지 않았기 때문에 표시됩니다. 이러한 파일은 나중에 최적화할 수 있습니다. [파일 최적화](application-setup.md#optimize_files)를 참조하세요.

### 데스크탑에서 탭을 사용하여 파일 업로드 {#upload-files-using-sps-desktop-application}

Adobe Dynamic Media Classic Desktop 응용 프로그램을 끌어 파일과 폴더를 업로드할 수 있습니다.

1. Adobe Dynamic Media Classic 데스크톱 응용 프로그램의 전역 탐색 표시줄에서 **[!UICONTROL 업로드]**&#x200B;를 선택합니다.
1. 업로드 페이지에서 **[!UICONTROL 데스크톱에서]** 탭을 선택합니다.
1. 업로드 페이지 왼쪽의 **[!UICONTROL 업로드할 파일 선택]** 영역에서 **[!UICONTROL 찾아보기]**&#x200B;를 선택하여 업로드할 파일 또는 폴더를 선택한 다음 **[!UICONTROL 열기]**&#x200B;를 선택합니다.
1. 업로드 페이지의 오른쪽의 선택한 **폴더 대상** 영역에서 업로드한 파일 또는 폴더를 추가하려는 대상 폴더로 이동합니다.
1. (선택 사항) [업로드] 페이지 하단 근처에 있는 [작업 이름] 텍스트 필드에 업로드 작업의 새 이름을 입력합니다. 또는 Adobe Dynamic Media Classic에서 제공하는 기본 시스템 생성 이름을 사용하면 됩니다. 업로드 및 게시 작업은 작업 페이지에 기록되며, 이 페이지에서 작업 상태를 확인할 수 있습니다. [작업 파일 확인](checking-job-files.md#checking_job_files)을 참조하십시오.
1. (선택 사항) 업로드 페이지 하단 근처에서 **[!UICONTROL 업로드 후 게시]**&#x200B;를 선택하면 업로드한 자산을 자동으로 게시할 수 있습니다.
파일을 게시하면 파일은 라이브 서버로 전송됩니다. 그런 다음 외부 웹 사이트와 애플리케이션에서 이러한 파일의 URL을 사용할 수 있습니다. 이와 동일한 옵션은 [작업 옵션] 대화 상자에서도 사용할 수 있습니다.
1. (선택 사항) [업로드] 페이지 하단 근처에 있는 **[!UICONTROL 확장명에 관계없이 같은 기본 에셋 이름으로 모든 폴더에 덮어쓰기]**&#x200B;를 선택합니다. 업로드하는 파일이 같은 이름으로 기존 파일을 바꾸도록 하려면. 이와 동일한 옵션은 [작업 옵션] 대화 상자에서도 사용할 수 있습니다.
이 옵션의 이름은 **[!UICONTROL 응용 프로그램 설정]** > **[!UICONTROL 일반 설정]** > **[!UICONTROL 응용 프로그램에 업로드]** > **[!UICONTROL 이미지 덮어쓰기]**&#x200B;의 설정에 따라 다를 수 있습니다.
1. [업로드] 페이지의 오른쪽 아래 모서리에서 **[!UICONTROL 작업 옵션]**&#x200B;을 선택한 다음 원하는 옵션을 지정합니다.

   [업로드 선택 사항](uploading-files.md#upload_options)을 참조하십시오.

1. 업로드 작업 옵션 대화 상자에서 **[!UICONTROL 저장]**&#x200B;을 선택합니다.
1. 업로드 페이지의 오른쪽 아래 모서리에서 **[!UICONTROL 업로드 제출]**&#x200B;을 선택합니다.
업로드 진행 상황을 보려면 전역 탐색 모음에서 **[!UICONTROL 작업]**&#x200B;을(를) 선택하십시오. Adobe Dynamic Media Classic에서 계속 작업할 수 있습니다. 언제든지 [작업] 페이지로 돌아가서 진행 중인 작업을 검토합니다. 진행 중인 업로드 작업을 취소하려면 [기간] 옆에 있는 **[!UICONTROL 취소]**&#x200B;를 선택합니다.

### FTP를 통해 탭을 사용하여 파일 업로드 {#upload-files-using-via-ftp}

1. 특정 지역에 해당하는 Adobe Dynamic Media Classic FTP 사이트에 로그온합니다. 관리자로부터 받은 FTP 사용자 이름과 암호를 사용합니다.
1. Adobe Dynamic Media Classic의 전역 탐색 모음에서 **[!UICONTROL 업로드]**&#x200B;를 선택합니다.
1. 업로드 페이지에서 **[!UICONTROL FTP를 통해]** 탭을 선택합니다.
1. 업로드 페이지 왼쪽의 **[!UICONTROL 업로드할 FTP 폴더 선택]** 영역에서 파일을 업로드할 FTP 폴더를 선택합니다.
1. 업로드 페이지의 오른쪽의 선택한 **[!UICONTROL Adobe Dynamic Media 폴더 대상]** 영역에서 Adobe Dynamic Media Classic의 대상 폴더를 선택합니다.
1. (선택 사항) [업로드] 페이지 하단 근처에 있는 [작업 이름] 텍스트 필드에 업로드 작업의 새 이름을 입력합니다. 또는 Adobe Dynamic Media Classic에서 제공하는 기본 시스템 생성 이름을 사용하면 됩니다. 업로드 및 게시 작업은 작업 페이지에 기록되며, 이 페이지에서 작업 상태를 확인할 수 있습니다.
[작업 파일 확인](checking-job-files.md#checking_job_files)을 참조하십시오.
1. (선택 사항) 업로드 페이지 하단 근처에서 **[!UICONTROL 업로드 후 게시]**&#x200B;를 선택하면 업로드하는 자산을 자동으로 게시할 수 있습니다.
파일을 게시하면 파일은 라이브 서버로 전송됩니다. 그런 다음 외부 웹 사이트와 애플리케이션에서 이러한 파일의 URL을 사용할 수 있습니다. 이와 동일한 옵션은 [작업 옵션] 대화 상자에서도 사용할 수 있습니다.
1. (선택 사항) [업로드] 페이지 하단 근처에 있는 **[!UICONTROL 확장명에 관계없이 같은 기본 에셋 이름으로 모든 폴더에 덮어쓰기]**&#x200B;를 선택합니다. 업로드하는 파일이 같은 이름으로 기존 파일을 바꾸도록 하려면. 이와 동일한 옵션은 [작업 옵션] 대화 상자에서도 사용할 수 있습니다.
이 옵션의 이름은 **[!UICONTROL 설정]** > **[!UICONTROL 응용 프로그램 설정]** > **[!UICONTROL 일반 설정]** > **[!UICONTROL 응용 프로그램에 업로드]** > **[!UICONTROL 이미지 덮어쓰기]**&#x200B;의 설정에 따라 다를 수 있습니다.
1. 선택 사항입니다. **[!UICONTROL FTP를 통해]** 탭을 선택한 경우에만 사용할 수 있습니다. 업로드 페이지 하단 근처에서 **[!UICONTROL 업로드 시 Zip 또는 Tar 파일 압축 해제]**&#x200B;를 선택하면 업로드한 ZIP 또는 TAR 파일에서 모든 파일을 자동으로 추출할 수 있습니다. 이와 동일한 옵션은 [작업 옵션] 대화 상자에서도 사용할 수 있습니다.
1. [업로드] 페이지의 오른쪽 아래 모서리에서 **[!UICONTROL 작업 옵션]**&#x200B;을 선택한 다음 원하는 옵션을 지정합니다.

   [업로드 선택 사항](uploading-files.md#upload_options)을 참조하십시오.

1. 업로드 작업 옵션 대화 상자에서 **[!UICONTROL 저장]**&#x200B;을 선택합니다.
1. 업로드 페이지의 오른쪽 아래 모서리에서 **[!UICONTROL 업로드 제출]**&#x200B;을 선택합니다.

   업로드 진행 상황을 보려면 전역 탐색 모음에서 **[!UICONTROL 작업]**&#x200B;을(를) 선택하십시오. 작업 페이지에 업로드 진행 상황이 표시됩니다. Adobe Dynamic Media Classic에서 계속 작업할 수 있습니다. 언제든지 [작업] 페이지로 돌아가서 진행 중인 작업을 검토합니다.

진행 중인 업로드 작업을 취소하려면 [기간] 옆에 있는 **[!UICONTROL 취소]**&#x200B;를 선택합니다.

## 업로드 작업 옵션 대화 상자 {#upload-options}

파일을 업로드할 때 [업로드 작업 옵션] 대화 상자에서 다음 옵션 중에서 선택할 수 있습니다.

* **작업**: 전체 업로드 작업에 영향을 주는 옵션을 선택하려면 **[!UICONTROL 작업]**&#x200B;을 선택하십시오.

  일반 설정에서 **[!UICONTROL 기본 업로드 옵션]** 대화 상자를 사용하여 작업을 업로드하는 *기본* 옵션을 선택할 수도 있습니다. **[!UICONTROL 설정]** > **[!UICONTROL 응용 프로그램 설정]** > **[!UICONTROL 일반 설정]** > **[!UICONTROL 기본 업로드 옵션]**(으)로 이동한 다음 원하는 기본 옵션을 설정합니다.

   * **[!UICONTROL When]**: 이 옵션은 **[!UICONTROL FTP를 통해]** 탭을 선택한 경우에만 사용할 수 있습니다.
      * **[!UICONTROL 한 번]**: 한 번 실행되는 업로드 작업을 지정합니다. 옵션에는 다음이 포함됩니다.
         * **[!UICONTROL 지금]**: [업로드 작업 옵션] 대화 상자에서 **[!UICONTROL 저장]**&#x200B;을 선택한 다음 [업로드] 페이지에서 **[!UICONTROL 업로드 제출]**&#x200B;을 선택한 직후에 업로드 작업을 실행합니다.
         * **[!UICONTROL 나중에 예약]**: 업로드 작업을 실행할 연도, 월, 일 및 시간(15분 단위)을 선택합니다.
      * **[!UICONTROL 반복]**: 매일, 매주 또는 매월 실행되는 업로드 작업을 지정합니다. 또는 업로드 작업을 원하는 사양에 맞게 사용자 정의합니다.
         * **[!UICONTROL 매일]**: 작업을 매일 실행할 시간을 설정합니다. 작업이 월요일부터 금요일까지 실행되도록 하려면 **[!UICONTROL 주중만]**&#x200B;을(를) 선택하십시오.
         * **[!UICONTROL 주별]**: 작업을 실행할 특정 요일과 시간을 선택합니다.
         * **[!UICONTROL 월별]**: 작업을 실행할 특정 요일 또는 요일(시작 시간 포함)을 선택합니다.
         * **[!UICONTROL 사용자 지정]**: 업로드 또는 게시 작업 시간 간격을 고유한 사양에 맞게 사용자 지정합니다. [사용자 지정 업로드 또는 게시 작업 시간 간격 만들기](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval)를 참조하십시오.

   * **[!UICONTROL 업로드 후 게시]**: **[!UICONTROL 데스크톱에서]** 탭 또는 **[!UICONTROL FTP를 통해]** 탭을 선택한 경우 사용할 수 있습니다. 업로드한 자산을 자동으로 게시할 수 있도록 이 옵션을 선택합니다. 파일을 게시하면 파일은 라이브 서버로 전송됩니다. 그런 다음 외부 웹 사이트와 애플리케이션에서 이러한 파일의 URL을 사용할 수 있습니다. 이 옵션은 업로드 페이지에서도 사용할 수 있습니다.

   * **[!UICONTROL 확장명에 관계없이 같은 기본 자산 이름으로 모든 폴더에 덮어쓰기]**: **[!UICONTROL 데스크탑에서]** 탭 또는 **[!UICONTROL FTP를 통해]** 탭을 선택한 경우 사용할 수 있습니다. 업로드한 파일이 동일한 이름을 가진 기존 파일을 대체하길 원하는 경우 이 선택 사항을 선택하십시오. 이 옵션은 업로드 페이지에서도 사용할 수 있습니다. 이 옵션의 이름은 **[!UICONTROL 설정]** > **[!UICONTROL 응용 프로그램 설정]** > **[!UICONTROL 일반 설정]** > **[!UICONTROL 응용 프로그램에 업로드]** > **[!UICONTROL 이미지 덮어쓰기]**&#x200B;의 설정에 따라 다를 수 있습니다.

   * **[!UICONTROL 업로드 시 Zip 또는 Tar 파일 압축 풀기]**: **[!UICONTROL 데스크탑에서]** 탭 또는 **[!UICONTROL FTP를 통해]** 탭을 선택한 경우 사용할 수 있습니다.
업로드한 ZIP 또는 TAR 파일에서 모든 파일을 자동으로 추출할 수 있도록 이 옵션을 선택합니다. 이와 동일한 옵션은 [작업 옵션] 대화 상자에서도 사용할 수 있습니다.

   * **[!UICONTROL 하위 폴더 포함]**: **[!UICONTROL FTP를 통해]** 탭을 선택한 경우에만 사용할 수 있습니다.
업로드 폴더의 하위 폴더를 업로드하려면 이 선택 사항을 선택하십시오. 업로드한 폴더 및 하위 폴더의 이름은 Adobe Dynamic Media Classic에 자동으로 입력됩니다.

   * **[!UICONTROL 메타데이터 파일 처리]**: **[!UICONTROL FTP를 통해]** 탭을 선택한 경우에만 사용할 수 있습니다. 탭으로 구분된 또는 XML 파일을 업로드하여 여러 에셋에 메타데이터를 추가하려면 이 옵션을 선택합니다.
[메타데이터 가져오기(FTP 사용)](viewing-adding-exporting-metadata.md#import-metadata)를 참조하십시오.

* **자르기 옵션**: 이미지에서 공백 픽셀을 자동으로 자릅니다. **[!UICONTROL 자르기]** 메뉴를 열고 **[!UICONTROL 수동]**&#x200B;을 선택한 다음 [위쪽], [오른쪽], [아래쪽] 및 [왼쪽] 텍스트 필드에 픽셀 측정값을 입력하여 옆에서 자릅니다. 자르기 메뉴에서 **[!UICONTROL 트리밍]**&#x200B;을 선택하고 다음 옵션을 선택할 수도 있습니다.

   * **[!UICONTROL 다음을 기준으로 트림]**: 색상 또는 투명도를 기준으로 자를지 여부를 선택합니다.
      * **[!UICONTROL 색상]**: 색상 옵션을 선택합니다. 그런 다음 [모퉁이] 메뉴를 선택하고 자르려는 공백 색상을 가장 잘 나타내는 색상으로 이미지의 모퉁이를 선택합니다.
색상을 기반으로 트림: 이미지 모서리에서 선택한 색상과 잘라낼 픽셀의 색상이 일치하는 경우에만 0으로 지정하십시오. 값이 1에 가까워질수록 색상 차이를 더 많이 허용합니다.
      * **[!UICONTROL 투명도]**: **[!UICONTROL 투명도]** 옵션을 선택합니다.
투명도를 기반으로 트리밍: 픽셀이 투명한 경우에만 자르도록 0을 지정합니다. 1에 가까운 숫자를 사용하면 투명도가 더 높아집니다.
      * **[!UICONTROL 허용 한도]**: 슬라이더를 드래그하여 0에서 1까지의 허용 한도를 지정하십시오.

* **색상 프로필 옵션**: Adobe Dynamic Media Classic 동적 게재에 사용되는 최적화된 파일을 만들 때 색상 변환을 선택하십시오.

   * **[!UICONTROL 기본 색상 보존]**: 이미지에 색상 공간 정보가 포함될 때마다 소스 이미지 색상을 유지합니다. 색상 변환은 없습니다. 거의 모든 이미지에는 현재 적절한 색상 프로필이 이미 포함되어 있습니다. 그러나 CMYK 소스 이미지에 포함된 색상 프로필이 없는 경우, 색상이 sRGB(표준 빨강 녹색 파랑) 색상 공간으로 변환됩니다. sRGB는 웹 페이지에 이미지를 표시하는 데 권장되는 색상 공간입니다.
   * **[!UICONTROL 원래 색상 공간 유지]**: Adobe Dynamic Media Classic으로 수집되는 시점에 색상 변환 없이 원래 색상을 유지합니다. 임베드된 색상 프로파일이 없는 이미지의 경우, 이미지에 대한 요청을 처리하는 데 필요한 색상 변환은 게시 설정에 구성된 대로 기본 색상 프로파일을 사용하여 수행됩니다. 이러한 색상 프로파일이 이 옵션을 사용하여 만든 파일의 색상과 항상 일치하지는 않습니다. 따라서 [기본 색상 유지] 옵션을 사용하는 것이 좋습니다.
   * **[!UICONTROL 사용자 지정 변환]** > **[!UICONTROL 변환]**: **[!UICONTROL 변환 변환]** 및 **[!UICONTROL 변환]** 색상 공간을 선택할 수 있도록 메뉴를 엽니다. 이 고급 옵션은 소스 파일에 포함된 모든 색상 정보를 무시합니다. 제출하는 모든 이미지에 잘못되거나 누락된 색상 프로파일 데이터가 포함된 경우에만 이 옵션을 선택합니다.

* **이미지 편집 옵션**: 이미지에서 클리핑 &lt;> 마스크를 유지하고 색상 프로파일을 선택할 수 있습니다.
업로드 시 [이미지 미세 조정 옵션](image-editing-options-upload.md#image-editing-options-at-upload)을 참조하십시오.

* **PostScript® 옵션**: PostScript® 파일을 래스터화하고, 파일을 자르고, 투명한 배경을 유지하고, 해상도를 선택하고, 색상 공간을 선택할 수 있습니다.
[PostScript 및 Illustrator 파일 작업](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files)을 참조하세요.

* **Photoshop 옵션**: Adobe® Photoshop® 파일에서 템플릿을 만들고, 레이어를 유지하고, 레이어 이름 지정 방법을 지정하고, 텍스트를 추출하고, 이미지가 템플릿에 고정되는 방법을 지정할 수 있습니다.
[PSD 업로드 선택 사항](psd-files.md#psd_upload_options)을 참조하십시오.

* **PDF 옵션**: 파일을 래스터화하고, 검색어와 링크를 추출하고, 전자 카탈로그를 자동 생성하고, 해상도를 설정하고, 색상 공간을 선택할 수 있습니다.
[PDF 업로드 선택 사항](pdfs.md#pdf_upload_options)을 참조하십시오.

* **Illustrator 옵션**: Adobe Illustrator® 파일을 래스터화하고, 투명한 배경을 유지하고, 해상도를 선택하고, 색상 공간을 선택할 수 있습니다.
[PostScript 및 Illustrator 파일 작업](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files)을 참조하세요.

* **EVIDEO 옵션**: 비디오 사전 설정을 선택하여 비디오 파일을 변환할 수 있습니다.
[비디오 인코딩 사전 설정 작업](uploading-encoding-videos.md#working_with_video_encoding_presets)을 참조하십시오.

* **추가 메타데이터**: 업로드할 파일을 설명하는 키워드를 입력하십시오. 키워드를 쉼표로 구분합니다. 키워드를 사용하면 자산을 더 쉽게 검색할 수 있습니다.
[고급 검색 실시](searching-assets.md#conducting_an_advanced_search)를 참조하십시오.
[키워드 업로드](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/548_upload-keywords_converted%20renamed_Done-AVS) 교육 비디오도 참조하세요.

* **일괄처리 집합 사전 설정**: 업로드한 파일에서 이미지 집합, 회전 집합 또는 견본 집합을 만들려면 사용할 사전 설정의 **[!UICONTROL 활성]** 열을 선택하십시오. 여러 개의 사전 설정을 선택할 수 있습니다. [응용 프로그램 설정/일괄처리 집합 사전 설정] 페이지에서 사전 설정을 만들 수 있습니다.
[배치 집합 사전 설정](application-setup.md#batch_set_presets)을 참조하십시오.

* **고급**: [다른 작업으로 업로드 팔로우](uploading-files.md#follow-an-upload-with-another-job)를 참조하십시오.

## 업로드 후 다른 작업 수행 {#follow-an-upload-with-another-job}

FTP를 사용하여 항목을 업로드할 때 업로드가 완료되면 후속 작업이 시작되도록 예약할 수 있습니다. 다른 작업이 시작되도록 예약된 경우 여기에서 예약한 작업은 이후 큐에 대기합니다.

새 작업은 지정한 주소로 알림을 전송하여 해당 위치의 코드가 트리거될 수 있도록 합니다. 이 후속 게시 작업은 업로드 작업과 동일한 이름을 사용하지만 시작 부분에 *Pub_* 텍스트가 추가됩니다.

**다른 작업으로 업로드 수행:**

1. **[!UICONTROL 업로드]**&#x200B;를 선택한 다음 **[!UICONTROL FTP를 통해]** 탭을 선택합니다.
1. 업로드 페이지의 오른쪽 아래 모서리에서 **[!UICONTROL 작업 옵션]**&#x200B;을 선택합니다.
1. 업로드 작업 옵션 대화 상자에서 **[!UICONTROL 고급]** 섹션을 확장합니다.
1. **[!UICONTROL 다른 작업과 함께 업로드 수행]** 드롭다운 목록에서 다음 중 하나를 선택하십시오.

   * 없음
   * HTTP 요청
   * 이미지 서비스 제공 게시
   * 이미지 렌더링 게시
   * 비디오 게시

1. HTTP 주소를 지정합니다.
1. 파일이 업로드된 경우에만 실행할지 여부를 지정합니다.
1. 이 작업이 완료될 때마다 또는 파일이 게시된 경우에만 이 요청을 실행할지 여부를 나타냅니다.

   >[!NOTE]
   >
   >정기적으로 예약된 작업을 수행하면 경우에 따라 파일이 게시되지 않을 수 있습니다.

>[!MORELIKETHIS]
>
>* [자산 폴더를 사용하여 작업](asset-folders.md#working_with_asset_folders)
>* [반복 업로드 및 게시 작업 처리](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [업로드 또는 게시 작업을 트리거로 사용](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)
