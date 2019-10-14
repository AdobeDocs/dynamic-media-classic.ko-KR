---
title: 휴지통 폴더 관리
seo-title: 휴지통 폴더 관리
description: 널
seo-description: 휴지통 폴더를 관리하는 방법을 알아봅니다.
uuid: 3992a5b8-1919-4924-b07d-7fb25565effd
contentOwner: 관리
content-type: 참조
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 553c95fc-0a41-4f06-af50-a62bc1438149
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# 휴지통 폴더 관리{#managing-the-trash-folder}

Scene7 Publishing System에서 삭제한 항목은 휴지통 폴더로 이동됩니다. 이러한 항목은 복원하거나 영구적으로 삭제할 때까지 이 폴더에 7일 동안 유지됩니다. 자산 라이브러리 하단에 있는 [휴지통] 아이콘 을 선택하고 휴지통 폴더에서 확인하여 삭제한 항목을 검사할 수 있습니다.

모든 사용자가 휴지통 폴더의 항목을 삭제되기 전의 폴더로 복원할 수 있습니다. 모든 사용자가 휴지통 폴더의 모든 내용을 비울 수도 있습니다.

휴지통 폴더에서 항목을 삭제하면 Scene7 Publishing System에서 항목이 영구적으로 삭제되며, 휴지통 폴더에서 삭제한 항목은 더 이상 복원할 수 없습니다. 휴지통에서 자산이 자동으로 삭제될 때 회사 관리자에게 알림을 보내도록 설정하는 방법에 대한 자세한 내용은 [[애플리케이션 일반 설정]](application-setup.md#general_settings)을 참조하십시오.

>[!NOTE]
>
>휴지통 폴더로 이동된 자산은 Scene7 Publishing System에 여전히 등록되어 있습니다. 휴지통 폴더에 있는 삭제된 파일과 이름이 같은 파일을 업로드하려고 하면 Dynamic Media Classic에서 업로드하려는 자산을 중복 자산으로 처리합니다. 따라서 자산 이름에 숫자가 추가됩니다.

## 휴지통 폴더 정보 {#about-the-trash-folder}

폴더에서 삭제한 항목은 휴지통 폴더에 배치됩니다. 항목을 삭제하고 휴지통 폴더로 이동하는 경우 다음 동작이 발생합니다.

* 항목이·Scene7·Publishing System 폴더에서 제거되었지만 휴지통 폴더에 유지되는 동안 해당 ID를 다른 자산에 지정할 수 없습니다. 휴지통 폴더에 있는 파일과 같은 이름의 자산을 업로드하려고 하면 Dynamic Media Classic에서 자산의 이름에 숫자를 추가합니다.
* 항목을 게시할 수 없습니다. 항목을 삭제할 때 게시로 표시된 경우에도 항목이 게시되지 않습니다.
* 항목은 복원되거나 7일이 경과하거나 [휴지통 비우기] 명령을 선택할 때까지 휴지통 폴더에 유지됩니다. 7일 후에는 자동 정리 작업에 의해 항목이 영구적으로 삭제됩니다.

## 휴지통 폴더에서 자산 복원 {#restoring-assets-from-the-trash-folder}

자산을 삭제한 사람이 복원해야 하는 것은 아니며 누구든지 휴지통 폴더에서 자산을 복원할 수 있습니다. 복원한 자산은 삭제되기 전의 폴더에 배치됩니다. 해당 폴더가 더 이상 없는 경우 Scene7 Publishing System에서 폴더를 다시 만듭니다. 복원한 자산은 다시 만들어진 폴더에 배치됩니다.

휴지통 폴더의 자산을 삭제되기 전의 폴더로 복원하려면 다음 단계를 수행합니다.

1. 휴지통 아이콘을 클릭하여 휴지통 폴더를 엽니다.
1. 복원하려는 자산을 선택합니다.
1. [파일] &gt; [휴지통에서 복원]을 선택합니다.

## 휴지통 폴더에서 영구적으로 자산 삭제 {#permanently-deleting-assets-in-the-trash-folder}

휴지통 폴더에서 삭제한 자산은 영구적으로 삭제됩니다. 7일 후에는 휴지통 폴더에서 자산이 자동으로 삭제됩니다.

휴지통 폴더에서 자산을 영구적으로 삭제하려면 [휴지통] 아이콘 을 선택하여 휴지통 폴더를 엽니다. 그런 다음 개별 자산을 삭제하거나 폴더에 있는 모든 자산을 삭제합니다.

* **개별 자산** 삭제 영구적으로 삭제할 자산을 선택하고 파일 &gt; 휴지통에서 **[!UICONTROL 비우기 를 클릭합니다]**.

* **모든 자산** 삭제 파일 **[!UICONTROL &gt; 빈 휴지통을 클릭합니다]**.

>[!MORELIKETHIS]
>
>* [자산 삭제](moving-renaming-deleting-assets.md#delete_assets)

