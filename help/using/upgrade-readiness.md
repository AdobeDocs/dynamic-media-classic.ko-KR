---
title: 업그레이드 준비
description: ' [!DNL Adobe Dynamic Media Classic] 에서  [!DNL Dynamic Media] on [!DNL Adobe Experience Manager](으)로 이동하려는 경우 업그레이드 준비 검사 목록.'
feature: Dynamic Media Classic
role: Admin,User
exl-id: 86537998-b7e9-449c-83eb-6fd04533a00f
topic: Administration, Migration
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 1%

---

# 업그레이드 준비 검사 목록

다음 체크리스트를 사용하여 [!DNL Dynamic Media Classic]에서 [!DNL Dynamic Media](으)로의 업그레이드를 이해하고 준비하십시오.

|  | 작업 | 설명 |
| :--- | :--- | --- |
| **1단계: 라이선스** | 계약 실행 | Adobe 계정 팀은 트래픽 및 스토리지를 기반으로 사용자와 함께 작업하여 [!DNL Dynamic Media] 라이선스에서 갱신할 [!DNL Dynamic Media Classic] 라이선스에서 전환합니다. |
| **2단계: 준비** | 기능 사용 확인 | [!DNL Dynamic Media Classic]에서 사용 중인 기능을 [!DNL Dynamic Media]에서 사용할 수 있는지 확인하십시오. [기능 비교](/help/using/upgrade-feature-comparison.md) 페이지를 참조하세요. [!DNL Dynamic Media]에서 아직 사용할 수 없는 주요 기능:<br>· Visual Configurator(이미지 작성자, 이미지 렌더링)<br>· 이미지 템플릿(1:1 템플릿).<br>· 전자 카탈로그.<br>위의 기능을 사용하는 경우 [!DNL Dynamic Media Classic]을(를) 통해 해당 기능에 액세스할 수 있다고 가정하고 업그레이드를 수행할 수 있습니다. |
|   | 자산 식별 | 업그레이드에 사용할 에셋 및 사전 설정을 찾아 준비하십시오. |
| **3단계: 환경** | [!DNL Adobe Experience Manager] 업그레이드 | [!DNL Adobe Experience Manager]의 모든 인스턴스를 최신 버전으로 업데이트해야 합니다. |
|   | [!DNL Dynamic Media] 설정 | Adobe Consulting 또는 파트너가 자격 증명으로 [!DNL Dynamic Media]을(를) 구성합니다. |
| **4단계: 업그레이드** | 에셋 복제 | 업그레이드 프로세스 중에 지정된 [!DNL Dynamic Media Classic]개의 자산이 Dynamic Media에 복제됩니다. |
| **5단계: 관리 설정** | 사용자 및 권한 설정 | 사용자를 만들고 적절한 권한을 부여합니다. |
|   | 비디오 인코딩 프로필 설정 | 비디오 인코딩 프로필을 만듭니다. |
|   | 뷰어 사전 설정 설정 | 뷰어 사전 설정을 만듭니다. |
|   | 이미지 사전 설정 설정 | 이미지 사전 설정을 설정합니다. |
| **6단계: 유효성 검사** | 유효성 확인 | 사용 사례, 에셋, 링크 및 API를 확인합니다. |
