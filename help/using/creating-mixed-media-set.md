---
title: 혼합 미디어 집합 만들기
description: Adobe Dynamic Media Classic에서 혼합 미디어 세트를 만드는 방법을 알아봅니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: 18669c65-a1c4-4012-8587-cd5095f4bd4e
topic: Content Management
level: Intermediate
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 68%

---

# 혼합 미디어 집합 만들기{#creating-a-mixed-media-set}

한 프레젠테이션에서 여러 유형의 뷰어를 결합하려는 경우 혼합 미디어 집합을 만듭니다. 혼합 미디어 집합에 추가하기 전에 파일, 이미지 집합, 견본 집합 및 회전 집합을 게시할 준비가 되었는지 확인합니다.

![혼합 미디어 집합](/help/using/assets/mm_mixed_media_set.png)

## 혼합 미디어 집합 만들기 {#create-a-mixed-media-set}

세트를 만들 때, **저장 후 게시** 옵션은 다음과 같이 세트와 세트 구성원에 영향을 줍니다.

| 저장하기 전에 &quot;저장 후 게시&quot; 옵션이 선택되었습니까? | 저장 후 세트 상태 | 저장 후 세트 구성원 상태 |
| --- | --- | --- |
| 예 | 게시됨 | 게시됨 |
| 아니요 | 게시 취소됨 | 세트 구성원은 게시된 상태나 게시되지 않은 상태를 유지합니다. |

[수동 자산 게시](publishing-files.md#manually_publishing_assets) 및 [수동 자산 게시 취소](publishing-files.md#manually_unpublishing_assets)를 참조하십시오.

**혼합 미디어 세트를 만들려면:**

1. 다음으로 이동 **[!UICONTROL 빌드]** > **[!UICONTROL 혼합 미디어 집합]**.
1. 비디오, 이미지 집합, 회전 집합 및 견본을 자산 라이브러리에서 [혼합 미디어 집합] 화면으로 드래그합니다.

   >[!NOTE]
   >
   >혼합 미디어 집합은 다음 문자가 포함된 파일 이름이 있는 자산을 지원하지 않습니다. `( ) { }`.

1. 다음 중 하나를 수행합니다.

   * 사운드트랙을 추가하려면 오디오 파일을 자산 라이브러리에서 사운드트랙 상자로 드래그합니다. 사운드트랙은 이미지가 표시되는 동안 재생됩니다. 비디오를 표시하면 중지됩니다.
   * 집합 순서를 변경하려면 집합을 [혼합 미디어 집합] 화면의 새 위치로 드래그합니다. 화면의 집합 순서에 따라 혼합 미디어 집합 뷰어에서 집합이 사용자에게 표시되는 왼쪽에서 오른쪽 순서가 결정됩니다.
   * (선택 사항) 뷰어에서 비디오를 나타낼 사용자 지정 썸네일을 추가하려면 자산 라이브러리의 이미지 파일을 [썸네일] 자리 표시자 상자로 드래그합니다.

1. 페이지 오른쪽 하단에서 **[!UICONTROL 저장 후 게시]**(기본값)가 선택되어 있는지 확인합니다.
1. 선택 **[!UICONTROL 저장]**.
1. 혼합 미디어 세트를 저장할 폴더를 선택한 다음 세트의 이름을 입력합니다.
1. 선택 **[!UICONTROL 저장]**.

   이미지 집합 뷰어에서 콤보 이미지 집합의 모양을 보려면 **[!UICONTROL 미리 보기]**.

## 혼합 미디어 집합 편집 {#edit-a-mixed-media-set}

혼합 미디어 집합을 편집할 수 있습니다. 혼합 미디어 집합 내의 한 집합을 편집하려면 집합을 개별적으로 열고 편집한 다음 저장합니다. 편집 내용이 혼합 미디어 집합에 표시됩니다.

게시된 세트를 편집하든 게시되지 않은 세트를 편집하든 **[!UICONTROL 저장 후 게시]** 옵션은 다음과 같은 방법으로 세트 및 세트 멤버에 영향을 줍니다.

| 세트를 이미 게시했습니까? | **[!UICONTROL 저장 후 게시]** 편집을 저장하기 전에 선택한 옵션입니까? | 저장 후 세트 상태 | 저장 후 세트 구성원 상태 |
| --- |--- |--- |--- |
| 예 | 예 | 게시됨 | 게시됨 |
| 예 | 아니요 | 게시됨 | 기존 집합 구성원은 게시된 상태를 유지합니다. 편집 중에 새로 추가한 모든 세트 구성원은 게시된 상태나 게시 취소된 상태를 유지합니다. |
| 아니요 | 예 | 게시됨 | 게시됨 |
| 아니요 | 아니요 | 게시 취소됨 | 기존 세트 구성원과 편집 중에 새로 추가한 모든 세트 구성원은 게시된 상태나 게시 취소된 상태를 유지합니다. |

[수동 자산 게시](publishing-files.md#manually_publishing_assets) 및 [수동 자산 게시 취소](publishing-files.md#manually_unpublishing_assets)를 참조하십시오.

**혼합 미디어 세트를 편집하려면:**

1. 혼합 미디어 세트의 롤오버 선택 **[!UICONTROL 편집]** 단추를 클릭합니다.
1. 다음 중 하나를 수행합니다.

   * 항목을 제거하려면 항목을 선택하고 **[!UICONTROL 삭제]**.
   * 항목을 다시 정렬하려면 새 위치로 드래그합니다.

1. 세트 편집을 완료하면 페이지 오른쪽 하단에서 **[!UICONTROL 저장 후 게시]**(기본값)가 선택되어 있는지 확인합니다.
1. 선택 **[!UICONTROL 저장]** 또는 **[!UICONTROL 다른 이름으로 저장]**.

## 혼합 미디어 집합 삭제

삭제된 세트는 휴지통으로 이동합니다. 그러나 해당 집합 내의 멤버(또는 &quot;하위&quot;)는 영향을 받지 않습니다. 대신 각 멤버는 기존의 게시 또는 게시 취소 상태를 유지합니다.

[수동 자산 게시](publishing-files.md#manually_publishing_assets) 및 [수동 자산 게시 취소](publishing-files.md#manually_unpublishing_assets)를 참조하십시오.

**혼합 미디어 세트를 삭제하려면:**

1. [격자 보기], [목록 보기] 또는 [상세 보기]에서 혼합 미디어 집합을 하나 이상 선택합니다.
1. 전역 탐색 모음에서 다음 위치로 이동합니다. **[!UICONTROL 파일]** > **[!UICONTROL 삭제]** > **[!UICONTROL 삭제]**.
