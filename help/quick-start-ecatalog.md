---
title: '"빠른 시작:eCatalogs"'
seo-title: '"빠른 시작:eCatalogs"'
description: 널
seo-description: eCatalog 기법을 빠르게 익히고 실행하는 데 도움이 되는 eCatalogs 소개 및 빠른 시작
uuid: 1ec41927-3df6-4845-8d9d-bb92cf6dca08
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 781dacd0-ef0c-42b7-92e0-12791994874d
translation-type: tm+mt
source-git-commit: 83b88623b898fdadd1b334b1c12901830c831c5c
workflow-type: tm+mt
source-wordcount: '1450'
ht-degree: 64%

---


# 빠른 시작:eCatalogs{#quick-start-ecatalogs}

eCatalog는 카탈로그, 브로셔, 전단, 제품 설명서 또는 광고 전단과 같은 인쇄물의 디지털 웹 버전입니다. eCatalog는 웹 사이트의 eCatalog 뷰어에 표시됩니다. 이 뷰어는 인쇄물을 읽는 경험을 시뮬레이션합니다. eCatalog에 대해 선택하는 설정에 따라 뷰어에서 다음을 수행할 수 있습니다.

* 카탈로그에서 키워드 또는 키워드를 검색합니다. 검색 결과는 카탈로그 왼쪽의 검색 패널에 축소판 목록으로 표시됩니다. 클릭할 수 있는 각 축소판은 강조 표시된 검색어가 있는 카탈로그 스프레드를 나타냅니다.

* 소셜 미디어를 통해 카탈로그 공유카탈로그를 다운로드하여 오프라인에서 보기즐겨찾기를 사용하여 빠르게 돌아갈 항목을 표시하거나 카탈로그를 인쇄합니다.
* 목차 또는 페이지 그리드 보기를 사용하여 카탈로그를 탐색합니다.페이지의 가운데 가장자리를 클릭하여 페이지 앞 또는 뒤로 이동시킬 수 있습니다.
* 확대, 축소 및 패닝하여 페이지의 항목을 검사합니다.
* 포인터를 페이지 영역(이미지 맵이라고 함) 위로 이동하여 항목에 대한 정보가 포함된 팝업 창을 표시합니다.
* 페이지 영역을 클릭하여 항목에 대한 자세한 정보가 포함된 새 웹 페이지를 엽니다.
* 스티커 메모를 써서 eCatalog 페이지에 첨부합니다.
* 이미지 맵 아이콘을 눌러 관련 웹 페이지나 컨텍스트 내 정보 패널을 시작합니다.
* 손가락을 모아 확대, 살짝 밀어 페이지 넘김 등의 제스처 상호 작용을 사용합니다.
* 키워드로 항목을 검색합니다.

![사용자에게 표시되는 eCatalog A) 전자 카탈로그 열기 페이지. B)eCatalog turned to page 2.](/help/assets/ec_cat_viewer_popup.png)

eCatalog를 만들려면 일반적으로 Adobe® Acrobat®이나 다른 인쇄 프로그램에서 만든 고해상도 PDF 파일을 사용하지만 이미지 파일에서 eCatalog를 만들 수도 있습니다.

eCatalog를 만드는 과정에서 페이지나 페이지 스프레드를 선택한 순서대로 정렬할 수 있습니다. 단일 페이지, 양면 페이지 스프레드 또는 복수 페이지 스프레드를 사용할 것인지를 선언할 수도 있습니다. 예를 들어 뷰어가 페이지의 한 영역을 클릭하여 웹 사이트에서 새 페이지를 열 수 있도록 페이지 영역에 대해 이미지 맵을 만들 수 있습니다. eCatalog 화면 내의 [정보 패널] 설정을 사용하여 표시되는 롤오버 텍스트를 관리할 수 있습니다. 100개보다 많은 구성 선택 사항 중에서 선택하여 eCatalog 뷰어를 구성할 수도 있습니다. 특정 타겟 사용자에 맞게 뷰어의 기능과 모양을 조정할 수 있습니다.

>[!NOTE]
>
>AEM Dynamic Media - Scene7 모드 사용자이고 eCatalogs를 사용하려면 CRXDE Lite에서 `pdfbrochure` 값을 편집해야 합니다. 이렇게 하려면 AEM에서 **[!UICONTROL 도구 > 일반 > CRXDE Lite을 클릭합니다]**. 왼쪽 패널 탐색 트리에서 로 이동합니다 `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`.
>
>오른쪽 아래 창의 **[!UICONTROL 속성]** 탭에서 `jobParam` 행을 선택합니다. 에서 `pdfbrochure` 로 값을 `false` 설정합니다 `true`. As in `pdfbrochure=true`
>
>CRXDE Lite 페이지의 왼쪽 위 모서리에서 모두 **[!UICONTROL 저장을 클릭합니다]**.
>
>이제 Dynamic Media Classic에서 eCatalogs를 작성할 수 있습니다.

**빠른 시작**

이 eCatalog 빠른 시작은 eCatalog를 빨리 시작하고 실행하는 데 도움이 됩니다. 1-7 단계를 수행하십시오. 각 단계 뒤에는 자세한 정보를 확인할 수 있는 항목 제목의 상호 참조가 있습니다.

**1. PDF 파일 업로드**

일반적으로 Adobe PDF 파일이 eCatalog의 소스입니다. 원래 인쇄용이기 때문에 PDF 파일에는 대체로 CMYK 이미지가 포함되어 있습니다. Dynamic Media Classic에서는 이러한 이미지를 감지하고 표준 CMYK 색상 프로파일을 사용하여 변환합니다. 그러나 사용자 지정 색상 프로필을 업로드하고 사용해야 할 수도 있습니다.

글로벌 탐색 막대에서 업로드를 클릭하여 eCatalog용 PDF 파일 또는 이미지를 업로드합니다. 데스크톱에서 또는 FTP를 통해 파일을 업로드할 수 있습니다. 100MB보다 큰 파일이나 많은 파일을 업로드하는 경우 FTP를 사용하는 것이 좋습니다.

[업로드] 화면의 [PDF 선택 사항] 아래에는 적절한 해상도와 올바른 색상 공간으로 PDF 파일을 업로드하기 위한 선택 사항이 제공됩니다. 인치당 150픽셀 해상도를 사용하는 것이 좋습니다. [eCatalog 자동 생성] 선택 사항을 선택하면 PDF 파일을 업로드할 때 eCatalog를 만들 수 있습니다.

[PDF 파일 업로드](uploading-pdf-files.md#uploading_the_pdf_files)를 참조하십시오.

**2. eCatalog 만들기**

찾아보기 패널에서 PDF 또는 이미지 파일을 선택하고 [작성] 단추를 클릭한 다음 [eCatalog]를 선택하여 eCatalog를 만듭니다. [eCatalog] 화면이 열립니다.

[주문 페이지] 탭에서 [레이아웃] 단추([1단계 위로], [2단계 위로] 또는 [사용자 지정])를 선택하여 단일, 양면 또는 사용자 지정 페이지 스프레드를 사용할 것인지를 선택합니다. 페이지 또는 스프레드를 끌거나 큰 eCatalog의 경우 [이동] 메뉴에서 페이지 이름을 선택하여 페이지 또는 스프레드를 다시 정렬할 수 있습니다.

페이지를 추가하려면 자산 라이브러리에서 폴더를 선택하고 PDF 또는 이미지 파일을 [주문 페이지] 화면으로 드래그합니다. 기본 페이지 번호 대신 사용자 지정 페이지 이름을 제공하거나 많은 페이지 이름을 가져올 수 있습니다.

[ **[!UICONTROL 저장]**]을 클릭하고 eCatalog의 이름을 입력한 다음 저장할 Dynamic Media Classic 폴더를 선택한 다음 [ **[!UICONTROL 저장]을 클릭합니다]**. Each time you change the page order or edit your eCatalog, save your changes by clicking **[!UICONTROL Save]**.

[eCatalog 만들기](creating-ecatalog.md)를 참조하십시오.

**3. 이미지 맵 만들기**

이미지 맵은 eCatalog 페이지에 다른 차원을 추가합니다. 이미지 맵은 항목에 대한 자세한 정보를 제공하는 페이지의 한 영역입니다. 뷰어가 포인터를 이미지 맵 위로 롤오버하면 항목에 대한 설명이 표시됩니다. 이미지 맵을 클릭하면 새 웹 페이지를 여는 외부 참조가 활성화되고, 이 페이지에서 항목에 대한 자세한 정보를 확인할 수 있습니다.

이미지 맵을 만들려면 eCatalog 화면을 엽니다. Then go to the **[!UICONTROL Map Pages]** tab of the eCatalog screen, and draw the map with the Rectangle Image Map tool or Polygon Image Map tool. [패닝] 도구 로 맵 테두리를 끌어 이미지 맵의 위치와 크기를 조정할 수 있습니다.

이미지 맵을 그린 후 [이미지 맵]을 클릭할 때 이동하려는 URL 주소를 입력합니다. 포인터를 이미지 맵 위로 이동할 때 표시되는 롤오버 텍스트를 입력할 수도 있습니다.

[eCatalog 이미지 맵 만들기](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps)를 참조하십시오.

[eCatalog에 리치 미디어를 임베드하기 위해 이미지 맵 사용](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog)을 참조하십시오.

eCatalog 화면의 [정보 패널] 설정을 사용하여 이미지 맵 텍스트를 설정하고 관리할 수 있습니다.

[정보 패널 컨텐츠 관리](info-panel-content.md#managing-info-panel-content)를 참조하십시오.

**4. eCatalog 뷰어 사전 설정 지정**

최종 사용자는 eCatalog 뷰어에서 eCatalog를 봅니다. 관리자는 eCatalog 뷰어를 구성할 수 있습니다. 윤곽 색상을 변경하고 새 &quot;스킨&quot;을 선택하여 eCatalog를 브랜딩할 수 있습니다. Dynamic Media Classic에는 여러 가지 &quot;우수 사례&quot; eCatalog 뷰어 사전 설정이 포함되어 있습니다. 이러한 사전 설정 중 하나를 선택하여 eCatalog를 표시할 수 있습니다. 관리자는 고유한 eCatalog 뷰어 사전 설정을 만들 수도 있습니다.

eCatalog 뷰어 사전 설정을 만들려면 전역 탐색 막대에서 [ **[!UICONTROL 설정]을 클릭하고 [뷰어 사전 설정]** ]을 **[!UICONTROL 선택합니다]**. Then click **[!UICONTROL Add]**, choose a platform, then click **[!UICONTROL eCatalog > Viewer]**.

[eCatalog 뷰어 사전 설정 지정](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets)을 참조하십시오.

**5. eCatalog 뷰어에서 eCatalog 미리 보기**

eCatalog 뷰어 사전 설정은 eCatalog 뷰어의 스타일과 동작을 결정합니다.

To find out how eCatalog Viewer Presets display your eCatalog, select your eCatalog in the Browse Panel and click **[!UICONTROL Preview]**. [미리 보기] 화면이 기본 뷰어에서 열립니다.

방향, 색상 구성표, 페이지 변경 컨트롤의 모양, 페이지를 넘길 때 페이지의 모양 등을 확인합니다. 

[eCatalog 뷰어에서 eCatalog 미리 보기](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer)를 참조하십시오.

**6. eCatalog 및 관련 PDF 게시**

eCatalog 및 관련 PDF를 게시하면 웹 사이트 및 애플리케이션에 전달할 수 있도록 Dynamic Media 이미지 서버에 해당 eCatalog를 배치할 수 있습니다. 게시 프로세스의 일부로 Dynamic Media Classic은 eCatalog에 대한 URL 문자열을 활성화합니다. 이 URL을 사용하여 다이내믹 미디어 이미지 서버에서 웹 사이트 또는 응용 프로그램으로 eCatalog를 호출합니다.

검색 패널에서 eCatalog 및 PDF를 게시로 표시한 후 글로벌 탐색 막대에서 [게시] 단추를 선택하여 게시를 시작합니다. On the Publish screen, click **[!UICONTROL Start Publish]**.

e카탈로그 [및 관련 PDF 게시를 참조하십시오](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs).

**7. eCatalog를 웹 페이지에 연결**

Dynamic Media Classic에서는 eCatalog를 Dynamic Media 이미지 서버에 게시할 때 eCatalog를 표시하는 데 필요한 URL 콜아웃 문자열을 활성화합니다. 패널에서 URL을 선택하면 [미리 보기] 화면과 찾아보기 패널(세부 사항 보기)에서 이 URL 문자열을 복사할 수 있습니다. 복사한 URL 문자열은 웹 사이트와 애플리케이션에서 사용할 수 있습니다.

IT 팀과 협력하여 eCatalog 링크를 웹 사이트의 적절한 위치에 배치합니다. 사용자가 링크를 클릭하면 eCatalog 뷰어가 나타나고 사용자가 eCatalog를 찾을 수 있습니다. 

[eCatalog를 웹 페이지에 연결](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page)을 참조하십시오.
