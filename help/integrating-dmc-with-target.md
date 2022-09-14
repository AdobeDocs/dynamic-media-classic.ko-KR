---
title: Adobe Dynamic Media Classic과 Adobe Target Standard/Premium 통합
description: Adobe Dynamic Media Classic을 Adobe Target Standard/Premium과 통합하는 방법을 알아봅니다.
uuid: d1c07a52-b058-4ae3-a31d-44c43dc27f65
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 3b4add18-4191-475e-a3a3-0184367a25fc
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: c6f217fb-89cb-4c8d-aa7f-309fc42f7d46
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 0%

---

# Adobe Dynamic Media Classic과 Adobe Target Standard/Premium 통합 {#integrating-dmc-with-target}

통합하기 전에 [!DNL Adobe Dynamic Media Classic] with [!DNL Target Standard/Premium]에 Target URL을 입력해야 합니다. [!DNL Adobe Dynamic Media Classic] 응용 프로그램 일반 설정 화면입니다. Target URL을 가져와서 응용 프로그램 일반 설정 페이지에 입력하려면 다음을 수행하십시오.

1. in [!DNL Adobe Experience Cloud], 다음 위치에 로그인 [!DNL Target Standard/Premium] 계정이 필요합니다.
1. 로그인한 후 브라우저의 주소 표시줄에서 URL을 최대 및 까지 복사합니다 `.com`.

   예를 들어 *허구* 주소 표시줄의 URL(URL 경로에는 항상 슬래시가 포함되며, 이 예제에서처럼 슬래시는 포함되지 않음)은 다음과 같습니다 `https:\\www.myfictionalsite.com/categories/admin/home.do`, 이 부분만 복사합니다. *허구* URL: `https:\\www.myfictionalsite.com`.

1. in [!DNL Adobe Dynamic Media Classic], 이동 **[!UICONTROL 설정]** > **[!UICONTROL 애플리케이션 설정]**.
1. 응용 프로그램 일반 설정 페이지의 **[!UICONTROL Target 서버 이름(&amp;A)]** 필드에서 2단계에서 복사한 URL을 붙여넣습니다.
1. 선택 **[!UICONTROL 닫기]**.
