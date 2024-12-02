---
title: '빠른 시작: Adobe Target Standard/Premium 통합'
description: Adobe Dynamic Media Classic에서 Adobe Target Standard/Premium 통합 기술을 빠르게 시작하고 실행하는 데 도움이 되는 Adobe Target Standard/Premium 소개 및 빠른 시작
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
topic: Integrations
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---

# 빠른 시작: Adobe Target Standard/Premium 통합{#quick-start-target-integration}

Adobe Target Standard/Premium은 마케터의 직접 제어 기능을 제공합니다. 이렇게 하면 여러 A/B 및 다변량 테스트를 빠르고 지속적으로 실행하고 효과를 측정하는 데 도움이 될 수 있습니다. 그리고, 세분화, 타겟팅, Automated Personalization 등을 통해 온라인 콘텐츠의 관련성을 높일 수 있다.

Adobe Dynamic Media Classic을 사용하면 Adobe Target Standard/Premium 캠페인에 대한 오퍼 및 오퍼 세트를 만들 수 있습니다. 예를 들어 동일한 리치 미디어 에셋의 변형 세 개를 사용하여 오퍼 세트를 만들 수 있습니다. 그런 다음 Adobe Target Standard 또는 Premium을 통해 더 나은 전환 상승도를 제공하는 에셋을 결정할 수 있습니다. 기본 템플릿 또는 개별 이미지에서 오퍼 및 오퍼 세트를 만들 수 있습니다. 오퍼가 mbox 및 경험과 연결된 Adobe Target Standard/Premium에 오퍼 세트를 푸시하거나 저장한 후 Adobe Target Standard/Premium에서 캠페인을 실행할 수 있습니다. 이러한 캠페인은 클릭스루 및 전환에 가장 잘 수행될 수 있는 웹 사이트의 변형을 결정합니다.

다이내믹 Adobe Dynamic Media Classic 콘텐츠를 보다 효율적으로 사용자 지정하려면 Adobe Target Standard/Premium HTML 오퍼를 사용하십시오. 자세한 내용은 [Adobe Target Standard/Premium 제품 설명서](https://experienceleague.adobe.com/en/docs/target)를 참조하세요.

>[!NOTE]
>
>Adobe Target에서 Adobe Target Standard/Premium을 사용하려면 유효한 Adobe Dynamic Media Classic Standard/Premium 계정이 필요합니다.

이 빠른 시작은 Adobe Target Standard/Premium HTML 오퍼 세트를 빠르게 시작하고 실행할 수 있도록 설계되었습니다. 1-3 단계를 수행하십시오. 각 단계 후에는 추가 정보를 찾을 수 있는 주제 머리글에 대한 상호 참조가 있습니다.

## 1. 애플리케이션 일반 설정 페이지에서 Adobe Target Standard/Premium URL을 입력합니다

Adobe Dynamic Media Classic을 Adobe Target Standard/Premium과 통합하려면 Adobe Target Standard/Premium URL이 필요합니다. `.com`까지 Adobe Target Standard/Premium URL의 일부를 복사하여 **[!UICONTROL 서버]** 그룹의 **[!UICONTROL Test&amp;Target 서버 이름]** 텍스트 필드에 있는 Adobe Dynamic Media Classic **[!UICONTROL 응용 프로그램 일반 설정]** 페이지에 입력하십시오. [Adobe Dynamic Media Classic과 Adobe Target Standard/Premium 통합](integrating-dmc-with-target.md#integrating-dmc-with-target)을 참조하세요.

## 2. 오퍼 집합 만들기

매개 변수가 있는 템플릿 또는 이미지를 사용하여 오퍼 집합을 만듭니다. Test&amp;Target HTML 세트 페이지에서 오퍼 세트를 만들 수 있습니다. 이 페이지를 열려면 템플릿 또는 이미지를 선택한 다음 전역 탐색 모음에서 **[!UICONTROL 빌드]** > **[!UICONTROL Test&amp;Target 오퍼 집합]**(으)로 이동합니다.

템플릿을 사용하여 오퍼를 만들려면 **[!UICONTROL 추가 및 미리 보기]**&#x200B;를 선택하십시오. 추가 및 미리 보기 페이지에서 매개 변수 값을 변경합니다.

이미지가 있는 오퍼를 만들려면 이미지를 Test&amp;Target 오퍼 집합 페이지로 드래그합니다. **[!UICONTROL 미리 보기]**&#x200B;를 선택하고 이미지 또는 오퍼 집합에 있는 모든 이미지에 대한 이미지 사전 설정을 선택합니다.

오퍼 세트를 만든 후 저장합니다.

[오퍼 집합 만들기](creating-offer-set.md#creating_an_offer_set)를 참조하세요.

## 3. Adobe Target Standard/Premium으로 오퍼 집합 푸시

Test&amp;Target 오퍼 집합 페이지에서 **[!UICONTROL 오퍼 푸시]**&#x200B;를 선택하고 Test&amp;Target 로그인 대화 상자에 로그인 자격 증명을 입력합니다. [Adobe Target Standard/Premium으로 오퍼 집합 푸시](pushing-offer-sets-target.md#pushing_offer_sets_to_target)를 참조하세요.
