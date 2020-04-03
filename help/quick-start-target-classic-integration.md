---
title: '"빠른 시작:Target Classic 통합"'
seo-title: '"빠른 시작:Target Classic 통합"'
description: 널
seo-description: Adobe Target Classic에 대한 소개 및 빠른 시작을 통해 Target Classic 통합 기술을 신속하게 시작하고 실행할 수 있습니다.
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# 빠른 시작:Target Classic 통합{#quick-start-target-classic-integration}

Adobe Target Classic을 사용하면 마케터는 직접 여러 A/B 및 다변량 테스트를 신속하고 지속적으로 실행할 수 있고, 효과성을 측정할 수 있으며, 세분화, 타깃팅 및 자동화된 개인화를 통해 온라인 컨텐츠의 연관성을 높일 수 있습니다.

Scene7 Publishing Systems를 사용하면 Target Classic 캠페인에 대한 오퍼 및 오퍼 세트를 만들 수 있습니다. 예를 들어 동일한 리치 미디어 자산의 세 가지 변형을 사용하여 오퍼 세트를 만들 수 있습니다. 그런 다음 Target Classic에서 전환 증가를 제공하는 자산을 결정하도록 할 수 있습니다. 기본 템플릿이나 개별 이미지에서 오퍼와 오퍼 집합을 만들 수 있습니다. 오퍼 세트가 Adobe Target Classic에 푸시되거나 저장된 후 오퍼가 mbox 및 경험과 연관되어 있는 Target Classic에서는 캠페인을 실행하여 클릭스루 및 전환에 가장 적합한 웹 사이트의 변형을 결정할 수 있습니다.

다이내믹 Dynamic Media Classic 컨텐츠를 보다 맞춤화하려면 Target Classic HTML 오퍼를 사용하십시오. 자세한 내용은 Target Classic 제품 설명서를 참조하십시오.

>[!NOTE]
>
>Scene7 Publishing System에서 Target Classic을 사용하려면 유효한 Adobe Target Classic 계정이 필요합니다.

**빠른 시작**

이 빠른 시작은 Target Classic HTML 오퍼 집합을 빠르게 시작하고 실행하는 데 도움이 됩니다. 1-3 단계를 수행하십시오. 각 단계 뒤에는 자세한 정보를 확인할 수 있는 항목 제목의 상호 참조가 있습니다.

**1. Enter your Target Classic URL in the Application General Settings screen.**

Target Classic과 통합하려면 Target Classic URL이 필요합니다. Copy the portion of your Target Classic URL up to and including *.com*, and enter it in the Dynamic Media Classic Application General Settings screen. Dynamic [Media Classic과 Target Classic 통합을 참조하십시오](integrating-scene7-target-classic.md#integrating_scene7_with_target_classic).

**2. 오퍼 집합 만들기**

매개 변수화된 템플릿이나 이미지를 사용하여 오퍼 집합을 만듭니다. [Target Classic 오퍼 집합] 화면에서 HTML 오퍼 집합을 만듭니다. To open this screen, select your template or images, and click **Build** > **Target Classic Offer Set**.

템플릿으로 오퍼를 만들려면 추가 및 미리 보기를 **클릭합니다**. [추가 및 미리 보기] 화면에서 매개 변수 값을 변경합니다.

이미지가 있는 오퍼를 만들려면 이미지를 Target Classic 오퍼 세트 화면으로 드래그합니다. Click **Preview** to choose an Image Preset for an image or all the images in the offer set.

오퍼 집합을 만든 후 저장합니다.

[오퍼 집합 만들기](creating-offer-set.md#creating_an_offer_set)를 참조하십시오.

**3. Push the offer set to Target Classic**

In the Target Classic Offer Set screen, click **Push Offers**, and enter your login credentials in the Target Classic Login dialog box. See [Pushing offer sets to Target Classic](pushing-offer-sets-target-classic.md#pushing_offer_sets_to_target_classic).
