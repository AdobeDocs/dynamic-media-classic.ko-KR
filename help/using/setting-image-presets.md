---
title: 이미지 사전 설정 설정
description: Adobe Dynamic Media Classic에서 이미지 사전 설정을 설정하는 방법을 알아봅니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic,Image Presets
role: User
exl-id: 336802cc-b032-49b2-b2e6-d699bc997ee5
topic: Content Management
level: Intermediate
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '667'
ht-degree: 32%

---

# 이미지 사전 설정 설정{#setting-up-image-presets}

매크로와 마찬가지로 이미지 사전 설정은 특정 이름으로 저장된 사전 정의된 크기 및 형식 지정 명령 모음입니다. 이미지 사전 설정의 작동 방식을 이해하려면 웹 사이트에서 각 제품 이미지를 500×500픽셀, 150×150픽셀 등 두 가지 크기로 표시해야 한다고 가정해 봅시다. 두 개의 이미지 사전 설정을 만듭니다. 하나는 500x500픽셀로 이미지를 표시하는 &quot;확대&quot;이고 다른 하나는 150×150픽셀로 이미지를 표시하는 &quot;썸네일&quot;입니다. Dynamic Media 이미지 서버는 &quot;확대&quot; 및 &quot;썸네일&quot; 크기로 이미지를 전달하기 위해 &quot;이미지 확대 사전 설정&quot; 및 &quot;썸네일 이미지 사전 설정&quot;의 정의를 조회합니다. 그런 다음 각 이미지 사전 설정의 크기 및 형식 지정 사양에 따라 이미지를 동적으로 생성합니다.

Adobe Dynamic Media Classic에는 사용자가 사용할 수 있도록 이미 설정된 몇 가지 &quot;모범 사례&quot; 이미지 사전 설정이 포함되어 있습니다. 관리자는 이미지 사전 설정을 만들 수도 있습니다. 이미지 사전 설정을 만들려면 처음부터 시작하거나 기존 이미지 사전 설정에서 시작하여 새 이름으로 저장합니다.

서버에서 동적으로 제공될 때 크기가 축소된 이미지는 선명도와 세부 사항이 손실될 수 있습니다. 이 때문에 각 이미지 사전 설정에는 특정 크기로 제공 시 이미지를 최적화하기 위한 형식 지정 컨트롤이 포함되어 있습니다. 이러한 컨트롤은 이미지가 웹 사이트나 응용 프로그램에 전달될 때 선명하고 선명하게 나타나도록 합니다.

## 이미지 사전 설정 만들기 {#creating-an-image-preset}

회사 관리자인 경우 이미지 사전 설정을 직접 만들 수 있습니다. 이미지 사전 설정을 만들거나 Adobe Dynamic Media Classic이 제공하는 기본 이미지 사전 설정으로 시작하여 편집하고 새 이름으로 저장할 수 있습니다.

**이미지 사전 설정을 만들려면:**

1. **[!UICONTROL 설정]** > **[!UICONTROL 이미지 사전 설정]**(으)로 이동합니다.

   이 화면에서 이미지 사전 설정 이름을 찾아 기존 이미지 사전 설정을 미리 볼 수 있습니다. 이미지 사전 설정 이름을 선택하면 [미리 보기] 창의 샘플 이미지 크기와 모양이 바뀝니다.

1. 다음 중 하나를 수행하십시오.

   * **이미지 사전 설정 만들기**: **[!UICONTROL 추가]**&#x200B;를 선택합니다.
   * **이미지 사전 설정 편집**: 만들려는 이미지 사전 설정과 가장 유사한 이미지 사전 설정을 찾은 다음 **[!UICONTROL 편집]**&#x200B;을 선택합니다.

1. 이미지 사전 설정의 이름을 입력합니다.
1. [너비] 및 [높이] 측정값을 픽셀 단위로 입력합니다. 이러한 측정값은 제공되는 이미지의 크기를 결정합니다.
1. [사전 설정 추가] 또는 [사전 설정 편집] 화면에 정보를 입력합니다. 자세한 내용은 [이미지 사전 설정 선택 사항](application-setup.md#image_preset_options)을 참조하십시오.

   Adobe Dynamic Media Classic은 다음과 같은 &quot;모범 사례&quot; 옵션 선택 사항을 시작할 것을 권장합니다.

   * **[!UICONTROL 형식]**: JPEG 또는 요구 사항에 맞는 다른 형식을 선택하십시오. 모든 웹 브라우저는 JPEG 이미지 형식을 지원합니다. 작은 파일 크기와 이미지 품질 사이의 적절한 균형을 제공합니다. 그러나 JPEG 이미지는 압축 설정이 너무 낮으면 원하지 않는 이미지 아티팩트를 가져올 수 있는 손실 압축 방식을 사용합니다. 이러한 이유로 Adobe Dynamic Media Classic에서는 압축 품질(슬라이더)을 75로 설정하는 것이 좋습니다. 이 설정은 이미지 품질과 작은 파일 크기의 적절한 균형을 유지합니다.

   * **[!UICONTROL 선명하게 하기]**: 선명하게 하기를 선택하지 마십시오. 이 선명하게 하기 필터는 **[!UICONTROL 언샵 마스킹]** 설정보다 적은 제어를 제공합니다.

   * **[!UICONTROL 다시 샘플링 모드]**: **[!UICONTROL 쌍입방]**&#x200B;을 선택하세요.

   * **[!UICONTROL 언샵 마스킹]**(USM): 다음 설정을 입력하십시오.

   | 사전 설정 유형 | 크기 | USM: 양 | USM: 반경 | USM: 임계값 |
   | --- | --- | --- | --- | --- |
   | 크로스셀(미니 썸네일) | 75×75 | 1.5 | 0.8 | 5 |
   | 썸네일 | 150×150 | 1.1 | 1 | 5 |
   | 주 | 350×350 | 1 | 1 | 6 |
   | 확대 | 500×500 | 1.2 | 1.2 | 5 |

1. **[!UICONTROL 저장]**&#x200B;을 선택합니다.

여기에 나열된 이미지 사전 설정을 만들기 위한 Adobe Dynamic Media Classic &quot;모범 사례&quot; 옵션은 일반적인 권장 사항이며, 선명하게 하기는 매우 주관적입니다. 이러한 &quot;모범 사례&quot; 설정은 2000× 2000 1차 이미지를 기반으로 합니다. 1차 파일의 크기가 크거나 작은 설정은 다를 수 있습니다. 언샵 마스킹 설정을 조정하려면 Adobe Dynamic Media Classic에서 다음 범위를 권장합니다.

* **[!UICONTROL 금액]**: `.8`에서 `1.5` 사이입니다.

* **[!UICONTROL 반경]**: `.6`에서 `2` 사이입니다.

* **[!UICONTROL 임계값]**: `1`부터 `6`까지.

이미지 사전 설정을 삭제하려면 이미지 사전 설정 화면에서 선택한 다음 **[!UICONTROL 삭제]**&#x200B;를 선택합니다.

>[!MORELIKETHIS]
>
>* [이미지 사전 설정 만들기 및 편집](application-setup.md#creating_and_editing_image_presets)
>* [이미지 사전 설정 옵션](application-setup.md#image_preset_options)
>* [이미지 사전 설정을 기반으로 이미지 에셋 미리 보기](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)
