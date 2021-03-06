---
title: 이미지 사전 설정 설정
description: Adobe Dynamic Media Classic에서 이미지 사전 설정을 설정하는 방법을 알아봅니다.
uuid: 90530948-dee9-41bd-b39e-684140446abc
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 1ec39fe5-7b2a-4034-9570-6b5595f97052
feature: Dynamic Media Classic,Image Presets
role: User
exl-id: 336802cc-b032-49b2-b2e6-d699bc997ee5
source-git-commit: e47c22508230adbb1ece323be0c1413a3f27ad89
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 54%

---

# 이미지 사전 설정 설정{#setting-up-image-presets}

매크로와 마찬가지로 이미지 사전 설정은 특정 이름으로 저장된 사전 정의된 크기 및 형식 지정 명령 모음입니다. 이미지 사전 설정 작동 방식을 이해하려면 웹 사이트에서 각 제품 이미지를 두 개의 서로 다른 크기로 표시해야 한다고 가정합니다. 500 x 500 픽셀 및 150 x 150 픽셀 두 개의 이미지 사전 설정, 즉 500x500 픽셀에서 이미지를 표시하기 위한 &quot;확대&quot; 이미지 사전 설정과 150x150 픽셀에서 이미지를 표시하기 위한 &quot;썸네일&quot; 이미지 사전 설정을 만듭니다. 이미지를 &quot;확대&quot; 및 &quot;축소판&quot; 크기로 전달하려면 Dynamic Media 이미지 서버가 이미지 사전 설정 확대 및 축소판 이미지 사전 설정의 정의를 확인합니다. 그런 다음 각 이미지 사전 설정의 크기 및 형식 지정 사양에 따라 이미지를 동적으로 생성합니다.

Adobe Dynamic Media Classic에는 사용할 수 있도록 이미 설정된 몇 가지 &quot;우수 사례&quot; 이미지 사전 설정이 포함되어 있습니다. 관리자는 이미지 사전 설정도 만들 수 있습니다. 이미지 사전 설정을 만들려면 처음부터 시작하거나 기존 이미지 사전 설정에서 시작하여 새 이름으로 저장합니다.

서버에서 동적으로 제공될 때 크기가 축소된 이미지는 선명도와 세부 사항이 손실될 수 있습니다. 이 때문에 각 이미지 사전 설정에는 특정 크기로 제공 시 이미지를 최적화하기 위한 형식 지정 컨트롤이 포함되어 있습니다. 이러한 컨트롤을 사용하면 이미지를 웹 사이트나 애플리케이션에 제공할 때 선명하게 유지할 수 있습니다.

## 이미지 사전 설정 만들기 {#creating-an-image-preset}

회사 관리자는 고유한 이미지 사전 설정을 만들 수 있습니다. 이미지 사전 설정을 만들거나 Dynamic Media Classic에서 제공하는 기본 이미지 사전 설정으로 시작하고, 편집하고, 새 이름으로 저장할 수 있습니다.

**이미지 사전 설정을 만들려면:**

1. **[!UICONTROL 설정]** > **[!UICONTROL 이미지 사전 설정]**&#x200B;으로 이동합니다.

   이 화면에서 이미지 사전 설정 이름을 찾아 기존 이미지 사전 설정을 미리 볼 수 있습니다. 이미지 사전 설정 이름을 선택하면 [미리 보기] 창의 샘플 이미지 크기와 모양이 바뀝니다.

1. 다음 중 하나를 수행하십시오.

   * **이미지 사전 설정 만들기**  - 추가 **[!UICONTROL 를 선택합니다]**.
   * **이미지 사전 설정 편집**  - 만들려는 이미지 사전 설정과 가장 유사한 이미지 사전 설정을 탐색한 다음  **[!UICONTROL 편집]**&#x200B;을 선택합니다.

1. 이미지 사전 설정의 이름을 입력합니다.
1. [너비] 및 [높이] 측정값을 픽셀 단위로 입력합니다. 이러한 측정값은 제공되는 이미지의 크기를 결정합니다.
1. [사전 설정 추가] 또는 [사전 설정 편집] 화면에 정보를 입력합니다. 자세한 내용은 [이미지 사전 설정 선택 사항](application-setup.md#image_preset_options)을 참조하십시오.

   Dynamic Media Classic Adobe에서는 다음과 같은 &quot;우수 사례&quot; 선택 사항을 시작할 것을 권장합니다.

   * **[!UICONTROL 형식]**  - JPEG 또는 요구 사항에 맞는 다른 형식을 선택합니다. JPEG 이미지 형식은 모든 웹 브라우저에서 지원되며, 작은 파일 크기와 이미지 품질의 적절한 균형을 유지합니다. 그러나 JPEG 형식 이미지는 손실 있는 압축 구성을 사용하므로 압축 설정이 너무 낮으면 불필요한 이미지 아티팩트가 발생할 수 있습니다. 이러한 이유로 Adobe Dynamic Media Classic에서는 슬라이더에서 압축 품질을 75로 설정할 것을 권장합니다. 이 설정은 이미지 품질과 작은 파일 크기의 적절한 균형을 유지합니다.

   * **[!UICONTROL 선명도]**  - 선명도 선택 안 함(이 선명도 필터는 [언샵  **[!UICONTROL 매싱 설정]보다 덜 제어]** 를 제공합니다.)

   * **[!UICONTROL 샘플 모드]**  -  **[!UICONTROL Bi-Cubic을 선택합니다]**.

   * **[!UICONTROL 언샵 마스킹]** (USM) - 다음 설정을 입력합니다.

   | 사전 설정 유형 | 크기 | USM: 양 | USM: 반경 | USM: 임계값 |
   | --- | --- | --- | --- | --- |
   | 크로스셀(미니 썸네일) | 75x75 | 1.5 | 0.8 | 5 |
   | 썸네일 | 150x150 | 1.1 | 1 | 5개 |
   | 주 | 350x350 | 1 | 1 | 6 |
   | 확대 | 500x500 | 1.2 | 1.2 | 5개 |

1. **[!UICONTROL 저장]**&#x200B;을 선택합니다.

여기에 나열된 이미지 사전 설정을 만들기 위한 Adobe Dynamic Media Classic &quot;우수 사례&quot; 옵션은 일반적인 권장 사항입니다. 선명하게 하는 것은 매우 주관적입니다. 이 &quot;우수 사례&quot; 설정은 2000x2000 마스터 이미지를 기준으로 작성되었습니다. 더 크거나 작은 마스터의 설정은 이와 다를 수 있습니다. 언샵 마스킹 설정을 조정하려는 경우 Dynamic Media Classic에서 다음 범위를 권장합니다.

* **[!UICONTROL 금액]**  - 0.8에서 1.5 사이.

* **[!UICONTROL 반경]**  - .6과 2 사이.

* **[!UICONTROL 임계값]**  - 1부터 6까지입니다.

이미지 사전 설정을 삭제하려면 이미지 사전 설정 화면에서 해당 이미지 사전 설정을 선택한 다음 **[!UICONTROL 삭제]**&#x200B;를 선택합니다.

>[!MORELIKETHIS]
>
>* [이미지 사전 설정 만들기 및 편집](application-setup.md#creating_and_editing_image_presets)
>* [이미지 사전 설정 선택 사항](application-setup.md#image_preset_options)
>* [이미지 사전 설정을 기반으로 이미지 자산 미리 보기](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)

