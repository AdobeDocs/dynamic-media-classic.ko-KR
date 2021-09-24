---
title: Adobe Analytics에 로그인
description: Adobe Dynamic Media Classic에서 Adobe Analytics에 로그인하는 방법을 알아봅니다.
uuid: 5614babe-1097-4228-a3dc-27e5a25366d5
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
source-git-commit: d18dbbf89a1bfe4df46cbe7d56cdf6f442595ddb
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 1%

---

# Adobe Analytics에 로그인{#log-in-to-adobe-analytics}

Adobe Analytics 보고서를 구성하고 Adobe Analytics 보고서 변수를 Dynamic Media Classic 이벤트에 일치시키기 위해 로그인하기 전에 Adobe Analytics에서 웹 서비스 액세스 그룹의 구성원인지 확인하십시오. 이 그룹의 구성원은 인터페이스에 설정된 권한에 관계없이 Experience Cloud의 웹 서비스 API를 통해 지정된 보고서 세트의 모든 보고서에 액세스할 수 있습니다. 그룹에 구성원을 추가하려면 Adobe Analytics에서 **[!UICONTROL 관리 도구]** > **[!UICONTROL 사용자 관리]** > **[!UICONTROL 그룹 편집]**&#x200B;으로 이동합니다.

로그인하면 Experience Cloud 조직 ID를 입력하여 최신 비디오 분석 구현을 사용할 수 있습니다. ID를 입력하지 않기로 선택해도 비디오 보고가 계속 작동합니다. 그러나 이로 인해 데이터가 Dynamic Media Classic 외부의 해당 클라이언트에 대한 다른 데이터와 올바르게 통합되지 않을 수 있습니다.

>[!NOTE]
>
>Adobe Analytics 계정이 로그인을 위해 Adobe IMS 기반 인증(Identity Management 시스템)으로 마이그레이션된 경우 직접 자격 증명을 입력할 수 없습니다.

**Adobe Dynamic Media Classic에서 Adobe Analytics에 로그인하려면 다음을 수행하십시오.**

Dynamic Media Classic과 Adobe Analytics OAuth를 통합함으로써 시작합니다. Dynamic Media Classic과의 Adobe Analytics OAuth 통합은 일반적으로 사용자당 한 번만 수행됩니다.

1. [Adobe 개발자 콘솔](https://developer.adobe.com/console)에 액세스합니다. 통합이 필요한 조직에 대한 관리자 권한이 계정에 있는지 확인합니다.
1. 홈 페이지의 오른쪽 위 모서리 근처에 있는 드롭다운 목록에서 해당 회사를 선택합니다. (아래 스크린샷은 정보 용도로만 제공됩니다.) 선택하는 실제 회사 이름은 다를 수 있습니다.)

   ![새 프로젝트를 만듭니다](assets/analytics-oauth1.png)

1. 다음 중 하나를 수행합니다.

   * 페이지 상단의 **[!UICONTROL 홈]** 탭에서 **[!UICONTROL 새 프로젝트 만들기]**&#x200B;를 선택합니다.
   * 페이지 상단의 **[!UICONTROL 프로젝트]** 탭에서 다음을 수행합니다. 페이지의 오른쪽 모서리에서 **[!UICONTROL 새 프로젝트 만들기]**&#x200B;를 선택합니다.

1. 프로젝트의 페이지에서 **[!UICONTROL API 추가]**&#x200B;를 선택합니다.
1. **[!UICONTROL API]** 페이지에서 **[!UICONTROL Adobe Analytics]**&#x200B;을 선택합니다.
1. 페이지의 오른쪽 아래 모서리에서 **[!UICONTROL 다음]**&#x200B;을 선택합니다.

   ![API 추가](assets/analytics-oauth2.png)

1. **[!UICONTROL API 구성]** 페이지에서 **[!UICONTROL 사용자 인증 OAuth]**&#x200B;를 선택합니다.
1. 페이지의 오른쪽 아래 모서리에서 **[!UICONTROL 다음]**&#x200B;을 선택합니다.
1. **[!UICONTROL API 구성]** 페이지에서 **[!UICONTROL OAUTH 2.0 Web]**&#x200B;을 선택합니다.
1. **[!UICONTROL 기본 리디렉션 URI]** 텍스트 필드에 표시된 대로 다음 경로를 입력합니다.

   `https://exploreadobe.com/dynamic-media-upgrade/`

1. **[!UICONTROL 리디렉션 URI 패턴]** 텍스트 필드에 표시된 대로 다음 경로를 입력합니다.

   `https://exploreadobe\.com/dynamic-media-upgrade/`

1. 페이지의 오른쪽 아래 모서리에서 **[!UICONTROL 구성된 API 저장]**&#x200B;을 선택합니다.
1. Adobe Analytics 페이지의 왼쪽에 있는 탐색 패널에서 **[!UICONTROL 자격 증명]**&#x200B;에서 **[!UICONTROL OAuth 웹]**&#x200B;을(를) 선택합니다.
1. **[!UICONTROL 자격 증명 세부 정보]**&#x200B;에서 다음을 수행합니다.
   * **[!UICONTROL 클라이언트 ID]**&#x200B;에서 **[!UICONTROL 복사]**&#x200B;를 선택하여 값을 복사합니다. 다음에 이어지는 Dynamic Media Classic 데스크탑 애플리케이션의 후속 Analytics 구성에 이 값이 필요합니다.
   * **[!UICONTROL 클라이언트 암호]**&#x200B;에서 **[!UICONTROL 클라이언트 암호 검색]**&#x200B;을 선택하여 연결된 값을 표시합니다. **[!UICONTROL 복사]**&#x200B;를 선택하여 값을 복사합니다. 다음에 이어지는 Dynamic Media Classic 데스크탑 애플리케이션의 후속 Adobe Analytics 구성에 이 값이 필요합니다.

**Dynamic Media Classic 데스크탑 애플리케이션에서 Adobe Analytics 구성**

>[!NOTE]
>
>Dynamic Media Classic에서 Adobe Analytics을 처음 구성한 후 구성을 재실행해야 하는 경우는 다음과 같습니다.
>
>* 새 보고서가 Analytics에 추가되고 사용자가 해당 새 보고서에 데이터 전송을 시작하려고 합니다.
>* 추적 서버가 Adobe Analytics에서 업데이트됩니다.
>* 새로운 추적 변수가 보고서에 도입되었으며 Dynamic Media Classic 사용자 인터페이스의 특정 뷰어 변수를 해당 새 Analytics 변수에 연결하려고 합니다.

>


1. Adobe Dynamic Media Classic 데스크탑 응용 프로그램의 오른쪽 위 모서리 근처에 있는 **[!UICONTROL 설정]** > **[!UICONTROL 응용 프로그램 설정]**&#x200B;으로 이동하십시오.
1. 왼쪽 패널의 **[!UICONTROL 응용 프로그램 설정]**&#x200B;에서 **[!UICONTROL Adobe Analytics]**&#x200B;을 선택합니다.
1. **[!UICONTROL Adobe Analytics 구성]** 페이지에서 **[!UICONTROL Adobe Analytics 로그인]**&#x200B;을 선택합니다.
1. **[!UICONTROL Adobe Analytics 로그인]** 대화 상자의 클라이언트 ID 필드 및 클라이언트 암호 필드에서 이전에 복사한 각 값을 붙여넣습니다.
1. IMS 로그인을 수행합니다.

   성공적으로 로그인하면 사용 가능한 회사에서 시작한 **[!UICONTROL COMPANIES]** 드롭다운 목록이 표시됩니다.

1. **[!UICONTROL 회사]** 드롭다운 목록에서 회사를 선택합니다.

   회사를 선택하면, 선택한 회사에 사용할 수 있는 보고서 세트에서 시작된 **[!UICONTROL SUITES]** 드롭다운 목록이 표시됩니다.

1. **[!UICONTROL SUITES]** 드롭다운 목록에서 보고서 세트를 선택합니다.

   >[!NOTE]
   >
   >기본적으로 사용자는 **[!UICONTROL COMPANIES]** 및 **[!UICONTROL SUITES]** 드롭다운 목록이 모두 비어 있다는 사실을 알고 있어야 합니다. 따라서 사용자는 각 목록에서 값을 선택해야 합니다. —>

1. 구성을 저장할 수 있도록 **[!UICONTROL 확인]**&#x200B;을 선택합니다.

>[!MORELIKETHIS]
>
>* [Adobe Analytics 보고서 구성](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

