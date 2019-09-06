---
title: PDF 파일 업로드
seo-title: PDF 파일 업로드
description: 널
seo-description: Ecatalog와 연관된 PDF 파일을 업로드하는 방법을 알아봅니다.
uuid: 9 E 178 BB 2-AC 09-427 A-B 61 A-AAD 4 E 87 A 5837
contentOwner: 관리
content-type: 참조
products: sg_ Experiencemanager/dynamic-media-scene -7
discoiquuid: 0097 CBA 5-C 886-4115-BC 35-7 AE 7 A 500202 F
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# PDF 파일 업로드{#uploading-the-pdf-files}

일반적으로 Adobe PDF 파일이 eCatalog의 소스입니다. 이 파일에는 모든 이미지 정보와 글꼴 및 벡터 그래픽이 들어 있습니다. 이미지를 사용하여 eCatalog를 작성할 수도 있습니다. 업로드할 PDF 파일을 준비한 후 글로벌 탐색 막대에서 [업로드] 단추를 선택하여 PDF 업로드를 시작합니다.

## PDF 파일 준비 {#preparing-your-pdf-files}

Scene7 Publishing System에 업로드하기 전에 PDF 파일을 준비합니다.

* 파일을 업로드하기 쉽도록 모든 파일을 컴퓨터나 네트워크의 동일한 폴더에 넣습니다.
* 페이지를 기준으로 파일 이름을 영숫자 순으로 지정합니다. 페이지를 정렬하면 파일이 업로드된 후 페이지를 올바른 순서대로 배치하기가 더 쉽습니다.
* [PDF] 페이지를 검사하여 절단선, 등록 타겟 또는 색상 막대가 포함되어 있는지 여부를 확인합니다. 이러한 표시는 문서를 인쇄할 때 용지를 절단하는 위치를 결정하며, eCatalog를 웹에 배치하기 전에 제거해야 합니다. Dynamic Media Classic 에서는 PDF 파일을 업로드할 때 자르는 옵션을 선택할 수 있습니다.
* 뷰어가 키워드로 eCatalog를 검색하게 하려면 PDF 파일이 "균일화"되었는지 확인합니다. 균일화된 PDF 파일에서는 검색어를 추출할 수 없습니다. PDF가 균일화되었는지 확인하려면 PDF 내에서 텍스트 선택을 시도합니다. 텍스트를 선택할 수 없으면 PDF가 균일화된 것이며 뷰어가 eCatalog에서 키워드로 검색할 수 없습니다.
* 원래 인쇄용이기 때문에 PDF 파일에는 대체로 CMYK 이미지가 포함되어 있습니다. 기본적으로 SPS는 이러한 CMYK 이미지를 지능적으로 검색하고 내부 CMYK 색상 프로필을 사용하여 전환합니다. 그러나 사용자 지정 색상 프로필을 사용하여 CMYK 이미지를 전환하려는 경우 이 작업도 가능합니다. 

   [ICC 프로필](icc-profiles.md#icc_profiles)을 참조하십시오.

## 우수 사례 PDF 업로드 선택 사항 {#best-practice-pdf-upload-options}

다양한 업로드 방법에 대한 자세한 내용은 [파일 업로드](uploading-files.md#uploading_your_files)를 참조하십시오.

업로드할 파일을 선택하고 다음과 같은 *우수 사례* PDF 선택 사항을 선택합니다.

**자르기페이지에** 재단선 표시, 등록 표시 또는 기타 기호가 포함되어 있는 경우 [자르기] 메뉴를 선택하고 [수동] 를 선택합니다. 페이지 위쪽, 오른쪽, 아래쪽 및 왼쪽에서 자를 픽셀 수를 입력합니다. 일반적으로 절단선은 1/2인치 여백으로 설정됩니다. 인치당 픽셀 해상도로 150(권장 설정)을 선택한다고 가정할 경우 [위쪽], [오른쪽], [아래쪽] 및 [왼쪽] 텍스트 상자에 각각 75, 75, 75, 75를 입력하면 여백에서 1/2인치가 잘립니다(150ppi에서 1/2인치는 75픽셀과 같음).

**처리** 처리 메뉴를 선택하고 래스터화를 선택합니다. eCatalog의 모든 페이지와 이미지를 표시할 수 있도록 PDF 파일이 래스터화되어야 합니다.

**검색어 추출 (선택 사항)** 뷰어에서 Ecatalog에서 키워드로 검색할 수 있게 하려면 이 옵션을 선택합니다.

**여러 페이지 PDF에서 ecatalog 자동 생성 (선택 사항)** 업로드할 때 ecatalog를 자동으로 만들려면 이 옵션을 선택합니다. 먼저 PDF 파일을 선택하고 [작성] 명령을 선택하지 않고 eCatalog 화면으로 바로 이동한 다음 eCatalog에서 작업을 시작할 수 있습니다. eCatalog 이름은 PDF 파일을 따서 지정됩니다.

**Dynamic** Media Classic 에서는 인치당 150 픽셀을 권장합니다.

**Colorspace** Dynamic Media Classic 에서는 자동으로 감지를 선택할 것을 권장합니다. 일반적으로 인쇄 출력용으로 만들어진 PDF는 CMYK를 사용하고 온라인 보기용 PDF는 RGB입니다. PDF에서 두 가지 색상 공간을 모두 사용하는 경우 [RGB로 강제 설정] 또는 [CMYK로 강제 설정]을 선택하여 특정 색상 공간을 선택할 수 있습니다. 예를 들어 페이지 그래픽은 CMYK 색상 공간을 사용하고 사진은 RGB를 사용하는 경우 PDF에서 두 가지 색상 공간을 모두 사용합니다. ICC 프로필을 업로드한 경우 해당 이름이 [색상 공간] 메뉴에 표시되며 여기서 프로필을 선택할 수 있습니다. 

[ICC 프로필](icc-profiles.md#icc_profiles)을 참조하십시오.

**색상 프로파일** 색상 프로필 선택 옵션:

**SRGB** 로 변환
SRGB (표준 빨강 녹색 파랑) 로 변환됩니다. SRGB는 웹 페이지에 이미지를 표시할 때 권장되는 색상 공간입니다.

**원본 색상 공간은 원래 색상 공간을** 유지합니다.

**사용자 지정 &gt; 메뉴를 여는 메뉴에서** 전환 및 색상 공간으로 변환을 선택할 수 있습니다. 표준 Photoshop 색상 공간이나 SPS로 업로드한 색상 공간을 선택할 수 있습니다.

[ICC 프로필](icc-profiles.md#icc_profiles)을 참조하십시오.

>[!NOTE]
>
>모든 PDF 선택 사항에 대한 자세한 내용은 [PDF 업로드 선택 사항](pdfs.md#pdf_upload_options)을 참조하십시오.

