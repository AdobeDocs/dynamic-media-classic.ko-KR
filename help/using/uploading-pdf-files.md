---
title: PDF 파일 업로드
description: Adobe Dynamic Media Classic에서 eCatalog와 연결된 PDF 파일을 업로드하는 방법을 알아봅니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
topic: Integrations, Development
level: Experienced
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 34%

---

# PDF 파일 업로드{#uploading-the-pdf-files}

일반적으로 Adobe PDF 파일은 eCatalog의 소스입니다. 이러한 파일에는 모든 이미지 정보, 글꼴 및 벡터 그래픽이 포함되어 있습니다. 이미지를 사용하여 eCatalog를 작성할 수도 있습니다. 업로드할 PDF 파일을 준비한 후 전역 탐색 모음에서 를 선택합니다. **[!UICONTROL 업로드]** PDF 업로드를 시작합니다.

페이지 추출을 위해 PDF을 업로드할 때 Adobe은 다음 제한을 적용합니다.

| PDF 제한 유형 | 제한 적용됨 | 2022년 12월 31일 제한 변경 |
| --- | --- | --- |
| 추출 시 고려할 PDF의 최대 페이지 수 | 5000(새 업로드용) | 100(모든 PDF) |

참조: [Dynamic Media 제한 사항](/help/using/limitations.md).

## PDF 파일 준비

Adobe Dynamic Media Classic에 업로드하기 전에 PDF 파일을 준비합니다.

* 파일을 더 쉽게 업로드할 수 있도록 모든 파일을 컴퓨터 또는 네트워크의 동일한 폴더에 배치합니다.
* 페이지를 기준으로 파일 이름을 영숫자 순으로 지정합니다. 페이지를 정렬하면 파일이 업로드된 후 페이지를 올바른 순서대로 배치하기가 더 쉽습니다.
* PDF 페이지에 자르기 표시, 등록 대상 또는 색상 막대가 포함되어 있는지 확인하려면 페이지를 검사합니다. 이러한 표시는 문서를 인쇄할 때 용지를 절단하는 위치를 결정하며, eCatalog를 웹에 배치하기 전에 제거해야 합니다. Adobe Dynamic Media Classic은 PDF 파일을 업로드할 때 자르기 표시 옵션을 제공합니다.
* 뷰어에서 키워드로 eCatalog를 검색하도록 하려면 PDF 파일이 &quot;병합됨&quot;인지 확인하십시오. 균일화된 PDF 파일에서는 검색어를 추출할 수 없습니다. PDF가 균일화되었는지 확인하려면 PDF 내에서 텍스트 선택을 시도합니다. 텍스트를 선택할 수 없는 경우 PDF이 병합되고 뷰어가 eCatalog에서 키워드로 검색할 수 없습니다.
* 원래 인쇄용이기 때문에 PDF 파일에는 대체로 CMYK 이미지가 포함되어 있습니다. 기본적으로 Adobe Dynamic Media Classic은 이러한 CMYK 이미지를 지능적으로 감지하고 내부 CMYK 색상 프로파일을 사용하여 변환할 수 있습니다. 그러나 사용자 지정 색상 프로필을 사용하여 CMYK 이미지를 전환하려는 경우 이 작업도 가능합니다. 

  다음을 참조하십시오 [ICC(International Color Consortium) 프로파일](icc-profiles.md#icc_profiles).

## 우수 사례 PDF 업로드 선택 사항 {#best-practice-pdf-upload-options}

다양한 업로드 방법에 대한 자세한 내용은 [파일 업로드](uploading-files.md#uploading_your_files)를 참조하십시오.

업로드할 파일을 선택한 다음 선택합니다 *모범 사례* PDF 옵션:

* **자르기 옵션** - 업로드 작업 옵션 대화 상자에서 다음을 선택합니다. **[!UICONTROL 자르기 옵션]**. PDF 페이지에 자르기 표시, 등록 표시 또는 기타 표시가 있는 경우 **[!UICONTROL 자르기]** 드롭다운 목록에서 선택 **[!UICONTROL 수동]**. 페이지 위쪽, 오른쪽, 아래쪽 및 왼쪽에서 자를 픽셀 수를 입력합니다. 자르기 표시는 종종 0.5인치 여백으로 설정됩니다. 다음을 선택했다고 가정해 보십시오. **[!UICONTROL 150]** (권장) 인치당 픽셀 해상도로 [위쪽], [오른쪽], [아래쪽] 및 [왼쪽] 텍스트 상자에 75, 75, 75, 75를 입력합니다. 이러한 경우 여백에서 0.5인치(150ppi에서 1.5은 75픽셀임)를 자릅니다.

* **처리 중** - 업로드 작업 옵션 대화 상자에서 다음을 선택합니다. **[!UICONTROL PDF 옵션]**. 다음에서 **[!UICONTROL 처리 중]** 드롭다운 목록에서 선택 **[!UICONTROL 래스터화]**. eCatalog의 모든 페이지와 이미지를 표시할 수 있도록 PDF 파일이 래스터화되어야 합니다.

* **검색어 추출(선택 사항)** - 업로드 작업 옵션 대화 상자에서 다음을 선택합니다. **[!UICONTROL PDF 옵션]**. 추출 드롭다운 목록에서 다음을 선택합니다 **[!UICONTROL 단어 검색]** 뷰어에서 eCatalog의 키워드별로 검색할 수 있도록 하려면 다음을 수행하십시오.

* **여러 페이지 PDF에서 eCatalog 자동 생성(선택 사항)** - 업로드 작업 옵션 대화 상자에서 다음을 선택합니다. **[!UICONTROL PDF 옵션]**. 선택 **[!UICONTROL 여러 페이지 PDF에서 eCatalog 자동 생성]** 업로드할 때 eCatalog를 자동으로 만들 수 있습니다. 먼저 PDF 파일을 선택하고 [작성] 명령을 선택하지 않고 eCatalog 화면으로 바로 이동한 다음 eCatalog에서 작업을 시작할 수 있습니다. eCatalog 이름은 PDF 파일을 따서 지정됩니다.

* **해결 방법** - 업로드 작업 옵션 대화 상자에서 다음을 선택합니다. **[!UICONTROL PDF 옵션]**. 다음에서 **[!UICONTROL 해결 방법]** 텍스트 필드에 값을 입력합니다. Adobe Dynamic Media Classic은 인치당 150픽셀을 권장합니다.

* **색상 공간** - 업로드 작업 옵션 대화 상자에서 다음을 선택합니다. **[!UICONTROL PDF 옵션]**. 색상 공간 드롭다운 목록에서 **[!UICONTROL 자동 감지]**. 일반적으로 인쇄 출력용으로 만들어진 PDF는 CMYK를 사용하고 온라인 보기용 PDF는 RGB입니다. PDF에서 두 가지 색상 공간을 모두 사용하는 경우 [RGB로 강제 설정] 또는 [CMYK로 강제 설정]을 선택하여 특정 색상 공간을 선택할 수 있습니다. 예를 들어 페이지 그래픽은 CMYK 색상 공간을 사용하고 사진은 RGB를 사용하는 경우 PDF에서 두 가지 색상 공간을 모두 사용합니다. ICC 프로필을 업로드한 경우 해당 이름이 [색상 공간] 메뉴에 표시되며 여기서 프로필을 선택할 수 있습니다. 

  다음을 참조하십시오 [ICC(International Color Consortium) 프로파일](/help/using/icc-profiles.md).

* **색상 프로파일 옵션** - 업로드 작업 옵션 대화 상자에서 다음을 선택합니다. **[!UICONTROL 색상 프로파일 옵션]**&#x200B;을 선택한 다음 색상 프로파일 옵션을 선택합니다.

   * **원래 색상 공간 유지** - 원래 색상 공간을 유지합니다.

   * **사용자 지정 시작 > 종료** - 하위 메뉴를 열어 **[!UICONTROL 변환 출처]** 및 **[!UICONTROL 변환 대상]** 색상 공간. 표준 Photoshop 색상 공간 또는 Adobe Dynamic Media Classic에 업로드한 색상 공간을 선택할 수 있습니다.

<!-- * **Convert To SRGB** - Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on web pages. -->

다음을 참조하십시오 [ICC(International Color Consortium) 프로파일](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>모든 PDF 선택 사항에 대한 자세한 내용은 [PDF 업로드 선택 사항](pdfs.md#pdf_upload_options)을 참조하십시오.
