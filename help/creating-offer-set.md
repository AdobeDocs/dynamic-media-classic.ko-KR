---
title: 오퍼 집합 만들기
seo-title: 오퍼 집합 만들기
description: 널
seo-description: 오퍼 세트를 만드는 방법을 알아봅니다.
uuid: 6d6a4af9-70c0-4cfa-9a8f-855d6adfcc8f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: 59b6437d-c21e-4929-9291-3032dbb34565
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Creating an offer set{#creating-an-offer-set}

다음 중 원하는 유형의 오퍼 집합을 만들 수 있습니다.

* 비디오
* 매개 변수화된 템플릿
* 이미지

For templates, click **Add and Preview**, then set the parameters you choose. 다른 오퍼 집합 유형에는 매개 변수가 포함되지 않지만 **미리 보기**&#x200B;를 클릭하고 사용 가능한 사전 설정을 변경하여 사용자 지정할 수 있습니다.

Dynamic Media Classic에서는 편집 및 오퍼 집합 만들기 도구를 제공합니다.

>[!NOTE]
>
>오퍼 집합을 만들기 전에 Scene7 Publishing System으로 설정된 세트에 사용할 모든 자산을 게시해야 합니다. [수동 자산 게시](publishing-files.md#manually_publishing_assets) 및 [수동 자산 게시 취소](publishing-files.md#manually_unpublishing_assets)를 참조하십시오.

## 오퍼 집합 유형 {#types-of-offer-sets}

다음 오퍼 집합 유형에서 오퍼 집합을 만듭니다.

* **이미지**&#x200B;오퍼 집합의 이미지를 결합할 수 있습니다. 각 이미지는 세트에 다른 오퍼를 포함합니다.

* **이미지**&#x200B;템플릿 작성 > 템플릿 기본 명령을 사용하여 Dynamic Media Classic에서 이미지 템플릿을 매개 변수화할 수 있습니다. 매개 변수를 통해 템플릿의 구성 요소(텍스트 프레임의 텍스트, 여러 이미지)를 바꾸고 사용자 지정할 수 있습니다. 예를 들어 오퍼 집합의 경우 템플릿 매개 변수를 사용하여 오퍼 집합에 동일한 이미지의 변형을 만들 수 있습니다. 이미지 템플릿을 만들고 매개 변수화하는 방법에 대한 자세한 내용은 템플릿 매개 변수 만들기를 참조하십시오.

* **비디오**&#x200B;오퍼 세트에 대한 비디오를 취합할 수 있습니다. 각 비디오는 집합에서 각기 다른 오퍼입니다.

## 매개 변수화된 템플릿으로 오퍼 집합 만들기 {#creating-an-offer-set-with-a-parameterized-template}

오퍼 집합을 만들 때, **저장 후 게시** 옵션은 다음과 같이 세트와 세트 구성원에 영향을 줍니다.

| 저장하기 전에 [저장 후 게시] 옵션을 선택했습니까? | 저장 후 세트 상태 | 저장 후 세트 구성원 상태 |
|--- |--- |--- |
| 예 | 게시됨 | 게시됨 |
| 아니요 | 게시 취소됨 | 세트 구성원은 게시된 상태나 게시되지 않은 상태를 유지합니다. |

[수동 자산 게시](publishing-files.md#manually_publishing_assets) 및 [수동 자산 게시 취소](publishing-files.md#manually_unpublishing_assets)를 참조하십시오.

**매개 변수화된 템플릿으로 오퍼 세트를 만들려면**

1. 템플릿 또는 배너를 선택합니다.
1. Click **Build** > **Target Classic Offer Set**.

   타겟 클래식 오퍼 세트 페이지에는 오퍼 세트의 오퍼가 나열됩니다. 목록에서 첫 번째 항목은 개체입니다.

1. 개체를 선택하고 **추가 및 미리 보기**&#x200B;를 클릭합니다.

   이 페이지의 왼쪽에는 템플릿의 매개 변수와 해당 값이 나열됩니다.

1. 매개 변수 값을 변경하여 오퍼를 만듭니다. 예를 들어 테스트 필드에 다른 텍스트를 입력하거나, 레이어 크기를 변경하거나, 한 이미지를 다른 이미지로 바꾸거나, 다른 뷰어 사전 설정을 선택합니다.
1. **저장** 또는 **다른 이름으로 저장**&#x200B;을 클릭하여 오퍼를 오퍼 집합의 일부로 저장합니다.

   타겟 클래식 오퍼 세트 페이지에는 사용자가 만든 오퍼가 나열됩니다.

1. 3-5 단계를 반복하여 집합에 대한 추가 오퍼를 만듭니다.
1. When you finish, near the lower-right corner of the page, ensure that **Publish after save** is selected (default).
1. Click **Close**, enter a name for the offer set, and then click **Save**.

Target Classic 오퍼 집합 페이지를 닫기 전에 오퍼 집합을 Target Classic으로 푸시합니다. See [Pushing offer sets to Target Classic](pushing-offer-sets-target-classic.md#pushing_offer_sets_to_target_classic).

## 이미지나 비디오를 사용하여 오퍼 집합 만들기 {#creating-an-offer-set-with-images-or-videos}

오퍼 집합을 만들 때, **저장 후 게시** 옵션은 다음과 같이 세트와 세트 구성원에 영향을 줍니다.

| 저장하기 전에 [저장 후 게시] 옵션을 선택했습니까? | 저장 후 세트 상태 | 저장 후 세트 구성원 상태 |
|--- |--- |--- |
| 예 | 게시됨 | 게시됨 |
| 아니요 | 게시 취소됨 | 세트 구성원은 게시된 상태나 게시되지 않은 상태를 유지합니다. |

[수동 자산 게시](publishing-files.md#manually_publishing_assets) 및 [수동 자산 게시 취소](publishing-files.md#manually_unpublishing_assets)를 참조하십시오.

**이미지나 비디오를 사용하여 오퍼 집합 만들기**

1. 오퍼 세트에 대한 이미지 또는 비디오를 어셈블합니다. 타겟 클래식 오퍼 세트 화면이나 격자 보기 또는 목록 보기에서 시작하고 다음 방법 중 하나를 사용합니다.

   * **타겟 클래식 오퍼 세트 화면**&#x200B;작성 > 타겟 클래식 오퍼 세트를 클릭합니다. 이미지나 비디오를 화면으로 드래그합니다. 다양한 크기의 비디오나 이미지를 만들려면 이미지나 비디오의 여러 복사본에서 끌어 각 크기를 개별적으로 설정합니다.

   * **격자 또는 목록 보기이미지 또는**&#x200B;비디오를 선택한 다음 [작성] > [Target Classic 오퍼 집합]을 클릭합니다.

1. 원할 경우, 이미지 또는 비디오를 선택하고 **미리 보기**&#x200B;를 클릭합니다. 오퍼 미리 보기 페이지에서 선택한 이미지 또는 비디오의 크기와 모양을 변경할 수 있습니다. 또는 오퍼 세트의 모든 이미지 또는 비디오를 변경할 수 있습니다.

   * 사전 설정을 선택하여 이미지나 비디오의 모양과 크기를 변경합니다.
   * [선택한 사전 설정 전체 적용] 확인란을 클릭하여 선택한 사전 설정을 오퍼 집합의 모든 오퍼에 적용합니다.
   **저장**&#x200B;을 클릭하여 변경 사항을 이미지나 비디오 오퍼에 저장합니다. Then click **Close** to return to the Target Classic Offer Set page.

1. After you finish creating offers for the offer set and choosing Image Presets for different images, ensure that **Publish after save** is selected (default).
1. **닫기**&#x200B;를 클릭하고, 오퍼 집합에 사용할 이름을 입력하고 **저장**&#x200B;을 클릭합니다.

Target Classic 오퍼 집합 페이지를 닫기 전에 오퍼 집합을 Target Classic으로 푸시합니다. See [Pushing offer sets to Target Classic](pushing-offer-sets-target-classic.md#pushing_offer_sets_to_target_classic).

## 오퍼 집합 편집 {#editing-an-offer-set}

편집 대상이 게시된 세트인지 게시 취소된 세트인지에 따라, **저장 후 게시** 옵션은 다음과 같이 세트와 세트 구성원에 영향을 줍니다.

| 세트를 이미 게시했습니까? | 편집 내용을 저장하기 전에 [저장 후 게시] 옵션을 선택했습니까? | 저장 후 세트 상태 | 저장 후 세트 구성원 상태 |
|--- |--- |--- |--- |
| 예 | 예 | 게시됨 | 게시됨 |
| 예 | 아니요 | 게시됨 | 기존 세트 구성원은 게시된 상태를 유지합니다.편집 중에 추가한 모든 새 세트 멤버는 게시되었거나 게시 취소된 상태를 유지합니다. |
| 아니요 | 예 | 게시됨 | 게시됨 |
| 아니요 | 아니요 | 게시 취소됨 | 기존 세트 구성원과 편집 중에 새로 추가한 모든 세트 구성원은 게시된 상태나 게시 취소된 상태를 유지합니다. |

[수동 자산 게시](publishing-files.md#manually_publishing_assets) 및 [수동 자산 게시 취소](publishing-files.md#manually_unpublishing_assets)를 참조하십시오.

**오퍼 집합 편집**

1. To edit an offer set, display the offer set in Grid view or List view, and then click its **Edit** rollover button.
1. 타겟 클래식 오퍼 세트 페이지에서 다음 중 하나를 수행합니다.

   * **오퍼**&#x200B;제거오퍼를 선택한 다음 **삭제를** 클릭하여 세트에서 오퍼를 제거합니다.
   * **오퍼**&#x200B;추가오퍼를 추가하는 방법은 작업 중인 오퍼 집합 유형에 따라 달라집니다.
   * **템플릿**&#x200B;추가 **및 미리 보기를**&#x200B;클릭하고 오퍼 추가 및 미리 보기 페이지에서 다른 오퍼를 만듭니다.
   * **이미지 및 비디오**&#x200B;이미지나 비디오를 Target Classic 오퍼 집합 페이지로 드래그합니다.
   >[!NOTE]
   >
   >캠페인과 연결된 오퍼 집합은 삭제할 수 없습니다. 캠페인과 연관된 오퍼 세트를 삭제하려면 Target Classic에 로그온하고 캠페인 연결을 먼저 제거합니다. 캠페인에서 연결을 해제한 후에도 자산은 Scene7 Publishing System에서만 삭제할 수 있으므로 Target Classic에 로그인하지 않고 Target Classic에서만 로그인할 수 있습니다.

1. When you finish editing, near the lower-right corner of the page, ensure that **Publish after save** is selected (default).
1. **저장**&#x200B;을 클릭하고 저장 폴더를 선택한 다음에 세트 이름을 입력하고 **저장**&#x200B;을 클릭합니다.

## 오퍼 집합 삭제 {#deleting-an-offer-set}

삭제된 오퍼 집합은 휴지통으로 이동합니다. 하지만 삭제된 세트 내의 구성원(또는 &quot;하위&quot;)은 휴지통으로 이동하지 않고, 각각 기존의 게시된 상태나 게시 취소된 상태를 유지합니다.

[수동 자산 게시](publishing-files.md#manually_publishing_assets) 및 [수동 자산 게시 취소](publishing-files.md#manually_unpublishing_assets)를 참조하십시오.

**오퍼 집합 삭제**

1. [격자 보기], [목록 보기] 또는 [상세 보기]에서 오퍼 집합을 하나 이상 선택합니다.
1. 글로벌 탐색 막대에서 **파일** > **삭제** > **삭제**&#x200B;를 클릭합니다.

>[!MORELIKETHIS]
>
>* [템플릿 매개 변수 만들기](creating-template-parameters.md#creating_template_parameters)

