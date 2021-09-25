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
source-git-commit: e3c2dcaa245e486ada62edd554db5a39d495483e
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 20%

---

# Adobe Analytics에 로그인{#log-in-to-adobe-analytics}

Adobe Analytics 보고서를 구성하고 Adobe Analytics 보고서 변수를 Dynamic Media Classic 이벤트에 일치시키기 위해 로그인하기 전에 Adobe Analytics에서 웹 서비스 액세스 그룹의 구성원인지 확인하십시오. 이 그룹의 구성원은 인터페이스에 설정된 권한에 관계없이 Experience Cloud의 웹 서비스 API를 통해 지정된 보고서 세트의 모든 보고서에 액세스할 수 있습니다. 그룹에 구성원을 추가하려면 Adobe Analytics에서 **[!UICONTROL 관리 도구]** > **[!UICONTROL 사용자 관리]** > **[!UICONTROL 그룹 편집]**&#x200B;으로 이동합니다.

로그인하면 Experience Cloud 조직 ID를 입력하여 최신 비디오 분석 구현을 사용할 수 있습니다. ID를 입력하지 않기로 선택해도 비디오 보고가 계속 작동합니다. 그러나 이로 인해 데이터가 Dynamic Media Classic 외부의 해당 클라이언트에 대한 다른 데이터와 올바르게 통합되지 않을 수 있습니다.

>[!NOTE]
>
>Adobe Analytics 계정이 로그인을 위해 Adobe IMS 기반 인증(Identity Management 시스템)으로 마이그레이션된 경우 직접 자격 증명을 입력할 수 없습니다.

**Adobe Analytics에 로그인하려면:**

1. Adobe Dynamic Media Classic 페이지의 오른쪽 위 모서리 근처에 있는 **[!UICONTROL 설정]** > **[!UICONTROL 애플리케이션 설정]**&#x200B;으로 이동합니다.
1. 왼쪽 창의 **[!UICONTROL 응용 프로그램 설정]**&#x200B;에서 **[!UICONTROL Adobe Analytics]**&#x200B;을 탭합니다.
1. Adobe Analytics 구성 페이지에서 **[!UICONTROL Adobe Analytics 로그인]**&#x200B;을 누릅니다.
1. **[!UICONTROL Adobe Analytics 로그인]** 대화 상자에서 회사 이름, Experience Cloud 조직 ID(선택 사항), 사용자 이름 및 **[!UICONTROL 암호]** 텍스트 필드에 *공유 암호* 키를 입력합니다.

   Analytics Admin Console에서 *공유 암호* 키를 검색할 수 있습니다. [사용자 계정에 대한 API 자격 증명을 가져오는 방법](https://github.com/AdobeDocs/analytics-2.0-apis/blob/master/create-oauth-client.md)을 참조하십시오.

1. **[!UICONTROL 로그인]**&#x200B;을 선택합니다.
1. **[!UICONTROL 보고서 세트]** 드롭다운 메뉴에서 보고서 세트를 선택한 다음 **[!UICONTROL 확인]**&#x200B;을 선택합니다.

   >[!NOTE]
   >
   >Adobe Analytics에 처음 로그인하면 보고서 세트 드롭다운 목록이 비어 있습니다. 처음 로그인할 때는 보고서 세트를 선택하지 않습니다. 처음 로그인한 후 로그아웃하고 Adobe Analytics 화면으로 돌아갑니다. 다시 로그인하면 보고서 세트를 선택할 수 있습니다.

>[!MORELIKETHIS]
>
>* [Adobe Analytics 보고서 구성](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

