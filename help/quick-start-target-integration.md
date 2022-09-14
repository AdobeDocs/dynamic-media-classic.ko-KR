---
title: "빠른 시작: Adobe Target Standard/Premium 통합"
description: Adobe Dynamic Media Classic에서 Adobe Target Standard/Premium 통합 기술을 사용하여 빠르게 시작하고 실행할 수 있는 Adobe Target Standard/Premium 소개 및 빠른 시작.
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 7%

---

# 빠른 시작: Adobe Target Standard/Premium 통합{#quick-start-target-integration}

Adobe Target Standard/Premium은 마케터가 직접 제어하여 여러 A/B 및 다변량 테스트를 신속하고 지속적으로 실행하고, 효과를 측정하며, 세그멘테이션, 타깃팅 및 Automated Personalization을 통해 온라인 컨텐츠의 관련성을 높일 수 있습니다.

Adobe Dynamic Media Classic을 사용하면 Adobe Target Standard/Premium 캠페인에 대한 오퍼 및 오퍼 세트를 만들 수 있습니다. 예를 들어 동일한 리치 미디어 자산의 3가지 변형으로 오퍼 세트를 만들 수 있습니다. 그러면 Adobe Target Standard/Premium에서 더 나은 전환 상승도를 제공하는 자산을 결정하도록 할 수 있습니다. 기본 템플릿이나 개별 이미지에서 오퍼와 오퍼 집합을 만들 수 있습니다. 오퍼 세트가 Adobe Target Standard/Premium에 푸시되거나 저장되면 Adobe Target Standard/Premium에서 오퍼가 mbox 및 경험과 연결된 캠페인을 실행할 수 있습니다. 이러한 캠페인은 클릭스루 및 전환에 가장 적합한 웹 사이트의 변형을 결정합니다.

다이내믹 Adobe Dynamic Media Classic 컨텐츠를 보다 사용자 지정하려면 Adobe Target Standard/Premium HTML 오퍼을 사용하십시오. 자세한 내용은 [Adobe Target Standard/Premium 제품 설명서](https://experienceleague.adobe.com/docs/target.html) 추가 정보.

>[!NOTE]
>
>Adobe Dynamic Media Classic에서 Adobe Target Standard/Premium을 사용하려면 유효한 Adobe Target Standard/Premium 계정이 필요합니다.

이 빠른 시작은 Adobe Target Standard/Premium HTML 오퍼 세트를 사용하여 빠르게 시작하고 실행할 수 있도록 설계되었습니다. 1-3 단계를 수행하십시오. 각 단계 후에는 추가 정보를 찾을 수 있는 주제 제목에 대한 상호 참조가 있습니다.

## 1. Application General Settings 페이지에서 Adobe Target Standard/Premium URL을 입력합니다

Adobe Dynamic Media Classic을 Adobe Target Standard/Premium과 통합하려면 Adobe Target Standard/Premium URL이 필요합니다. Adobe Target Standard/Premium URL의 부분을 최대 및 포함하여 복사합니다. `.com`를 입력한 다음 Adobe Dynamic Media Classic에 입력합니다 **[!UICONTROL 응용 프로그램 일반 설정]** 페이지, **[!UICONTROL 서버]** 그룹, **[!UICONTROL Target 서버 이름(&amp;A)]** 텍스트 필드. 자세한 내용은 [Adobe Dynamic Media Classic과 Adobe Target Standard/Premium 통합](integrating-dmc-with-target.md#integrating-dmc-with-target).

## 2. 오퍼 세트를 만듭니다

매개 변수화된 템플릿이나 이미지를 사용하여 오퍼 집합을 만듭니다. HTML 오퍼 세트 테스트 및 Target 페이지에서 오퍼 세트를 만듭니다. 이 페이지를 열려면 템플릿이나 이미지를 선택한 다음 전역 탐색 막대에서 **[!UICONTROL 빌드]** > **[!UICONTROL 테스트 및 Target 오퍼 집합]**.

템플릿으로 오퍼를 만들려면 **[!UICONTROL 추가 및 미리 보기]**. 추가 및 미리 보기 페이지에서 매개변수 값을 변경합니다.

이미지로 오퍼를 만들려면 이미지를 Test&amp;Analysis Workspace 오퍼 세트 페이지로 끌어다 놓습니다. 선택 **[!UICONTROL 미리 보기]** 이미지 또는 오퍼 세트에 있는 모든 이미지에 대한 이미지 사전 설정 을 선택합니다.

오퍼 집합을 만든 후 저장합니다.

자세한 내용은 [오퍼 세트 만들기](creating-offer-set.md#creating_an_offer_set).

## 3. Adobe Target Standard/Premium으로 오퍼 세트를 푸시합니다

Target 오퍼 세트 페이지에서 을(를) 선택합니다 **[!UICONTROL 푸시 오퍼]**&#x200B;및 [Target 로그인] 대화 상자에 로그인 자격 증명을 입력합니다. 자세한 내용은 [Adobe Target Standard/Premium으로 오퍼 세트 푸시](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
