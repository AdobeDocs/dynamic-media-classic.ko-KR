---
title: 미디어 포털 사용자에게 내보내기 옵션 지정 가능
seo-title: 미디어 포털 사용자에게 내보내기 옵션 지정 가능
description: 널
seo-description: Media Portal 사용자가 사용할 수 있는 내보내기 옵션을 지정하는 방법을 알아봅니다.
uuid: 5258 B 8 A 4-0704-43 CD -97 D 1-C 9 AF 2 E 4 E 298 B
contentOwner: 관리
content-type: 참조
products: sg_ Experiencemanager/dynamic-media-scene -7
discoiquuid: 9 bfd 95 da -3714-4 e 38-98 af -331 a 04 c 685 f 5
translation-type: tm+mt
source-git-commit: 0f6c8e6ac69e29aab7a48425aab76c10170d9ddf

---


# Media Portal 사용자가 사용할 수 있는 내보내기 선택 사항 지정 {#specifying-export-options-available-to-media-portal-users}

관리자가 권한을 부여한 경우 Media Portal 사용자는 이미지를 내보낼 때 형식을 다시 지정할 수 있습니다. 예를 들어 크기, 파일 형식 및 이미지 품질을 변경할 수 있습니다. 이미지를 내보낼 때 자동으로 형식을 다시 지정하면 별도로 이미지 형식을 다시 지정할 필요가 없기 때문에 시간이 절약됩니다. 또한 관리자는 사전 설정된 이미지 형식 설정 선택인 사전 설정을 만들 수 있습니다. 이미지를 내보낼 때 사전 설정을 사용하여 회사 사양에 맞게 형식을 다시 지정할 수 있습니다.

사용자 지정 전환을 통해 이미지 자산을 내보내거나 원본 마스터 이미지를 내보내는 경우 다음 두 가지 제한이 적용됩니다.

* 내보내기 작업에 대해 ZIP 압축 내보내기 파일의 최대 파일 크기는 1 GB입니다.
* 내보내기 작업당 최대 총 500개의 자산을 가질 수 있습니다.

또한 [Scene7 Publishing System에서 자산 내보내기](exporting-assets-scene7-publishing-system.md#exporting_assets_from_scene7_publishing_system)를 참조하십시오.

**Media Portal 사용자가 사용할 수 있는 내보내기 선택 사항을 지정하려면**

1. **[설정]** &gt; **[이미지 사전 설정]**&#x200B;을 클릭합니다.
1. [이미지 사전 설정] 창에서 다음 중 원하는 선택 사항을 선택합니다.

   **사용자 정의된 전환** 활성화 이 옵션을 선택하면 사용자가 선택한 자산 내보내기 창의 크기 드롭다운 목록에서 다른 항목을 선택할 수 있습니다. 그런 다음 사용자는 픽셀 또는 센티미터와 같은 측정 단위를 선택하고 원하는 너비와 높이를 지정할 수 있습니다. 이러한 파일을 내보내거나 다운로드하는 경우 이미지 파일 형식이 다시 지정됩니다.

   **크기** 드롭 다운 목록에서 **픽셀**&#x200B;을 선택한 경우, 결과 이미지의 너비 x 높이가 1억 픽셀을 초과 할 수 없습니다. 이는 정사각형 이미지의 경우 10,000 x 10,000 픽셀과, 또는 2x3 종횡비 이미지의 경우 약 8,000 x 12,000 픽셀과 동일합니다. 이 크기 제한은 원본 마스터 이미지를 내보낼 경우에는 적용되지 않습니다.

   사용자가 파일을 다운로드할 때 형식을 다시 지정하지 않고 다운로드하게 하려는 경우 이 선택 사항을 선택 취소합니다.

   **원본** 내보내기 활성화 원본 마스터 이미지를 내보낼 수 있습니다. 사용자는 [선택한 자산 내보내기] 패널에서 [전환] 드롭다운 메뉴를 열고 [원본 내보내기]를 선택하여 원본 파일을 내보낼 수 있습니다. 사용자가 이미지를 내보낼 때 이미지 사전 설정을 선택하거나 전환 선택 사항을 선택하도록 강제하려는 경우 이 선택 사항을 선택 취소합니다.

>[!MORELIKETHIS]
>
>* [Image Presets](application-setup.md#image_presets)
>* [그룹의 이미지 사전 설정 액세스 권한 선택](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)

