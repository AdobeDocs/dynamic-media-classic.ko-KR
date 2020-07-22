---
title: 이미지 자르기
seo-title: 이미지 자르기
description: 널
seo-description: 이미지를 자르는 방법을 알아봅니다.
uuid: 84f199de-cbfc-4d06-877f-6e9148e82e15
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 99dfa476-4f11-4569-a27e-a76ed7787674
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 86%

---


# 이미지 자르기{#cropping-an-image}

Dynamic Media Classic에서 이미지를 자를 수 있습니다. 이미지를 원본 상태로 복원할 수 있도록 잘린 이미지에 대한 정보가 시스템에 유지됩니다. 이미지를 자르고 잘린 버전을 새 이름으로 저장할 수도 있습니다.

이미지를 잘라 주위 공백을 제거하거나 이미지의 한 영역을 자를 수 있습니다.

>[!NOTE]
>
>자른 후 [다른 이름으로 저장] 단추를 클릭하여 이미지의 잘린 버전을 다른 이름으로 저장할 수 있습니다. [다른 이름으로 저장] 창에서 [새 마스터로 저장]을 선택하여 이미지의 두 번째 복사본을 저장합니다. 원본과 잘린 버전을 다른 이름으로 저장하려면 [마스터 추가 보기로 저장]을 선택합니다. 이미지를 자른 원본 파일을 삭제하려면 [원본 바꾸기]를 선택합니다. 그런 다음 이미지 이름을 입력하고 [전송] 단추를 선택합니다.

## 이미지 주위를 잘라 공백 제거 {#crop-to-remove-white-space-around-an-image}

이미지 가장자리에서 투명 또는 단색 픽셀을 자를 수 있습니다.

1. 이미지를 자르려면 롤오버 [편집] 단추를 클릭하고 [자르기]를 선택하거나 [세부 사항 보기]의 찾아보기 패널에 표시하고 [자르기] 단추 를 클릭합니다. [자르기 편집기] 화면이 열립니다.
1. 다음 중 하나를 수행하십시오.

   * 색상 픽셀을 트림하려면 [트림] 메뉴를 선택한 다음 [색상]을 선택합니다. [색상별 자동 자르기] 대화 상자가 나타납니다. [모서리] 메뉴를 선택한 다음 자를 배경색이 있는 모서리를 선택합니다. 0에서 1 사이의 허용 오차 설정을 입력합니다. 0을 설정하면 이미지 모서리에서 선택한 색상과 정확하게 일치하는 경우에만 픽셀이 잘립니다. 값이 1에 가까워질수록 색상 차이를 더 많이 허용합니다. [자르기] 단추를 선택합니다.
   * 투명 픽셀을 트림하려면 [트림] 메뉴를 선택한 다음 [투명]을 선택합니다. [투명도별 자동 자르기] 대화 상자가 나타납니다. 0에서 1 사이의 허용 오차 설정을 입력합니다. 0을 설정하면 완전 투명인 경우에만 픽셀이 잘립니다. 1에 가까운 숫자를 설정하면 더 투명해집니다. [자르기] 단추를 선택합니다.

1. **[저장]**&#x200B;을 클릭합니다.

>[!NOTE]
>
>이미지를 자른 후 원래 상태로 복원하려면 [자르기 편집기] 화면에 이미지를 표시하고 [재설정] 단추를 선택합니다.

## 자를 영역 선택 {#select-an-area-to-crop}

1. To crop an image, click its rollover Edit button and choose **Crop**, or display it in the Browse Panel in Detail view and click **Crop**.

1. [자르기 편집기] 창에서 자르기 상자에 자르기를 원하지 않는 이미지 부분을 배치합니다. What appears inside the box remains when you click **Save** and crop the image.
1. 자르기 영역을 조정하려면 다음 중 하나를 수행합니다.

   * 상자 측면이나 모서리를 드래그합니다. Shift 키를 누른 상태로 끌어 크기를 변경하지만 자르기 상자의 종횡비(모양)는 유지합니다.
   * [크기] 상자에 픽셀 측정값을 입력합니다.
   * 자르기 상자를 끌어서 이동합니다. 포인터를 상자 경계 안으로 이동합니다. 십자형 화살표가 표시되면 상자를 이미지의 새 위치로 드래그합니다.

1. **[저장]**&#x200B;을 클릭합니다.

>[!NOTE]
>
>이미지를 자른 후 원래 상태로 복원하려면 [자르기 편집기] 화면에 이미지를 표시하고 [재설정] 단추를 선택합니다.

>[!MORELIKETHIS]
>
>* [업로드 시 이미지 편집 선택 사항](image-editing-options-upload.md#image-editing-options-at-upload)
>* [PDF 파일에서 공백 자르기](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [PDF 페이지 측면에서 자르기](pdfs.md#cropping_from_the_sides_of_pdf_pages)

