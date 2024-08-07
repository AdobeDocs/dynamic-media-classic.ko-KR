---
title: 템플릿 만들기
description: Adobe Dynamic Media Classic에서 템플릿을 만드는 방법을 알아봅니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: 23ac1a0f-c90b-4250-ae36-93702fb5ebd9
topic: Content Management
level: Experienced
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '3433'
ht-degree: 35%

---

# 템플릿 만들기

템플릿을 만들려면 **[!UICONTROL 빌드]** > **[!UICONTROL 템플릿 기본 사항]**(으)로 이동하십시오. [디자이너] 또는 [개발자]를 선택합니다. 이 페이지에서 이미지 및 텍스트 레이어를 추가할 수 있습니다. 레이어 순서를 조정하고, 레이어의 크기와 위치를 변경하고, 이미지와 텍스트에 그림자 및 후광 효과를 적용할 수도 있습니다.

[템플릿 기본 사항](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) 교육 비디오도 참조하세요.

>[!NOTE]
>
>이전 버전의 Adobe Dynamic Media Classic에서 만든 템플릿을 편집하는 경우 &quot;캔버스 레이어를 추가하시겠습니까?&quot;를 저장할 때 묻는 메시지가 표시됩니다. 기본 레이어를 추가하지 않으려면 **[!UICONTROL 아니요]**&#x200B;를 선택하십시오. 실수로 **[!UICONTROL 예]**&#x200B;를 선택한 경우 URL에서 `&allowCanvasPrompt` 및 `&layer=0` 수정자를 삭제하고 **[!UICONTROL Enter]** 또는 **[!UICONTROL Return]**&#x200B;을 누르십시오.

## 초기 템플릿 만들기 {#creating-the-initial-template}

템플릿 집합을 만들 때 **[!UICONTROL 저장 후 Publish]** 옵션은 다음과 같은 방법으로 집합 및 집합 구성원에 영향을 줍니다.

| 저장하기 전에 **[!UICONTROL 저장 후 Publish]** 옵션을 선택했습니까? | 저장 후 세트 상태 | 저장 후 세트 구성원 상태 |
| --- | --- | --- |
| 예 | 게시됨 | 게시됨 |
| 아니요 | 게시 취소됨 | 세트 구성원은 게시된 상태나 게시되지 않은 상태를 유지합니다. |

[수동 자산 게시](publishing-files.md#manually_publishing_assets) 및 [수동 자산 게시 취소](publishing-files.md#manually_unpublishing_assets)를 참조하십시오.

기존 템플릿에서 템플릿을 만들 수 있습니다. 템플릿을 열고 **[!UICONTROL 다른 이름으로 저장]**&#x200B;을 선택한 다음 [다른 이름으로 저장] 대화 상자에 새 이름을 입력합니다.

**초기 템플릿을 만들려면:**

1. 초기 템플릿을 만들려면 다음 방법 중 하나를 사용합니다.

   * **먼저 PSD 또는 이미지를 선택하십시오**: 검색 패널에서 템플릿에 사용할 PSD 파일 또는 이미지를 선택하고 **[!UICONTROL 빌드]** > **[!UICONTROL 템플릿 기본 사항]**(으)로 이동합니다.

   * **템플릿 화면에서 시작**: **[!UICONTROL 빌드]** > **[!UICONTROL 템플릿 기본 사항]**&#x200B;으로 이동합니다. [디자이너] 또는 [개발자]를 선택합니다.

1. 캔버스 크기 입력 대화 상자에서 템플릿에 대한 너비와 높이 측정값을 입력합니다.
1. 자산 라이브러리에서 폴더를 선택하고 템플릿에 사용할 PSD 파일이나 이미지를 [템플릿] 화면으로 드래그합니다.
1. 완료되면 페이지의 오른쪽 아래 모서리 근처에서 **[!UICONTROL 저장 후 Publish]**&#x200B;이 선택되었는지 확인합니다(기본값).
1. **[!UICONTROL 저장]**&#x200B;을 선택합니다.
1. 템플릿을 저장할 폴더를 선택하고 템플릿 이름을 입력한 다음 **[!UICONTROL 제출]**&#x200B;을 선택합니다.

   Adobe Dynamic Media Classic은 필요한 경우 템플릿을 정의하기 위한 템플릿 화면의 영역인 캔버스에 맞게 이미지를 축소합니다.

## 템플릿 집합 편집 {#editing-a-template-set}

게시된 집합 또는 게시되지 않은 템플릿 집합을 편집하든 관계없이 **[!UICONTROL 저장 후 Publish]** 옵션은 다음과 같은 방법으로 집합 및 집합 구성원에 영향을 줍니다.

| 세트를 이미 게시했습니까? | 편집을 저장하기 전에 **[!UICONTROL 저장 후 Publish]** 옵션이 선택되었습니까? | 저장 후 세트 상태 | 저장 후 세트 구성원 상태 |
| --- | --- | --- | --- |
| 예 | 예 | 게시됨 | 게시됨 |
| 예 | 아니요 | 게시됨 | 기존 집합 구성원은 게시된 상태를 유지합니다. 편집 중에 새로 추가한 모든 세트 구성원은 게시된 상태나 게시 취소된 상태를 유지합니다. |
| 아니요 | 예 | 게시됨 | 게시됨 |
| 아니요 | 아니요 | 게시 취소됨 | 기존 세트 구성원과 편집 중에 새로 추가한 모든 세트 구성원은 게시된 상태나 게시 취소된 상태를 유지합니다. |

[수동 자산 게시](publishing-files.md#manually_publishing_assets) 및 [수동 자산 게시 취소](publishing-files.md#manually_unpublishing_assets)를 참조하십시오.

**템플릿 집합을 편집하려면:**

1. 눈금 보기에서 템플릿 집합을 찾은 다음 이미지 아래에서 **[!UICONTROL 편집]**&#x200B;을 선택합니다.
1. 필요에 따라 템플릿을 변경합니다.
1. 편집을 마치면 페이지의 오른쪽 아래 모서리에서 **[!UICONTROL 저장 후 Publish]**&#x200B;이 선택되었는지 확인합니다(기본값).
1. **[!UICONTROL 저장]**&#x200B;을 선택하고 저장소 폴더를 선택한 다음 집합 이름을 입력한 다음 **[!UICONTROL 저장]**&#x200B;을 선택합니다.

## 템플릿 삭제

템플릿 세트를 삭제하면 세트 자체가 휴지통으로 이동됩니다. 그러나 해당 집합 내의 멤버(또는 &quot;하위&quot;)는 영향을 받지 않습니다. 대신 각 멤버는 기존의 게시 또는 게시 취소 상태를 유지합니다.

[수동 자산 게시](publishing-files.md#manually_publishing_assets) 및 [수동 자산 게시 취소](publishing-files.md#manually_unpublishing_assets)를 참조하십시오.

**템플릿을 삭제하려면:**

1. [격자 보기], [목록 보기] 또는 [상세 보기]에서 템플릿을 하나 이상 선택합니다.
1. 전역 탐색 모음에서 **[!UICONTROL 파일]** > **[!UICONTROL 삭제]** > **[!UICONTROL 삭제]**(으)로 이동합니다.

## 템플릿 이해 화면 {#understanding-the-template-screen}

[템플릿] 화면에서는 레이어를 조작하고 매개 변수화하기 위한 도구를 제공합니다.

템플릿을 만들 수 있도록 템플릿 화면에서 다음 도구를 사용합니다.

* **[!UICONTROL 패닝]**: 레이어를 선택하거나 캔버스 주위로 이동하거나 크기를 조정하거나 회전할 수 있습니다.

* **[!UICONTROL 텍스트]**: 텍스트 레이어를 만듭니다. 캔버스에서 끌어 텍스트 레이어를 만든 다음 레이어의 텍스트를 입력합니다. [텍스트 레이어 만들기](#creating-a-text-layer)를 참조하십시오.

* **[!UICONTROL 미리 보기]**: 미리 보기 화면을 열고 확대/축소 뷰어에 템플릿을 표시합니다. 웹 사이트 또는 애플리케이션에서 사용자에게 템플릿이 어떻게 표시되는지 확인합니다.

* **[!UICONTROL 매개 변수 요약]** 매개 변수 요약 화면을 엽니다. 템플릿의 각 레이어 이름과 각 레이어에서 활성화된 매개 변수 이름을 확인할 수 있습니다.

* **[!UICONTROL 텍스트 편집기 v4.3 및 텍스트 편집기 v4.2]**: 가장 최신의 모든 기능을 갖춘 텍스트 편집기를 사용하십시오. 텍스트 편집기 v4.3 또는 이전 텍스트 편집기 v4.2를 사용하도록 선택할 수 있습니다. 템플릿을 만들 때 기본적으로 텍스트 편집기 v4.3이 선택됩니다. 이전 템플릿을 편집할 때는 기본적으로 텍스트 편집기 v4.2가 선택됩니다. 텍스트 편집기 v4.3은 현재 자동 줄 바꿈을 지원하지 않으므로 자동 줄 바꿈을 사용하는 이전 템플릿을 편집할 때는 텍스트 편집기 v4.2를 사용하여 템플릿의 충실도를 그대로 유지합니다. 이전 템플릿에서 자동 줄바꿈을 사용하지 않는 경우 텍스트 편집기 v4.3을 선택하여 제공되는 여러 가지 새로운 기능을 활용할 수 있습니다. 예를 들어 여백을 늘리고 여백을 줄이며 텍스트를 모두 대문자로 설정하고 맞춤 텍스트를 복사합니다.

  >[!NOTE]
  >
  >텍스트 편집기 v4.2는 Adobe Dynamic Media Classic에서 옵션으로 제거할 예정입니다. 가능하면 텍스트 편집기 4.3을 사용하는 것이 좋습니다. **[!UICONTROL 자동 줄 바꿈]** 옵션은 텍스트 편집기의 향후 릴리스에 통합됩니다.

* **[!UICONTROL Designer 및 개발자]**: 역할을 가장 잘 설명하는 옵션을 선택합니다.

* **[!UICONTROL Canvas]**: 서식 파일을 정의하는 데 사용할 수 있는 총 영역을 픽셀 단위로 정의합니다. 기본 크기는 300 × 300픽셀입니다. 레이어가 캔버스에 배치됩니다.

* **[!UICONTROL 레이어 목록]**: 템플릿의 레이어 이름을 나열합니다. 레이어를 선택하려면 [레이어] 목록에서 해당 이름을 선택합니다. [레이어] 목록에서는 레이어에 효과를 추가하고, 레이어를 삭제하고, 레이어 순서를 조정하고, 레이어를 매개 변수화하기 위한 도구를 제공합니다. [레이어를 사용한 작업](#working-with-layers)을 참조하세요.

* **[!UICONTROL 레이어 속성 영역]**: 이 영역에서는 레이어의 배경색, 불투명도, 크기 및 위치를 변경할 수 있는 도구를 제공합니다. 캔버스의 배경색, 불투명도 및 크기를 변경할 수도 있습니다. 그림자 및 후광 효과를 조정할 수도 있습니다. [레이어를 사용한 작업](#working-with-layers)을 참조하세요.

## 이미지 레이어 만들기 {#creating-image-layers}

1. 자산 라이브러리에서 캔버스로 이미지를 드래그합니다.

   이미지의 ID 이름이 [레이어] 목록에 표시됩니다.

   >[!NOTE]
   >
   >필요한 경우 Adobe Dynamic Media Classic에서는 이미지 레이어를 만들 때 이미지를 축소하여 캔버스에 맞춥니다.

## 텍스트 레이어 만들기 {#creating-a-text-layer}

1. **[!UICONTROL 텍스트]** 도구를 선택합니다.
1. 캔버스나 이미지에 텍스트 상자를 끌어서 만듭니다.
1. 텍스트 화면이 열리면 미리보기 탭에서 다음 중 하나를 수행하여 텍스트를 추가합니다.

   * 텍스트 상자에 텍스트를 입력합니다. [맞춤 텍스트 복사]를 선택하여 텍스트 상자에 텍스트를 맞춥니다.
   * 클립보드의 텍스트를 텍스트 상자에 붙여 넣습니다.

1. **[!UICONTROL 적용]**&#x200B;을 선택한 다음 텍스트 화면을 닫습니다.

### 텍스트 서식 지정 {#format-text}

텍스트 레이어에서 텍스트 서식을 지정하려면 다음을 수행합니다.

1. [레이어] 목록에서 편집하려는 텍스트가 포함된 텍스트 상자의 이름을 두 번 클릭합니다. 텍스트 편집기가 열립니다.
1. 텍스트 편집기의 텍스트 상자에서 서식을 지정할 텍스트를 선택합니다. 모든 텍스트, 일부 또는 개별 문자를 선택할 수 있습니다.
1. 다음 서식 옵션을 지정한 다음 **[!UICONTROL 적용]**&#x200B;을 선택합니다.

   * **[!UICONTROL 글꼴]**: 글꼴 메뉴에서 글꼴을 선택합니다. 원하는 글꼴이 메뉴에 나타나지 않으면 Adobe Dynamic Media Classic에 업로드할 수 있습니다. 글꼴을 참조하십시오.

   * **[!UICONTROL 글꼴 크기]**: 메뉴에서 글꼴 크기를 선택하거나 상자에 특정 크기를 입력하거나 **[!UICONTROL 위쪽]** 또는 **[!UICONTROL 아래쪽]** 화살표를 선택하여 크기를 두 포인트 늘리거나 줄입니다.

   * **[!UICONTROL 색상]**: 텍스트 색상을 선택하려면 선택하십시오.

   * **[!UICONTROL 굵게]**, **[!UICONTROL 기울임꼴]** 또는 **[!UICONTROL 밑줄]**: 텍스트를 선택한 다음 텍스트에 적용할 서식 유형의 아이콘을 선택합니다.

   * **[!UICONTROL 모두 대문자]**, **[!UICONTROL 위 첨자]** 또는 **[!UICONTROL 아래 첨자]**: 텍스트를 선택한 다음 텍스트에 적용할 서식 유형의 아이콘을 선택합니다.

   * **[!UICONTROL 정렬]**: 텍스트 레이어에서 텍스트를 왼쪽, 가운데 또는 오른쪽 정렬하려면 [정렬] 단추를 선택하십시오.

   * **[!UICONTROL 추적]**: 단어 사이의 간격을 조정할 숫자 값을 입력하거나 선택합니다.

   * **[!UICONTROL 커닝]**: 문자 사이의 간격을 조정할 숫자 값을 입력하거나 선택합니다.

   * **[!UICONTROL 줄 간격]**: 줄 간격 크기를 조정할 숫자 값을 입력하거나 선택합니다.

   * **[!UICONTROL 기준선 이동]**: 주변 텍스트의 기준선을 기준으로 선택한 문자를 위나 아래로 이동할 숫자 값을 입력하거나 선택합니다. 이 옵션은 분수를 수동으로 설정하거나 인라인 그래픽의 위치를 조정할 때 특히 유용합니다.

>[!NOTE]
>
>마지막 작업을 취소하려면 **[!UICONTROL 실행 취소]**&#x200B;를 선택하십시오. **[!UICONTROL 실행 취소]**&#x200B;를 선택한 후 작업을 되돌리려면 **[!UICONTROL 다시 실행]**&#x200B;을 선택하세요.

### 단락 서식 적용하기 {#format-paragraphs}

1. [레이어] 목록에서 편집하려는 텍스트가 포함된 텍스트 상자의 이름을 두 번 클릭합니다. 텍스트 편집기가 열립니다.
1. 서식을 지정할 단락을 선택합니다.
1. 다음 서식 옵션을 지정한 다음 **[!UICONTROL 적용]**&#x200B;을 선택합니다.

   * **[!UICONTROL 정렬]**: **[!UICONTROL 왼쪽 정렬]**, **[!UICONTROL 가운데 정렬]**, **[!UICONTROL 오른쪽 정렬]** 또는 **[!UICONTROL 양쪽 맞춤]**&#x200B;을 클릭하여 정렬 유형을 지정합니다.

   * **[!UICONTROL 단락 양쪽 맞춤 끝]**: 단락의 마지막 줄에 대한 양쪽 맞춤 유형을 지정하려면 선택합니다. 마지막 줄은 왼쪽으로 정렬되고, 마지막 줄은 가운데로 정렬되며, 마지막 줄은 오른쪽으로 정렬됩니다.

   * **[!UICONTROL 줄 간격]**: 단락의 모든 줄 사이의 간격을 조정할 숫자 값을 입력하거나 선택합니다.

   * **[!UICONTROL 모두 들여쓰기]**: 텍스트를 들여쓰려면 선택합니다.

   * **[!UICONTROL 들여쓰기 제거]**: 텍스트를 들여쓸 양을 줄이려면 선택합니다.

   * **[!UICONTROL 첫 줄 들여쓰기]**: 텍스트의 첫 줄을 들여쓸 양을 지정합니다.

   * **[!UICONTROL 단락 앞 공백]**: 단락의 첫 번째 텍스트 줄 위에 표시할 공백의 크기를 지정합니다.

   * **[!UICONTROL 단락 뒤 공백]**: 단락의 마지막 텍스트 줄 아래에 표시할 공백의 크기를 지정합니다.

   * **[!UICONTROL 세로 맞춤]**: 텍스트 상자 내에서 텍스트를 세로로 표시할 위치를 선택합니다(위쪽, 중간, 아래쪽).

   * **[!UICONTROL 텍스트 방향]**: 텍스트를 표시할 방향(오른쪽에서 왼쪽 또는 왼쪽에서 오른쪽)을 선택합니다.

### 텍스트 레이어 속성 조정 {#adjust-text-layer-properties}

1. [템플릿 기본] 화면에서 조정하려는 텍스트 상자를 선택합니다.
1. [레이어 속성] 패널에서 다음 중 원하는 선택 사항을 선택합니다.

   * **[!UICONTROL 텍스트 축소(텍스트 편집기 v4.2만 해당)]**: 텍스트 상자 안에 맞도록 텍스트를 축소하려면 이 옵션을 선택하십시오.

   * **[!UICONTROL 줄 바꿈(텍스트 편집기 v4.2만 해당)]**: 텍스트 줄 바꿈 여부 또는 방법을 지정하려면 줄 바꿈 옵션을 선택하십시오.

   * **[!UICONTROL 줄 바꿈]**: 가로로 너무 작은 텍스트 상자에 맞게 텍스트를 줄바꿈합니다.

   * **[!UICONTROL 줄 바꿈 안 함]**: 텍스트 상자가 가로로 너무 작으면 텍스트를 줄바꿈하지 않고 대신 텍스트 일부를 잘라냅니다.

   * **[!UICONTROL 줄바꿈을 사용하지 않는 줄 바꿈]**: 텍스트 상자에 맞게 텍스트를 줄바꿈하고 단어를 줄바꿈하지 않습니다.

   * **[!UICONTROL 위치]**: 캔버스에서 텍스트 상자의 위치를 지정합니다.

   * **[!UICONTROL 패딩]**: 여백을 추가하거나 레이어 사각형을 자릅니다. [왼쪽], [위쪽], [아래쪽] 및 [오른쪽]에 추가하거나 제거할 픽셀 수를 지정합니다. 자르기에 여백이나 음수를 추가하려면 양수를 입력합니다.

### 텍스트 소스 코드 보기 및 편집 {#view-and-edit-text-source-code}

텍스트 편집기의 Source 탭에 제공된 정보는 참조용입니다. 소스 코드 편집에 익숙한 경우에만 텍스트를 편집합니다.

1. [레이어] 목록에서 편집하려는 텍스트가 포함된 텍스트 상자의 이름을 두 번 클릭합니다. 텍스트 편집기가 열립니다.
1. 텍스트 편집기에서 텍스트에 대한 소스 코드를 표시하려면 텍스트 편집기에서 **[!UICONTROL Source]** 탭을 선택합니다.
1. 원하는 대로 텍스트를 보거나 편집합니다.

   [미리 보기]와 [소스] 보기를 전환하는 경우 변경 사항이 유지됩니다.

1. **[!UICONTROL 적용]**&#x200B;을 선택하여 편집 내용을 렌더링합니다.

## 레이어를 사용한 작업 {#working-with-layers}

[레이어] 목록과 [레이어 속성] 영역을 사용하여 레이어 작업을 수행합니다. 레이어 순서를 조정하고, 레이어 크기와 위치를 변경하고, 레이어를 회전하고, 레이어의 배경색, 전경색, 불투명도 및 혼합 모드를 결정할 수 있습니다.

캔버스 크기를 변경하고, 배경색을 선택하고, 불투명도 설정을 변경할 수도 있습니다.

### 레이어 순서 바꾸기 {#reordering-layers}

특히 투명도나 중복 인쇄가 포함된 경우 레이어 순서를 변경하면 모양새에 영향을 줄 수 있습니다. 변경 사항을 커밋하기 전에 결과를 미리 봐야 합니다.

1. 템플릿의 레이어 순서를 조정하려면 다음 기술 중 하나를 사용합니다.

   * [레이어] 목록에서 레이어를 선택합니다. 그런 다음 **[!UICONTROL 위로]** 또는 **[!UICONTROL 아래로]**&#x200B;을(를) 필요한 횟수만큼 선택하여 목록에서 올바른 위치에 배치합니다.
   * [레이어] 목록에서 레이어를 위나 아래로 드래그합니다.

### 레이어 및 캔버스의 크기 및 위치 변경 {#changing-the-size-and-position-of-layers-and-the-canvas}

레이어는 캔버스에 들어갈 만큼 작아야 합니다. 수동으로 또는 크기 측정값을 입력하여 레이어나 캔버스 크기를 변경할 수 있습니다. 수동으로 또는 오프셋 측정값을 입력하여 레이어 위치를 변경할 수 있습니다. 레이어를 회전할 수도 있습니다.

>[!NOTE]
>
>Adobe Dynamic Media Classic에서는 템플릿과 정확한 크기의 이미지 사전 설정을 만들 것을 권장합니다. 이미지 사전 설정 크기를 템플릿 크기와 일치시키면 템플릿의 최종 출력 크기와 선명하게 하기 선택 사항이 올바르게 설정됩니다. 이 이미지 사전 설정을 만든 후 [템플릿 미리 보기] 화면의 [사전 설정 적용] 메뉴에서 선택할 수 있습니다. 서버에서 이미지가 제공될 때의 이미지 모양이 화면에 표시됩니다. [이미지 사전 설정 설정](setting-image-presets.md#setting_up_image_presets)을 참조하십시오.

* **레이어 크기 변경**: 레이어 또는 캔버스의 크기를 변경하려면 [레이어] 목록에서 레이어 또는 캔버스를 선택하고 다음 방법 중 하나를 사용하십시오.

* **수동으로 크기 변경**: 레이어 또는 캔버스의 모서리를 선택하여 드래그합니다. 텍스트 레이어의 경우 레이어 측면을 끌 수도 있습니다. Shift 키를 누른 채 드래그하여 크기를 변경하고 종횡비(모양)를 유지합니다.

* **레이어 크기 측정 입력**: [레이어 속성] 영역의 [W(폭)] 및 [H(높이)] 텍스트 상자에 픽셀 측정을 입력합니다.

레이어 크기를 변경하는 것은 물론 레이어를 패딩할 수 있습니다. 이렇게 하려면 [레이어 속성] 영역의 [왼쪽], [오른쪽], [위쪽] 및 [아래쪽] 상자에 패딩 측정값을 입력합니다. 패딩은 현재 레이어에 여백을 추가하여 기본 레이어의 경계에서 오프셋합니다. 패딩은 그림자 적용 또는 외부 후광 효과를 추가하고 이 효과를 더 강조하려는 경우에 유용합니다. 패딩을 사용하면 레이어 크기가 늘어나고 배경색이 확장된 패딩 영역에 표시됩니다. 새 레이어 크기를 기준으로 기본 레이어의 위치가 조정됩니다. 예를 들어 현재 레이어가 기본 레이어 가운데에 있는 경우 레이어 왼쪽을 확장하면 기본 레이어 오른쪽으로 이동합니다.

* **레이어 위치 변경**: 캔버스에서 레이어의 위치를 변경하려면 [레이어] 목록에서 해당 이름을 선택하고 다음 방법 중 하나를 사용하십시오.

* **위치를 수동으로 변경**: 포인터를 레이어 경계 근처로 이동하되 위로 이동하지 않고, 화살표가 4개인 화살표 커서가 표시되면 선택한 후 드래그를 시작합니다.

* **위치 오프셋 측정 입력**: X 및 Y 텍스트 상자에 X 및 Y 오프셋 측정을 입력합니다. 이러한 측정값은 앵커 지점의 x, y 오프셋을 픽셀 단위로 나타냅니다.

* **레이어 회전**: 회전 상자에 레이어가 회전된 각도가 나열됩니다. 레이어를 회전하려면 [레이어] 목록에서 레이어 이름을 선택하고 다음 기술 중 하나를 사용합니다.

* **수동으로 회전**: 커서를 레이어의 모퉁이 근처로 이동하지 않습니다. 회전 커서가 표시되면 레이어 모서리를 드래그합니다. Shift 키를 누른 상태로 끌어 15도 증분으로 회전합니다.

* **도 측정 입력**: 레이어를 회전할 도 수를 입력합니다. 회전은 시계 방향으로 수행됩니다. 시계 반대 방향으로 회전하려면 음수를 입력합니다.

**레이어 또는 레이어 효과 숨기기:**

레이어 이름 또는 효과 이름 옆에 있는 눈 모양 아이콘을 선택하여 레이어 또는 레이어 효과를 숨길 수 있습니다. 숨겨진 레이어는 미리 보기나 출력에 표시되지 않습니다. 레이어 정보는 URL에서 삭제되지 않습니다. 대신 `hide=1`이(가) URL에 추가되어 레이어가 보기에서 숨겨집니다. 예:

`layer=5&src=is{PortalCo/title}&pos=274,192&effect=-1&.effect=Drop Shadow&blendmode`

`layer=5&src=is{PortalCo/title}&pos=274,192&hide=1&effect=-1&.effect=Drop Shadow&blendmode`

### 배경색, 불투명도 및 혼합 모드 결정

레이어나 캔버스의 배경색, 불투명도 및 혼합 모드를 선택하려면 레이어나 캔버스를 선택하고 다음 기술을 사용합니다.

* **전경색**: **[!UICONTROL 전경색]**&#x200B;을 선택하고 색상 견본을 선택하여 그림자 또는 광선 색상을 변경합니다. 상자에 색상-값 매개 변수를 입력할 수도 있습니다. 배경색은 투명도를 사용하는 레이어에만 적용됩니다. 예를 들어 가격 태그의 부분적으로 투명한 레이어나 텍스트 필드의 배경에 적용됩니다. 투명도가 켜진 Psd, TIFF 또는 PNG 이미지로 구성된 레이어는 투명 배경을 사용할 수 있습니다.

* **배경색**: **[!UICONTROL 배경색]**&#x200B;을 선택하고 색상 견본을 선택하여 패딩한 영역의 색상을 변경합니다.

* **불투명도**: [불투명도] 슬라이더를 드래그하여 모든 레이어를 반투명하게 만들어 기본 이미지의 일부가 표시되도록 합니다. 100% 설정은 불투명하며 0은 투명합니다.

* **혼합 모드**: Photoshop에서 사용할 수 있는 혼합 모드 중 하나를 시뮬레이션하려면 옵션을 선택하십시오. 선택 사항은 [보통], [디졸브], [밝게], [어둡게], [곱하기] 및 [화면]입니다. 이러한 선택 사항은 캔버스가 아니라 레이어에 사용할 수 있습니다.

## 레이어에 그림자 및 광선 효과 사용 {#using-shadow-and-glow-effects-on-layers}

레이어에 그림자나 후광을 적용할 수 있습니다. 그림자 또는 광선은 레이어 둘레에 적용되며 선택한 그림자 또는 광선 옵션에 따라 안쪽 또는 바깥쪽으로 확장됩니다. 템플릿이 그림자 및 광선 효과가 있는 PSD 파일에서 시작된 경우 Adobe Dynamic Media Classic에서 이러한 효과를 조정할 수 있습니다.

그림자 또는 후광 효과를 적용한 후 [템플릿] 화면의 [레이어 속성] 영역에서 크기, 색상, 불투명도 및 위치를 조정할 수 있습니다.

### 레이어에 그림자 또는 광선 효과 적용 {#applying-a-shadow-or-glow-effect-to-a-layer}

1. [레이어] 목록에서 레이어를 선택합니다.
1. **[!UICONTROL `Add Effect`]** 메뉴를 선택하고 옵션을 선택하십시오.

   * **[!UICONTROL 그림자]**: 레이어의 아래쪽과 오른쪽에 그림자를 적용합니다.

   * **[!UICONTROL 내부 그림자]**: 레이어의 모든 가장자리 안에 그림자 효과를 적용합니다.

   * **[!UICONTROL 외부 광선]**: 레이어의 모든 가장자리에 광선 효과를 적용합니다.

   * **[!UICONTROL 내부 광선]**: 레이어의 모든 가장자리 안에 광선 효과를 적용합니다.

효과를 적용하면 효과 이름이 [레이어] 목록에 표시됩니다. 효과를 삭제하려면 [레이어] 목록에서 해당 이름을 선택한 다음 **[!UICONTROL 삭제]**&#x200B;를 선택합니다.

>[!NOTE]
>
>기본 레이어가 표시될 만큼 충분히 크지 않으면 그림자 또는 외부 광선의 효과를 볼 수 없는 경우가 있습니다. 그림자나 광선이 표시되지 않으면 레이어에 패딩 값을 추가하거나 레이어를 재정렬하는 것이 좋습니다. [레이어 및 캔버스의 크기 및 위치 변경](creating-template.md#changing_the_size_and_position_of_layers_and_the_canvas) 및 [레이어 순서 변경](creating-template.md#reordering_layers)을 참조하십시오.

### 그림자 또는 광선 효과 조정 {#adjusting-a-shadow-or-glow-effect}

그림자 또는 후광 효과를 조정하려면 먼저 [레이어] 목록에서 해당 이름을 선택합니다. [템플릿] 화면의 [레이어 속성] 영역에서 설정을 변경합니다.

* **[!UICONTROL 색상]**: [색상] 단추를 선택하고 색상 견본을 선택하여 그림자 또는 광선의 색상을 변경합니다. 상자에 색상-값 매개 변수를 입력할 수도 있습니다.

* **[!UICONTROL 불투명도]**: 슬라이더를 드래그하여 효과의 강도를 결정합니다. 덜 불투명한 효과는 더 투명합니다.

* **[!UICONTROL 혼합 모드]**: Photoshop에서 사용할 수 있는 혼합 모드 중 하나를 시뮬레이션하려면 옵션을 선택하십시오. 선택 사항은 [보통], [디졸브], [밝게], [어둡게], [곱하기] 및 [화면]입니다.

* **[!UICONTROL 크기]**: 그림자 효과를 확대하거나 축소하려면 X 및 Y 상자에 측정값을 입력하십시오. 크기 선택 사항은 내부 그림자와 외부 그림자에만 사용할 수 있습니다.

* **[!UICONTROL 증가]**: 슬라이더를 드래그하여 안쪽 또는 바깥쪽으로 효과를 확장합니다.

* **[!UICONTROL 흐림 효과]**: 슬라이더를 드래그하여 효과 가장자리의 페더링을 제어합니다. 더 흐린 효과가 더 패더링됩니다.

## 마스크 레이어 {#masking-layers}

[레이어] 목록은 레이어의 마스크 또는 알파 채널을 사용하는 방법을 지정하는 [마스크] 단추를 제공합니다. [마스크] 단추를 사용하여 특정 레이어나 템플릿의 전체 상위 레이어에 배경 레이어 효과를 적용할 수 있습니다. [레이어] 목록에서 레이어를 선택하고 **[!UICONTROL 마스크]**&#x200B;를 선택하여 다음 상태를 순환합니다.

* 레이어 배경이 불투명합니다.
* 레이어 컨텐츠가 반전되고 레이어 배경에 검정색이 채워집니다.
* 레이어 배경에 검정색이 채워집니다.
