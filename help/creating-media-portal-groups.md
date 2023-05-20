---
title: Media Portal 그룹 만들기 및 관리
description: Adobe Dynamic Media Classic에서 Media Portal 그룹을 만들고 관리하는 방법에 대해 알아봅니다.
uuid: 23f360e1-ddcb-491b-ab9f-428f3ac9c316
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 91524d36-b77a-4dc4-acba-a7bd85297e98
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: 0deb7133-b895-4c3f-8e5e-8604a6f2d16b
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 56%

---

# Media Portal 그룹 만들기 및 관리{#creating-and-managing-media-portal-groups}

*그룹*&#x200B;은 Media Portal 사용자를 관리하는 데 도움이 됩니다. 자산에 액세스하려면 사용자가 해당 자산에 대한 액세스 권한이 있는 하나 이상 그룹의 구성원이어야 합니다. 사용자를 추가할 때 하나 이상의 그룹에 지정합니다. 이렇게 하면 그룹이 지정된 폴더에 대한 액세스 권한이 사용자에게 부여됩니다. 그룹에 사용할 수 있는 이미지 사전 설정을 선택할 수도 있습니다.

## 그룹을 사용하여 폴더, 에셋 및 이미지 사전 설정에 대한 액세스를 제한합니다 {#using-groups-to-restrict-access-to-folders-assets-and-image-presets}

각기 다른 수준의 액세스 권한을 부여하기 위해 그룹을 만듭니다. 각 그룹에 서로 다른 폴더 및 폴더의 자산에 대한 읽기, 쓰기 및 삭제 권한을 지정합니다. 또한 그룹에 사용할 수 있는 이미지 사전 설정을 결정합니다. 그런 다음 사용자를 그룹에 지정합니다. 한 사용자가 여러 그룹의 구성원이 될 수 있습니다. 그룹 개념을 사용하면 전체 컨텐츠 중 제한된 집합에 대한 액세스 권한을 유연하게 지정할 수 있습니다.

에셋 또는 폴더에 그룹 권한을 특별히 부여하지 않으면 해당 에셋 또는 폴더는 상위 폴더(폴더 계층 구조에서 상위 폴더)에 할당한 권한을 상속합니다. 모든 하위 폴더가 동일한 권한을 상속하게 하려는 경우 상위 폴더에 권한을 부여합니다.

>[!NOTE]
>
>사용자는 여러 그룹에 속할 수 있습니다. 사용자가 폴더에 대한 액세스 권한이 서로 다른 두 그룹에 속해 있는 경우 가장 높은 액세스 권한이 부여됩니다.

## 그룹 추가 {#adding-a-group}

1. 다음으로 이동 **[!UICONTROL 설정]** > **[!UICONTROL Media Portal 설정]** > **[!UICONTROL 그룹]**.
1. 선택 **[!UICONTROL 추가]**.
1. 그룹 추가 대화 상자의 그룹 이름 상자에 그룹 이름을 입력한 다음 을 선택합니다 **[!UICONTROL 그룹 추가]**.
1. 원하는 경우 사용자 이름 옆에 있는 상자를 선택하여 새 그룹에 사용자를 추가할 수 있습니다.
1. 지금 액세스 권한을 지정하려면 **[!UICONTROL 자산 액세스 권한]** 탭을 클릭한 다음 원하는 옵션을 지정합니다.

   [그룹의 자산 액세스 권한 설정](creating-media-portal-groups.md#establishing_asset_access_permissions_for_a_group)을 참조하십시오.

1. 그룹에서 사용할 수 있는 이미지 사전 설정을 선택하려면 **[!UICONTROL 이미지 사전 설정 액세스 권한]** 을 탭하고 그룹이 사용할 수 있는 이미지 사전 설정을 선택합니다.

   [그룹의 이미지 사전 설정 액세스 권한 선택](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)을 참조하십시오.

1. 선택 **[!UICONTROL 닫기]**.

## 그룹의 자산 액세스 권한 설정 {#establishing-asset-access-permissions-for-a-group}

1. 다음으로 이동 **[!UICONTROL 설정]** > **[!UICONTROL Media Portal 설정]** > **[!UICONTROL 그룹]**.
1. [그룹] 목록 페이지에서 다음 중 하나를 수행합니다.

   * 그룹을 추가하고 권한을 지정하려면 **[!UICONTROL 추가]**. [그룹 추가] 대화 상자에서 그룹 이름을 입력하고 **[!UICONTROL 그룹 추가]**&#x200B;을 클릭하고 사용자를 그룹에 추가합니다.
   * 그룹의 권한을 편집하려면 그룹을 선택한 다음 을 선택합니다 **[!UICONTROL 편집]**.

1. 그룹 추가 또는 그룹 편집 대화 상자에서 **[!UICONTROL 자산 액세스 권한]** 탭. 탭의 오른쪽에는 폴더와 자산에 대한 읽기, 쓰기 및 삭제 권한을 설정하는 상자가 제공됩니다. 왼쪽 창에서 폴더와 하위 폴더를 확장하고 축소할 수 있습니다.
1. 폴더나 개별 자산에 대한 권한을 지정하려면 왼쪽 창에서 폴더를 선택합니다. 폴더 내용이 오른쪽 창에 표시됩니다. 오른쪽 창에서 해당 파일이나 폴더의 상자를 선택하여 그룹에 권한을 지정합니다.

   다음 표에서는 각 작업을 읽기, 쓰기 및 삭제 권한에 매핑합니다.

   | 작업 | 읽음 | 쓰기 | 삭제 |
   | --- | --- | --- | --- |
   | 폴더 및 파일 찾아보기 | X |  |  |
   | 파일 편집(자르기, 선명하게, 조정) |  | X |  |
   | 파일 이름 변경 |  | X |  |
   | 파일을 다른 폴더로 이동 |  | X |  |
   | 파일 이름 변경 |  | X |  |
   | 파일 삭제 |  |  | X |

1. 선택 **[!UICONTROL 닫기]**.

>[!NOTE]
>
>상자를 선택하면 액세스 권한이 설정됩니다. 폴더에 대한 권한을 지정하면 하위 폴더와 이 폴더에 있는 모든 파일에 상위 폴더와 동일한 권한이 부여됩니다. 그러나 개별 하위 폴더와 자산 파일에 대해 다른 권한을 지정할 수 있습니다.

## 그룹의 이미지 사전 설정 액세스 권한 선택 {#choosing-image-preset-access-permissions-for-a-group}

그룹 구성원이 Media Portal을 사용하여 자산을 내보낼 때 사용할 수 있는 이미지 사전 설정을 지정하려는 경우 그룹의 이미지 사전 설정 액세스 권한을 선택합니다.

참조: [Media Portal 사용자가 사용할 수 있는 내보내기 옵션 지정](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

**그룹에 대한 이미지 사전 설정 액세스 권한을 선택하려면 다음을 수행하십시오.**

1. 다음으로 이동 **[!UICONTROL 설정]** > **[!UICONTROL Media Portal 설정]** > **[!UICONTROL 그룹]**.
1. [그룹] 목록 페이지에서 다음 중 하나를 수행합니다.

   * 그룹을 추가하고 사용 가능한 이미지 사전 설정을 지정하려면 다음을 선택합니다 **[!UICONTROL 추가]**. [그룹 추가] 대화 상자에서 그룹 이름을 입력하고 **[!UICONTROL 그룹 추가]**&#x200B;을 클릭하고 사용자를 그룹에 추가합니다.
   * 그룹의 이미지 사전 설정 옵션을 편집하려면 그룹을 선택한 다음 을 선택합니다 **[!UICONTROL 편집]**.

1. 그룹 추가 또는 그룹 편집 대화 상자에서 **[!UICONTROL 이미지 사전 설정 액세스 권한]** 탭.
1. Media Portal 사용자가 에셋을 내보낼 때 사용할 수 있는 사전 설정을 지정하려면 이미지 사전 설정을 선택하거나 선택 취소합니다.
1. 선택 **[!UICONTROL 닫기]**.

## 그룹 편집 및 삭제 {#edit-and-delete-groups}

1. 다음으로 이동 **[!UICONTROL 설정]** > **[!UICONTROL Media Portal 설정]** > **[!UICONTROL 그룹]**.
1. [그룹 목록] 페이지에서 그룹을 선택하고 편집하거나 삭제합니다.

   **그룹 편집** - 선택 **[!UICONTROL 편집]**&#x200B;을 클릭하고 [그룹 편집] 대화 상자에서 옵션을 선택합니다.

   **그룹 삭제** - 선택 **[!UICONTROL 삭제]**.
