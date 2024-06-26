---
title: "빠른 시작: 이미지 집합"
description: Adobe Dynamic Media Classic의 이미지 세트 기술을 빠르게 시작하고 실행하는 데 도움이 되는 이미지 세트에 대한 소개 및 빠른 시작입니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 280e7201-84d6-46b1-94bb-0499beca2992
topic: Content Management
level: Beginner
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 10%

---

# 빠른 시작: 이미지 집합{#quick-start-image-sets}

Adobe Dynamic Media Classic 이미지 세트는 사용자에게 통합된 보기 환경을 제공합니다. 동적 이미지 세트 뷰어에서 사용자는 썸네일 이미지를 선택하여 항목의 다양한 보기를 볼 수 있습니다. 이미지 세트 를 사용하면 항목의 대체 고해상도 보기를 표시할 수 있습니다.

이미지 집합 뷰어에서는 이미지를 자세히 검사하기 위해 확대/축소 도구를 제공합니다. 원하는 경우 안내식 확대/축소 대상 및 이미지 맵 을 이미지 세트의 일부로 만들 수 있습니다. 이미지 집합은 보다 조화롭고 친근한 보기 환경을 제공합니다.

다음을 참조하십시오 [이미지 및 스핀 세트: Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS) 교육 비디오입니다.

이미지 집합을 만들 때 Adobe은 다음 모범 사례를 권장하며 다음 제한을 적용합니다.

| 제한 유형 | 우수 사례 | 제한 적용됨 |
| --- | --- | --- |
| 세트당 중복 에셋 수 | 중복 항목 없음 | 20‡ |
| 세트당 최대 이미지 수 | 세트당 5-10개 이미지 | 1000 |

‡ 우수 사례는 집합 내에 중복 에셋을 두지 않는 것입니다. 단일 자산에 대한 중복 횟수는 20회로 제한됩니다. 해당 에셋에 대해 다른 중복을 추가하면 해당 세트 내에서 요청에 오류가 발생하거나 중복을 무시합니다.

참조: [Dynamic Media 제한 사항](/help/using/limitations.md).

다음 이미지 세트 빠른 시작은 Adobe Dynamic Media Classic의 이미지 세트 기술을 사용하여 빠르게 시작하고 실행할 수 있도록 설계되었습니다.

## 1. 여러 보기 및 견본에 대한 기본 이미지 업로드

먼저 이미지 집합에 사용할 이미지를 업로드합니다. 사용자는 이미지 세트 뷰어에서 이미지를 확대할 수 있으므로 이미지를 선택할 때 이 기능을 고려해야 합니다. 이미지의 크기가 2000픽셀 이상인지 확인하십시오. Adobe Dynamic Media Classic은 다양한 이미지 파일 형식을 지원하지만 무손실 TIFF, PNG 및 EPS 이미지가 권장됩니다.

전역 탐색 모음에서 를 선택합니다. **[!UICONTROL 업로드]** 컴퓨터에서 Adobe Dynamic Media Classic의 폴더로 파일을 업로드합니다.

다음을 참조하십시오 [업로드할 이미지 세트 자산 준비](preparing-image-set-assets-upload.md#preparing-image-set-assets-for-upload) 및 [파일 업로드](uploading-files.md#uploading-your-files).

## 2. 이미지 집합 만들기

이미지 세트에서 사용자는 이미지 세트 뷰어에서 썸네일 이미지를 선택하여 다른 측면 또는 각도의 이미지를 봅니다.

이미지 집합을 만들려면 전역 탐색 모음에서 **[!UICONTROL 빌드]**&#x200B;을 선택한 다음 을 선택합니다. **[!UICONTROL 이미지 집합]**. 이미지 세트 창에서 이미지를 페이지로 드래그하여 이미지 세트를 작성합니다. 필요한 경우 이미지를 구성, 추가, 삭제합니다.

다음을 참조하십시오 [이미지 집합 만들기](creating-image-set.md#creating-an-image-set).

참조: [이미지 집합에 확대/축소 대상 및 이미지 맵 포함](/help/using/including-zoom-targets-image-maps-image-sets.md)

## 3. 필요에 따라 이미지 세트 뷰어 사전 설정 준비

관리자는 이미지 집합 뷰어 사전 설정을 만들거나 수정할 수 있습니다. Adobe Dynamic Media Classic에는 각 리치 미디어 유형에 대한 기본 뷰어 사전 설정이 포함되어 있습니다. 확대/축소 뷰어 사용: **[!UICONTROL 사용자 정의]** > **[!UICONTROL 이미지]** 또는 **[!UICONTROL 이미지 집합]**/**[!UICONTROL 여러 보기]** 이미지 집합을 보는 사전 설정입니다.

응용 프로그램 설정 화면에서 뷰어 사전 설정을 추가하거나 편집할 수 있습니다.

다음을 참조하십시오 [뷰어 사전 설정 만들기 및 편집](application-setup.md#adding-and-editing-viewer-presets).

## 4. 이미지 집합 미리 보기

[찾아보기] 패널에서 [이미지 세트]를 선택한 다음 를 선택합니다 **[!UICONTROL 미리 보기]**. 미리 보기 페이지에서 썸네일 아이콘을 선택하여 선택한 뷰어에서 이미지 세트를 검사합니다. [사전 설정] 메뉴에서 다른 뷰어를 선택할 수 있습니다.

다음을 참조하십시오 [에셋 미리보기](previewing-asset.md#previewing-an-asset).

## 5. 이미지 집합 게시

이미지 집합을 게시하면 Adobe Dynamic Media Classic 서버에 표시되고 URL 문자열이 활성화됩니다.

>[!NOTE]
>
>을(를) 선택한 경우 이 단계는 필요하지 않습니다. **[!UICONTROL 저장 후 게시]** (기본값) 이미지 세트를 생성하고 저장할 때 를 선택합니다.

선택 **[!UICONTROL 게시로 표시]** [찾아보기] 패널에서 이름 왼쪽에 있는 아이콘. 그런 다음 을 선택합니다 **[!UICONTROL 게시]**. 게시 페이지에서 를 선택합니다. **[!UICONTROL 게시 제출]**.

다음을 참조하십시오 [파일 게시](publishing-files.md#publishing-files).

## 6. 웹 사이트에 이미지 세트 연결

Adobe Dynamic Media Classic은 이미지 세트에 대한 URL 호출을 생성하고 게시한 후 활성화합니다. [미리 보기] 화면에서 이러한 URL을 복사할 수 있습니다.

이미지 세트를 선택한 다음 를 선택합니다. **[!UICONTROL 미리 보기]**. 이제 이미지 집합 뷰어 사전 설정을 선택한 다음 **[!UICONTROL URL 복사]** 단추를 클릭합니다.

다음을 참조하십시오 [웹 페이지에 이미지 집합 연결](linking-image-set-web-page.md#linking-an-image-set-to-a-web-page).
