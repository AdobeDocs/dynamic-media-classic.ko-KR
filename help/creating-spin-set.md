---
title: 스핀 세트 만들기
description: Adobe Dynamic Media Classic에서 스핀 세트를 만드는 방법을 알아봅니다.
uuid: 697bd78f-5e39-46bf-aa6d-ad8ab99fe40e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 735b5867-e249-4627-a5a5-25c19c2255bf
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 35e8e7fc-5b3c-441a-959c-df2e39ea0d4b
source-git-commit: 92a28b7868e03802f4ef1c113ec3f8b34f57ed56
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 53%

---

# 스핀 세트 만들기{#creating-a-spin-set}

효과적인 회전 집합을 만들려면 이미지를 올바르게 촬영해야 합니다. [빌드] 단추를 선택하고 [스핀 세트]를 선택하여 Adobe Dynamic Media Classic에서 스핀 세트를 만들 수 있습니다. [회전 집합] 화면에서 회전 집합을 편집합니다.

>[!NOTE]
>
>이전 버전의 Adobe Dynamic Media Classic에서는 2차원 스핀 세트를 제공하지 않았습니다. 이전 버전의 Adobe Dynamic Media Classic에서 스핀 세트를 만든 경우, 먼저 다른 이름으로 저장하지 않고는 1차원 스핀 세트를 저장할 수 없습니다. 선택 **[!UICONTROL 다른 이름으로 저장]** 스핀 세트 화면에서 새 이름을 입력하여 Adobe Dynamic Media Classic에서 편집할 수 있습니다.

## 회전 집합 이미지 촬영에 대한 지침 {#guidelines-for-shooting-spin-set-images}

일반적으로 회전 집합에 있는 이미지 수가 많을수록 이미지 회전 효과가 향상됩니다. 그러나 집합에 많은 이미지를 포함하면 이미지를 로드하는 데 걸리는 시간도 증가합니다. Adobe Dynamic Media Classic에서는 스핀 세트에서 사용할 이미지를 촬영하기 위해 다음 지침을 권장합니다.

* 적어도, 1차원 스핀 세트에 8-12개의 이미지와 2차원 스핀 세트에 있는 16-24개의 이미지를 사용합니다.
* 손실 없는 형식을 사용합니다. TIFF 및 PNG가 권장됩니다.
* 항목이 완전 흰색이나 다른 고대비 배경으로 표시되도록 모든 이미지를 마스킹합니다. 선택적으로 그림자를 추가합니다.
* 제품 세부 사항의 광원과 초점이 적절한지 확인합니다.
* 마네킨이나 모델을 사용하여 패션 의류의 회전 이미지를 촬영합니다. 마네킹은 종종 마스킹되거나(유리 마네킹을 사용), 스티처리된 마네킹/드레싱이 이미지에 표시됩니다. 각도 수를 정의하여 모델 회전 집합을 만들 수 있습니다. 모델을 단계별로 안내하고 각 샷의 방향을 확인할 수 있도록 바닥에 있는 테이프로 각 각도를 표시합니다.

## 스핀 세트 만들기 {#create}

Adobe Dynamic Media Classic에서 스핀 세트를 작성하거나 만들 순서는 중요합니다. 이미지를 [스핀 세트] 페이지의 그리드에 드래그 앤 드롭할 때 자산의 순서를 지정한 방법에 따라 스핀 세트가 특정 방향으로 회전합니다. 따라서 빌더에 시각적으로 표시되는 순서는 사용자가 마우스 포인터를 이동하거나 손가락을 왼쪽으로 이동할 때 자산이 회전하는 방식입니다.

세트를 만들 때, **[!UICONTROL 저장 후 게시]** 옵션은 다음과 같이 세트와 세트 구성원에 영향을 줍니다.

| **[!UICONTROL 저장 후 게시]** 저장하기 전에 선택한 옵션 | 저장 후 세트 상태 | 저장 후 세트 구성원 상태 |
| --- | --- | --- |
| 예 | 게시됨 | 게시됨 |
| 아니요 | 게시 취소됨 | 세트 구성원은 게시된 상태나 게시되지 않은 상태를 유지합니다. |

[수동 자산 게시](publishing-files.md#manually-publishing-assets) 및 [수동 자산 게시 취소](publishing-files.md#manually-unpublishing-assets)를 참조하십시오.

스핀 세트를 만들 때, Adobe은 다음 모범 사례를 권장하고 다음 제한을 적용합니다.

| 스핀 세트 제한 유형 | 우수 사례 | 제한 적용 |
| --- | --- | --- |
| 2D 세트당 최대 행/열 수 | 세트당 12-18개 이미지 | 1000 |

참조 - [Dynamic Media 제한 사항](/help/limitations.md).

스핀 세트를 저장한 후 [작성: 스핀 세트] 페이지의 [미리 보기]를 사용하여 기본 뷰어에서 스핀 세트가 어떻게 표시되는지 확인할 수 있습니다.

**스핀 세트 만들기:**

1. 설정 **[!UICONTROL 빌드]** 드롭다운 메뉴에서 **[!UICONTROL 스핀 세트]**.
1. [회전 집합 크기] 대화 상자에서 원하는 행과 셀 수를 설정합니다.

   1차원 회전 집합을 만들려면 한 행만 선택합니다.

   2차원 회전 집합을 만들려면 두 개 이상의 행을 선택합니다.

1. 선택 **[!UICONTROL 확인]**.
1. 이미지를 [회전 집합] 화면의 그리드로 끌어서 놓습니다.
1. 완료하면 페이지 오른쪽 하단에서 **저장 후 게시**(기본값)가 선택되어 있는지 확인합니다.
1. 선택 **[!UICONTROL 저장]**.
1. [저장] 대화 상자에서 회전 집합을 저장할 폴더를 선택합니다. [파일 이름] 필드에 회전 집합 이름을 입력합니다.
1. 선택 **[!UICONTROL 저장]**.

## 스핀 세트 편집 {#editing-a-spin-set}

게시된 세트를 편집하든 게시 취소된 세트를 편집하든 간에 **[!UICONTROL 저장 후 게시]** 옵션은 다음과 같은 방법으로 세트 및 설정 멤버에 영향을 줍니다.

| 세트를 이미 게시했습니까? | **[!UICONTROL 저장 후 게시]** 편집을 저장하기 전에 선택한 옵션 | 저장 후 세트 상태 | 저장 후 세트 구성원 상태 |
| --- | --- | --- | --- |
| 예 | 예 | 게시됨 | 게시됨 |
| 예 | 아니요 | 게시됨 | 기존 세트 구성원은 게시된 상태를 유지합니다. 편집 중에 새로 추가한 모든 세트 구성원은 게시된 상태나 게시 취소된 상태를 유지합니다. |
| 아니요 | 예 | 게시됨 | 게시됨 |
| 아니요 | 아니요 | 게시 취소됨 | 기존 세트 구성원과 편집 중에 새로 추가한 모든 세트 구성원은 게시된 상태나 게시 취소된 상태를 유지합니다. |

[수동 자산 게시](publishing-files.md#manually-publishing-assets) 및 [수동 자산 게시 취소](publishing-files.md#manually-unpublishing-assets)를 참조하십시오.

**스핀 세트 편집:**

1. 스핀 세트의 롤오버를 선택합니다 **[!UICONTROL 편집]** 버튼을 클릭합니다.
1. 다음 중 하나를 수행합니다.

   * **이미지 제거** - 이미지를 선택한 다음 을 선택합니다 **[!UICONTROL 삭제]**.

   * **이미지 추가** - 이미지를 셀로 드래그합니다.

   * **행 순서 조정(2차원 스핀 세트)** - 행 선택기 상자(행 왼쪽)를 선택한 다음 을 선택합니다 **[!UICONTROL 행 아래로 이동]** 또는 **[!UICONTROL 위로 행 이동]**.

   * **행 및 셀 추가** - 행 상자 및 셀 상자에 숫자를 입력하여 행 수와 각 행의 셀 수를 결정합니다.

1. 편집을 완료하면 페이지 오른쪽 하단에서 **[!UICONTROL 저장 후 게시]**(기본값)가 선택되어 있는지 확인합니다.
1. 선택 **[!UICONTROL 저장]**&#x200B;를 클릭하고 저장소 폴더를 선택하고 세트의 이름을 입력한 다음 을 선택합니다 **[!UICONTROL 저장]**.

## 스핀 세트 삭제 {#deleting-a-spin-set}

삭제된 세트는 휴지통으로 이동합니다. 하지만 삭제된 세트 내의 구성원(또는 &quot;하위&quot;)은 휴지통으로 이동하지 않고, 각각 기존의 게시된 상태나 게시 취소된 상태를 유지합니다.

[수동 자산 게시](publishing-files.md#manually-publishing-assets) 및 [수동 자산 게시 취소](publishing-files.md#manually-unpublishing-assets)를 참조하십시오.

**스핀 세트 삭제:**

1. [격자 보기], [목록 보기] 또는 [상세 보기]에서 스핀 세트를 하나 이상 선택합니다.
1. 전역 탐색 막대에서 **[!UICONTROL 파일]** > **[!UICONTROL 삭제]** > **[!UICONTROL 삭제]**.
