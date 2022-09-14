---
title: 이미지 자르기
description: Adobe Dynamic Media Classic에서 이미지를 자르는 방법을 알아봅니다.
uuid: 84f199de-cbfc-4d06-877f-6e9148e82e15
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 99dfa476-4f11-4569-a27e-a76ed7787674
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: aec4c256-f5ed-4307-afec-dec848be95f9
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 35%

---

# 이미지 자르기{#cropping-an-image}

Adobe Dynamic Media Classic에서 이미지를 자를 수 있습니다. 이미지를 원본 상태로 복원할 수 있도록 잘린 이미지에 대한 정보가 시스템에 유지됩니다. 이미지를 자르고 잘린 버전을 새 이름으로 저장할 수도 있습니다.

이미지를 잘라 주위 공백을 제거하거나 이미지의 한 영역을 자를 수 있습니다.

>[!NOTE]
>
>자르면 다음을 선택할 수 있습니다 **[!UICONTROL 다른 이름으로 저장]** 이미지의 잘려진 버전을 다른 이름으로 저장합니다. 다른 이름으로 저장 창에서 **[!UICONTROL 새 기본으로 저장]** 이미지의 두 번째 복사본을 저장하려면 을 클릭합니다. 선택 **[!UICONTROL 기본 추가 보기로 저장]** 따라서 원본과 잘린 버전을 다른 이름으로 저장할 수 있습니다. 선택 **[!UICONTROL 원래 바꾸기]** 이미지를 잘라낸 원본 파일을 삭제하려면 그런 다음 이미지의 이름을 입력하고 을(를) 선택합니다 **[!UICONTROL 제출]**.

## 이미지 주위를 잘라 공백 제거 {#crop-to-remove-white-space-around-an-image}

이미지 가장자리에서 투명 또는 단색 픽셀을 자를 수 있습니다.

1. 이미지를 자르려면 롤오버를 선택합니다 **[!UICONTROL 편집]** 단추를 누른 다음 **[!UICONTROL 자르기]**&#x200B;또는 세부 사항 보기의 찾아보기 패널에 표시하고 **[!UICONTROL 자르기]** 버튼을 클릭합니다.
1. 자르기 편집기 페이지에서 다음 중 하나를 수행합니다.

   * 색상 픽셀을 자르려면 **[!UICONTROL Trim]** > **[!UICONTROL 색상]**. 에서 **[!UICONTROL 색상별 자동 자르기]** 대화 상자에서 **[!UICONTROL 코너]** 메뉴에서 잘라낼 배경색이 있는 모서리를 선택합니다. 그런 다음 **[!UICONTROL 허용치]** 0에서 1까지입니다. 0을 설정하면 이미지 모서리에서 선택한 색상과 정확하게 일치하는 경우에만 픽셀이 잘립니다. 값이 1에 가까워질수록 색상 차이를 더 많이 허용합니다. 선택 **[!UICONTROL 자르기]**.
   * 투명 픽셀을 트리밍하려면 다음 위치로 이동하십시오. **[!UICONTROL Trim]** > **[!UICONTROL 투명]**. 에서 **[!UICONTROL 투명도로 자동 자르기]** 대화 상자에서 0~1의 공차 설정을 입력합니다. 0 설정은 투명 픽셀만 자릅니다. 1에 가까운 숫자를 설정하면 더 투명해집니다. 선택 **[!UICONTROL 자르기]**.

1. 선택 **[!UICONTROL 저장]**.

>[!NOTE]
>
>이미지를 잘라낸 후 원래 상태로 복원하려면 [자르기 편집기] 화면에 이미지를 표시하고 를 선택합니다 **[!UICONTROL 재설정]**.

## 자를 영역 선택 {#select-an-area-to-crop}

1. 이미지를 자르려면 롤오버를 선택합니다 **[!UICONTROL 편집]** 버튼을 클릭하고 **[!UICONTROL 자르기]**&#x200B;또는 세부 사항 보기의 찾아보기 패널에 표시하고 를 선택합니다 **[!UICONTROL 자르기]**.

1. [자르기 편집기] 창에서 자르지 않을 이미지 부분을 자르기 상자에 배치합니다. 상자 내에 나타나는 것은 선택 후 남아 있는 것입니다 **[!UICONTROL 저장]** 이미지를 자릅니다.
1. 자르기 영역을 조정하려면 다음 중 하나를 수행합니다.

   * 상자 측면이나 모서리를 드래그합니다. Shift 키를 누른 상태로 끌어 크기를 변경하지만 자르기 상자의 종횡비(모양)는 유지합니다.
   * [크기] 상자에 픽셀 측정값을 입력합니다.
   * 자르기 상자를 끌어서 이동합니다. 포인터를 상자 경계 안으로 이동합니다. 십자형 화살표가 표시되면 상자를 이미지의 새 위치로 드래그합니다.

1. 선택 **[!UICONTROL 저장]**.

>[!NOTE]
>
>이미지를 잘라낸 후 원래 상태로 복원하려면 [자르기 편집기] 화면에 이미지를 표시하고 를 선택합니다 **[!UICONTROL 재설정]**.

>[!MORELIKETHIS]
>
>* [업로드 시 이미지 편집 옵션](image-editing-options-upload.md#image-editing-options-at-upload)
>* [PDF 파일에서 공백 자르기](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [PDF 페이지 양쪽에서 자르기](pdfs.md#cropping_from_the_sides_of_pdf_pages)

