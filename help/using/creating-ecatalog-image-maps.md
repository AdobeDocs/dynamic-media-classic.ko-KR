---
title: eCatalog 이미지 맵 만들기
description: Adobe Dynamic Media Classic에서 eCatalog 이미지 맵을 만드는 방법을 알아봅니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 5e7f39a5-36a6-40df-8752-064a582c9346
topic: Integrations, Development
level: Experienced
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '1494'
ht-degree: 26%

---

# eCatalog 이미지 맵 만들기{#creating-ecatalog-image-maps}

이미지 맵은 eCatalog 페이지의 영역으로서 마우스로 롤오버하거나 다양한 종류의 작업을 트리거하도록 선택할 수 있습니다. 예를 들어 이미지 맵 위로 포인터를 이동하면 항목에 대한 롤오버 텍스트 설명이 표시됩니다. 이미지 맵을 선택하면 다른 작업이 시작됩니다. 예를 들어, 사용자가 항목에 대해 자세히 알아보거나 구매할 수 있도록 웹 페이지를 열거나, 사용 중인 항목을 보기 위해 비디오를 시작할 수 있습니다.

## eCatalog 이미지 맵 그리기 {#drawing-ecatalog-image-maps}

eCatalog의 경우 eCatalog 화면의 [맵 페이지] 탭에서 이미지 맵을 그립니다. 이 화면은 eCatalog 페이지가 표시되는 [이미지 맵] 영역과 오른쪽의 [이미지 맵] 목록으로 구성됩니다. 이미지 맵을 만들 때 이미지 맵 목록에 이름이 입력됩니다.

1. 전자 카탈로그의 롤오버 **[!UICONTROL 편집]** 단추를 선택합니다.
1. **[!UICONTROL 페이지 매핑]**&#x200B;을 선택합니다.
1. [맵 페이지] 화면 왼쪽에서 원하는 페이지를 선택합니다.
1. [이미지 맵] 영역에서 사각형 또는 다각형(다변형) 이미지 맵을 그립니다.

   * **사각형 맵**: 사각형 이미지 맵 도구를 선택하고 페이지에서 드래그하여 사각형을 만듭니다.

   * **다각형 맵**: [다각형 이미지 맵] 도구를 선택한 다음 이미지의 둘레를 필요한 횟수만큼 선택합니다. 선택하면 Adobe Dynamic Media Classic이 이미지 맵의 테두리를 그립니다.

     이미지 맵을 그리면 Adobe Dynamic Media Classic에서 이미지 맵 목록에 이름을 지정합니다. 이 이름을 형성하기 위해 Adobe Dynamic Media Classic은 작업 중인 eCatalog 페이지의 이름에 순차적 번호를 추가합니다.

1. (선택 사항) 이미지 맵 목록의 [!UICONTROL 이름] 열에서 이미지 맵의 새 이름을 입력할 수 있습니다. 입력한 이름에 공백을 포함하지 마십시오.
1. 뷰어가 이미지 맵을 선택하면 새 웹 페이지를 열 수 있습니다. [이미지 맵] 목록 패널의 URL 열에 웹 페이지의 URL을 입력합니다.

   URL(Href 템플릿)을 더 쉽게 입력하려면 **[!UICONTROL 편집]**&#x200B;을 선택하고 템플릿을 입력하십시오.

[템플릿을 사용하여 JavaScript 및 URL 입력](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls)을 참조하십시오.

1. (선택 사항) [표시] 드롭다운 목록에서 **[!UICONTROL 롤오버 텍스트]**&#x200B;를 선택한 다음 사용자가 이미지 맵 위로 포인터를 이동할 때 화면에 표시할 텍스트를 입력합니다.
1. (선택 사항) [표시] 드롭다운 목록에서 **[!UICONTROL 다른 작업]**&#x200B;을 선택하고, 사용자가 이미지 맵 위로 포인터를 이동할 때 흐림 또는 포커스 작업을 트리거할 특성을 입력합니다.

   [이미지 맵에 대한 다른 작업 정의](creating-image-maps.md#defining_other_actions_for_image_maps)를 참조하십시오.

1. **[!UICONTROL 저장]**&#x200B;을 선택합니다.
1. (선택 사항) 기본 eCatalog 뷰어 사전 설정으로 eCatalog를 보려면 **[!UICONTROL 미리 보기]**&#x200B;를 선택합니다.

이미지 맵을 삭제하려면 이미지 맵 목록에서 이름을 선택하고 **[!UICONTROL 삭제]**&#x200B;를 선택합니다. 이미지 맵을 삭제하지 않고 페이지에서 이미지 맵을 일시적으로 비활성화할 수 있습니다. [이미지 맵] 목록 패널에서 [이미지 맵 기준] 옵션을 선택합니다.

## eCatalog에 리치 미디어 포함 {#embedding-rich-media-in-an-ecatalog}

eCatalog의 리치 미디어 옵션을 사용하여 eCatalog에 추가한 이미지 맵에 MP4 형식의 비디오나 회전 집합을 추가할 수 있습니다. 사용자가 eCatalog에서 이미지 맵 영역을 선택하면 관련 회전 집합 또는 비디오가 표시됩니다. 이 기능은 고객이 사용 중인 항목을 보거나 다른 각도 및 관점에서 항목을 보려는 경우 특히 유용합니다.

고객이 이미지 맵 위로 포인터를 이동하면 고객이 선택한 항목을 알 수 있도록 툴팁 텍스트를 선택적으로 표시할 수도 있습니다.

**eCatalog에 리치 미디어를 포함하려면:**

1. eCatalog 이미지 맵을 그립니다.

   [전자 카탈로그 이미지 맵 그리기](creating-ecatalog-image-maps.md#drawing_ecatalog_image_maps)를 참조하십시오.

1. 표시 드롭다운 목록에서 **[!UICONTROL 리치 미디어]**&#x200B;를 선택합니다.
1. 왼쪽의 Assets 추가 패널에서 포함할 회전 집합 또는 비디오(MP4 형식) 자산이 포함된 폴더로 이동합니다.
1. 자산을 이미지 맵으로 드래그합니다.
1. (선택 사항) 이미지 맵 목록 패널의 **[!UICONTROL 도구 설명]** 열 머리글 아래에 뷰어가 이미지 맵 위로 포인터를 이동할 때 화면에 표시할 텍스트를 입력합니다.
1. **[!UICONTROL 저장]**&#x200B;을 선택합니다.

## eCatalog 이미지 맵 편집 {#editing-ecatalog-image-maps}

eCatalog 화면의 [맵 페이지] 탭에서 시작하여 다음 기술을 통해 eCatalog 이미지 맵을 편집합니다.

* **위치 조정**: 패닝 도구를 선택하고 포인터를 맵 테두리 근처로 이동하되 그 근처로는 이동하지 마십시오. 포인터에 네 방향 화살표가 표시되면 전체 이미지 맵을 새 위치로 드래그합니다.

  [이미지 맵의 위치, 모양 및 크기 조정](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps)을 참조하세요.

* **모양 및 크기 변경**: 사각형 이미지 맵의 크기를 조정하려면 패닝 도구를 선택합니다. 포인터를 경계선 또는 모서리로 이동하고 양방향 화살표 아이콘이 표시되면 드래그합니다. 다각형 이미지 맵의 크기를 조정하려면 사각형 선택 핸들을 드래그합니다. 선택 핸들을 만들려면 이미지 맵의 테두리를 선택하고 드래그합니다.

  [이미지 맵의 위치, 모양 및 크기 조정](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps)을 참조하세요.

* **이미지 맵 삭제**: 패닝 도구를 선택하고 이미지 맵을 선택하여 선택한 다음 **[!UICONTROL 삭제]**&#x200B;를 선택합니다.

  eCatalog에서 모든 이미지 맵을 제거하려면 **[!UICONTROL 페이지 순서 지정]** 탭을 선택한 다음 **[!UICONTROL 맵 지우기]**&#x200B;를 선택하십시오.

* **겹치는 이미지 맵 처리**: 이미지 맵 목록에서 이미지 맵 순서를 변경하려면 드래그하십시오.

  [중복 이미지 맵 처리](creating-image-maps.md#handling_overlapping_image_maps)를 참조하십시오.

* **다른 페이지에 이미지 맵 복사**: **[!UICONTROL 다음 페이지에 맵 복사]**&#x200B;를 선택합니다(맵 페이지 탭에 있는지 확인). 이미지 선택 화면에서 이미지 맵을 복사할 페이지를 선택하고 **[!UICONTROL 선택]**&#x200B;을 선택합니다.

  [다른 이미지에 이미지 맵 복사](creating-image-maps.md#copying_image_maps)를 참조하십시오.

>[!NOTE]
>
>eCatalog의 다른 페이지에 이미지 맵을 복사할 때 eCatalog의 모든 이미지 맵을 다른 eCatalog에 복사할 수 있습니다. [다른 전자 카탈로그 간에 이미지 맵 복사](creating-ecatalog-image-maps.md#copying_image_maps_between_ecatalogs)를 참조하세요.

## 이미지 맵 데이터 검토 및 가져오기 {#reviewing-and-importing-image-map-data}

[맵 요약] 화면에서는 eCatalog에 대한 메타데이터를 제공합니다. [맵 요약] 화면에서 시작하여 eCatalog의 이미지 맵 데이터를 일괄 가져올 수도 있습니다. 이런 방식으로 이미지 맵 데이터를 가져오면 이미지 맵 URL과 롤오버 텍스트를 쉽게 입력할 수 있습니다.

맵 요약 화면을 보려면 eCatalog 화면의 맵 페이지 탭에서 **[!UICONTROL 요약]**&#x200B;을(를) 선택하십시오.

### 이미지 맵 데이터 요약 검토 {#review-image-map-data-summary}

1. [페이지 매핑] 화면에서 **[!UICONTROL 요약]**&#x200B;을 선택합니다.

   맵 요약 화면에는 eCatalog에 있는 이미지 맵, URL, 롤오버 텍스트 설명 및 기타 작업의 수가 표시됩니다.

1. 롤오버 키 오류가 있는 경우 **[!UICONTROL Rollover_Key 오류]** 열에서 오류를 선택하여 오류를 수정하기 위해 스프레드시트에서 변경해야 하는 내용을 확인합니다. 이 메시지에서 텍스트를 선택하고 복사한 다음 스프레드시트에 붙여 넣을 수 있습니다.
1. eCatalog 뷰어에서 페이지를 검사할 수 있도록 **[!UICONTROL 미리 보기]**&#x200B;를 선택하십시오. X를 선택하여 요약 화면을 닫고 [맵 페이지] 화면으로 돌아가거나 **[!UICONTROL 닫기]**&#x200B;를 선택하여 [찾아보기]로 돌아갑니다.

### 이미지 맵 데이터 가져오기 {#import-image-map-data}

각 페이지에서 이미지 맵 데이터를 입력하는 대신 전체 eCatalog의 데이터를 [맵 요약] 화면으로 가져올 수 있습니다. 탭으로 구분된 파일이나 XML DTD 형태로 이미지 맵 데이터를 가져옵니다. 파일의 필드는 [맵 요약] 화면에 표시된 순서대로 정렬되어야 합니다(이름, 목차 레이블, 맵, URL, 롤오버 텍스트, 다른 작업 및 검색 문자열). 이미지 맵 데이터를 가져오면 각 이미지 맵을 만들 때 이미지 맵 목록에 데이터를 입력하는 문제를 줄일 수 있습니다.

>[!NOTE]
>
>이미지 맵 데이터를 가져오기 전에 이미지 맵이 이미 만들어져 있어야 합니다.

[맵 요약] 화면에서 시작하여 다음 단계에 따라 직접 만든 이미지 맵의 이미지 맵 데이터를 가져옵니다.

1. **[!UICONTROL 맵 데이터 가져오기]**&#x200B;를 선택합니다.
1. 메타데이터 가져오기 대화 상자에서 **[!UICONTROL 찾아보기]**&#x200B;를 선택한 다음 탭으로 구분된 또는 XML DTD 파일을 선택합니다.
1. [작업 이름] 필드에 파일 이름을 입력합니다. 확장자를 유지해야 합니다.
1. **[!UICONTROL 업로드]**&#x200B;를 선택합니다.

## 다른 전자 카탈로그 간 이미지 맵 복사 {#copying-image-maps-between-ecatalogs}

eCatalog에 있는 모든 이미지 맵을 다른 eCatalog로 복사할 수 있습니다. 이런 방식의 이미지 맵 복사는 동일한 eCatalog의 외국어 번역 간에 이미지 맵을 복사하는 편리한 방법입니다. 복사가 성공하려면 Adobe Dynamic Media Classic에서는 페이지 수가 동일한 eCatalogs와 이미지가 동일한 간에 복사하는 것이 좋습니다.

>[!NOTE]
>
>이미지 맵을 복사하는 타겟 eCatalog에 이미지 맵이 이미 포함되어 있으면 복사 시 해당 이미지 맵이 삭제됩니다.

한 eCatalog의 모든 이미지 맵을 다른 eCatalog에 복사하려면 다음을 수행하십시오.

1. 복사하려는 이미지 맵이 있는 eCatalog를 선택하고 eCatalog의 롤오버 **[!UICONTROL 편집]** 단추를 선택합니다.
1. 페이지 순서 탭에서 **[!UICONTROL 맵 복사]**&#x200B;를 선택합니다.
1. 자산 선택 대화 상자에서 이미지 맵을 복사할 eCatalog를 선택한 다음 **[!UICONTROL 선택]**&#x200B;을 선택합니다.

Adobe Dynamic Media Classic은 이미지 맵을 복사하는 대상 eCatalog에 크기가 다른 페이지 또는 이미지 수가 있는 경우 경고 메시지를 표시합니다. 경고에도 불구하고 이미지 맵을 복사하려면 **[!UICONTROL 계속]**&#x200B;을(를) 선택하십시오.
