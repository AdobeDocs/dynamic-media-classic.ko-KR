---
title: 오퍼 집합 만들기
description: Adobe Dynamic Media Classic에서 오퍼 세트를 만드는 방법을 알아봅니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 05f2cce0-72bf-4933-87ab-c9003c848e35
topic: Integrations, Development
level: Experienced
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '1236'
ht-degree: 21%

---

# 오퍼 집합 만들기 {#creating-an-offer-set}

다음 유형의 오퍼 세트를 만들 수 있습니다.

* 비디오
* 매개 변수화된 템플릿
* 이미지

템플릿의 경우 **[!UICONTROL 추가 및 미리 보기]**&#x200B;를 선택한 다음 선택한 매개 변수를 설정합니다. 다른 오퍼 집합 유형에는 매개 변수가 포함되어 있지 않지만, **[!UICONTROL 미리 보기]**&#x200B;를 선택하고 사용 가능한 사전 설정을 변경하여 매개 변수를 사용자 지정할 수 있습니다.

Adobe Dynamic Media Classic은 오퍼 세트를 만들고 편집할 수 있는 도구를 제공합니다.

>[!NOTE]
>
>오퍼 세트를 만들기 전에 세트에 사용할 모든 자산을 Adobe Dynamic Media Classic에 게시해야 합니다. [수동 자산 게시](publishing-files.md#manually_publishing_assets) 및 [수동 자산 게시 취소](publishing-files.md#manually_unpublishing_assets)를 참조하십시오.

## 오퍼 집합 유형 {#types-of-offer-sets}

다음 유형의 오퍼 세트에서 오퍼 세트를 만듭니다.

* **이미지**: 오퍼 집합에 대한 이미지를 조합할 수 있습니다. 각 이미지에는 세트에 다른 오퍼가 포함됩니다.

* **이미지 템플릿**: **[!UICONTROL 빌드]** > 템플릿 기본 사항 명령을 사용하여 Adobe Dynamic Media Classic에서 이미지 템플릿을 매개 변수화할 수 있습니다. 매개 변수를 통해 템플릿의 구성 요소, 텍스트 프레임의 텍스트, 다른 이미지를 스왑하고 사용자 정의할 수 있습니다. 오퍼 세트의 경우, 예를 들어 템플릿 매개 변수를 사용하여 오퍼 세트의 동일한 이미지에 변형을 만들 수 있습니다. 이미지 템플릿을 만들고 매개 변수화하는 방법에 대한 자세한 내용은 [템플릿 매개 변수 만들기](creating-template-parameters.md#creating_template_parameters)를 참조하십시오.

[템플릿 기본 사항](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) 교육 비디오도 참조하세요.

* **비디오**: 오퍼 집합에 대한 비디오를 조합할 수 있습니다. 각 비디오는 집합에서 각기 다른 오퍼입니다.

## 매개 변수가 있는 템플릿으로 오퍼 집합 만들기 {#creating-an-offer-set-with-a-parameterized-template}

오퍼 집합을 만들 때 **[!UICONTROL 저장 후 Publish]** 옵션은 다음과 같은 방법으로 집합 및 집합 구성원에 영향을 줍니다.

| 저장하기 전에 **[!UICONTROL 저장 후 Publish]** 옵션을 선택했습니까? | 저장 후 세트 상태 | 저장 후 세트 구성원 상태 |
| --- | --- | --- |
| 예 | 게시됨 | 게시됨 |
| 아니요 | 게시 취소됨 | 세트 구성원은 게시된 상태나 게시되지 않은 상태를 유지합니다. |

[수동 자산 게시](publishing-files.md#manually_publishing_assets) 및 [수동 자산 게시 취소](publishing-files.md#manually_unpublishing_assets)를 참조하십시오.

**매개 변수가 있는 템플릿을 사용하여 오퍼 집합을 만들려면:**

1. 템플릿 또는 배너를 선택합니다.
1. **[!UICONTROL 빌드]** > **[!UICONTROL Test&amp;Target 오퍼 집합]**(으)로 이동합니다.

   Test&amp;Target 오퍼 세트 페이지에 오퍼 세트의 오퍼가 나열됩니다. 목록에서 첫 번째 항목은 개체입니다.

1. 개체를 선택하고 **[!UICONTROL 추가 및 미리 보기]**&#x200B;를 선택합니다.

   이 페이지의 왼쪽에는 템플릿의 매개 변수와 해당 값이 나열됩니다.

1. 매개 변수 값을 변경하여 오퍼를 만듭니다. 예를 들어 텍스트 필드에 다른 텍스트를 입력하거나, 레이어의 크기를 변경하거나, 한 이미지를 다른 이미지로 바꾸거나, 다른 뷰어 사전 설정을 선택할 수 있습니다.
1. 오퍼를 오퍼 집합의 일부로 저장하려면 **[!UICONTROL 저장]** 또는 **[!UICONTROL 다른 이름으로 저장**]**&#x200B;을 선택하십시오.

   Test&amp;Target 오퍼 집합 페이지에 만든 오퍼가 나열됩니다.

1. 3-5 단계를 반복하여 집합에 대한 추가 오퍼를 만듭니다.
1. 완료되면 페이지의 오른쪽 아래 모서리에서 **[!UICONTROL 저장 후 Publish*]**&#x200B;이 선택되었는지 확인합니다(기본값).
1. **[!UICONTROL 닫기]**&#x200B;를 선택하고 오퍼 집합의 이름을 입력한 다음 **[!UICONTROL 저장]**&#x200B;을 선택합니다.

Test&amp;Target 오퍼 세트 페이지를 닫기 전에 오퍼 세트를 Adobe Target Standard/Premium으로 푸시합니다. [Test&amp;Target에 오퍼 집합 푸시](pushing-offer-sets-target.md#pushing_offer_sets_to_target)를 참조하십시오.

## 이미지 또는 비디오로 오퍼 집합 만들기 {#creating-an-offer-set-with-images-or-videos}

오퍼 집합을 만들 때 **[!UICONTROL 저장 후 Publish]** 옵션은 다음과 같은 방법으로 집합 및 집합 구성원에 영향을 줍니다.

| 저장하기 전에 **[!UICONTROL 저장 후 Publish]** 옵션을 선택했습니까? | 저장 후 세트 상태 | 저장 후 세트 구성원 상태 |
| --- | --- | --- |
| 예 | 게시됨 | 게시됨 |
| 아니요 | 게시 취소됨 | 세트 구성원은 게시된 상태나 게시되지 않은 상태를 유지합니다. |

[수동 자산 게시](publishing-files.md#manually_publishing_assets) 및 [수동 자산 게시 취소](publishing-files.md#manually_unpublishing_assets)를 참조하십시오.

**이미지 또는 비디오로 오퍼 집합을 만들려면:**

1. 오퍼 세트에 대한 이미지 또는 비디오를 조합합니다. Test&amp;Target 오퍼 세트 화면이나 그리드 보기 또는 목록 보기에서 시작하여 다음 방법 중 하나를 사용합니다.

   * **Test&amp;Target 오퍼 집합 화면**: **[!UICONTROL 빌드]** > **[!UICONTROL Test&amp;Target 오퍼 집합]**&#x200B;으로 이동합니다. 이미지나 비디오를 화면으로 드래그합니다. 다양한 크기의 비디오나 이미지를 만들려면 이미지나 비디오의 여러 복사본에서 끌어 각 크기를 개별적으로 설정합니다.

   * **눈금 보기 또는 목록 보기**: 이미지 또는 비디오를 선택한 다음 **[!UICONTROL 빌드]** > **[!UICONTROL Test&amp;Target 오퍼 집합]**(으)로 이동합니다.

1. 필요한 경우 이미지 또는 비디오를 선택하고 **[!UICONTROL 미리 보기]**&#x200B;를 선택합니다. 오퍼 미리 보기 페이지에서 선택한 이미지 또는 비디오의 크기와 모양을 변경할 수 있습니다. 또는 오퍼 세트의 모든 이미지 또는 비디오를 변경할 수 있습니다.

   * 사전 설정을 선택하여 이미지나 비디오의 모양과 크기를 변경합니다.
   * 선택한 사전 설정을 오퍼 집합의 모든 오퍼에 적용하려면 **[!UICONTROL 모든 오퍼에 사전 설정 선택]** 확인란을 선택합니다.

   **[!UICONTROL 저장]**&#x200B;을 선택하여 이미지 또는 비디오 오퍼에 대한 변경 사항을 저장합니다. 그런 다음 **[!UICONTROL 닫기]**&#x200B;를 선택하여 Test&amp;Target 오퍼 집합 페이지로 돌아갑니다.

1. 오퍼 집합에 대한 오퍼를 만들고 다른 이미지에 대한 이미지 사전 설정을 선택한 후 **[!UICONTROL 저장 후 Publish]**&#x200B;이 선택되었는지 확인합니다(기본값).
1. **[!UICONTROL 저장]**&#x200B;을 선택하고 오퍼 집합의 이름을 입력한 다음 **[!UICONTROL 저장]**&#x200B;을 선택합니다.

Test&amp;Target 오퍼 세트 페이지를 닫기 전에 오퍼 세트를 Adobe Target Standard/Premium으로 푸시합니다. [Test&amp;Target에 오퍼 집합 푸시](pushing-offer-sets-target.md#pushing_offer_sets_to_target)를 참조하십시오.

## 오퍼 집합 편집 {#editing-an-offer-set}

게시된 집합을 편집하든 게시되지 않은 집합을 편집하든 **[!UICONTROL 저장 후 Publish]** 옵션은 다음과 같은 방법으로 집합 및 집합 구성원에 영향을 줍니다.

| 세트를 이미 게시했습니까? | 편집을 저장하기 전에 **[!UICONTROL 저장 후 Publish]** 옵션이 선택되었습니까? | 저장 후 세트 상태 | 저장 후 세트 구성원 상태 |
| --- | --- | --- | --- |
| 예 | 예 | 게시됨 | 게시됨 |
| 예 | 아니요 | 게시됨 | 기존 집합 구성원은 게시된 상태를 유지합니다. 편집 중에 새로 추가한 모든 세트 구성원은 게시된 상태나 게시 취소된 상태를 유지합니다. |
| 아니요 | 예 | 게시됨 | 게시됨 |
| 아니요 | 아니요 | 게시 취소됨 | 기존 세트 구성원과 편집 중에 새로 추가한 모든 세트 구성원은 게시된 상태나 게시 취소된 상태를 유지합니다. |

[수동 자산 게시](publishing-files.md#manually_publishing_assets) 및 [수동 자산 게시 취소](publishing-files.md#manually_unpublishing_assets)를 참조하십시오.

**오퍼 집합을 편집하려면:**

1. 오퍼 집합을 편집하려면 [표 보기] 또는 [목록 보기]에서 오퍼 집합을 표시한 다음 해당 **[!UICONTROL 편집]** 롤오버 단추를 선택하십시오.
1. Test&amp;Target 오퍼 집합 페이지에서 다음 중 하나를 수행합니다.

   * **오퍼 제거**: 오퍼를 선택한 다음 **[!UICONTROL 삭제]**&#x200B;를 선택하여 집합에서 오퍼를 제거합니다.
   * **오퍼 추가**: 오퍼 추가 방법은 작업 중인 오퍼 집합의 유형에 따라 다릅니다.
      * **템플릿**: **[!UICONTROL 추가 및 미리 보기]**&#x200B;를 선택하고 오퍼 추가 및 미리 보기 페이지에서 다른 오퍼를 만드십시오.
      * **이미지 및 비디오**: 이미지 또는 비디오를 Test&amp;Target 오퍼 집합 페이지로 끌어옵니다.

   >[!NOTE]
   >
   >캠페인과 연결된 오퍼 세트는 삭제할 수 없습니다. 캠페인과 연결된 오퍼 세트를 삭제하려면 Adobe Target Standard/Premium에 로그인한 다음 캠페인 연결을 먼저 제거하십시오. 캠페인에서 연결을 해제한 후에도 에셋은 Adobe Dynamic Media Classic에서만 삭제할 수 있으며 Adobe Target Standard/Premium 내에서는 삭제되지 않고 Adobe Target Standard/Premium에 로그인해야 합니다.

1. 편집을 마치면 페이지의 오른쪽 아래 모서리에서 **[!UICONTROL 저장 후 Publish]**&#x200B;이 선택되었는지 확인합니다(기본값).
1. **[!UICONTROL 저장]**&#x200B;을 선택하고 저장소 폴더를 선택한 다음 집합 이름을 입력한 다음 **[!UICONTROL 저장]**&#x200B;을 선택합니다.

## 오퍼 집합 삭제 {#delet-an-offer-set}

삭제된 오퍼 집합은 휴지통으로 이동합니다. 그러나 해당 집합 내의 멤버(또는 &quot;하위&quot;)는 영향을 받지 않습니다. 대신 각 멤버는 기존의 게시 또는 게시 취소 상태를 유지합니다.

[수동 자산 게시](publishing-files.md#manually_publishing_assets) 및 [수동 자산 게시 취소](publishing-files.md#manually_unpublishing_assets)를 참조하십시오.

**오퍼 집합을 삭제하려면:**

1. 그리드 보기, 목록 보기 또는 세부 사항 보기에서 오퍼 집합 하나 이상을 선택합니다.
1. 전역 탐색 모음에서 **[!UICONTROL 파일]** > **[!UICONTROL 삭제]** > **삭제**(으)로 이동합니다.

>[!MORELIKETHIS]
>
>* [템플릿 매개 변수를 만드는 중](creating-template-parameters.md#creating_template_parameters)
