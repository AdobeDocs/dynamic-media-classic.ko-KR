---
title: Adobe Analytics에 로그온
description: Adobe Dynamic Media Classic에서 Adobe Analytics에 로그온하는 방법에 대해 알아봅니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
topic: Integrations, Development
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 0%

---

# Adobe Analytics에 로그온{#log-in-to-adobe-analytics}

Adobe Analytics에서 웹 서비스 액세스 그룹의 구성원인지 확인합니다. 로그인하기 전에 Adobe Analytics 보고서를 구성하고 Adobe Analytics 보고서 변수를 Adobe Dynamic Media Classic 이벤트에 일치시키십시오. 이 그룹의 구성원은 지정된 보고서 세트의 모든 보고서에 액세스할 수 있습니다. 인터페이스에 설정된 권한에 관계없이 Experience Cloud의 웹 서비스 API를 사용하여 작업을 수행합니다. 그룹에 구성원을 추가하려면 Adobe Analytics에서 **[!UICONTROL 관리 도구]** > **[!UICONTROL 사용자 관리]** > **[!UICONTROL 그룹 편집]**(으)로 이동합니다.

로그인하면 Experience Cloud 조직 ID를 입력하여 최신 비디오 분석 구현을 사용할 수 있습니다. ID를 입력하지 않도록 선택하면 비디오 보고가 계속 작동합니다. 하지만 이로 인해 Adobe Dynamic Media Classic 외부에서 해당 클라이언트에 대한 다른 데이터와 데이터가 올바르게 통합되지 않을 수 있습니다.

>[!NOTE]
>
>Adobe Analytics 계정이 로그인을 위해 Adobe IMS 기반 인증(Identity Management 시스템)으로 마이그레이션된 경우 직접 자격 증명을 입력할 수 없습니다.

## Adobe Dynamic Media Classic에서 Adobe Analytics에 로그온 {#log-in-to-analytics-from-dmc}

Dynamic Media Classic을 Adobe Analytics OAuth와 통합해 보십시오. Dynamic Media Classic과의 Adobe Analytics OAuth 통합은 일반적으로 사용자당 한 번만 수행됩니다.

1. [Adobe Developer Console](https://developer.adobe.com/console)에 액세스합니다. 계정에 통합이 필요한 조직에 대한 관리자 권한이 있는지 확인하십시오.
1. 홈 페이지의 오른쪽 상단 모서리 근처에 있는 드롭다운 목록에서 적절한 회사를 선택합니다. (아래 스크린샷은 정보용으로만 사용되며, 선택하는 실제 회사 이름은 다를 수 있습니다.)

   ![새 프로젝트 만들기](assets/analytics-oauth1.png)

1. 다음 중 하나를 수행합니다.

   * 페이지 상단의 **[!UICONTROL 홈]** 탭에서 **[!UICONTROL 새 프로젝트 만들기]**&#x200B;를 선택합니다.
   * 페이지 상단의 **[!UICONTROL 프로젝트]** 탭에서 페이지의 오른쪽 모서리 근처에서 **[!UICONTROL 새 프로젝트 만들기]**&#x200B;를 선택합니다.

1. 프로젝트의 페이지에서 **[!UICONTROL API 추가]**&#x200B;를 선택합니다.
1. **[!UICONTROL API 추가]** 페이지에서 **[!UICONTROL Adobe Analytics]**&#x200B;을(를) 선택합니다.
1. 페이지의 오른쪽 아래 모서리에서 **[!UICONTROL 다음]**&#x200B;을 선택합니다.

   ![API 추가](assets/analytics-oauth2.png)

1. **[!UICONTROL `Configure API`]** 페이지에서 **[!UICONTROL 사용자 인증 OAuth]**&#x200B;을(를) 선택합니다.
1. 페이지의 오른쪽 아래 모서리에서 **[!UICONTROL 다음]**&#x200B;을 선택합니다.
1. **[!UICONTROL `Configure API`]** 페이지에서 **[!UICONTROL OAUTH 2.0 웹]**&#x200B;을 선택합니다.
1. **[!UICONTROL 기본 리디렉션 URI]** 텍스트 필드에 다음과 같이 경로를 정확하게 입력하십시오.

   `https://exploreadobe.com/dynamic-media-upgrade/`

1. **[!UICONTROL 리디렉션 URI 패턴]** 텍스트 필드에 다음 경로를 표시된 대로 정확하게 입력하십시오.

   `https://exploreadobe\.com/dynamic-media-upgrade/`

1. 페이지의 오른쪽 아래 모서리에서 **[!UICONTROL 구성된 API 저장]**&#x200B;을 선택합니다.
1. 탐색 패널의 Adobe Analytics 페이지 왼쪽에 있는 **[!UICONTROL 자격 증명]**&#x200B;에서 **[!UICONTROL OAuth 웹]**&#x200B;을 선택합니다.
1. **[!UICONTROL 자격 증명 세부 정보]**&#x200B;에서 다음을 수행하십시오.
   * **[!UICONTROL 클라이언트 ID]**&#x200B;에서 **[!UICONTROL 복사]**&#x200B;를 선택하여 값을 복사합니다. Dynamic Media Classic 데스크탑 애플리케이션에서 따라야 하는 후속 Analytics 구성에는 이 값이 필요합니다.
   * **[!UICONTROL 클라이언트 암호]**&#x200B;에서 **[!UICONTROL 클라이언트 암호 검색]**&#x200B;을 선택하여 연결된 값을 표시합니다. 값을 복사하려면 **[!UICONTROL 복사]**&#x200B;를 선택하십시오. 다음에 오는 Dynamic Media Classic 데스크탑 애플리케이션의 후속 Adobe Analytics 구성에 이 값이 필요합니다.

## Adobe Dynamic Media Classic에서 Adobe Analytics 구성 {#configure-analytics-in-dmc}

>[!NOTE]
>
>Dynamic Media Classic에서 Adobe Analytics을 처음 구성한 후 구성을 다시 실행해야 하는 경우는 다음과 같습니다.
>
>* 새 보고서가 Analytics에 추가되고 사용자가 해당 새 보고서에 데이터를 보내기 시작하려고 합니다.
>* 추적 서버는 Adobe Analytics에서 업데이트됩니다.
>* 새 추적 변수는 보고서에 도입되며 Dynamic Media Classic 사용자 인터페이스의 특정 뷰어 변수를 해당 새 Analytics 변수에 연결하려고 합니다.
>

1. Adobe Dynamic Media Classic 데스크톱 응용 프로그램의 오른쪽 상단 모서리에서 **[!UICONTROL 설정]** > **[!UICONTROL 응용 프로그램 설정]**(으)로 이동합니다.
1. 왼쪽 패널의 **[!UICONTROL 응용 프로그램 설정]**&#x200B;에서 **[!UICONTROL Adobe Analytics]**&#x200B;을(를) 선택합니다.
1. **[!UICONTROL Adobe Analytics 구성]** 페이지에서 **[!UICONTROL Adobe Analytics 로그인]**&#x200B;을 선택합니다.
1. **[!UICONTROL Adobe Analytics 로그인]** 대화 상자의 **[!UICONTROL 클라이언트 ID]** 필드와 **[!UICONTROL 클라이언트 암호]** 필드에 이전에 복사한 각각의 값을 붙여 넣습니다.
1. 대화 상자의 오른쪽 아래 모서리에서 **[!UICONTROL 로그인]**&#x200B;을 선택하고 Adobe IMS(Identity Management 서비스) 로그인을 수행합니다.

   성공적으로 로그인하면 사용 가능한 회사에서 시작한 **[!UICONTROL 회사]** 드롭다운 목록과 함께 Adobe Analytics 로그인 대화 상자가 다시 나타납니다.

1. **[!UICONTROL 회사]** 드롭다운 목록에서 회사를 선택합니다.

   회사를 선택하면 선택한 회사에 사용할 수 있는 보고서 세트에 의해 시작된 **[!UICONTROL SUITES]** 드롭다운 목록이 표시됩니다.

1. **[!UICONTROL 세트]** 드롭다운 목록에서 보고서 세트를 선택합니다.

   >[!NOTE]
   >
   >기본적으로 사용자는 **[!UICONTROL COMPANIES]** 및 **[!UICONTROL SUITES]** 드롭다운 목록이 모두 비어 있다는 사실을 알고 있어야 합니다. 따라서 사용자는 각 목록에서 값을 선택해야 합니다.

1. 구성을 저장하려면 **[!UICONTROL 확인]**&#x200B;을 선택하세요.

   >[!NOTE]
   >
   >**[!UICONTROL Adobe Analytics 서버]** 필드는 **[!UICONTROL 확인]**&#x200B;을 선택하면 Analytics 네임스페이스와 일치하는 추천 타사 추적 서버로 채워집니다. 다른 추적 서버를 사용하는 경우 이 필드에서 업데이트하여 데이터 손실을 방지합니다.

1. Adobe Analytics 구성 페이지의 왼쪽 아래에서 **[!UICONTROL 저장]**&#x200B;을 선택하여 Adobe Analytics 계정 구성을 업데이트합니다.

>[!MORELIKETHIS]
>
>* [Adobe Analytics 보고서 구성](configuring-analytics-reports.md#configuring_adobe_analytics_reports)
