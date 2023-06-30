---
title: 에셋 이동, 이름 변경 및 삭제
description: Adobe Dynamic Media Classic에서 에셋을 이동하고, 이름을 변경하고, 삭제하는 방법에 대해 알아봅니다.
uuid: deff6521-0ad0-4db9-b4e0-e3211ff97740
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 1c9e29f0-3083-4d22-a439-2a01faf59683
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 391eb7ce-ed89-47a8-a6c6-5adb3e95bf78
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 31%

---

# 에셋 이동, 이름 변경 및 삭제{#moving-renaming-and-deleting-assets}

찾아보기 패널에서 자산을 이동하고 이름을 바꾸고 삭제할 수 있습니다. 텍스트 파일을 사용하여 많은 자산을 동시에 삭제할 수도 있습니다.

## 자산 이동 {#move-assets}

찾아보기 패널에서 자산을 각기 다른 폴더로 이동할 수 있습니다.

**자산을 이동하려면 다음을 수행합니다.**

1. 찾아보기 패널에서 자산을 선택하고 다음 중 하나를 수행합니다.

   * 에셋을 에셋 라이브러리에서 이동할 폴더를 표시하고 에셋을 폴더로 드래그합니다.
   * 다음으로 이동 **[!UICONTROL 파일]** > **[!UICONTROL 이동]**&#x200B;를 클릭하고 에셋 이동 창에서 폴더를 선택한 다음 를 선택합니다 **[!UICONTROL 이동]**.

## 자산 이름 바꾸기 {#rename-assets}

1. 찾아보기 패널에서 자산을 선택하고 다음 중 하나를 수행합니다.

   * 이름을 선택하고 새 이름을 입력한 다음 키를 누릅니다 **[!UICONTROL 입력]** 또는 이름에서 나가기를 선택합니다.
   * 다음으로 이동 **[!UICONTROL 파일]** > **[!UICONTROL 이름 바꾸기]**. 자산 이름이 강조 표시됩니다. 새 이름을 입력하고 키를 누릅니다 **[!UICONTROL 입력]**. 기존 Adobe Dynamic Media Classic 에셋의 이름을 입력하지 않도록 하십시오.

## 자산 삭제 {#delete-assets}

찾아보기 패널에서 선택한 에셋을 삭제하고 전체 폴더를 삭제할 수 있습니다. 삭제한 자산과 폴더는 휴지통 폴더로 이동되며, 여기서 영구적으로 삭제되기 전에 7일 동안 유지됩니다.

자산을 삭제하면 이 자산에서 파생된 모든 자산도 삭제됩니다. 예를 들어 확대/축소 타겟을 만든 이미지를 삭제하면 이미지와 함께 확대/축소 타겟도 삭제됩니다.

확대/축소 타겟, 이미지 특성 및 내역 항목은 이 항목이 파생된 자산을 삭제할 때 영구적으로 삭제됩니다. 자산과 함께 휴지통 폴더로 이동되지 않으며 휴지통에서 복원할 수 없습니다.

>[!IMPORTANT]
>
>대량 삭제는 집중적인 작업입니다. 대량 삭제를 동시에 많이 수행하는 삭제 작업이 아니라 순차적으로 실행해야 합니다. Adobe은 삭제 작업을 시간당 5000개 이하의 에셋 삭제로 제한하는 것을 권장합니다. 시간당 5000보다 큰 숫자는 속도 제한을 초래할 수 있습니다.

**에셋을 삭제하려면:**

1. 다음 중 하나를 수행합니다.

   * 하나 이상의 에셋을 삭제하려면 [검색] 패널에서 에셋을 선택하고 키를 누릅니다 **[!UICONTROL 삭제]** 또는 다음으로 이동 **[!UICONTROL 파일]** > **[!UICONTROL 삭제]**.
   * 폴더를 삭제하려면 자산 라이브러리에서 폴더를 선택한 다음 을 선택합니다 **[!UICONTROL 폴더 제거]**.

     폴더를 삭제하면 폴더, 폴더의 모든 에셋 및 그 하위 폴더의 모든 에셋이 삭제됩니다.

Adobe Dynamic Media Classic에서는 에셋 파일을 삭제하는 이유가 동일한 이름으로 다른 에셋 파일로 바꾸는 것인 경우 에셋 파일을 삭제하는 것보다 덮어쓰는 것을 권장합니다.

## 텍스트 파일을 사용하여 여러 자산 삭제 {#delete-multiple-assets-with-a-text-file}

자산 라이브러리 전체에서 한 번에 많은 자산을 삭제하려면 삭제할 자산을 텍스트 파일에 나열한 다음 목록을 Adobe Dynamic Media Classic에 제출할 수 있습니다.

Adobe Dynamic Media Classic ID 목록을 만들고 텍스트(.txt) 파일로 저장합니다. 각 Adobe Dynamic Media Classic ID는 고유한 줄에 있어야 합니다(그 뒤에는 하드 반환).

목록을 만든 후 다음 단계를 수행하여 자산을 삭제하는 데 사용합니다.

1. 다음으로 이동 **[!UICONTROL 파일]** > **[!UICONTROL 자산 목록 삭제]**.
1. 에셋 목록 삭제 대화 상자에서 삭제할 에셋 목록이 있는 텍스트 파일의 경로를 찾아보거나 입력합니다.
1. 선택 **[!UICONTROL 삭제]**.

텍스트 파일이 있는 에셋을 삭제할 때 목록에 Adobe Dynamic Media Classic ID가 없으면 &quot;목록에 있는 이러한 항목의 유효성을 검사할 수 없습니다.&quot;라는 메시지가 표시됩니다. 항목 목록도 표시됩니다. 단, Adobe Dynamic Media Classic에서는 작업 페이지에 오류가 발생하지 않습니다.

>[!MORELIKETHIS]
>
>* [찾아보기 패널에서 에셋 선택](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [업로드할 자산 및 폴더 준비](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [휴지통 폴더에서 자산 복원](trash-folder.md#restoring_assets_from_the_trash_folder)
