---
title: Adobe Target Standard/Premium과 Adobe Dynamic Media Classic 통합
description: Adobe Dynamic Media Classic을 Adobe Target Standard/Premium과 통합하는 방법을 알아봅니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: c6f217fb-89cb-4c8d-aa7f-309fc42f7d46
topic: Integrations, Development
level: Experienced
source-git-commit: 914fde11270dc731a261da3305b29dd573584d93
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 0%

---

# Adobe Target Standard/Premium과 Adobe Dynamic Media Classic 통합 {#integrating-dmc-with-target}

[!DNL Adobe Dynamic Media Classic]을(를) [!DNL Target Standard/Premium]과(와) 통합하려면 먼저 [!DNL Adobe Dynamic Media Classic] 응용 프로그램 일반 설정 화면에 Target URL을 입력해야 합니다. Target URL을 가져와서 [응용 프로그램 일반 사항 설정] 페이지에 입력하려면 다음을 수행합니다.

1. [!DNL Adobe Experience Cloud]에서 [!DNL Target Standard/Premium] 계정에 로그인합니다.
1. 로그인 후 브라우저의 주소 표시줄에 `.com`을(를) 포함하여 URL을 복사합니다.

   예를 들어, 주소 표시줄의 *가상* URL(URL 경로에 항상 슬래시가 포함되어 있고 이 예제와 같이 역슬래시가 아닌 슬래시가 포함되어 있음)이 `https:\\www.myfictionalsite.com/categories/admin/home.do`인 경우 *가상* URL `https:\\www.myfictionalsite.com`의 이 부분만 복사하십시오.

1. [!DNL Adobe Dynamic Media Classic]에서 **[!UICONTROL 설정]** > **[!UICONTROL 응용 프로그램 설정]**(으)로 이동합니다.
1. 응용 프로그램 일반 설정 페이지의 **[!UICONTROL Test&amp;Target 서버 이름]** 필드에 2단계에서 복사한 URL을 붙여 넣습니다.
1. **[!UICONTROL 닫기]**&#x200B;를 선택합니다.
