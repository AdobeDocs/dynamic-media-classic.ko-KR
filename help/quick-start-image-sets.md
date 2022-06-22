---
title: '"빠른 시작: 이미지 집합"'
description: Adobe Dynamic Media Classic의 이미지 세트 기술을 사용하여 신속하게 시작하고 실행할 수 있는 이미지 세트 소개 및 빠른 시작 .
uuid: daf17d13-9c06-41f0-8fc5-2e56d460d341
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: 612a425f-2840-46c4-8e5a-c0bc5f738f4e
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 280e7201-84d6-46b1-94bb-0499beca2992
source-git-commit: d5293a2983e1105c65005634e7eb4147e17e8328
workflow-type: tm+mt
source-wordcount: '675'
ht-degree: 21%

---

# 빠른 시작: 이미지 집합{#quick-start-image-sets}

Adobe Dynamic Media Classic 이미지 세트는 사용자에게 통합된 보기 환경을 제공합니다. 동적 이미지 집합 뷰어에서는 사용자가 썸네일 이미지를 클릭하여 항목의 여러 보기를 확인할 수 있습니다. 이미지 세트를 사용하면 항목의 대체 고해상도 보기를 표시할 수 있습니다.

이미지 집합 뷰어에서는 이미지를 자세히 검사하기 위해 확대/축소 도구를 제공합니다. 필요한 경우 유도된 확대/축소 타겟과 이미지 맵을 이미지 집합에 포함할 수 있습니다. 이미지 집합은 보다 조화롭고 친근한 보기 환경을 제공합니다.

자세한 내용은 [이미지 및 스핀 세트: Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS) 교육 비디오.

이미지 세트를 생성할 때 Adobe은 다음 우수 사례를 권장하고 다음 제한을 적용합니다.

| 이미지 집합 제한 유형 | 우수 사례 | 구현된 제한 | 제한 변경: 2022년 12월 31일 |
| --- | --- | --- | --- |
| 세트당 중복 자산 수 | 중복 없음 | 100년 | 20년 |
| 설정당 최대 이미지 수 | 세트당 5-10개 이미지 | 1000 |

다음 이미지 세트 빠른 시작 은 Adobe Dynamic Media Classic의 이미지 세트 기술을 사용하여 빠르게 시작하고 실행할 수 있도록 설계되었습니다.

## 1. 여러 보기 및 견본에 대한 기본 이미지를 업로드합니다

먼저 이미지 집합에 사용할 이미지를 업로드합니다. 사용자가 이미지 세트 뷰어에서 이미지를 확대할 수 있으므로 이미지를 선택할 때 이 기능을 고려해야 합니다. 이미지의 크기가 가장 큰 2000픽셀 이상인지 확인하십시오. Adobe Dynamic Media Classic에서는 많은 이미지 파일 형식을 지원하지만, 무손실 TIFF, PNG 및 EPS 이미지가 좋습니다.

전역 탐색 모음에서 를 선택합니다 **[!UICONTROL 업로드]** 컴퓨터의 파일을 Adobe Dynamic Media Classic의 폴더로 업로드합니다.

자세한 내용은 [업로드할 이미지 세트 자산 준비](preparing-image-set-assets-upload.md#preparing-image-set-assets-for-upload) 및 [파일 업로드](uploading-files.md#uploading-your-files).

## 2. 이미지 세트 만들기

이미지 세트에서 사용자는 이미지 세트 뷰어에서 축소판 이미지를 선택하여 다른 측면 또는 각도에서 이미지를 확인합니다.

이미지 세트를 만들려면 전역 탐색 막대에서 을 선택합니다 **[!UICONTROL 빌드]**, 그런 다음 **[!UICONTROL 이미지 세트]**. 이미지 세트 창에서 이미지를 페이지로 드래그하여 이미지 세트를 작성합니다. 필요한 경우 이미지를 구성, 추가, 삭제합니다.

자세한 내용은 [이미지 세트 만들기](creating-image-set.md#creating-an-image-set).

참조 - [이미지 세트에 확대/축소 대상 및 이미지 맵 포함](/help/including-zoom-targets-image-maps-image-sets.md)

## 3. 필요에 따라 이미지 세트 뷰어 사전 설정을 준비합니다

관리자는 이미지 집합 뷰어 사전 설정을 만들거나 수정할 수 있습니다. Adobe Dynamic Media Classic에는 각 리치 미디어 유형에 대한 기본 뷰어 사전 설정이 포함되어 있습니다. 확대/축소 뷰어 사용: **[!UICONTROL 사용자 지정]** > **[!UICONTROL 이미지]** 또는 **[!UICONTROL 이미지 세트]**/**[!UICONTROL 여러 보기]** 사전 설정을 사용하여 이미지 세트를 볼 수 있습니다.

[애플리케이션 설정] 화면에서 뷰어 사전 설정을 추가하거나 편집합니다.

자세한 내용은 [뷰어 사전 설정 만들기 및 편집](application-setup.md#adding-and-editing-viewer-presets).

## 4. 이미지 세트 미리 보기

찾아보기 패널에서 이미지 세트를 선택한 다음 를 선택합니다 **[!UICONTROL 미리 보기]**. 미리 보기 페이지에서 축소판 아이콘을 선택하여 선택한 뷰어에서 이미지 세트를 검사합니다. [사전 설정] 메뉴에서 다른 뷰어를 선택할 수 있습니다.

자세한 내용은 [자산 미리 보기](previewing-asset.md#previewing-an-asset).

## 5. 이미지 세트 게시

이미지 세트를 게시하면 Adobe Dynamic Media Classic 서버에 배치하고 URL 문자열을 활성화합니다.

>[!NOTE]
>
>이미지 세트를 만들고 저장할 때 **[!UICONTROL 저장 후 게시]**(기본값)를 선택한 경우에는 이 단계가 필요하지 않습니다.

선택 **[!UICONTROL 게시로 표시]** 찾아보기 패널에서 이름 왼쪽에 있는 아이콘 그런 다음 **[!UICONTROL 게시]**. 게시 페이지에서 을 선택합니다 **[!UICONTROL 게시 제출]**.

자세한 내용은 [파일 게시](publishing-files.md#publishing-files).

## 6. 웹 사이트에 이미지 세트 연결

Adobe Dynamic Media Classic은 이미지 세트에 대한 URL 호출을 생성하고 게시 후 활성화합니다. [미리 보기] 화면에서 이러한 URL을 복사할 수 있습니다.

이미지 세트를 선택한 다음 을 선택합니다 **[!UICONTROL 미리 보기]**. 이제 이미지 세트 뷰어 사전 설정을 선택한 다음 를 선택합니다 **[!UICONTROL URL 복사]**.

자세한 내용은 [웹 페이지에 이미지 집합 연결](linking-image-set-web-page.md#linking-an-image-set-to-a-web-page).
