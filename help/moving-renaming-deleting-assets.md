---
title: 자산 이동, 이름 변경 및 삭제
description: Adobe Dynamic Media Classic에서 자산을 이동, 이름 변경 및 삭제하는 방법에 대해 알아봅니다.
uuid: deff6521-0ad0-4db9-b4e0-e3211ff97740
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 1c9e29f0-3083-4d22-a439-2a01faf59683
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 391eb7ce-ed89-47a8-a6c6-5adb3e95bf78
source-git-commit: 741e31e64125a2dfe3f801480837ffbaf81767aa
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 31%

---

# 자산 이동, 이름 변경 및 삭제{#moving-renaming-and-deleting-assets}

찾아보기 패널에서 자산을 이동하고 이름을 바꾸고 삭제할 수 있습니다. 텍스트 파일을 사용하여 많은 자산을 동시에 삭제할 수도 있습니다.

## 자산 이동 {#move-assets}

찾아보기 패널에서 자산을 각기 다른 폴더로 이동할 수 있습니다.

**자산을 이동하려면 다음을 수행하십시오.**

1. 찾아보기 패널에서 자산을 선택하고 다음 중 하나를 수행합니다.

   * 자산을 자산 라이브러리에서 로 이동할 폴더를 표시하고 자산을 폴더로 드래그합니다.
   * 이동 **[!UICONTROL 파일]** > **[!UICONTROL 이동]**&#x200B;를 클릭하고 자산 이동 창에서 폴더를 선택한 다음 을 선택합니다 **[!UICONTROL 이동]**.

## 자산 이름 바꾸기 {#rename-assets}

1. 찾아보기 패널에서 자산을 선택하고 다음 중 하나를 수행합니다.

   * 이름을 선택하고 새 이름을 입력한 다음 키를 누릅니다 **[!UICONTROL Enter 키]** 또는 이름에서 바깥쪽을 선택합니다.
   * 이동 **[!UICONTROL 파일]** > **[!UICONTROL 이름 변경]**. 자산 이름이 강조 표시됩니다. 새 이름을 입력하고 키를 누릅니다 **[!UICONTROL Enter 키]**. 기존 Adobe Dynamic Media Classic 자산의 이름을 입력하지 마십시오.

## 자산 삭제 {#delete-assets}

찾아보기 패널에서 선택한 자산을 삭제하고 전체 폴더를 삭제할 수 있습니다. 삭제한 자산과 폴더는 휴지통 폴더로 이동되며, 여기서 영구적으로 삭제되기 전에 7일 동안 유지됩니다.

자산을 삭제하면 이 자산에서 파생된 모든 자산도 삭제됩니다. 예를 들어 확대/축소 타겟을 만든 이미지를 삭제하면 이미지와 함께 확대/축소 타겟도 삭제됩니다.

확대/축소 타겟, 이미지 특성 및 내역 항목은 이 항목이 파생된 자산을 삭제할 때 영구적으로 삭제됩니다. 자산과 함께 휴지통 폴더로 이동되지 않으며 휴지통에서 복원할 수 없습니다.

>[!IMPORTANT]
>
>대량 삭제는 많은 작업이 필요합니다. 대량 삭제 작업은 동시 삭제 작업이 아닌 순차적으로 실행해야 합니다. Adobe은 삭제 작업을 시간당 5000개 이하의 자산 삭제로 제한하는 것이 좋습니다. 시간당 5000보다 큰 숫자를 지정하면 속도 제한이 발생할 수 있습니다.

**자산을 삭제하려면 다음을 수행하십시오.**

1. 다음 중 하나를 수행합니다.

   * 자산을 한 개 이상 삭제하려면 [찾아보기] 패널에서 자산을 선택하고 키를 누릅니다 **[!UICONTROL 삭제]** 또는 **[!UICONTROL 파일]** > **[!UICONTROL 삭제]**.
   * 폴더를 삭제하려면 자산 라이브러리에서 폴더를 선택하고 을(를) 선택합니다 **[!UICONTROL 폴더 제거]**.

      폴더를 삭제하면 폴더, 폴더의 모든 자산 및 해당 하위 폴더의 모든 자산이 삭제됩니다.

자산 파일을 삭제하는 이유는 동일한 이름으로 다른 파일로 대체하기 위한 경우 자산 파일을 삭제하는 대신 덮어쓰는 것이 좋습니다.

## 텍스트 파일을 사용하여 여러 자산 삭제 {#delete-multiple-assets-with-a-text-file}

자산 라이브러리 전체에서 한 번에 많은 자산을 삭제하려면 텍스트 파일에서 삭제할 자산을 나열하고 목록을 Adobe Dynamic Media Classic에 제출할 수 있습니다.

Adobe Dynamic Media Classic ID 목록을 만들고 텍스트(.txt) 파일로 저장합니다. 각 Adobe Dynamic Media Classic ID는 자체 줄에 있어야 합니다(뒤에 하드 리턴).

목록을 만든 후 다음 단계를 수행하여 자산을 삭제하는 데 사용합니다.

1. 이동 **[!UICONTROL 파일]** > **[!UICONTROL 자산 목록 삭제]**.
1. 자산 목록 삭제 대화 상자에서 삭제할 자산 목록이 있는 텍스트 파일의 경로를 찾아보거나 입력합니다.
1. 선택 **[!UICONTROL 삭제]**.

텍스트 파일로 자산을 삭제할 때 목록에 Adobe Dynamic Media Classic ID가 없으면 &quot;목록에서 이러한 항목의 유효성을 검사할 수 없습니다.&quot;라는 메시지가 표시됩니다. 항목 목록도 표시됩니다. 하지만 Adobe Dynamic Media Classic에서는 작업 페이지에 오류가 생성되지 않습니다.

>[!MORELIKETHIS]
>
>* [찾아보기 패널에서 자산 선택](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [업로드할 자산 및 폴더 준비](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [휴지통 폴더에서 자산 복원](trash-folder.md#restoring_assets_from_the_trash_folder)

