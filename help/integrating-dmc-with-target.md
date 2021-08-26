---
title: Dynamic Media Classic과 Adobe Target Standard/Premium 통합
description: Adobe Dynamic Media Classic을 Adobe Target Standard/Premium과 통합하는 방법을 알아봅니다.
uuid: d1c07a52-b058-4ae3-a31d-44c43dc27f65
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 3b4add18-4191-475e-a3a3-0184367a25fc
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: c6f217fb-89cb-4c8d-aa7f-309fc42f7d46
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 0%

---

# Dynamic Media Classic과 Adobe Target Standard/Premium 통합 {#integrating-dmc-with-target}

[!DNL Adobe Dynamic Media Classic]을 [!DNL Target Standard/Premium]과 통합하려면 먼저 [!DNL Adobe Dynamic Media Classic] 응용 프로그램 일반 설정 화면에 Target URL을 입력해야 합니다. Target URL을 가져와서 응용 프로그램 일반 설정 페이지에 입력하려면 다음을 수행하십시오.

1. [!DNL Adobe Experience Cloud]에서 [!DNL Target Standard/Premium] 계정에 로그인합니다.
1. 로그인한 후 브라우저의 주소 표시줄에 URL을 최대 및 `.com`까지 복사합니다.

   예를 들어, 주소 표시줄의 *가공상* URL(URL 경로에 항상 슬래시가 포함되고, 이 예에서처럼 백슬래시가 아님)이 `https:\\www.myfictionalsite.com/categories/admin/home.do`이면 *가공상* URL의 이 부분만 복사합니다. `https:\\www.myfictionalsite.com`

1. [!DNL Adobe Dynamic Media Classic]에서 **[!UICONTROL 설치]** > **[!UICONTROL 응용 프로그램 설정]**&#x200B;으로 이동합니다.
1. 응용 프로그램 일반 설정 페이지의 **[!UICONTROL Test&amp;Target 서버 이름]** 필드에서 복사한 URL을 2단계에서 붙여넣습니다.
1. **[!UICONTROL 닫기]**&#x200B;를 선택합니다.
