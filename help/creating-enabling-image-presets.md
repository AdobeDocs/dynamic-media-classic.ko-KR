---
title: 이미지 사전 설정 만들기 및 활성화
description: Adobe Dynamic Media Classic에서 이미지 사전 설정을 만들고 활성화하는 방법을 알아봅니다.
uuid: 62cfc6fa-da91-4c42-a3ed-10956384d633
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 84257b2a-681c-4fe9-a6e5-3633c1d61d8c
feature: Dynamic Media Classic,Collaboration,Image Presets,Asset Management
role: Admin,User
exl-id: 94c6c388-226b-4172-a6c7-a8dcf9c0f0cf
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 72%

---

# 이미지 사전 설정 만들기 및 활성화{#creating-and-enabling-image-presets}

사용자는 Media Portal을 사용하여 이미지 자산을 내보낼 때 [선택한 자산 내보내기] 대화 상자에서 이미지 사전 설정을 선택할 수 있습니다. 이미지 사전 설정은 이미지를 내보낼 때 크기, 이미지 품질, 형식, 해상도 및 이미지 모양의 기타 측면을 변경하는 사전 정의된 설정 모음입니다.

Media Portal 관리자는 이미지 사전 설정을 만들어 이미지를 내보낼 때 형식을 다시 지정하는 방법을 제어할 수 있습니다. 이미지 사전 설정은 사용자가 Adobe Dynamic Media Classic에서 이미지를 내보낼 때 회사 사양에 맞게 이미지를 다시 포맷합니다. 사용자는 직접 이미지 형식을 다시 지정하는 대신 이미지 사전 설정의 정확한 사양으로 이미지를 내보냅니다.

이미지 자산을 내보낼 때 다음 제한이 적용됩니다.

* 너비x높이는 이미지당 100MB 이하여야 합니다. 예를 들어 이미지는 10Kx10K 또는 8Kx12K와 같은 아래 종횡비 변형을 초과할 수 없습니다.
* 내보내기 작업당 최대 1GB의 총 파일 크기가 있습니다.
* 내보내기 작업당 최대 총 500개의 자산을 가질 수 있습니다.

>[!NOTE]
>
>이러한 제한 사항은 기본 파일의 내보내기가 아니라 파생된 이미지 자산의 내보내기에만 적용됩니다.

이미지 사전 설정을 만들려면 [이미지 사전 설정](application-setup.md#image_presets)을 참조하십시오.

사용자가 파일을 내보낼 때 이미지 사전 설정을 선택할 수 있게 하려면 [Media Portal 사용자가 사용할 수 있는 내보내기 선택 사항 지정](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users)을 참조하십시오.

그룹 구성원이 사용할 수 있는 이미지 사전 설정을 선택하려면 [그룹의 이미지 사전 설정 액세스 권한 선택](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)을 참조하십시오.
