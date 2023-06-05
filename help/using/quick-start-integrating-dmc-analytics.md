---
title: "빠른 시작: Adobe Dynamic Media Classic 및 Adobe Analytics 통합"
description: Adobe Dynamic Media Classic과 Adobe Analytics을 통합하여 신속하게 시작하고 실행할 수 있는 방법에 대한 소개 및 빠른 시작입니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: a8fa2414-af01-4a58-bb33-dfd12c1056cc
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 27%

---

# 빠른 시작: Adobe Dynamic Media Classic 및 Adobe Analytics 통합 {#quick-start-integrating-dmc-analytics}

Adobe Analytics는 여러 마케팅 채널을 통한 모든 온라인 이니셔티브의 통합 데이터를 측정, 분석 및 최적화할 수 있는 단일 장소를 마케터에게 제공하는 업계 선도적인 제품입니다.

Adobe Analytics을 Adobe Dynamic Media Classic과 통합하면 웹 사이트에서 Adobe Dynamic Media Classic 뷰어를 사용하는 웹 사이트 방문자의 동작에 대한 보고서를 얻을 수 있습니다. 예를 들어 웹 사이트 방문자가 Adobe Dynamic Media Classic 확대/축소 뷰어에서 확대/축소 대상을 클릭하면 Adobe Analytics이 이 작업을 기록합니다. Adobe Analytics 보고서는 Adobe Dynamic Media Classic 뷰어에서 사용자 활동에 대한 누적 정보를 수집할 수 있습니다.

Adobe Analytics 보고서를 사용하면 웹 사이트의 고객 활동을 명확하게 파악할 수 있습니다. 어떤 제품 프레젠테이션이 전환을 유도하고 어떤 것이 고객의 관심을 끌지 못하는지 결정할 수 있습니다.

참조: [Adobe Analytics에서 비디오 측정](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

>[!NOTE]
>
>Analytics를 Adobe Dynamic Media Classic과 통합하고 Analytics 보고서를 생성하려면 유효한 Adobe Analytics 계정이 필요합니다.

이 빠른 시작은 Adobe Analytics 계측 키트를 빨리 시작하고 실행하는 데 도움이 됩니다.

## 1. Adobe Dynamic Media Classic을 통해 Adobe Analytics에 로그인하고 Adobe Analytics 보고서 변수를 다운로드합니다

>[!NOTE]
>
>Adobe Analytics 보고서를 구성하고 Adobe Analytics 보고서 변수를 Adobe Dynamic Media Classic 이벤트에 일치시키려면 먼저 Adobe Analytics에서 웹 서비스 액세스 그룹의 구성원으로 추가되었는지 확인하십시오. 이 그룹의 구성원은 인터페이스에 설정된 권한에 관계없이 Experience Cloud의 웹 서비스 API를 통해 지정된 보고서 세트에 있는 모든 보고서에 액세스할 수 있습니다. 그룹에 멤버를 추가하려면 Adobe Analytics에서 **[!UICONTROL 관리 도구]** > **[!UICONTROL 사용자 관리]** > **[!UICONTROL 그룹 편집]**.

Adobe Dynamic Media Classic에서 웹 서비스 액세스 그룹의 구성원임을 확인한 후 **[!UICONTROL 설정]** > **[!UICONTROL 응용 프로그램 설정]** > **[!UICONTROL Adobe Analytics]**. Adobe Analytics 구성 페이지에서 **[!UICONTROL Adobe Analytics 로그인]**.

[Adobe Analytics에 로그인](log-analytics.md#log_in_to_adobe_analytics)을 참조하십시오.

Adobe Analytics 로그인 대화 상자에서 Experience Cloud 조직 ID(선택 사항)와 전체 자격 증명을 입력한 다음 을 선택합니다 **[!UICONTROL 로그인]**. 보고서 세트 드롭다운 메뉴에서 사용하려는 보고서 세트 이름을 선택합니다.

## 2. Adobe Analytics 보고서 변수를 Adobe Dynamic Media Classic 뷰어 이벤트 및 Adobe Dynamic Media Classic 변수에 할당

Adobe Analytics 구성 페이지에서 Adobe Analytics 보고서에 원하는 정보를 지정합니다. 정보를 보려는 각 Adobe Dynamic Media Classic 뷰어 이벤트에 대해 보고서 세트에서 Adobe Analytics 변수와 Adobe Dynamic Media Classic 변수를 선택합니다.

* 뷰어 이벤트는 보고서에서 측정하려는 사용자 이벤트에 대해 설명합니다.
* Adobe Dynamic Media Classic 변수는 보고서가 전달할 사용자 이벤트에 대한 데이터를 설명합니다.

Adobe Analytics 구성에서는 뷰어 이벤트를 활성화, 편집 및 삭제하는 도구도 제공합니다.

다음을 선택한 후 **[!UICONTROL 저장]** Adobe Analytics 구성 페이지에서 사용자 활동을 측정하기 위한 사용자 지정 추적 코드가 Adobe Dynamic Media Classic 뷰어에 삽입됩니다. 이 기능을 사용하면 Adobe Analytics 보고서에서 사용자 활동을 추적할 수 있습니다.

다음을 참조하십시오 [Adobe Analytics 보고서 구성](configuring-analytics-reports.md#configuring_adobe_analytics_reports).

## 3. Adobe Dynamic Media Classic 뷰어 게시

Adobe Dynamic Media Classic 뷰어를 게시하여 뷰어(Adobe Analytics 보고서에서 사용자 활동을 추적하는 코드와 함께)가 Adobe Dynamic Media Classic 서버에 로드되도록 합니다. 게시하면 이 정보가 뷰어에 포함되며 Adobe Analytics의 분석에 사용될 수 있습니다.

다음을 참조하십시오 [구성 정보 게시](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## 4. 웹 사이트에 Adobe Dynamic Media Classic 뷰어 배치

웹 사이트에 Adobe Analytics 추적 코드가 있는 Adobe Dynamic Media Classic 뷰어를 배치합니다.

## 5. Adobe Analytics 보고서를 보고 Adobe Analytics 통합 테스트

Adobe Analytics 보고서를 보려면, Adobe Analytics 웹 사이트로 이동합니다. [보고] 페이지에서는 데이터를 보고 그래프와 차트를 생성하여 각기 다른 뷰어로 사용자 활동을 측정할 수 있습니다.

다음을 참조하십시오 [Adobe Analytics 보고서를 보고 Adobe Analytics 통합 테스트](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report).
