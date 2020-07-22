---
title: '"빠른 시작: Target Standard/Premium 통합"'
seo-title: '"빠른 시작: Target Standard/Premium 통합"'
description: 널
seo-description: Target Standard/Premium 통합 기술을 사용하여 신속하게 작업을 시작하고 실행할 수 있는 Adobe Target Standard/Premium 소개 및 빠른 시작을 참조하십시오.
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
translation-type: tm+mt
source-git-commit: 38f5cf5264f9775a225d354ed9dc2f6caee236f2
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 19%

---


# 빠른 시작: Target Standard/Premium 통합{#quick-start-target-integration}

Adobe Target Standard/Premium을 사용하면 마케터는 세분화, 타깃팅 및 자동화된 개인화를 통해 다양한 A/B 및 다변량 테스트를 신속하고 지속적으로 실행하고 효과를 측정하며 온라인 컨텐츠의 연관성을 높일 수 있습니다.

Dynamic Media Classic에서는 Target Standard/프리미엄 캠페인에 대한 오퍼 및 오퍼 세트를 만들 수 있습니다. 예를 들어 동일한 리치 미디어 자산의 세 가지 변형을 사용하여 오퍼 세트를 만들 수 있습니다. 그런 다음 Target Standard/Premium으로 전환율을 높이는 자산을 결정할 수 있습니다. 기본 템플릿이나 개별 이미지에서 오퍼와 오퍼 집합을 만들 수 있습니다. 오퍼가 mbox 및 경험과 연결된 Adobe Target Standard/Premium에 푸시되거나 저장된 후 Target Standard/Premium은 캠페인을 실행하여 클릭스루 및 전환에 가장 적합한 웹 사이트의 변형을 결정할 수 있습니다.

동적 Dynamic Media Classic 컨텐츠를 보다 맞춤화하려면 Target Standard/Premium HTML 오퍼를 사용하십시오. 자세한 내용은 Target Standard/Premium 제품 설명서를 참조하십시오.

>[!NOTE]
>
>Target Standard Classic에서 Dynamic Media/Premium을 사용하려면 유효한 Adobe Target Standard/Premium 계정이 필요합니다.

**빠른 시작**

이 빠른 시작은 Target Standard/프리미엄 HTML 오퍼 세트를 사용하여 빠르게 시작할 수 있도록 고안되었습니다. 1-3 단계를 수행하십시오. 각 단계 뒤에는 자세한 정보를 확인할 수 있는 항목 제목의 상호 참조가 있습니다.

**1. Enter your Target Standard/Premium URL in the Application General Settings screen.**

Target Standard/Premium과 통합하려면 Dynamic Media/프리미엄 URL이 필요합니다. Copy the portion of your Target Standard/Premium URL up to and including *.com*, and enter it in the Dynamic Media Classic Application General Settings screen. Dynamic Media [Classic과 Target Standard/Premium 통합을 참조하십시오](integrating-dmc-with-target.md#integrating-dmc-with-target).

**2. 오퍼 집합 만들기**

매개 변수화된 템플릿이나 이미지를 사용하여 오퍼 집합을 만듭니다. [Test&amp;Target 오퍼 집합] 화면에서 HTML 오퍼 집합을 만듭니다. To open this screen, select your template or images, and click **Build** > **Test&amp;Target Offer Set**.

템플릿으로 오퍼를 만들려면 추가 및 미리 **보기를 클릭합니다**. 추가 및 미리 보기 화면에서 매개 변수 값을 변경합니다.

이미지를 사용하여 오퍼를 만들려면 이미지를 [Test&amp;Target 오퍼 집합] 화면으로 드래그합니다. Click **Preview** to choose an Image Preset for an image or all the images in the offer set.

오퍼 집합을 만든 후 저장합니다.

[오퍼 집합 만들기](creating-offer-set.md#creating_an_offer_set)를 참조하십시오.

**3. 오퍼를 Target Standard/Premium으로 푸시합니다.**

In the Test&amp;Target Offer Set screen, click **Push Offers**, and enter your login credentials in the Test&amp;Target Login dialog box. 오퍼 [집합을 Target Standard/Premium으로 푸시를 참조하십시오](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
