---
title: 견본 집합 만들기
description: Adobe Dynamic Media Classic에서 견본 세트를 만드는 방법을 알아봅니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/swatch_sets
feature: Dynamic Media Classic,Viewers
role: User
exl-id: 426b6e6b-daed-4ca6-b095-99bb06604b07
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '715'
ht-degree: 49%

---

# 견본 집합 만들기{#creating-a-swatch-set}

견본 집합을 통해 사용자는 각기 다른 색상, 패턴 또는 마무리로 항목을 볼 수 있습니다. 색상 견본이 포함된 견본 집합을 만들려면 사용자에게 제공하려는 각 색상, 패턴 또는 마무리에 대해 하나의 이미지가 필요합니다. 또한 각 색상, 패턴 또는 마무리에 대해 하나의 색상, 패턴 또는 마무리 견본이 필요합니다.

예를 들어 각기 다른 색상의 챙이 있는 캡의 이미지를 제공한다고 가정합니다. 챙은 빨간색, 녹색 및 파란색입니다. 이 경우 동일한 캡의 세 가지 촬영이 필요합니다. 각각 빨간색, 녹색 및 파란색 챙이 사용된 하나의 촬영이 필요합니다. 빨간색, 녹색 및 파란색 색상 견본도 필요합니다. 색상 견본은 사용자가 견본 집합 뷰어에서 선택하여 빨간불, 초록불 또는 파란불 캡을 보는 썸네일 역할을 합니다.

## 견본 집합 만들기 {#create}

집합을 만들 때 **저장 후 Publish** 옵션은 다음과 같은 방법으로 집합 및 집합 구성원에 영향을 줍니다.

| 저장하기 전에 **[!UICONTROL 저장 후 Publish]** 옵션을 선택했습니까? | 저장 후 세트 상태 | 저장 후 세트 구성원 상태 |
| --- | --- | --- |
| 예 | 게시됨 | 게시된 |
| 아니요 | 게시 취소됨 | 세트 구성원은 게시된 상태나 게시되지 않은 상태를 유지합니다. |

[수동 자산 게시](publishing-files.md#manually_publishing_assets) 및 [수동 자산 게시 취소](publishing-files.md#manually_unpublishing_assets)를 참조하십시오.

**견본 집합을 만들려면:**

1. 다음 중 하나를 수행하십시오.

   * **먼저 이미지 선택**: [찾아보기] 패널에서 이미지를 선택한 다음 **[!UICONTROL 빌드]** > **[!UICONTROL 견본 집합]**(으)로 이동합니다.

   * **견본 집합 화면에서 시작**: **[!UICONTROL 빌드]** > **[!UICONTROL 견본 집합]**&#x200B;으로 이동합니다. 자산 라이브러리에서 폴더를 선택하고 이미지를 [견본 집합] 페이지의 [보기] 섹션으로 드래그합니다.

1. 견본 색상, 패턴 또는 마무리를 [견본 집합] 페이지의 [견본] 자리 표시자 상자로 드래그합니다.

   각 자리 표시자로 끄는 색상, 패턴 또는 마무리 견본이 인접한 이미지의 색상, 패턴 또는 마무리를 나타내는지 확인합니다.

1. 견본 집합에서 이미지 순서를 변경하려면 이미지를 새 위치로 드래그합니다.
1. 페이지의 오른쪽 아래 모서리 근처에서 **[!UICONTROL 저장 후 Publish]**&#x200B;이 선택되었는지 확인합니다(기본값).
1. **[!UICONTROL 저장]**&#x200B;을 선택하고 색상 견본 집합을 저장할 폴더를 선택한 다음 집합 이름을 입력하고 **[!UICONTROL 제출]**&#x200B;을 선택합니다.
1. 견본 집합 뷰어에서 견본 집합을 보려면 견본 집합 화면에서 **[!UICONTROL 미리 보기]**&#x200B;를 선택하십시오. 견본 집합 뷰어에서 견본 축소판을 선택하여 해당 축소판의 동작 방식을 확인할 수 있습니다.

## 견본 집합 편집 {#editing-a-swatch-set}

게시된 집합이든 게시되지 않은 집합이든 관계없이 **[!UICONTROL 저장 후 Publish]** 옵션은 다음과 같은 방법으로 집합 및 집합 구성원에 영향을 줍니다.

| 세트를 이미 게시했습니까? | 편집을 저장하기 전에 **[!UICONTROL 저장 후 Publish]** 저장 옵션을 선택했습니까? | 저장 후 세트 상태 | 저장 후 세트 구성원 상태 |
|--- | --- | --- | --- |
| 예 | 예 | 게시됨 | 게시됨. |
| 예 | 아니요 | 게시됨 | 기존 집합 구성원은 게시된 상태를 유지합니다. 편집 중에 새로 추가한 모든 세트 구성원은 게시된 상태나 게시 취소된 상태를 유지합니다. |
| 아니요 | 예 | 게시됨 | 게시됨. |
| 아니요 | 아니요 | 게시 취소됨 | 기존 세트 구성원과 편집 중에 새로 추가한 모든 세트 구성원은 게시된 상태나 게시 취소된 상태를 유지합니다. |

[수동 자산 게시](publishing-files.md#manually_publishing_assets) 및 [수동 자산 게시 취소](publishing-files.md#manually_unpublishing_assets)를 참조하십시오.

**견본 집합을 편집하려면:**

1. 눈금 보기에서 SwatchSet을 찾은 다음 이미지 아래에서 **[!UICONTROL 편집]**&#x200B;을 선택합니다.
1. 다음 중 하나를 수행합니다.

   * 이미지를 추가하려면(게시 또는 게시 취소) Assets 추가 폴더의 이미지를 견본 집합의 **[!UICONTROL 보기]** 페이지로 끕니다.
   * 이미지를 제거하려면 이미지를 선택한 다음 도구 모음에서 **[!UICONTROL 삭제]**&#x200B;를 선택합니다.
   * 이미지를 다시 정렬하려면 원하는 이미지를 새 위치로 드래그합니다.

1. 페이지의 오른쪽 아래 모서리 근처에서 집합 편집을 마쳤으면 **[!UICONTROL 저장 후 Publish]**&#x200B;이 선택되었는지 확인합니다(기본값).
1. **[!UICONTROL 저장]**&#x200B;을 선택하고 저장소 폴더를 선택한 다음 집합 이름을 입력한 다음 **[!UICONTROL 저장]**&#x200B;을 선택합니다.

## 견본 집합 삭제

삭제된 세트는 휴지통으로 이동합니다. 그러나 해당 집합 내의 멤버(또는 &quot;하위&quot;)는 영향을 받지 않습니다. 대신 각 멤버는 기존의 게시 또는 게시 취소 상태를 유지합니다.

[수동 자산 게시](publishing-files.md#manually_publishing_assets) 및 [수동 자산 게시 취소](publishing-files.md#manually_unpublishing_assets)를 참조하십시오.

**견본 집합을 삭제하려면:**

1. [격자 보기], [목록 보기] 또는 [세부 사항 보기]에서 하나 이상의 견본 집합을 선택합니다.
1. 전역 탐색 모음에서 **[!UICONTROL 파일]** > **[!UICONTROL 삭제]** > **[!UICONTROL 삭제]**(으)로 이동합니다.
