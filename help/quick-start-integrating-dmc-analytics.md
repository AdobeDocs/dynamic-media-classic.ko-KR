---
title: '"빠른 시작:Dynamic Media Classic 및 Adobe Analytics " 통합'
seo-title: '"빠른 시작:Dynamic Media Classic 및 Adobe Analytics " 통합'
description: 널
seo-description: 빠르게 시작하고 실행하는 데 도움이 되는 Dynamic Media Classic 및 Adobe 분석 통합을 소개하는 소개 및 빠른 시작.
uuid: 3f9e2c91-15d4-4b53-8220-9b1ca57c0b1d
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: abec9a85-013c-4030-b129-bf27a89cb464
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 44%

---


# 빠른 시작:Dynamic Media Classic 및 Adobe Analytics {#quick-start-integrating-dmc-analytics} 통합

Adobe Analytics는 여러 마케팅 채널을 통한 모든 온라인 이니셔티브의 통합 데이터를 측정, 분석 및 최적화할 수 있는 단일 장소를 마케터에게 제공하는 업계 선도적인 제품입니다.

Adobe Analytics을 Dynamic Media Classic과 통합한 후 웹 사이트에서 Dynamic Media Classic 뷰어를 사용하는 웹 사이트 방문자의 동작에 대한 보고서를 볼 수 있습니다. 예를 들어 웹 사이트 방문자가 Dynamic Media Classic 확대/축소 뷰어에서 확대/축소 타겟을 클릭하면 Adobe Analytics에서 이 작업을 기록합니다. Adobe Analytics 보고서는 Dynamic Media Classic 뷰어에서 사용자 활동에 대한 누적 정보를 수집할 수 있습니다.

Adobe Analytics 보고서를 사용하면 웹 사이트의 고객 활동을 명확하게 파악할 수 있습니다. 전환을 발생시키는 제품 프레젠테이션과 고객의 관심을 끌지 못한 제품 프레젠테이션을 확인할 수 있습니다.

[Adobe Analytics에서 비디오 측정](https://docs.adobe.com/content/help/en/media-analytics/using/media-overview.html)을 참조하십시오.

>[!NOTE]
>
>Analytics를 Dynamic Media Classic과 통합하고 Analytics 보고서를 생성하려면 유효한 Adobe Analytics 계정이 필요합니다.

**빠른 시작**

이 빠른 시작은 Adobe Analytics 계측 키트를 빨리 시작하고 실행하는 데 도움이 됩니다.

**1. Dynamic Media Classic을 통해 Adobe Analytics에 로그인하고 Adobe Analytics 보고서 변수** 다운로드

>[!NOTE]
>
>Adobe Analytics 보고서를 구성하고 Adobe Analytics 보고서 변수를 Dynamic Media Classic 이벤트와 일치시키기 전에 Adobe Analytics에서 웹 서비스 액세스 그룹의 구성원으로 추가되었는지 확인합니다. 이 그룹의 구성원은 인터페이스에 설정된 권한에 상관없이 Marketing Cloud의 웹 서비스 API를 통해 지정된 보고서 세트의 모든 보고서에 액세스할 수 있습니다. 그룹에 구성원을 추가하려면, Adobe Analytics에서 **관리 도구** > **사용자 관리** > **그룹 편집**&#x200B;을 클릭합니다.

웹 서비스 액세스 그룹의 구성원인지 확인한 후 Dynamic Media Classic에서 **설정** > **응용 프로그램 설정** > **Adobe Analytics**&#x200B;을 클릭합니다. Adobe Analytics 구성 페이지에서 **Adobe Analytics 로그인**&#x200B;을 클릭합니다.

[Adobe Analytics에 로그인](log-analytics.md#log_in_to_adobe_analytics)을 참조하십시오.

Adobe Analytics 로그인 대화 상자에서 Marketing Cloud 조직 ID(선택 사항) 및 전체 자격 증명을 입력한 다음 **로그인**&#x200B;을 클릭합니다. 보고서 세트 드롭다운 메뉴에서 사용하려는 보고서 세트 이름을 선택합니다.

**2. Adobe Analytics 보고서 변수를 Dynamic Media Classic 뷰어 이벤트 및 Dynamic Media Classic 변수**&#x200B;에 할당

Adobe Analytics 구성 페이지에서 Adobe Analytics 보고서에 원하는 정보를 지정합니다. 정보를 원하는 각 Dynamic Media Classic 뷰어 이벤트에 대해 보고서 세트에서 Adobe Analytics 변수와 Dynamic Media Classic 변수를 선택합니다.

* 뷰어 이벤트는 보고서에서 측정하려는 사용자 이벤트에 대해 설명합니다.
* Dynamic Media Classic 변수는 보고서를 제공할 사용자 이벤트에 대한 데이터를 설명합니다.

Adobe Analytics 구성에서는 뷰어 이벤트를 활성화, 편집 및 삭제하는 도구도 제공합니다.

[Adobe Analytics 구성] 화면에서 [저장]을 클릭하면 사용자 활동을 측정하기 위해 사용자 정의된 추적 코드가 Dynamic Media Classic 뷰어에 삽입됩니다. 이 기능을 사용하면 Adobe Analytics 보고서에서 사용자 활동을 추적할 수 있습니다.

[Adobe Analytics 보고서 구성](configuring-analytics-reports.md#configuring_adobe_analytics_reports)을 참조하십시오.

**3. Dynamic Media Classic 뷰어 게시**

Dynamic Media Classic 뷰어를 게시하여 뷰어(Adobe Analytics 보고서의 사용자 활동 추적 코드 포함)가 Dynamic Media Classic 서버에 로드되도록 합니다. 게시하면 이 정보가 뷰어에 포함되며 Adobe Analytics의 분석에 사용될 수 있습니다.

[구성 정보 게시](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information)를 참조하십시오.

**4. 웹 사이트에 Dynamic Media Classic 뷰어 배치**

웹 사이트에 Adobe Analytics 추적 코드가 포함된 Dynamic Media Classic 뷰어를 배치합니다.

**5. Adobe Analytics 보고서를 보고 Adobe Analytics 통합 테스트**

Adobe Analytics 보고서를 보려면, Adobe Analytics 웹 사이트로 이동합니다. [보고] 페이지에서는 데이터를 보고 그래프와 차트를 생성하여 각기 다른 뷰어로 사용자 활동을 측정할 수 있습니다.

[Adobe Analytics 보고서를 보고 Adobe Analytics 통합 테스트](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report)를 참조하십시오.
