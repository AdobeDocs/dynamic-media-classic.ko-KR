---
title: Adobe Target Standard/Premium으로 오퍼 세트 푸싱
description: Adobe Target Standard/Premium에 오퍼 세트를 푸시하는 방법을 알아봅니다.
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
source-git-commit: c4e2b8b42b56420269087d0d4f262490464270c0
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 6%

---

# Adobe Target Standard/Premium으로 오퍼 세트 푸싱 {#pushing-offer-sets-to-target}

오퍼 세트를 만들거나 편집한 후 다음 단계에 따라 Adobe Target Standard/Premium으로 푸시합니다.

1. Target 오퍼 세트 테스트 화면에서 **[!UICONTROL 푸시 오퍼]**&#x200B;를 클릭합니다.
1. 클라이언트 코드와 로그인 자격 증명을 입력합니다.
1. **[!UICONTROL 로그인]**&#x200B;을 클릭합니다.

Adobe Target Standard/Premium으로 전송하는 동안 접두사 `S7_`이 오퍼 이름의 시작 부분에 자동으로 첨부됩니다. 이 접두사는 Test&amp;Target 오퍼 목록에서 Dynamic Media Classic 오퍼를 쉽게 찾을 수 있도록 첨부됩니다. 예를 들어 오퍼가 `S7_<name of offer set>_<offer name>`(으)로 나타납니다.

Dynamic Media Classic은 Adobe Target Standard/Premium 위젯 오퍼를 푸시합니다. 위젯 오퍼를 사용하여 Adobe Target Standard/Premium 외부에서 고유한 오퍼 콘텐츠를 호스팅할 수 있습니다. 위젯 오퍼는 Adobe Target Standard/Premium 외부에서 호스팅된 표준 오퍼와 유사합니다. Adobe Target Standard/Premium에서는 서버에 저장된 오퍼 컨텐츠를 배포할 수 있으므로 보다 정교하고 동적인 사용을 가능하게 해줍니다. 위젯 오퍼는 URL에서 컨텐트를 검색하고 대략 2시간 동안 해당 컨텐트를 캐싱 및 제공합니다. 위젯 오퍼는 Adobe Target Standard/Premium 외부의 다른 오퍼에서 제공하지 않는 몇 가지 동적 컨텐츠 생성 기능을 제공합니다. 오퍼를 제공하는 mbox에 `mboxProductID` 및 `mbox.offerId`과 같은 mbox 매개 변수가 포함되어 있으면 `productId=[PRODUCT_ID]` 및 `offerID=[OFFERID]` URL 매개 변수가 요청된 URL에 추가됩니다. 이러한 매개 변수는 위젯 오퍼 URL에서 사용할 수 있는 서비스에서 mbox의 제품 또는 주문 정보를 사용하는 Adobe Target Standard/Premium 외부의 콘텐츠를 반환할 수 있습니다. 또한 API를 통해 위젯 오퍼에 액세스하여 Adobe Target Standard/Premium 외부에서 오퍼를 프로그래밍 방식으로 만들 수도 있습니다.
