---
title: 이미지 사전 설정 지정
seo-title: 이미지 사전 설정 지정
description: 널
seo-description: 이미지 사전 설정을 설정하는 방법을 알아봅니다.
uuid: 90530948-Dee 9-41 BD-B 39 E -684140446 ABC
contentOwner: 관리
content-type: 참조
products: sg_ Experiencemanager/dynamic-media-scene -7
geptopics: sg_ scenesevenondemand_ pk/categories/image_ sizing
discoiquuid: 1 EC 39 FE 5-7 B 2 A -4034-9570-6 B 5595 F 97052
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# 이미지 사전 설정 지정{#setting-up-image-presets}

매크로와 마찬가지로 이미지 사전 설정은 특정 이름으로 저장된 사전 정의된 크기 및 형식 지정 명령 모음입니다. 이미지 사전 설정의 작동 방식을 이해하려면 웹 사이트에서 각 제품 이미지가 500x500 픽셀과 150x150 픽셀의 두 가지 크기로 표시되어야 한다고 가정해 보십시오. 두 개의 이미지 사전 설정, 즉 500x500 픽셀에서 이미지를 표시하기 위한 "확대" 이미지 사전 설정과 150x150 픽셀에서 이미지를 표시하기 위한 "썸네일" 이미지 사전 설정을 만듭니다. «확대» 및 «썸네일» 크기로 이미지를 제공하기 위해 다이내믹 미디어 이미지 서버가 확대 이미지 사전 설정과 썸네일 이미지 사전 설정의 정의를 조회합니다. 그런 다음 각 이미지 사전 설정의 크기 및 형식 지정 사양에 따라 이미지를 동적으로 생성합니다.

Dynamic Media Classic 에는 이미 설정한 몇 가지 "우수 사례" 이미지 사전 설정이 포함되어 있습니다. 관리자는 새 이미지 사전 설정을 만들 수도 있습니다. 이미지 사전 설정을 만들려면 처음부터 시작하거나 기존 이미지 사전 설정에서 시작하여 새 이름으로 저장합니다.

서버에서 동적으로 제공될 때 크기가 축소된 이미지는 선명도와 세부 사항이 손실될 수 있습니다. 이 때문에 각 이미지 사전 설정에는 특정 크기로 제공 시 이미지를 최적화하기 위한 형식 지정 컨트롤이 포함되어 있습니다. 이러한 컨트롤을 사용하면 이미지를 웹 사이트나 애플리케이션에 제공할 때 선명하게 유지할 수 있습니다.

## 이미지 사전 설정 만들기 {#creating-an-image-preset}

회사 관리자는 고유한 이미지 사전 설정을 만들 수 있습니다. 새 이미지 사전 설정을 만들거나 Dynamic Media Classic에서 제공하는 기본 이미지 사전 설정으로 시작하여 편집하고 새 이름으로 저장할 수 있습니다.

**이미지 사전 설정을 만들려면**

1. **[설정]** &gt; **[이미지 사전 설정]**&#x200B;을 클릭합니다.

   이 화면에서 이미지 사전 설정 이름을 찾아 기존 이미지 사전 설정을 미리 볼 수 있습니다. 이미지 사전 설정 이름을 선택하면 [미리 보기] 창의 샘플 이미지 크기와 모양이 바뀝니다.

1. 다음 중 하나를 수행하십시오.

   **이미지 사전 설정** 만들기를 클릭합니다.

   **이미지 사전 설정** 편집 만들려는 이미지와 가장 유사한 이미지 사전 설정을 찾은 다음 편집을 클릭합니다.

1. 이미지 사전 설정의 이름을 입력합니다.
1. [너비] 및 [높이] 측정값을 픽셀 단위로 입력합니다. 이러한 측정값은 제공되는 이미지의 크기를 결정합니다.
1. [사전 설정 추가] 또는 [사전 설정 편집] 화면에 정보를 입력합니다. 자세한 내용은 [이미지 사전 설정 선택 사항](application-setup.md#image_preset_options)을 참조하십시오.

   Dynamic Media Classic 에서는 다음과 같은 "모범 사례" 옵션 선택을 권장합니다.

   **포맷요구 사항에** 맞는 JPEG 또는 다른 형식을 선택합니다. JPEG 이미지 형식은 모든 웹 브라우저에서 지원되며, 작은 파일 크기와 이미지 품질의 적절한 균형을 유지합니다. 그러나 JPEG 형식 이미지는 손실 있는 압축 구성을 사용하므로 압축 설정이 너무 낮으면 불필요한 이미지 아티팩트가 발생할 수 있습니다. 따라서 Dynamic Media Classic 에서는 슬라이더의 압축 품질을 75로 설정할 것을 권장합니다. 이 설정은 이미지 품질과 작은 파일 크기의 적절한 균형을 유지합니다.

   **선명하게 하기는** 선명하게 하기를 선택하지 않습니다 (이 선명하게 하기 필터는 언샵 마스킹 설정보다 제어 기능이 더 낮습니다.).

   **리샘플링 모드에서** Bi-Cubic를 선택합니다.

   **Unsharp Masking (USM) options** 여기에 표시된 설정을 입력합니다.

   | 사전 설정 유형 | 크기 | USM: 양 | USM: 반경 | USM: 임계값 |
   |--- |--- |--- |--- |--- |
   | 크로스셀(미니 썸네일) | 75x75 | 1.5 | 0.8 | 5 |
   | 썸네일 | 150x150 | 1.1 | 1 | 5 |
   | 주 | 350x350 | 1 | 1 | 6 |
   | 확대 | 500x500 | 1.2 | 1.2 | 5 |

1. **[저장]**&#x200B;을 클릭합니다.

여기에 나열된 이미지 사전 설정을 만들기 위한 Dynamic Media Classic «우수 사례» 옵션은 일반 권장 사항입니다. 선명하게 하기는 주관적인 요소입니다. 이 "우수 사례" 설정은 2000x2000 마스터 이미지를 기준으로 작성되었습니다. 더 크거나 작은 마스터의 설정은 이와 다를 수 있습니다. Unsharp Masking 설정을 조정하려는 경우 Dynamic Media Classic 에서는 다음 범위를 권장합니다.

**.8** 와 1.5 사이의 금액.

**Radius** between .6 and 2.

**1-6의 한계값입니다** .

이미지 사전 설정을 삭제하려면 [이미지 사전 설정] 화면에서 사전 설정을 선택하고 [삭제] 단추를 선택합니다.

>[!MORELIKETHIS]
>
>* [이미지 사전 설정 만들기 및 편집](application-setup.md#creating_and_editing_image_presets)
>* [이미지 사전 설정 선택 사항](application-setup.md#image_preset_options)
>* [이미지 사전 설정을 기준으로 이미지 자산 미리 보기](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)
