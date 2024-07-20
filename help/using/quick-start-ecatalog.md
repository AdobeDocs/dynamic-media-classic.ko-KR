---
title: "빠른 시작: 전자 카탈로그"
description: Adobe Dynamic Media Classic의 eCatalog 기술을 빠르게 시작하고 실행하는 데 도움이 되는 eCatalog 소개 및 빠른 시작입니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 9e2df814-465d-412a-a032-ef3e8cb462ba
topic: Integrations
level: Experienced
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '1470'
ht-degree: 25%

---

# 빠른 시작: eCatalog{#quick-start-ecatalogs}

eCatalog는 카탈로그, 브로슈어, 전단지, 제품 설명서 또는 광고 순환 등 인쇄 자료의 디지털 웹 버전입니다. eCatalog는 웹 사이트의 eCatalog 뷰어에 표시됩니다. 이 뷰어는 인쇄물을 읽는 경험을 시뮬레이션합니다.

다음 교육 비디오도 참조하십시오.

* [빠른 시작 1: 전자 카탈로그](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/561_Quick%20Start%20-%20Part%201_converted%20renamed_eCatalogs-AVS)
* [빠른 시작 2: 전자 카탈로그](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/562_Quick%20Start%20-%20Part%202_converted%20renamed_eCatalogs-AVS)

eCatalog에 대해 선택하는 설정에 따라 뷰어에서는 다음을 수행할 수 있습니다.

* 카탈로그에서 키워드 또는 키워드를 검색합니다. 검색 결과는 카탈로그의 왼쪽에 있는 검색 패널에 축소판 목록으로 표시됩니다. 각 클릭 가능한 썸네일은 강조 표시된 검색어가 있는 카탈로그 스프레드를 나타냅니다.

* 소셜 미디어를 통해 카탈로그를 공유합니다. 오프라인으로 보려면 카탈로그를 다운로드하십시오. 즐겨찾기를 활성화하여 돌아갈 항목을 빠르게 표시하거나 카탈로그를 인쇄하십시오.
* 목차 또는 페이지 그리드 보기를 사용하여 카탈로그를 탐색합니다. 페이지의 중간 가장자리를 선택하여 페이지를 앞이나 뒤로 이동합니다.
* 확대, 축소 및 패닝하여 페이지의 항목을 검사합니다.
* 항목에 대한 정보가 있는 팝업 창을 볼 수 있도록 포인터를 페이지 영역(이미지 맵이라고 함) 위로 이동합니다.
* 항목에 대한 자세한 정보가 있는 새 웹 페이지를 열 수 있도록 페이지 영역을 선택합니다.
* 스티커 메모를 써서 eCatalog 페이지에 첨부합니다.
* 관련 웹 페이지 또는 컨텍스트 내 정보 패널을 실행하려면 이미지 맵 아이콘을 탭합니다.
* 손가락을 모아 확대, 살짝 밀어 페이지 넘김 등의 제스처 상호 작용을 사용합니다.
* 키워드로 항목을 검색합니다.

![사용자에게 표시되는 전자 카탈로그입니다. A) eCatalog에서 페이지를 여는 중 B)eCatalog가 페이지 2.](/help/using/assets/ec_cat_viewer_popup.png)(으)로 전환됨

eCatalog를 만들려면 일반적으로 Adobe Acrobat 또는 다른 인쇄 프로그램에서 만든 고해상도 PDF 파일을 사용하지만, 이미지 파일에서 eCatalog를 만들 수도 있습니다.

eCatalog를 만드는 과정에서 페이지나 페이지 스프레드를 선택한 순서대로 정렬할 수 있습니다. 단일 페이지, 양면 페이지 스프레드 또는 복수 페이지 스프레드를 사용할 것인지를 선언할 수도 있습니다. 페이지 영역에 대한 이미지 맵을 만들어 뷰어가 페이지에서 영역을 선택하고 웹 사이트에서 새 페이지를 여는 등의 작업을 수행할 수 있습니다. eCatalog 화면 내의 [정보 패널] 설정을 사용하여 표시되는 롤오버 텍스트를 관리할 수 있습니다. 100개보다 많은 구성 선택 사항 중에서 선택하여 eCatalog 뷰어를 구성할 수도 있습니다. 특정 타겟 사용자에 맞게 뷰어의 기능과 모양을 조정할 수 있습니다.

>[!NOTE]
>
>Dynamic Media: Scene7 모드 사용자이고 eCatalogs를 사용하려면 CRXDE Lite에서 `pdfbrochure` 값을 편집하십시오. 이렇게 하려면 Adobe Experience Manager에서 **[!UICONTROL 도구]** > **[!UICONTROL 일반]** > **[!UICONTROL CRXDE Lite]**(으)로 이동하십시오. 왼쪽 패널 탐색 트리에서 `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`(으)로 이동합니다.
>
>오른쪽 아래 창의 **[!UICONTROL 속성]** 탭에서 `jobParam` 행을 선택합니다. `pdfbrochure`의 값을 `false`에서 `true`(으)로 설정합니다. `pdfbrochure=true`에서와 같이
>
>CRXDE Lite 페이지의 왼쪽 상단 모서리에서 **[!UICONTROL 모두 저장]**&#x200B;을 선택합니다.
>
>이제 Adobe Dynamic Media Classic에서 eCatalogs를 작성할 수 있습니다.

이 eCatalog 빠른 시작은 eCatalog를 빨리 시작하고 실행하는 데 도움이 됩니다. 1-7 단계를 수행하십시오. 각 단계 후에는 추가 정보를 찾을 수 있는 주제 머리글에 대한 상호 참조가 있습니다.

## 1. PDF 파일 업로드

일반적으로 Adobe PDF 파일이 eCatalog의 소스입니다. 원래 인쇄용이기 때문에 PDF 파일에는 대체로 CMYK 이미지가 포함되어 있습니다. Adobe Dynamic Media Classic은 이러한 이미지를 감지하고 표준 CMYK 색상 프로파일을 사용하여 변환합니다. 하지만 사용자 정의 색상 프로파일을 업로드하고 사용해야 합니다.

전역 탐색 모음에서 **[!UICONTROL 업로드]**&#x200B;를 선택하여 eCatalog에 대한 PDF 파일 또는 이미지 업로드를 시작합니다. 데스크톱이나 FTP를 통해 파일을 업로드할 수 있습니다. 100MB가 넘는 파일이나 파일이 많은 경우 FTP가 권장됩니다.

[업로드] 화면의 [PDF 선택 사항] 아래에는 적절한 해상도와 올바른 색상 공간으로 PDF 파일을 업로드하기 위한 선택 사항이 제공됩니다. 인치당 150픽셀 해상도를 사용하는 것이 좋습니다. PDF 파일을 업로드할 때 **[!UICONTROL 전자 카탈로그 자동 생성]** 옵션을 선택하여 전자 카탈로그를 만들 수 있습니다.

[PDF 파일 업로드](uploading-pdf-files.md#uploading_the_pdf_files)를 참조하십시오.

## 2. eCatalog 만들기

[찾아보기] 패널에서 PDF 또는 이미지 파일을 선택하여 eCatalog를 만듭니다. **[!UICONTROL 빌드]**&#x200B;를 선택한 다음 **[!UICONTROL 전자 카탈로그]**&#x200B;를 선택하십시오.

eCatalog 페이지의 **[!UICONTROL 페이지 순서]** 탭에서 레이아웃 옵션을 선택하십시오. **[!UICONTROL 1 Up]**, **[!UICONTROL 2 Up]** 또는 **[!UICONTROL Custom]**. 페이지 또는 스프레드를 끌거나 큰 eCatalog의 경우 [이동] 메뉴에서 페이지 이름을 선택하여 페이지 또는 스프레드를 다시 정렬할 수 있습니다.

페이지를 추가하려면 자산 라이브러리에서 폴더를 선택하고 PDF 또는 이미지 파일을 [주문 페이지] 화면으로 드래그합니다. 기본 페이지 번호 대신 사용자 지정 페이지 이름을 제공하거나 많은 페이지 이름을 가져올 수 있습니다.

**[!UICONTROL 저장]**&#x200B;을 선택하고 전자 카탈로그의 이름을 입력한 다음 저장할 Adobe Dynamic Media Classic 폴더를 선택한 다음 **[!UICONTROL 저장]**&#x200B;을 선택합니다. 페이지 순서를 변경하거나 전자 카탈로그를 편집할 때마다 **[!UICONTROL 저장]**&#x200B;을 선택하여 변경 사항을 저장하십시오.

[전자 카탈로그 만들기](creating-ecatalog.md)를 참조하세요.

## 3. 이미지 맵 만들기

이미지 맵은 eCatalog 페이지에 다른 측면을 추가합니다. 이미지 맵은 항목에 대한 자세한 정보를 제공하는 페이지의 한 영역입니다. 뷰어가 포인터를 이미지 맵 위로 롤오버하면 항목에 대한 설명이 표시됩니다. 이미지 맵을 클릭하면 항목에 대해 자세히 알아볼 수 있는 새 웹 페이지를 여는 외부 참조가 활성화됩니다.

이미지 맵을 만들려면 eCatalog 화면을 엽니다. 그런 다음 eCatalog 화면의 **[!UICONTROL 페이지 매핑]** 탭으로 이동하여 Rectangle Image Map 도구 또는 Polygon Image Map 도구를 사용하여 맵을 프레임화합니다. [패닝] 도구로 맵 테두리를 드래그하여 이미지 맵의 위치와 크기를 조정할 수 있습니다.

이미지 맵의 프레임을 만든 후 이미지 맵을 선택할 때 이동할 URL 주소를 입력합니다. 포인터를 이미지 맵 위로 이동할 때 표시되는 롤오버 텍스트를 입력할 수도 있습니다.

[전자 카탈로그 이미지 맵 만들기](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps)를 참조하세요.

[이미지 맵을 사용하여 전자 카탈로그에 리치 미디어 포함](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog)을 참조하십시오.

eCatalog 화면의 정보 패널 설정을 사용하여 이미지 맵 텍스트를 설정하고 관리할 수 있습니다.

[전자 카탈로그의 정보 패널 콘텐츠 관리](/help/using/info-panel-content-ecatalog.md)를 참조하십시오.

## 4. eCatalog 뷰어 사전 설정 설정

최종 사용자는 eCatalog 뷰어에서 eCatalog를 봅니다. 관리자는 eCatalog 뷰어를 구성할 수 있습니다. 윤곽선 색상을 변경하고 새 &quot;스킨&quot;을 선택하여 eCatalog를 브랜딩할 수 있습니다. Adobe Dynamic Media Classic에는 몇 가지 &quot;모범 사례&quot; eCatalog 뷰어 사전 설정이 포함되어 있습니다. 이러한 사전 설정 중 하나를 선택하여 eCatalog를 표시할 수 있습니다. 관리자는 고유한 eCatalog 뷰어 사전 설정을 만들 수도 있습니다.

eCatalog 뷰어 사전 설정을 만들려면 전역 탐색 모음에서 **[!UICONTROL 설정]**&#x200B;을 선택한 다음 **[!UICONTROL 뷰어 사전 설정]**&#x200B;을 선택하십시오. **[!UICONTROL 추가]**&#x200B;를 선택하고 플랫폼을 선택한 다음 **[!UICONTROL 전자 카탈로그]** > **[!UICONTROL 뷰어]**&#x200B;를 선택합니다.

[eCatalog 뷰어 사전 설정 설정 설정](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets)을 참조하세요.

## 5. eCatalog 뷰어에서 eCatalog 미리 보기

eCatalog 뷰어 사전 설정은 eCatalog 뷰어의 스타일과 동작을 결정합니다.

eCatalog 뷰어 사전 설정에서 eCatalog를 표시하는 방법을 알아보려면 [찾아보기] 패널에서 eCatalog를 선택한 다음 **[!UICONTROL 미리 보기]**&#x200B;를 선택하십시오. [미리 보기] 화면이 기본 뷰어에서 열립니다.

방향, 색상 구성표, 페이지 변경 컨트롤의 모양, 페이지를 넘길 때 페이지의 모양 등을 확인합니다. 

[eCatalog 뷰어에서 전자 카탈로그 미리 보기](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer)를 참조하십시오.

## 6. Publish eCatalog 및 관련 PDF

eCatalog와 관련 PDF을 게시하면 웹 사이트 및 애플리케이션에 전달될 수 있도록 이 카탈로그가 Dynamic Media 이미지 서버에 배치됩니다. 게시 프로세스의 일부로 Adobe Dynamic Media Classic이 eCatalog에 대한 URL 문자열을 활성화합니다. 이 URL을 사용하여 Dynamic Media 이미지 서버에서 웹 사이트 또는 애플리케이션으로 eCatalog를 호출합니다.

찾아보기 패널에서 게시할 eCatalog 및 PDF을 표시한 후 전역 탐색 막대에서 Publish 버튼을 선택하여 게시를 시작합니다. 게시 페이지에서 **[!UICONTROL Publish 제출]**&#x200B;을 선택합니다.

[Publish eCatalogs 및 관련 PDF](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs)를 참조하십시오.

## 7. 웹 페이지에 eCatalog 연결

Adobe Dynamic Media Classic은 사용자가 Dynamic Media 이미지 서버에 게시할 때 eCatalog를 표시하는 데 필요한 URL 콜아웃 문자열을 활성화합니다. 패널에서 URL을 선택하여 미리보기 화면 및 찾아보기 패널(세부 사항 보기)에서 이 URL 문자열을 복사할 수 있습니다. URL 문자열을 복사하면 웹 사이트 및 애플리케이션에서 사용할 수 있습니다.

IT 팀과 함께 eCatalog에 대한 링크를 웹 페이지의 적절한 위치에 배치합니다. 사용자가 링크를 선택하면 eCatalog 뷰어가 나타나고 사용자는 eCatalog를 검색할 수 있습니다.

[웹 페이지에 전자 카탈로그 연결](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page)을 참조하세요.
