---
title: 자산 이동, 이름 바꾸기 및 삭제
seo-title: 자산 이동, 이름 바꾸기 및 삭제
description: 널
seo-description: 자산을 이동, 이름 변경 및 삭제하는 방법에 대해 알아봅니다.
uuid: deff 6521-0 ad 0-4 db 9-b 4 e 0-e 3211 ff 97740
contentOwner: 관리
content-type: 참조
products: sg_ Experiencemanager/dynamic-media-scene -7
geptopics: sg_ scenesevenondemand_ pk/categories/managing_ assets
discoiquuid: 1 C 9 E 29 F 0-3083-4 D 22-A 439-2 A 01 FAF 59683
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# 자산 이동, 이름 바꾸기 및 삭제{#moving-renaming-and-deleting-assets}

찾아보기 패널에서 자산을 이동하고 이름을 바꾸고 삭제할 수 있습니다. 텍스트 파일을 사용하여 많은 자산을 동시에 삭제할 수도 있습니다.

## 자산 이동 {#move-assets}

찾아보기 패널에서 자산을 각기 다른 폴더로 이동할 수 있습니다.

1. 찾아보기 패널에서 자산을 선택하고 다음 중 하나를 수행합니다.

   * 자산 라이브러리에서 자산을 이동하려는 폴더를 표시하고 자산을 폴더로 드래그합니다.
   * [파일] &gt; [이동]을 선택하고 [자산 이동] 창에서 폴더를 선택한 다음 [이동]을 선택합니다.

## 자산 이름 바꾸기 {#rename-assets}

자산 이름을 바꾸려면

1. 찾아보기 패널에서 자산을 선택하고 다음 중 하나를 수행합니다.

   * 이름을 선택하고 새 이름을 입력한 다음 Enter 키를 누르거나 이름에서 떨어진 곳을 클릭합니다.
   * [파일] &gt; [이름 변경]을 선택합니다. 자산 이름이 강조 표시됩니다. 새 이름을 입력하고 Enter 키를 누릅니다.

기존 Scene7 Publishing System 자산의 이름을 입력하면 안 됩니다.

## 자산 삭제 {#delete-assets}

찾아보기 패널에서 선택한 자산을 삭제하고 전체 폴더를 삭제할 수 있습니다. 삭제한 자산과 폴더는 휴지통 폴더로 이동되며, 여기서 영구적으로 삭제되기 전에 7일 동안 유지됩니다.

자산을 삭제하면 이 자산에서 파생된 모든 자산도 삭제됩니다. 예를 들어 확대/축소 타겟을 만든 이미지를 삭제하면 이미지와 함께 확대/축소 타겟도 삭제됩니다.

>[!NOTE]
>
>확대/축소 타겟, 이미지 특성 및 내역 항목은 이 항목이 파생된 자산을 삭제할 때 영구적으로 삭제됩니다. 자산과 함께 휴지통 폴더로 이동되지 않으며 휴지통에서 복원할 수 없습니다.

1. 다음 중 하나를 수행합니다.

   * 자산을 하나 이상 삭제하려면 찾아보기 패널에서 자산을 선택하고 Delete 키를 누르거나 [파일] &gt; [삭제]를 선택합니다.
   * To delete a folder, select the folder in the Asset Library, and click **Remove Folder**.

      폴더를 삭제하면 폴더, 폴더의 모든 자산 및 하위 폴더의 모든 자산이 삭제됩니다.

>[!NOTE]
>
>에셋 파일을 삭제하는 이유가 동일한 이름으로 다른 이름으로 교체되는 경우 Dynamic Media Classic 에서는 에셋 파일을 삭제하지 않고 덮어쓰는 것이 좋습니다.

## 텍스트 파일을 사용하여 여러 자산 삭제 {#delete-multiple-assets-with-a-text-file}

자산 라이브러리에서 한 번에 많은 자산을 삭제하려면 텍스트 파일에서 삭제할 자산을 나열하고 Dynamic Media Classic에 목록을 제출할 수 있습니다.

Scene7 Publishing System ID 목록을 만들고 텍스트(.txt) 파일로 저장합니다. 각 Scene7 Publishing System ID가 별도의 라인에 표시되어야 합니다(뒤에 하드 리턴이 와야 함).

목록을 만든 후 다음 단계를 수행하여 자산을 삭제하는 데 사용합니다.

1. [파일] &gt; [자산 목록 삭제]를 선택합니다.
1. [자산 목록 삭제] 대화 상자에서 삭제하려는 자산 목록이 포함된 텍스트 파일을 찾거나 경로를 입력합니다.
1. [삭제] 단추를 클릭합니다.

텍스트 파일로 자산을 삭제할 때 Scene 7 Publishing System ID가 목록에 없으면 Dynamic Media Classic 이 "목록에서 해당 항목의 유효성을 검사할 수 없습니다. » 를 클릭합니다. 그러나 Dynamic Media Classic 에서는 작업 화면에 오류가 발생하지 않습니다.

>[!MORELIKETHIS]
>
>* [찾아보기 패널에서 자산 선택](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [업로드할 자산 및 폴더 준비](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [휴지통 폴더에서 자산 복원](trash-folder.md#restoring_assets_from_the_trash_folder)

