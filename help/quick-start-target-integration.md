---
title: '"빠른 시작: Adobe Target Standard/Premium 통합"'
description: Adobe Dynamic Media Classic에서 Adobe Target Standard/Premium 통합 기술을 빠르게 시작하고 실행할 수 있도록 지원하기 위한 Adobe Target Standard/Premium 소개 및 빠른 시작.
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
source-git-commit: 36f9aa3c2b4dc66e4cb851c2ce6837ae0ad4f64c
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 10%

---

# 빠른 시작: Adobe Target Standard/Premium 통합{#quick-start-target-integration}

Adobe Target Standard/Premium은 마케터가 직접 제어하여 여러 A/B 및 다변량 테스트를 신속하고 지속적으로 실행하고, 효과를 측정하며, 세그멘테이션, 타깃팅 및 Automated Personalization을 통해 온라인 컨텐츠의 관련성을 높일 수 있습니다.

Adobe Dynamic Media Classic을 사용하면 Adobe Target Standard/Premium 캠페인에 대한 오퍼 및 오퍼 세트를 만들 수 있습니다. 예를 들어 동일한 리치 미디어 자산의 3가지 변형으로 오퍼 세트를 만들 수 있습니다. 그러면 Adobe Target Standard/Premium에서 더 나은 전환 상승도를 제공하는 자산을 결정하도록 할 수 있습니다. 기본 템플릿이나 개별 이미지에서 오퍼와 오퍼 집합을 만들 수 있습니다. 오퍼 세트가 Adobe Target Standard/Premium에 푸시되거나 저장되면 Adobe Target Standard/Premium에서 오퍼가 mbox 및 경험과 연결된 캠페인을 실행할 수 있습니다. 이러한 캠페인은 클릭스루 및 전환에 가장 적합한 웹 사이트의 변형을 결정합니다.

Dynamic Media Classic 콘텐츠의 사용자 지정을 확대하려면 Adobe Target Standard/Premium HTML 오퍼를 사용하십시오. 자세한 내용은 [Adobe Target Standard/Premium 제품 설명서](https://experienceleague.adobe.com/docs/target.html)를 참조하십시오.

>[!NOTE]
>
>Adobe Dynamic Media Classic에서 Adobe Target Standard/Premium을 사용하려면 유효한 Adobe Target Standard/Premium 계정이 필요합니다.

이 빠른 시작은 Adobe Target Standard/Premium HTML 오퍼 세트를 사용하여 빠르게 시작하고 실행할 수 있도록 설계되었습니다. 1-3 단계를 수행하십시오. 각 단계 뒤에는 자세한 정보를 확인할 수 있는 항목 제목의 상호 참조가 있습니다.

## 1. Application General Settings 페이지에서 Adobe Target Standard/Premium URL을 입력합니다

Adobe Dynamic Media Classic을 Adobe Target Standard/Premium과 통합하려면 Adobe Target Standard/Premium URL이 필요합니다. Adobe Target Standard/Premium URL의 일부를 `.com`까지 복사하고 **[!UICONTROL Servers]** 그룹, **[!UICONTROL Test&amp;Target 서버 이름]** 텍스트 필드에 Dynamic Media Classic **[!UICONTROL 응용 프로그램 일반 설정]** 페이지에 입력합니다. [Adobe Dynamic Media Classic과 Adobe Target Standard/Premium 통합](integrating-dmc-with-target.md#integrating-dmc-with-target)을 참조하십시오.

## 2. 오퍼 세트를 만듭니다

매개 변수화된 템플릿이나 이미지를 사용하여 오퍼 집합을 만듭니다. Target 오퍼 세트 페이지에서 HTML 오퍼 세트를 만듭니다. 이 페이지를 열려면 템플릿이나 이미지를 선택한 다음, 전역 탐색 막대에서 **[!UICONTROL 빌드]** > **[!UICONTROL Target 오퍼 세트]**&#x200B;로 이동합니다.

템플릿으로 오퍼를 만들려면 **[!UICONTROL 추가 및 미리 보기]**&#x200B;를 선택합니다. 추가 및 미리 보기 페이지에서 매개변수 값을 변경합니다.

이미지로 오퍼를 만들려면 이미지를 Test&amp;Analysis Workspace 오퍼 세트 페이지로 끌어다 놓습니다. **[!UICONTROL 미리 보기]**&#x200B;를 선택하고 이미지 또는 오퍼 세트의 모든 이미지에 대한 이미지 사전 설정을 선택합니다.

오퍼 집합을 만든 후 저장합니다.

[오퍼 세트 만들기](creating-offer-set.md#creating_an_offer_set)를 참조하십시오.

## 3. Adobe Target Standard/Premium으로 오퍼 세트를 푸시합니다

Target 오퍼 세트 테스트 페이지에서 **[!UICONTROL 푸시 오퍼]**&#x200B;를 선택하고 Test&amp;Target 로그인 대화 상자에 로그인 자격 증명을 입력합니다. [Adobe Target Standard/Premium](pushing-offer-sets-target.md#pushing_offer_sets_to_target)에 푸시 오퍼 세트를 참조하십시오.
