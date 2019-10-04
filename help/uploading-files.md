---
title: 파일 업로드
seo-title: 파일 업로드
description: 널
seo-description: 파일을 업로드하는 방법을 알아봅니다.
uuid: B 3025 F 84-4 F 28-4276-BC 9 C-F 0 C 0 C 2 A 26 E 12
contentOwner: 관리
content-type: 참조
products: sg_ Experiencemanager/dynamic-media-scene -7
discoiquuid: B 2 BC 3 BF 9-E 313-481 A -8670-C 3 Bedde 21 B 1 A
translation-type: tm+mt
source-git-commit: 684950586bf9b1df897ac46b52d84a21f4cb4120

---


# 파일 업로드{#uploading-files}

자산·파일을·Scene7·Publishing System에 업로드하기 전에 자산 파일의 이름이 올바른지, 폴더 구조가 원하는 방식으로 설정 및 구성되었는지 확인합니다. Dynamic Media Classic에서 제공하는 FTP 사이트나 컴퓨터나 네트워크에서 직접 파일을 업로드할 수 있습니다. Dynamic Media Classic 에서는 파일을 업로드할 때 최적화하기 위한 옵션을 제공합니다. Adobe Scene7 Publishing System 데스크톱 애플리케이션을 설치한 경우 데스크톱에서 직접 파일과 폴더를 드래그하여 업로드할 수 있습니다. [[애플리케이션 일반 설정]](application-setup.md#general_settings)을 참조하십시오.

## 업로드할 자산 및 폴더 준비 {#preparing-your-assets-and-folders-for-uploading}

자산을 Scene7 Publishing System에 업로드하기 전에 자산이 올바른 형식과 크기인지 확인합니다. 또한 자산 이름 지정에 대한 Dynamic Media Classic 규칙을 준수해야 합니다. 폴더 구성 및 파일 구조를 설정함으로써 간편하게 파일을 찾고 작업할 수 있습니다.

### 지원되는 자산 파일 형식 {#supported-asset-file-formats}

이 표에는 Scene7 Publishing System에서 지원하는 자산 파일 형식이 나열되어 있습니다. For information on supported Camera Raw files, see [www.adobe.com/go/learn_s7_cameraraw_en](https://www.adobe.com/go/learn_s7_cameraraw_en).

| 자산 파일 형식 | 설명 |
|--- |--- |
| 오디오 | AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3 |
| 계단식 스타일 시트 | CSS |
| 색상 프로필 | ICC, ICM |
| 글꼴 | AFM, OTF, PFB, PFM, PhotoFont, TTC, TTF |
| FXG | FXG |
| Illustrator | AI, FXG |
| 이미지 | BMP, FPX, GIF, JPEG, JPG, PNG, PICT(Windows 전용), TIF, TIFF |
| InDesign | INDD, INDT |
| MS Office | DOC, PPT, RTF, XLS |
| PDF | PDF |
| Photoshop | PSD, FXG 및 카메라 원시 |
| PostScript | EPS, PS |
| Dynamic Media Classic 이미지 제작 | VNC, VNT, VNW |
| SVG | SVG, SVGX |
| TAR | TAR |
| 비디오 | 3GP, AVI, M2P, M2T, M2TS, M2V, M4V, MOV, MP4, MPEG, MPG, MTS, OGV, TS, VOB, WMV/ASF |
| XML | XML |
| ZIP | ZIP |

TAR 및 ZIP 업로드 지원에는 파일 압축을 풀 때 선택하는 확인란이 들어 있습니다.

### 자산 유형 {#asset-types}

Dynamic Media Classic 플랫폼에서 최적의 결과를 얻으려면 권장 파일 형식 및 크기를 사용하십시오. 이 표에는 자산 유형 및 자주 사용하는 자산의 권장 형식과 파일 크기가 나열되어 있습니다.

| 자산 유형 | 설명/권장 사항 |
|--- |--- |
| 오디오 | 입력 오디오 자산 형식에는 AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3가 포함됩니다. 오디오를 MP3, AAC 및 HE-AAC로 트랜스코딩할 수 있습니다. |
| 이미지(이미지 크기 조정, 확대/축소, 이미지 집합, 회전 집합) | 이미지는 가장 긴 크기가 2000픽셀 이상이어야 합니다. 일반적인 이미지 크기는 가장 긴 크기가 1500픽셀에서 2500픽셀 사이입니다. TIFF 및 PNG 파일을 비롯한 손실 없는 이미지 형식이 권장됩니다. JPEG 이미지를 사용하는 경우에는 최고 품질 설정을 사용합니다. 애니메이션 GIF 파일은 다른 정적 컨텐츠처럼 처리됩니다. |
| eCatalog | Adobe® Acrobat® 또는 Creative Suite 애플리케이션에서 만들고 "인쇄용"으로 저장한 고해상도 PDF 파일을 사용합니다. PDF에는 필요한 모든 글꼴, 이미지, 마스크 및 참조된 그래픽 요소가 단일 페이지, 양면 스프레드 또는 다중 페이지 형식으로 포함되어 있습니다. 파일 이름을 영숫자 순으로 지정하여 페이지를 정렬합니다. 업로드하기 쉽도록 eCatalog에 대한 모든 PDF를 단일 폴더에 배치합니다. 업로드 시 자르기 선택 사항을 선택하여 절단선, 등록 타겟 또는 색상 막대를 비롯한 트림 영역을 PDF에서 제거할 수 있습니다. 대부분의 인쇄용 PDF 파일은 CMYK 색상 공간에 있으므로 PDF 파일에 사용된 CMYK ICC 색상 프로필을 가져오는 것이 중요합니다. |
| 템플릿 | 텍스트, 이미지 및 레이어를 포함할 수 있는 계층화된 이미지 또는 레이아웃 디자인입니다. 변수 데이터를 사용자 지정할 수 있도록 이미지 레이어, 텍스트 문자열, 특성(예: 색상 및 크기)을 매개 변수화할 수 있습니다. 템플릿에 사용하기 위한 이미지 요구 사항은 다른 이미지와 같습니다. Photoshop 또는 다른 이미지 편집 프로그램에서 그래픽을 준비합니다. 각 그래픽을 TIFF 또는 PNG 형식의 평면화된 투명 파일로 저장합니다. 이미지 해상도가 필요한 용도에 적합한지 확인합니다. 인쇄용 이미지는 300ppi여야 합니다. |
| 비디오 | Dynamic Media Classic는 OGV 및 MP 4 형식으로 저장된 비디오 파일을 지원합니다. 업로드 [시 파일을 MP 4 형식으로 트랜스코딩할 수 있습니다. 지원되는 에셋 파일 형식을 참조하십시오](#supported-static-file-formats). |
| 글꼴 | 업로드한 TrueType, Type1(Windows 전용), OpenType 글꼴 및 PhotoFonts입니다. |
| 이미지 | 이미지 및 계층화된 이미지 파일입니다. |
| 이미지 집합 및 견본 집합 | 뷰어에 표시할 수 있는 관련 이미지 집합입니다. |
| ICC 프로필 | 업로드한 이미지를 소스 색상 공간에서 다른 색상 공간으로 전환하는 데 사용할 수 있는 색상 프로필입니다. |
| 비네팅 | 이미지 작성 프로그램에서 작성된 이미지 및 관련 파일입니다. |
| 컨텐츠 파일 | Adobe InDesign, Illustrator 또는 Photoshop 컨텐츠 파일입니다. |
| FXG 파일 | 인쇄, 웹, 이메일, 데스크톱 및 장치 출력용 사용자 지정 가능한 템플릿을 만드는 데 사용할 수 있는 해상도 독립적인 그래픽 형식 파일입니다. |
| SVG 파일 | 이미지 제공 서버가 렌더링할 수 있는 확장 가능한 벡터 그래픽 파일입니다. |
| XML 파일 | 요청의 경로와 쿼리 부분을 수정하는 데 사용되는 전처리 규칙을 정의하는 파일입니다. |
| 계단식 스타일 시트 파일 | HTML5 뷰어 사용자 지정에 사용되는 CSS 스킨을 업로드합니다. |
| JavaScript 파일 | Javascript 파일은 뷰어 계측에서 계정 정보를 저장하는 데 사용됩니다. 사이트 간 스크립팅을 방지하기 위해 이 파일은 별도의 도메인을 전달에 사용하는 클라이언트 계정에만 사용하는 것이 좋습니다. |

>[!NOTE]
>
>이미지 파일과 PDF를 SPS로 업로드하면 이러한 소스 파일이 P-TIFF(Pyramid TIFF) 파일로 전환됩니다. 이러한 P-TIFF는 나중에 다이내믹 미디어 이미지 서버에 게시되는 파일입니다. Dynamic Media Classic는 Dynamic Media Classic 확대/축소 뷰어로 볼 때 빠르게 확대/축소할 수 있는 다양한 확대/축소 비율이 포함되어 있으므로 피라미드형 TIFF 파일 형식을 사용합니다.

### 지원되는 정적 파일 형식 {#supported-static-file-formats}

Dynamic Media Classic는 여러 정적 파일 형식을 지원합니다. 정적 컨텐트는 CSS, PDF, SVG, XML 등과 같이 "있는 그대로" 게시된 모든 자산입니다.

다음과 같은 파일 유형을 게시할 수 있습니다.

* 애니메이션 GIF
* 오디오 파일
* CSS
* JavaScript(회사가 고유한 도메인으로 구성된 경우)
* 마스터 비디오
* PDF(기존 eCatalog/PDF 워크플로에 대한 모든 PDF 제공을 방지하기 위해 PDF가 업로드 후 게시로 특별히 표시된 경우)
* PrX 비디오
* SVG
* XML
* ZIP

Dynamic Media Classic 에서는 정적 컨텐츠의 미리 보기 URL를 생성하는 옵션을 제공하지 않습니다.

### 파일 이름 요구 사항 {#filename-requirements}

업로드 프로세스 동안 파일 이름에서 파일 이름 확장자가 제거되므로 파일에 동일한 루트 이름을 사용할 수 없습니다. Dynamic Media Classic 시스템에서 자산 파일 이름은 파일 이름 확장자를 뺀 값에서 자산의 자산 ID가 됩니다. 이 때문에 동일한 이름을 가진 자산이 있으면 안 됩니다.

회사의 모든 사용자가 다음과 같은 파일 이름 지정 규칙을 이해해야 합니다.

* 시스템에서 이름과 정확하게 일치하는 자산 ID는 허용되지 않습니다.
* 자산 ID는 대/소문자를 구분합니다.
* 우수 사례로, 자산 ID에 공백이 포함되지 않도록 합니다(예: black jacket.tif 및 blue jacket.jpg). Dynamic Media Classic는 에셋 이름을 사용하여 URL 문자열을 구성할 때 에셋 이름에서 빈 공간을 인코딩합니다. 이러한 ASCII 코드는 읽기 어려우며 URL 읽기가 더 어려워질 수 있습니다.
* 언어 관련 문자는 파일 이름에 허용됩니다. 그러나 다음 문자는 파일 이름에 허용되지 않습니다.

   \ ; / ? : @ &amp; = + $ , * " &lt; &gt; | ' { } %

   파일 이름에 위 문자 중 하나 이상이 포함된 경우 업로드 시 해당 문자가 파일 이름에서 제거됩니다.

대부분의 경우 자산 파일 이름은 다음과 같이 항목 번호, 제품 SKU 또는 기타 이름과 같을 수 있습니다.

| 항목 | 파일 이름 | 자산 ID |
|--- |--- |--- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### 폴더 구성 및 구조 {#folder-organization-and-structure}

시스템에 컨텐츠를 업로드하기 전에 Scene7 Publishing System에 컨텐츠의 폴더와 하위 폴더를 구성합니다. 이렇게 미리 계획하면 다음과 같은 두 가지 주요 장점이 있습니다.

* FTP를 통해 컨텐츠를 SPS로 업로드할 때 업로드 시 폴더 구조를 복제하도록 시스템에 지정할 수 있습니다. 이렇게 하면 컨텐츠가 SPS에서 사용자 컴퓨터 또는 네트워크와 동일한 폴더 및 하위 폴더로 구성됩니다. SPS에서 폴더 구조를 복제하려면 FTP를 통해 자산을 업로드할 때 [하위 폴더 포함] 선택 사항을 선택합니다.
* 파일을 업로드한 후 시스템 내에서 폴더를 다시 구성하는 것이 신중하게 고려된 폴더 구조로 시작하는 것보다 훨씬 더 어렵습니다.

Scene7·Publishing System에 컨텐츠를 저장하기 위해 선택하는 폴더 이름 지정 방법과 구조는 조직의 요구에 따라 달라집니다. 다음은 몇 가지 샘플 폴더 구조입니다.

**SKU 기반** 폴더는 SKU 또는 항목 번호에 따라 이름이 지정됩니다. 예를 들어 모든 0-, 20-, 30- 번호 시리즈에 대해 별도의 폴더가 만들어집니다.

**다양한 브랜드 라인과 다른 회사의 브랜드를 마케팅하는 소매업체를** 위한 브랜드 기반 브랜드 및 다른 브랜드에 대해 이름이 지정된 제품 폴더로 파일을 구분합니다.

**프로젝트 기반** 폴더는 롤아웃/드롭 날짜 또는 프로젝트 이름에 따라 구성됩니다. 주로 eCatalog를 생성하는 클라이언트가 이 방법을 선호합니다.

**웹 사이트 폴더 계층 구조 미러** 이 폴더 구조는 제품 카테고리에 대한 폴더 구조로, 웹 사이트의 폴더 구조를 미러링합니다.

## 파일 업로드 정보 {#uploading-your-files}

데스크톱에서 개별 파일을 업로드하거나 FTP를 통해 폴더를 업로드할 수 있습니다. If you want to upload more than 100 MB of files or upload entire folders and subfolders, select the **VIA FTP** tab.

Scene 7 Publishing System 데스크탑 애플리케이션을 설치한 경우 데스크탑에서 대상 업로드 폴더로 파일 및 폴더를 직접 드래그할 수 있습니다.

업로드 작업이 시작되고 종료될 때 확인하고 문제를 알리기 위해 Scene7 Publishing System에서 이메일 메시지를 보냅니다.

큰 업로드 작업 중이나 직후에 일부 새 항목이 "이미지가 아직 최적화되지 않음" 메시지를 표시할 수도 있습니다. 이 메시지는 파일이 아직 완전히 처리되지 않아 SPS에 추가되기 때문에 나타납니다. 이러한 파일은 나중에 최적화할 수 있습니다. [파일 최적화](application-setup.md#optimize_files)를 참조하십시오.

### 데스크탑 탭에서 파일 업로드 {#upload-files-using-sps-desktop-application}

Scene7 Publishing System Desktop 애플리케이션에서는 끌기를 통해 파일과 폴더를 업로드할 수 있습니다.

1. Scene7 Publishing System 데스크톱 애플리케이션의 글로벌 탐색 막대에서 **업로드**&#x200B;를 클릭합니다.
1. On the Upload page, click the **FROM DESKTOP** tab.
1. 업로드 페이지의 왼쪽의 업로드할 파일 **선택** 영역에서 **찾아보기를** 클릭하여 업로드할 파일이나 폴더를 선택한 ****&#x200B;다음 열기를 클릭합니다.
1. 업로드 페이지의 오른쪽에서 폴더 대상 **선택** 영역에서 업로드된 파일이나 폴더를 추가할 대상 폴더로 이동합니다.
1. (선택 사항) 업로드 페이지의 하단에서 **작업 이름** 필드에 업로드 작업의 새 이름을 지정합니다. SPS에서 제공하는 기본 시스템 생성 이름을 사용할 수도 있습니다. 작업과 다른 업로드 및 게시 작업은 작업 페이지에 기록되어 작업 상태를 확인할 수 있습니다.
[작업 파일 확인](checking-job-files.md#checking_job_files)을 참조하십시오.
1. (선택 사항) 업로드한 자산을 자동으로 **게시하려면 업로드 페이지 하단에서 업로드** 후 게시를 선택합니다.
파일을 게시하면 파일은 라이브 서버로 전송됩니다. 그런 다음 외부 웹 사이트와 애플리케이션에서 이러한 파일의 URL을 사용할 수 있습니다. [작업 옵션] 대화 상자에서도 이와 동일한 옵션을 사용할 수 있습니다.
1. (선택 사항) 업로드 페이지의 하단에서 업로드하는 **파일이 동일한 이름으로 기존 파일을 대체하도록 하려는 경우 확장과** 관계없이 모든 폴더에서 덮어쓰기를 선택합니다. [작업 옵션] 대화 상자에서도 이와 동일한 옵션을 사용할 수 있습니다.
The name of this option could be different, depending on the settings in **Application Setup &gt; General Settings &gt; Upload to Application &gt; Overwrite Images**.
1. Near the lower-right corner of the Upload page, click **Job Options**, then specify the options you want.

   [업로드 선택 사항](uploading-files.md#upload_options)을 참조하십시오.

1. [업로드 작업 옵션] 대화 상자에서 **저장**&#x200B;을 클릭합니다.
1. 업로드 페이지의 오른쪽 하단에서 업로드 **제출을 클릭합니다**.
업로드 진행 상황을 보려면, 글로벌 탐색 막대에서 **작업**&#x200B;을 클릭합니다. Scene7 Publishing System을 계속 사용하면서 필요할 때마다 언제든지 작업 페이지로 돌아와 진행 중인 작업을 검토할 수 있습니다. 진행 중인 업로드 작업을 취소하려면 [기간] 옆에 있는 **취소**&#x200B;를 선택합니다.

### FTP를 통해 파일 업로드 탭 {#upload-files-using-via-ftp}

1. 특정 지역과 관련된 Dynamic Media Classic FTP 사이트에 로그인합니다. 관리자로부터 받은 FTP 사용자 이름과 암호를 사용합니다.
1. Dynamic Media Classic의 글로벌 탐색 막대에서 **업로드를 클릭합니다**.
1. On the Upload page, click the **VIA FTP** tab.
1. 업로드 페이지의 왼쪽에 있는 [업로드할 FTP 폴더 **선택** ] 영역에서 파일을 업로드할 FTP 폴더를 선택합니다.
1. 업로드 페이지의 오른쪽에서 SPS 폴더 대상 **선택** 영역의 Scene 7 Publishing System에서 대상 폴더를 선택합니다.
1. (선택 사항) 업로드 페이지의 하단에서 **작업 이름** 필드에 업로드 작업의 새 이름을 지정합니다. SPS에서 제공하는 기본 시스템 생성 이름을 사용할 수도 있습니다. 작업과 다른 업로드 및 게시 작업은 작업 페이지에 기록되어 작업 상태를 확인할 수 있습니다.
[작업 파일 확인](checking-job-files.md#checking_job_files)을 참조하십시오.
1. (선택 사항) 업로드한 자산을 자동으로 **게시하려면 업로드 페이지 하단에서 업로드** 후 게시를 선택합니다.
파일을 게시하면 파일은 라이브 서버로 전송됩니다. 그런 다음 외부 웹 사이트와 애플리케이션에서 이러한 파일의 URL을 사용할 수 있습니다. [작업 옵션] 대화 상자에서도 이와 동일한 옵션을 사용할 수 있습니다.
1. (선택 사항) 업로드 페이지의 하단에서 업로드하는 **파일이 동일한 이름으로 기존 파일을 대체하도록 하려는 경우 확장과** 관계없이 모든 폴더에서 덮어쓰기를 선택합니다. [작업 옵션] 대화 상자에서도 이와 동일한 옵션을 사용할 수 있습니다.
The name of this option could be different, depending on the settings in **Application Setup &gt; General Settings &gt; Upload to Application &gt; Overwrite Images**.
1. (옵션; 업로드 페이지의 아래쪽에 있는 [FTP **]** 탭을 클릭해야만 사용할 수 있습니다. 업로드한 **zip 또는 tar 파일에서 모든 파일을 자동으로 추출하려면 업로드** 시 zip 또는 tar 파일 압축을 해제합니다. [작업 옵션] 대화 상자에서도 이와 동일한 옵션을 사용할 수 있습니다.
1. Near the lower-right corner of the Upload page, click **Job Options**, then specify the options you want.

   [업로드 선택 사항](uploading-files.md#upload_options)을 참조하십시오.

1. [업로드 작업 옵션] 대화 상자에서 **저장**&#x200B;을 클릭합니다.
1. 업로드 페이지의 오른쪽 하단에서 업로드 **제출을 클릭합니다**.

   업로드 진행 상황을 보려면, 글로벌 탐색 막대에서 **작업**&#x200B;을 클릭합니다. 작업 페이지에 업로드 진행 상황이 표시됩니다. Scene7 Publishing System을 계속 사용하면서 필요할 때마다 언제든지 작업 페이지로 돌아와 진행 중인 작업을 검토할 수 있습니다.

진행 중인 업로드 작업을 취소하려면 [기간] 옆에 있는 **취소**&#x200B;를 클릭합니다.

## 업로드 작업 옵션 대화 상자 {#upload-options}

파일을 업로드할 때 업로드 작업 옵션 대화 상자에서 다음 옵션 중 하나를 선택할 수 있습니다.

* **작업** — **작업을** 클릭하여 전체 업로드 작업에 영향을 주는 옵션을 선택합니다.

   일반 설정에서 기본 업로드 옵션 대화 상자를 사용하여 작업 업로드에 *대한 기본* **옵션을** 선택할 수도 있습니다. **설정 &gt; 애플리케이션 설정 &gt; 일반 설정 &gt; 기본 업로드 옵션을**&#x200B;클릭한 다음 원하는 기본 옵션을 설정합니다.

   * **** — **When** 옵션은 FTP VIA 탭을 **선택한 경우에만 사용할** 수 있습니다.
      * **** 일회성— 한 번 실행되는 업로드 작업을 지정합니다. 옵션은 다음과 같습니다.
         * **** —— 업로드 작업 옵션 대화 상자에서 **저장을** 클릭한 다음 업로드 페이지에서 업로드 제출을 클릭하면 **업로드 작업을** 즉시 실행합니다.
         * **나중에 예약** — 업로드 작업을 실행할 연도, 월, 일, 시간 (15 분 단위로 증분) 를 선택합니다.
      * **반복** — 일별, 주별 또는 월별로 실행되는 업로드 작업을 지정합니다. 또는 업로드 작업을 고유한 사양에 맞게 사용자 정의합니다.
         * **일별** — 작업을 매일 실행할 시간을 설정합니다. 작업이 월요일에만 실행되도록 하려면 **[주중 전용**] 를 선택합니다.
         * **주별** — 작업을 실행할 특정 요일 및 시간을 선택합니다.
         * **월별** — 작업을 실행할 날짜 또는 요일 (시작 시간을 포함하여) 를 선택합니다.
         * **사용자** 정의— 업로드 또는 게시 작업 시간 간격을 고유한 사양에 맞게 사용자 정의할 수 있습니다. [사용자 지정 업로드 또는 게시 작업 시간 간격 만들기](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval)를 참조하십시오.
   * **업로드** 후 게시— **[데스크탑에서]** 탭이나 [FTP **]** 탭을 선택한 경우 사용할 수 있습니다. 이 옵션을 선택하면 업로드한 자산이 자동으로 게시됩니다. 파일을 게시하면 파일은 라이브 서버로 전송됩니다. 그런 다음 외부 웹 사이트와 애플리케이션에서 이러한 파일의 URL을 사용할 수 있습니다. 이 옵션은 업로드 페이지에서도 사용할 수 있습니다.

   * **확장자에 관계없이 동일한 기본 자산 이름 폴더에 덮어쓰기** — **[데스크탑에서]** 탭이나 [FTP **]** 탭을 선택한 경우 사용할 수 있습니다. 업로드한 파일이 동일한 이름을 가진 기존 파일을 대체하길 원하는 경우 이 선택 사항을 선택하십시오. 이 옵션은 업로드 페이지에서도 사용할 수 있습니다. The name of this option could be different, depending on the settings in **Application Setup &gt; General Settings &gt; Upload to Application &gt; Overwrite Images**.

   * **업로드 시 ZIP 또는 TAR 파일 압축 해제** — **[데스크탑에서]** 탭이나 [FTP **]** 탭을 선택한 경우 사용할 수 있습니다.
업로드된 zip 또는 tar 파일에서 모든 파일을 자동으로 추출하려면 이 옵션을 선택합니다. [작업 옵션] 대화 상자에서도 이와 동일한 옵션을 사용할 수 있습니다.

   * **하위 폴더** 포함— FTP **를 통해** 탭을 선택한 경우에만 사용할 수 있습니다.
업로드 폴더의 하위 폴더를 업로드하려면 이 선택 사항을 선택하십시오. 업로드하는 폴더 및 하위 폴더의 이름이 SPS에 자동으로 입력됩니다.

   * **메타데이터 파일** 처리— [FTP **사용]** 탭을 선택한 경우에만 사용할 수 있습니다. 탭으로 구분된 파일이나 XML 파일을 업로드하여 여러 자산에 메타데이터를 추가하려는 경우 이 선택 사항을 선택합니다. [메타데이터 가져오기(FTP 사용)](viewing-adding-exporting-metadata.md#import-metadata)를 참조하십시오.


* **자르기 옵션** — 이미지에서 공백 픽셀을 자동으로 자르려면 [자르기] 메뉴를 열고 [수동] 를 선택한 다음 맨 위, 오른쪽, 아래쪽 및 왼쪽 필드에 픽셀 측정값을 입력하여 측면에서 자릅니다. [자르기] 메뉴에서 [트림]을 선택하고 다음 선택 사항을 선택할 수도 있습니다.

   * **트리밍 기준** — 색상 또는 투명도를 기반으로 자를 것인지 여부를 선택할 수 있습니다.

      * **Color** — 색상 옵션을 선택합니다. [모서리] 메뉴를 선택한 다음 자르려는 공백 색상을 가장 잘 나타내는 색상이 지정된 이미지 모서리를 선택합니다.

         색상을 기반으로 트림: 이미지 모서리에서 선택한 색상과 잘라낼 픽셀의 색상이 일치하는 경우에만 0으로 지정하십시오. 값이 1에 가까워질수록 색상 차이를 더 많이 허용합니다.

      * **투명도** — 투명도 옵션을 선택합니다.

         투명도를 기반으로 트림: 완전 투명한 경우에만 픽셀을 자르려면 0을 지정합니다. 숫자가 1에 가까울수록 허용되는 투명도가 증가합니다.

      * **허용치** — 슬라이더를 드래그하여 0에서 1 사이의 허용치를 지정합니다.

* **색상 프로파일 옵션** — Dynamic Media Classic Dynamic Delivery에 사용되는 최적화된 파일을 만들 때 색상 변환을 선택합니다.

   * **기본 색상 보존** — 이미지에 색상 공간 정보가 포함될 때마다 소스 이미지 색상을 유지합니다. 색상 변환은 없습니다. 거의 모든 이미지에는 현재 적절한 색상 프로필이 이미 포함되어 있습니다. 그러나 CMYK 소스 이미지에 포함된 색상 프로필이 없는 경우, 색상이 sRGB(표준 빨강 녹색 파랑) 색상 공간으로 변환됩니다. sRGB는 웹 페이지에 이미지를 표시할 때 권장되는 색상 공간입니다.

   * **원본 색상 공간** 유지— Scene 7 Publishing System에 도입했을 때 색상 변환 없이 원래 색상을 유지합니다. 포함된 색상 프로필이 없는 이미지의 경우, 이미지 요청을 처리하기 위한 필수 색상 변환은 게시 설정에서 구성된 대로 기본 색상 프로필을 사용하여 수행됩니다. 이 색상 프로필은 이 옵션으로 만든 파일에 있는 색상과 맞지 않을 수 있습니다. 따라서 [기본 색상 유지] 옵션을 사용하는 것이 좋습니다.

   * **사용자 지정** &gt; 에서 전환 및 색상 공간으로 변환을 선택할 수 있도록 메뉴를 엽니다. 이 고급 옵션은 소스 파일에 포함된 모든 색상 정보를 무시합니다. 제출하는 모든 이미지에 잘못되었거나 누락된 색상 프로필 데이터가 포함되어 있는 경우에만 이 옵션을 선택해야 합니다.

* **이미지 편집 옵션** — 이미지의 클리핑 &lt; &gt; 마스크를 보존하고 색상 프로필을 선택할 수 있습니다.
[업로드 시 이미지 편집 선택 사항](image-editing-options-upload.md#image-editing-options-at-upload)을 참조하십시오.

* **POSTSCRIPT 옵션** — PostScript® 파일을 래스터화하고, 파일을 자르고, 투명 배경을 유지하고, 해상도를 선택하고, 색상 공간을 선택할 수 있습니다.
[PostScript 및 Illustrator 파일 작업](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files)을 참조하십시오.

* **PHOTOSHOP 옵션** — Adobe® Photoshop® 파일에서 템플릿을 만들고, 레이어를 유지하며, 레이어의 이름을 지정하는 방법을 지정하고, 텍스트를 추출하고, 이미지가 템플릿에 고정되는 방식을 지정할 수 있습니다.
[PSD 업로드 선택 사항](psd-files.md#psd_upload_options)을 참조하십시오.

* **PDF 옵션** — 파일을 래스터화하고, 검색 단어 및 링크를 추출하고, 전자 카탈로그를 자동으로 생성하고, 해상도를 설정하고, 색상 공간을 선택할 수 있습니다.
[PDF 업로드 선택 사항](pdfs.md#pdf_upload_options)을 참조하십시오.

* **ILLUSTRATOR 옵션** — Adobe Illustrator® 파일을 래스터화하고 투명 배경을 유지하며 해상도를 선택하고 색상 공간을 선택할 수 있습니다.
[PostScript 및 Illustrator 파일 작업](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files)을 참조하십시오.

* **Evideo 옵션** — 비디오 사전 설정을 선택하여 비디오 파일을 트랜스코딩할 수 있습니다.
[비디오 인코딩 사전 설정으로 작업](uploading-encoding-videos.md#working_with_video_encoding_presets)을 참조하십시오.

* **추가 메타데이터** — 업로드할 파일을 설명하는 키워드를 입력합니다. 키워드를 쉼표로 구분합니다. 키워드를 사용하면 자산을 쉽게 검색할 수 있습니다. [고급 검색 수행](searching-assets.md#conducting_an_advanced_search)을 참조하십시오.

* **일괄적인 집합 사전 설정** — 업로드한 파일에서 이미지 세트, 다축 스핀 세트 또는 견본 집합을 만들려면 사용하려는 사전 설정에 대해 활성 열을 클릭합니다. 여러 개의 사전 설정을 선택할 수 있습니다. 애플리케이션 설정/배치 집합 사전 설정 페이지에서 사전 설정을 만듭니다.
[배치 집합 사전 설정](application-setup.md#batch_set_presets)을 참조하십시오.

* **고급** — 다른 작업과 함께 업로드를 [참조하십시오](uploading-files.md#follow-an-upload-with-another-job).

## 업로드 후 다른 작업 수행 {#follow-an-upload-with-another-job}

FTP를 사용하여 항목을 업로드할 때 업로드가 완료되는 즉시 시작되도록 후속 작업을 예약할 수 있습니다. 이때 다른 작업이 시작되도록 예약하면 여기서 예약한 작업이 이후의 큐에 놓입니다.

새 작업은 지정한 주소로 알림을 보내 해당 위치의 코드가 트리거될 수 있도록 합니다. 이 후속 게시 작업은 업로드 작업과 동일한 이름을 사용하지만 시작 부분에 *Pub_* 텍스트가 추가됩니다.

**업로드 후 다른 작업을 수행하려면**

1. **업로드를**&#x200B;클릭한 다음 FTP **사용** 탭을 클릭합니다.
1. In the lower-right corner of the Upload page, click **Job Options**.
1. 업로드 작업 옵션 대화 상자에서 **고급** 섹션을 확장합니다.
1. 다른 작업과 함께 업로드 **드롭다운 목록에서 다음 중 하나를** 선택합니다.

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
   >정기 예약된 작업에서는 파일이 게시되지 않을 수도 있습니다.

>[!MORELIKETHIS]
>
>* [자산 폴더 작업](asset-folders.md#working_with_asset_folders)
>* [Handling recurring upload and publish jobs](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [업로드 또는 게시 작업을 트리거로 사용](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)
