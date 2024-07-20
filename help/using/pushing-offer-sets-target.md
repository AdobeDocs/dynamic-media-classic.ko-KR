---
title: Adobe Target Standard/Premium에 오퍼 집합 푸시
description: Adobe Dynamic Media Classic에서 Adobe Target Standard/Premium으로 오퍼 세트를 푸시하는 방법을 알아봅니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
topic: Integrations, Development
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---

# Adobe Target Standard/Premium에 오퍼 집합 푸시 {#pushing-offer-sets-to-target}

오퍼 세트를 만들거나 편집한 후 다음 단계를 수행하여 Adobe Target Standard/Premium으로 푸시합니다.

1. Test&amp;Target 오퍼 집합 화면에서 **[!UICONTROL 오퍼 푸시]**&#x200B;를 선택합니다.
1. 클라이언트 코드 및 로그인 자격 증명을 입력합니다.
1. **[!UICONTROL 로그인]**&#x200B;을 선택합니다.

Adobe Target Standard/Premium으로 전송하는 동안 `S7_` 접두사가 오퍼 이름 시작 부분에 자동으로 첨부됩니다. 이 접두사는 Test&amp;Target 오퍼 목록에서 Adobe Dynamic Media Classic 오퍼를 쉽게 찾을 수 있도록 첨부됩니다. 예를 들어 오퍼는 `S7_<name of offer set>_<offer name>`(으)로 표시됩니다.

Adobe Dynamic Media Classic은 Adobe Target Standard/Premium 위젯 오퍼를 푸시합니다. 위젯 오퍼를 사용하여 Adobe Target Standard/Premium에서 제공하는 콘텐츠를 직접 호스팅할 수 있습니다. 위젯 오퍼는 Adobe Target Standard/Premium에서 호스팅하는 표준 오퍼와 유사합니다. Adobe Target Standard/Premium에서는 서버에 저장된 오퍼 컨텐츠를 배포할 수 있으므로 보다 정교하고 동적인 사용이 가능합니다. 위젯 오퍼는 URL에서 컨텐츠를 검색하고 약 2시간 동안 해당 컨텐츠를 캐싱하고 제공할 수 있습니다. 위젯 오퍼는 Adobe Target Standard/Premium 외부의 다른 오퍼에서는 제공하지 않는 일부 다이내믹 콘텐츠 생성 기능을 제공합니다. 오퍼를 제공하는 mbox에 `mboxProductID` 및 `mbox.offerId`과(와) 같은 mbox 매개 변수가 포함되어 있으면 `productId=[PRODUCT_ID]` 및 `offerID=[OFFERID]` URL 매개 변수가 요청된 URL에 추가됩니다. 이러한 매개 변수는 위젯 오퍼 URL에서 사용 가능한 서비스에서 mbox의 제품 또는 주문 정보를 사용하는 Adobe Target Standard/Premium 외부 콘텐츠를 반환하는 데 사용됩니다. 또한 API를 통해 위젯 오퍼에 액세스할 수 있으므로 Adobe Target Standard/Premium 외부에서 오퍼를 프로그래밍 방식으로 만들 수 있습니다.
