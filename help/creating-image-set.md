---
title: 이미지 집합 만들기
description: Adobe Dynamic Media Classic에서 이미지 세트를 만드는 방법을 알아봅니다.
uuid: 689fdc14-4f51-4c94-8515-cd8551e101d8
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: 3f356410-b30e-4870-ad95-6e5a9dc126c8
feature: Dynamic Media Classic,Viewers,Image Sets,Spin Sets
role: User
exl-id: c18bb98c-b087-45d0-a4c9-44f58a3b514f
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 59%

---

# 이미지 집합 만들기{#creating-an-image-set}

다중 보기 이미지 집합을 만들려면 다른 관점에서 항목을 표시하거나 동일한 항목의 다른 측면을 표시하는 이미지가 필요합니다. 뷰어가 항목의 모양이나 기능을 명확하게 파악할 수 있도록 항목의 이미지를 제공하는 데 목적이 있습니다.

## 이미지 집합 만들기 {#create}

세트를 만들 때, **[!UICONTROL 저장 후 게시]** 옵션은 다음과 같이 세트와 세트 구성원에 영향을 줍니다.

| **[!UICONTROL 저장 후 게시]** 저장하기 전에 옵션을 선택했습니까? | 저장 후 세트 상태 | 저장 후 세트 구성원 상태 |
| --- | --- | --- |
| 예 | 게시됨 | 게시됨 |
| 아니요 | 게시 취소됨 | 세트 구성원은 게시된 상태나 게시되지 않은 상태를 유지합니다. |

[수동 자산 게시](publishing-files.md#manually_publishing_assets) 및 [수동 자산 게시 취소](publishing-files.md#manually_unpublishing_assets)를 참조하십시오.

이미지 집합을 만들 때 Adobe은 다음 모범 사례를 권장하며 다음 제한을 적용합니다.

| 제한 유형 | 우수 사례 | 제한 적용됨 |
| --- | --- | --- |
| 세트당 중복 에셋 수 | 중복 항목 없음 | 20 |
| 세트당 최대 이미지 수 | 세트당 5-10개 이미지 | 1000 |

참조: [Dynamic Media 제한 사항](/help/limitations.md).

**이미지 세트 만들기:**

1. 다음 중 하나를 수행하십시오.

   * **먼저 이미지 선택** - [찾아보기] 패널에서 이미지 세트에 대해 원하는 이미지를 선택하고 **[!UICONTROL 빌드]** > **[!UICONTROL 이미지 집합]**.

   * **이미지 세트 화면에서 시작** - 이동 **[!UICONTROL 빌드]** > **[!UICONTROL 이미지 집합]**. [이미지 집합] 화면이 열립니다. 자산 라이브러리에서 폴더를 선택하고 이미지 집합에 사용할 이미지를 [이미지 집합] 화면으로 드래그합니다.

1. 이미지 순서를 변경하려면 이미지를 새 위치로 드래그합니다.
1. 페이지 오른쪽 하단에서 **[!UICONTROL 저장 후 게시]**(기본값)가 선택되어 있는지 확인합니다.
1. 선택 **[!UICONTROL 저장]**&#x200B;이미지 집합을 저장할 폴더를 선택하고 집합 이름을 입력한 다음 을 선택합니다 **[!UICONTROL 저장]**.
1. 이미지 집합 뷰어에서 이미지 집합을 보려면 **[!UICONTROL 미리 보기]** 이미지 세트 화면에서 다음을 수행합니다. 이미지 세트 뷰어에서 견본 썸네일을 선택하여 해당 썸네일의 동작 방식을 확인할 수 있습니다.

## 이미지 집합 편집 {#editing-an-image-set}

게시된 세트를 편집하든 게시되지 않은 세트를 편집하든 **[!UICONTROL 저장 후 게시]** 옵션은 다음과 같은 방법으로 세트 및 세트 멤버에 영향을 줍니다.

| 세트를 이미 게시했습니까? | **[!UICONTROL 저장 후 게시]** 편집을 저장하기 전에 선택한 옵션입니까? | 저장 후 세트 상태 | 저장 후 세트 구성원 상태 |
| --- | --- | --- | --- |
| 예 | 예 | 게시됨 | 게시됨 |
| 예 | 아니요 | 게시됨 | 기존 세트 구성원은 게시된 상태를 유지합니다. 편집 중에 새로 추가한 모든 세트 구성원은 게시된 상태나 게시 취소된 상태를 유지합니다. |
| 아니요 | 예 | 게시됨 | 게시됨 |
| 아니요 | 아니요 | 게시 취소됨 | 기존 세트 구성원과 편집 중에 새로 추가한 모든 세트 구성원은 게시된 상태나 게시 취소된 상태를 유지합니다. |

[수동 자산 게시](publishing-files.md#manually_publishing_assets) 및 [수동 자산 게시 취소](publishing-files.md#manually_unpublishing_assets)를 참조하십시오.

**이미지 세트 편집:**

1. 격자 보기에서 이미지 집합을 찾은 다음 이미지 아래에서 **[!UICONTROL 편집]**.
1. 다음 중 하나를 수행합니다.

   * 이미지(게시되었거나 게시 취소된 이미지)를 추가하려면 [자산 추가]에 있는 폴더에서 이미지를 [이미지 세트]의 **[!UICONTROL 보기]** 페이지로 드래그합니다.
   * 이미지를 제거하려면 이미지를 선택한 다음 을 선택합니다 **[!UICONTROL 삭제]** 을 클릭합니다.
   * 이미지를 다시 정렬하려면 원하는 이미지를 새 위치로 드래그합니다.

1. 세트 편집을 완료하면 페이지 오른쪽 하단에서 **[!UICONTROL 저장 후 게시]**(기본값)가 선택되어 있는지 확인합니다.
1. 선택 **[!UICONTROL 저장]**&#x200B;세트에 대한 저장소 폴더를 선택하고 세트의 이름을 입력한 다음 을 선택합니다 **[!UICONTROL 저장]**.

## 이미지 세트 삭제 {#deleting-an-image-set}

삭제된 세트는 휴지통으로 이동합니다. 하지만 삭제된 세트 내의 구성원(또는 &quot;하위&quot;)은 휴지통으로 이동하지 않고, 각각 기존의 게시된 상태나 게시 취소된 상태를 유지합니다.

[수동 자산 게시](publishing-files.md#manually_publishing_assets) 및 [수동 자산 게시 취소](publishing-files.md#manually_unpublishing_assets)를 참조하십시오.

**이미지 세트 삭제:**

1. [격자 보기], [목록 보기] 또는 [세부 사항 보기]에서 이미지 세트를 한 개 이상 선택합니다.
1. 전역 탐색 모음에서 다음 위치로 이동합니다. **[!UICONTROL 파일]** > **[!UICONTROL 삭제]** > **[!UICONTROL 삭제]**.
