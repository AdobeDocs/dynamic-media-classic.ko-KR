---
title: Adobe Target Classic에 오퍼 집합 푸시
seo-title: Adobe Target Classic에 오퍼 집합 푸시
description: 널
seo-description: 오퍼 세트를 Adobe Target Classic에 푸시하는 방법을 알아봅니다.
uuid: 8 c 895 a 7 c -21 b 4-4 d 85-8 b 0 b-a 3 d 2 a 420 bf 2 e
contentOwner: 관리
content-type: 참조
products: sg_ Experiencemanager/dynamic-media-scene -7
geptopics: sg_ scenesevenondemand_ pk/categories/target_ classic_ integration
discoiquuid: 39 A 05654-4 F 66-4 F 1 E-AEC 5-EBE 6 D 174353 F
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Adobe Target Classic에 오퍼 집합 푸시{#pushing-offer-sets-to-adobe-target-classic}

오퍼 집합을 만들거나 편집한 후 다음 단계에 따라 Target Classic에 푸시합니다.

1. [기본 오퍼 오퍼 집합] 화면에서 [오퍼 푸시] 단추를 클릭합니다.
1. 로그인 자격 증명을 입력합니다.
1. [로그인] 단추를 클릭합니다.

Target Classic로 전송하는 동안 접두사 s 7_ 가 오퍼 이름 시작 부분에 자동으로 첨부됩니다. 이 접두사는 Target Classic 오퍼 목록에서 Dynamic Media Classic 오퍼를 쉽게 찾을 수 있도록 첨부됩니다. 예를 들어 오퍼가 S7_&lt;오퍼 집합 이름&gt;_&lt;오퍼 이름&gt;으로 표시됩니다.

SPS는 Target Classic 위젯 오퍼에 푸시합니다. 위젯 오퍼를 사용하여 Target Classic 외부에서 자체 오퍼 컨텐츠를 호스팅할 수 있습니다. 위젯 오퍼는 Target Classic 외부에 호스팅된 표준 오퍼와 유사합니다. Target Classic 에서는 Target Classic 이 서버에 저장된 오퍼 컨텐츠를 배포하여 보다 세련되고 동적인 사용을 허용합니다. 위젯 오퍼는 URL에서 컨텐트를 검색하고 대략 2시간 동안 해당 컨텐트를 캐싱 및 제공합니다. 위젯 오퍼는 Target Classic 외부의 다른 오퍼가 제공하지 않는 몇 가지 동적 컨텐츠 생성 기능을 제공합니다. If the mbox serving the offer contains mbox parameters such as `mboxProductID` and `mbox.offerId`, the `productId=[PRODUCT_ID]`and `offerID=[OFFERID]` URL parameters are appended to the requested URL. 위젯 오퍼 URL에서 사용 가능한 서비스는 이러한 매개 변수를 사용하여 mbox의 제품 또는 주문 정보를 사용하는 Target Classic 외부에서 컨텐츠를 반환할 수 있습니다. API를 통해 위젯 오퍼에 액세스하여 Target Classic 외부에서 오퍼를 프로그래밍 방식으로 만들 수도 있습니다.
