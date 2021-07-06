---
title: '"빠른 시작: 이미지 집합"'
description: 이미지 세트 기술을 사용하여 신속하게 시작하고 실행할 수 있는 이미지 세트 소개 및 빠른 시작 .
uuid: daf17d13-9c06-41f0-8fc5-2e56d460d341
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: 612a425f-2840-46c4-8e5a-c0bc5f738f4e
feature: Dynamic Media Classic,뷰어,이미지 세트
role: User
exl-id: 280e7201-84d6-46b1-94bb-0499beca2992
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 41%

---

# 빠른 시작: 이미지 집합{#quick-start-image-sets}

Dynamic Media Classic 이미지 세트는 사용자에게 통합된 보기 환경을 제공합니다. 동적 이미지 집합 뷰어에서는 사용자가 썸네일 이미지를 클릭하여 항목의 여러 보기를 확인할 수 있습니다. 이미지 세트를 사용하면 항목의 대체 고해상도 보기를 표시할 수 있습니다.

이미지 집합 뷰어에서는 이미지를 자세히 검사하기 위해 확대/축소 도구를 제공합니다. 필요한 경우 유도된 확대/축소 타겟과 이미지 맵을 이미지 집합에 포함할 수 있습니다. 이미지 집합은 보다 조화롭고 친근한 보기 환경을 제공합니다.

이 이미지 세트 빠른 시작은 Dynamic Media Classic의 이미지 세트 기술을 사용하여 빠르게 시작하고 실행하도록 설계되었습니다.

## 1. 여러 보기 및 견본을 위한 마스터 이미지 업로드

먼저 이미지 집합에 사용할 이미지를 업로드합니다. 사용자가 이미지 세트 뷰어에서 이미지를 확대할 수 있으므로 이미지를 선택할 때 이 기능을 고려해야 합니다. 이미지의 크기가 가장 큰 2000픽셀 이상인지 확인하십시오. Dynamic Media Classic에서는 많은 이미지 파일 형식을 지원하지만, 무손실 TIFF, PNG 및 EPS 이미지가 권장됩니다.

전역 탐색 모음에서 **[!UICONTROL 업로드]**&#x200B;를 클릭하여 컴퓨터의 파일을 Dynamic Media Classic의 폴더로 업로드합니다.

[업로드할 이미지 집합 자산 준비](preparing-image-set-assets-upload.md#preparing-image-set-assets-for-upload) 및 [파일 업로드](uploading-files.md#uploading-your-files)를 참조하십시오.

## 2. 이미지 세트 만들기

이미지 집합에서 사용자는 이미지 집합 뷰어의 썸네일 이미지를 클릭하여 이미지를 다른 측면이나 각도에서 표시합니다.

이미지 세트를 만들려면 전역 탐색 막대에서 **[!UICONTROL 빌드]**&#x200B;를 클릭한 다음 **[!UICONTROL 이미지 세트]**&#x200B;를 선택합니다. 이미지 세트 창에서 이미지를 페이지로 드래그하여 이미지 세트를 작성합니다. 필요한 경우 이미지를 구성, 추가, 삭제합니다.

[이미지 집합 만들기](creating-image-set.md#creating-an-image-set)를 참조하십시오.

[이미지 집합에 확대/축소 타겟 및 이미지 맵 포함](including-zoom-targets-image-maps.md#including-zoom-targets-and-image-maps-in-image-sets)을 참조하십시오.

## 3. 필요에 따라 이미지 세트 뷰어 사전 설정 설정

관리자는 이미지 집합 뷰어 사전 설정을 만들거나 수정할 수 있습니다. Dynamic Media Classic에는 각 리치 미디어 유형에 대한 기본 뷰어 사전 설정이 포함되어 있습니다. [확대/축소 뷰어: 사용자 지정] > [이미지] 또는 [이미지 집합/다중 보기] 사전 설정을 사용하여 이미지 집합을 봅니다.

[애플리케이션 설정] 화면에서 뷰어 사전 설정을 추가하거나 편집합니다.

[뷰어 사전 설정 만들기 및 편집](application-setup.md#adding-and-editing-viewer-presets)을 참조하십시오.

## 4. 이미지 세트 미리 보기

찾아보기 패널에서 이미지 세트를 선택한 다음 **[!UICONTROL 미리 보기]**&#x200B;를 클릭합니다. 미리 보기 페이지에서 축소판 아이콘을 클릭하여 선택한 뷰어에서 이미지 세트를 검사합니다. [사전 설정] 메뉴에서 다른 뷰어를 선택할 수 있습니다.

[자산 미리 보기](previewing-asset.md#previewing-an-asset)를 참조하십시오.

## 5. 이미지 세트 게시

이미지 세트를 게시하면 Dynamic Media Classic 서버에 해당 이미지 세트가 배치되고 URL 문자열이 활성화됩니다.

>[!NOTE]
>
>이미지 세트를 만들고 저장할 때 **[!UICONTROL 저장 후 게시]**(기본값)를 선택한 경우에는 이 단계가 필요하지 않습니다.

찾아보기 패널에서 이름 왼쪽에 있는 **[!UICONTROL 게시 표시]** 아이콘을 클릭합니다. 그런 다음 **[!UICONTROL 게시]**&#x200B;를 클릭합니다. 게시 페이지에서 **[!UICONTROL 게시]**&#x200B;를 클릭합니다.

[게시](publishing-files.md#publishing-files)를 참조하십시오.

## 6. 이미지 세트를 웹 사이트에 연결

Dynamic Media Classic은 이미지 세트에 대한 URL 호출을 생성하고 게시 후 활성화합니다. [미리 보기] 화면에서 이러한 URL을 복사할 수 있습니다.

이미지 세트를 선택한 다음 **[!UICONTROL 미리 보기]**&#x200B;를 클릭합니다. 이제 이미지 세트 뷰어 사전 설정을 선택한 다음 **[!UICONTROL URL 복사]**&#x200B;를 클릭합니다.

[이미지 집합을 웹 페이지에 연결](linking-image-set-web-page.md#linking-an-image-set-to-a-web-page)을 참조하십시오.
