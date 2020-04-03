---
title: Adobe Target Classic으로 오퍼 집합 푸시
seo-title: Adobe Target Classic으로 오퍼 집합 푸시
description: 널
seo-description: 오퍼 집합을 Adobe Target Classic으로 푸시하는 방법을 알아봅니다.
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Adobe Target Classic으로 오퍼 집합 푸시{#pushing-offer-sets-to-adobe-target-classic}

오퍼 집합을 만들거나 편집한 후 다음 단계에 따라 Target Classic에 푸시합니다.

1. 타겟 클래식 오퍼 세트 화면에서 오퍼 푸시 단추를 클릭합니다.
1. 로그인 자격 증명을 입력합니다.
1. [로그인] 단추를 클릭합니다.

Target Classic으로 전송하는 동안 접두사 S7_은 오퍼 이름 시작에 자동으로 첨부됩니다. 이 접두사는 Target Classic 오퍼 목록에서 Dynamic Media Classic 오퍼를 쉽게 찾을 수 있도록 첨부됩니다. 예를 들어 오퍼가 S7_&lt;오퍼 집합 이름>_&lt;오퍼 이름>으로 표시됩니다.

SPS가 Target Classic 위젯 오퍼로 푸시됩니다. 위젯 오퍼를 사용하여 Target Classic 외부에서 자체 오퍼 컨텐츠를 호스팅할 수 있습니다. 위젯 오퍼는 Target Classic 외부에서 호스팅된 표준 오퍼와 유사합니다. Target Classic에서 서버에 저장된 오퍼 컨텐츠를 배포할 수 있으므로 보다 정교하고 동적인 사용이 가능합니다. 위젯 오퍼는 URL에서 컨텐트를 검색하고 대략 2시간 동안 해당 컨텐트를 캐싱 및 제공합니다. 위젯 오퍼는 Target Classic 외부의 다른 오퍼가 제공하지 않는 일부 동적 컨텐츠 생성 기능을 제공합니다. If the mbox serving the offer contains mbox parameters such as `mboxProductID` and `mbox.offerId`, the `productId=[PRODUCT_ID]`and `offerID=[OFFERID]` URL parameters are appended to the requested URL. 이러한 매개 변수는 위젯 오퍼 URL에서 사용 가능한 서비스가 mbox의 제품 또는 주문 정보를 사용하는 Target Classic 외부의 컨텐츠를 반환하는 데 사용할 수 있습니다. API를 통해 위젯 오퍼에 액세스하여 Target Classic 외부에서 프로그래밍 방식으로 오퍼를 만들 수도 있습니다.
