---
title: 유도된 확대/축소의 확대/축소 타겟 만들기
seo-title: 유도된 확대/축소의 확대/축소 타겟 만들기
description: 널
seo-description: 안내 확대/축소에 대한 확대/축소 타겟을 만드는 방법을 알아봅니다.
uuid: 501ea37b-adc5-4290-87eb-52a3501e5d26
contentOwner: 관리
content-type: 참조
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: e7b4673c-8681-4741-912e-9a31cf106449
translation-type: tm+mt
source-git-commit: 6ff0141d1e8e96278b95f61c00602780984aaf67

---


# 유도된 확대/축소의 확대/축소 타겟 만들기{#creating-zoom-targets-for-guided-zoom}

확대/축소 타겟은 뷰어를 이미지의 특정 부분으로 유도합니다. 자유형 확대/축소뿐 아니라 뷰어가 확대/축소 타겟 썸네일을 클릭하여 주의해야 할 이미지 부분을 확대/축소할 수도 있습니다. 확대/축소 타겟을 사용하여 이미지의 매력적인 부분이나 흥미로운 부분을 강조 표시할 수 있습니다.

![Creating zoom targets for Guided Zoom](/help/assets/zo_guided_zoom.png)

## 확대/축소 타겟 정보 {#about-zoom-targets}

확대/축소 타겟의 최대 확대/축소 비율은 100%입니다. 다음 표와 같이 최소 확대/축소 비율은 뷰어 크기 및 이미지 크기의 조합을 기반으로 합니다.

| 이미지 크기 | 뷰어 크기 | 확대/축소 비율 |
|--- |--- |--- |
| 큼 | 더 작음 | 더 작은 최소값 |
| 작음 | 더 큼 | 더 큰 최소값 |

웹 페이지에서 사용되는 크기와 일치하도록 확대/축소 뷰어의 크기를 변경할 수 있습니다. 이 설정을 영구적으로 변경하려면 관리자는 [설정] 화면에서 뷰어 크기를 변경할 수 있습니다. [확대/축소 뷰어 사전 설정 지정](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets)을 참조하십시오.

## 확대/축소 타겟 만들기 및 편집 {#creating-and-editing-zoom-targets}

[확대/축소 타겟 편집기] 화면에서 확대/축소 타겟을 만들고 편집합니다. 이 화면을 열려면 이미지를 선택하고 다음 중 하나를 수행합니다.

* Click the rollover **[!UICONTROL Edit]** button and choose Zoom Targets.
* In the Browse Panel, display the image in **[!UICONTROL Detail View]**, then click **[!UICONTROL Zoom Targets]**.

On the Zoom Target Editor screen, click **[!UICONTROL Select Target]** button (arrow) to select a target before changing its size or position. Click **[!UICONTROL Add Targets]** (rectangle) to create a zoom target on the image. [확대/축소 타겟 편집기] 화면에서는 확대/축소 타겟을 삭제 및 복사하고 이름을 지정하는 도구도 제공합니다.

### 확대/축소 타겟 만들기 {#creating-a-zoom-target}

확대/축소 타겟을 만들려면 [확대/축소 타겟 편집기] 화면을 열고 다음 단계를 수행합니다.

1. Click **[!UICONTROL Add Targets]** (rectangle), move the pointer over the image, and click where you want to the zoom target to be.

   확대/축소 타겟의 썸네일 이미지가 화면 오른쪽 패널에 표시됩니다.

1. Click **[!UICONTROL Select Target]** (arrow), click to select the zoom target you created, and adjust the size and position of the target.

   * **크기**&#x200B;조정확대/축소 대상의 모서리 위로 포인터를 이동하고 드래그하여 대상을 확대하거나 축소할 수 있습니다.

   * **위치**&#x200B;확대/축소 대상 위로 포인터를 이동하고 다른 위치로 드래그합니다.

1. [이름] 상자에 확대/축소 타겟의 이름을 입력합니다.

   >[!NOTE]
   >
   >[이름] 상자에 입력한 내용은 이름 이상의 의미가 있습니다. 사용자가 포인터를 확대/축소 타겟 위로 이동하면 [이름] 상자에 입력한 내용이 표시됩니다. 사용자가 확대/축소할 수 있는 타겟을 알 수 있도록 [이름] 상자에 확대/축소 타겟에 대한 간단한 설명을 입력합니다.

1. 선택적으로, [사용자 데이터] 필드에 사용자 데이터를 입력합니다. 이 필드는 웹 사이트 디자이너가 확대/축소 타겟에 정보를 추가하는 데 사용됩니다.
1. Click **[!UICONTROL Save]**.

   확대/축소 타겟의 좌표와 확대/축소 수준이 저장됩니다. 확대/축소 타겟의 썸네일이 입력한 이름과 함께 화면 오른쪽에 표시됩니다.

>[!NOTE]
>
>확대/축소 뷰어에서 확대/축소 타겟이 표시되는 모양을 확인하려면 [확대/축소 타겟 편집기] 화면에서 [미리 보기] 단추를 클릭하고 [미리 보기] 화면에서 확대/축소 뷰어를 선택합니다. 이 화면에 대한 자세한 내용은 [다른 확대/축소 뷰어에서 이미지 미리 보기](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers)를 참조하십시오.

### 확대/축소 타겟 편집 {#editing-zoom-targets}

[확대/축소 타겟 편집기] 화면에서 다음 기술을 사용하여 확대/축소 타겟을 편집합니다.

* **위치**&#x200B;변경 대상 선택 단추(화살표)를 사용하여 대상을 클릭하여 선택합니다. 타겟을 다른 위치로 드래그합니다.

* **크기**&#x200B;조정 타겟 선택 버튼(화살표)을 사용하여 대상을 클릭하여 선택합니다. 포인터를 확대/축소 타겟의 모서리 위로 이동하고 드래그하여 타겟을 확대하거나 축소합니다.

* **삭제**&#x200B;화면 오른쪽에 있는 대상의 축소판 이미지를 클릭합니다. 그런 다음 타겟 **[!UICONTROL 삭제를 클릭합니다]**.

* **이름**&#x200B;바꾸기 화면 오른쪽에 있는 대상의 축소판 이미지를 클릭합니다. Then enter a name in the **[!UICONTROL Name]** text field and click **[!UICONTROL Save]**.

### 확대/축소 타겟 복사 {#copying-zoom-targets}

한 이미지에서 다른 이미지로 확대/축소 타겟을 복사할 수 있습니다. 두 이미지가 비슷한 컨텐츠를 제공하고 확대/축소 타겟이 동일한 위치에 속하는 경우 타겟을 복사합니다. 확대/축소 타겟을 다른 이미지로 복사하려면 다음 단계를 수행합니다.

1. [확대/축소 타겟 편집기] 화면에서 복사하려는 확대/축소 타겟이 있는 이미지를 엽니다.
1. 대상 **[!UICONTROL 복사를 클릭합니다]**.
1. In the Select Images dialog box, select an image and click **[!UICONTROL Select]**.

