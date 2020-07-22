---
title: Adobe Dynamic Media Classic 플랫폼 개요
seo-title: Adobe Dynamic Media Classic 플랫폼 개요
description: 널
seo-description: Dynamic Media Classic 플랫폼 및 워크플로우 프로세스에 대한 개요입니다.
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 32%

---


# Adobe Dynamic Media Classic 플랫폼 개요{#adobe-scene-platform-overview}

Dynamic Media Classic은 통합 리치 미디어 관리, 게시 및 서비스 환경입니다. 웹, 인쇄물, 이메일 캠페인, 웹 포털, 데스크톱 및 장치를 비롯한 모든 마케팅 및 판매 채널에 리치 미디어를 제공할 수 있습니다.

## 워크플로우 프로세스 {#workflow-process}

주요 Dynamic Media 클래식 워크플로우 단계는 다음과 같습니다.

* **자산 업로드 및 관리**&#x200B;미디어 자산을 Dynamic Media Classic에 업로드합니다. 시스템의 자산을 구성하고, 찾아보고, 검색할 수 있습니다. 메타데이터를 자산에 적용할 수도 있습니다.

* **리치 미디어**&#x200B;를 제작eCatalogs, 이미지 세트, 스핀 세트, 견본 집합, 혼합 미디어 집합, 기본 템플릿 및 FXG 템플릿과 같은 다양한 자산 구성을 만듭니다. 자세한 내용은 리치 미디어 정보를 참조하십시오.

* **자산 게시 및 관리** Dynamic Media Classic Saas 네트워크에 자산을 게시하고 게시 시 자산 상태를 모니터링하며 사용자 권한을 관리하고 보안을 유지합니다.

* **서버** Dynamic Media Classic SaaS 네트워크에서 웹 페이지, 애플리케이션 및 모바일 디바이스로 미디어 전달 미디어는 성능 최적화 기능으로 전달되고 CDN 캐싱으로 전달됩니다. Dynamic Media Classic에서는 각 자산에 대한 URL을 제공합니다. 자산을 게시하면 URL이 활성화됩니다.

![Dynamic Media Classic 워크플로우 프로세스](/help/assets/gs_workflow.png)

## 단일 마스터 이미지 및 단일 URL 호출 {#single-master-images-and-single-url-calls}

Dynamic Media Classic은 Dynamic Media Classic을 사용하여 단일 마스터 자산 및 URL 호출에서 동적으로 미디어를 전달할 수 있으므로 다른 시스템과 근본적으로 다릅니다.

Dynamic Media Classic으로 생성하는 URL 문자열에는 자산이 전달될 때 자산을 표시하는 방법을 설명하는 지침이 포함되어 있습니다. 예를 들어 동일한 마스터 이미지를 다른 크기, 형식, 두께, 색상 및 확대/축소 보기로 제공할 수 있습니다. Dynamic Media Classic을 사용하여 미디어 에셋을 작성하고 게시하는 작업의 일부로 효과를 시각적으로 구성할 수 있습니다. 이렇게 하면 마스터 자산을 애플리케이션에 제공하는 방법을 서버에 올바르게 지정하는 URL 호출이 만들어집니다.

![Dynamic Media Classic에서는 서로 다른 크기와 형식의 다양한 미디어에 동일한 마스터 이미지를 전달할 수 있습니다.](/help/assets/gs_dynamic_publishing.png)

## 컨텐츠 캐싱 {#content-caching}

Dynamic Media Classic에서 동적으로 생성하는 이미지는 캐시 친화적입니다. 대부분의 경우 JPEG 이미지는 고유한 URL 호출이 있는 JPEG 이미지입니다. 이미지는 컨텐츠를 더 빨리 제공하기 위해 인터넷에서 네트워크로 연결된 서버 시스템인 CDN(Content Delivery Network)을 통해 제공됩니다. 전 세계에 있는 서버에서 컴퓨터로 이미지가 배포됩니다. CDN 공급자를 사용하여 캐싱 메커니즘을 구현할 때 CDN 지원 Dynamic Media 이미지 서버를 가리키도록 서버 이름을 변경하면 됩니다. 모든 Dynamic Media Classic 에디션에는 번들로 제공되는 CDN 캐싱이 포함되어 있습니다.