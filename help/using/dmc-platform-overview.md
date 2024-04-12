---
title: Adobe Dynamic Media Classic 프로그램 개요
description: Adobe Dynamic Media Classic 프로그램 및 전체 워크플로우 프로세스에 대한 개요입니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
feature: Dynamic Media Classic
role: Admin,User
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
topic: Administration
level: Beginner
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 17%

---

# Adobe Dynamic Media Classic 프로그램 개요{#adobe-scene-platform-overview}

Adobe Dynamic Media Classic은 통합되고 리치 미디어 관리, 게시 및 서비스 환경입니다. 웹, 인쇄물, 이메일 캠페인, 웹 포털, 데스크톱 및 장치를 비롯한 모든 마케팅 및 판매 채널에 리치 미디어를 제공할 수 있습니다.

참조: [플랫폼 개요](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/572_Platform%20Overview_converted%20renamed_Getting%20Started-AVS) 교육 비디오입니다.

## 워크플로우 프로세스 {#workflow-process}

주요 Adobe Dynamic Media Classic 워크플로우 단계는 다음과 같습니다.

* **에셋 업로드 및 관리** - 미디어 에셋을 Adobe Dynamic Media Classic에 업로드합니다. 시스템의 자산을 구성하고, 찾아보고, 검색할 수 있습니다. 에셋에 메타데이터를 적용할 수도 있습니다.

* **리치 미디어 만들기** - eCatalogs, 이미지 세트, 스핀 세트, 견본 세트, 혼합 미디어 세트, 기본 템플릿 및 FXG 템플릿과 같은 다양한 에셋 구성을 만들 수 있습니다.

* **게시 및 관리** - Adobe Dynamic Media Classic SaaS 네트워크에 자산을 게시합니다. 에셋이 게시될 때 에셋 상태를 모니터링합니다. 사용자 권한을 관리하고 보안을 유지합니다.

* **서비스** - Adobe Dynamic Media Classic SaaS 네트워크의 미디어를 웹 페이지, 애플리케이션 및 모바일 디바이스에 전달합니다. 미디어는 성능에 최적화되고 CDN 캐싱과 함께 제공됩니다. Adobe Dynamic Media Classic은 각 에셋에 대한 URL을 제공합니다. 자산을 게시하면 URL이 활성화됩니다.

![Adobe Dynamic Media Classic 워크플로 프로세스](/help/using/assets/gs_workflow.png)

## 단일 1차 이미지 및 단일 URL 호출 {#single-master-images-and-single-url-calls}

Adobe Dynamic Media Classic은 Adobe Dynamic Media Classic을 사용하여 단일 기본 에셋 및 URL 호출에서 동적으로 미디어를 게재할 수 있으므로 다른 시스템과 근본적으로 다릅니다.

Adobe Dynamic Media Classic으로 생성한 URL 문자열에는 에셋이 배달될 때 해당 에셋을 표시하는 방법을 서버에 알려 주는 지침이 포함되어 있습니다. 예를 들어 동일한 1차 이미지가 서로 다른 크기, 형식, 무게, 색상 및 확대/축소 보기로 제공될 수 있습니다. Adobe Dynamic Media Classic을 사용하여 미디어 에셋을 구축하고 게시하는 과정의 일부로 효과를 시각적으로 구성합니다. 이렇게 하면 기본 자산을 응용 프로그램에 제공하는 방법을 서버에 올바르게 알려주는 URL 호출을 만듭니다.

![Adobe Dynamic Media Classic은 동일한 1차 이미지를 크기와 형식이 다른 다양한 미디어에 제공할 수 있습니다.](/help/using/assets/gs_dynamic_publishing.png)
*Adobe Dynamic Media Classic은 크기나 대역폭에 관계없이 모든 화면에 일관된 품질 경험을 제공합니다.*

## 컨텐츠 캐싱 {#content-caching}

Adobe Dynamic Media Classic이 동적으로 생성하는 이미지는 캐시에 유용합니다. 일반적으로 이미지는 자신을 식별하는 고유한 URL 호출이 있는 JPEG 이미지입니다. 이미지는 컨텐츠를 더 빨리 제공하기 위해 인터넷에서 네트워크로 연결된 서버 시스템인 CDN(Content Delivery Network)을 통해 제공됩니다. 전 세계에 있는 서버에서 컴퓨터로 이미지가 배포됩니다. CDN 공급업체를 사용하여 캐싱 메커니즘을 구현하는 경우, CDN이 활성화된 Dynamic Media 이미지 서버를 가리키도록 서버 이름을 변경하기만 하면 됩니다. 모든 Adobe Dynamic Media Classic 버전에는 번들 CDN 캐싱이 포함되어 있습니다.
