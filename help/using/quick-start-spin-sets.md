---
title: "빠른 시작: 회전 집합"
description: Adobe Dynamic Media Classic에서 빠르게 시작하고 실행하는 데 도움이 되는 소개 및 빠른 스핀 세트 시작입니다.
uuid: d0af9db6-cb6f-48f0-89f6-f3ab2da0659f
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 282b8e83-b20f-43f7-b9f8-6eebd5b1c5a7
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 26e3cd5b-f070-4b92-af36-25631723460e
source-git-commit: 38d7f8d6e5888e1c5ba9260ada45b79fb16b338f
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 22%

---

# 빠른 시작: 회전 집합{#quick-start-spin-sets}

회전 집합은 개체를 회전하는 실제 동작을 시뮬레이션하여 검사합니다. 회전 집합을 사용하면 임의 각도에서 항목을 보고 모든 각도에서 주요 시각적 세부 사항을 얻을 수 있습니다. 회전 세트는 360도 보기 환경을 시뮬레이션합니다. Adobe Dynamic Media Classic에서는 뷰어가 항목을 회전할 수 있는 1차원 스핀 세트와 뷰어가 항목을 회전하고 전환할 수 있는 2차원 스핀 세트를 제공합니다. 또한 사용자는 몇 번의 간단한 마우스 클릭만으로 &quot;자유 형식의&quot; 확대/축소를 수행하고 모든 보기를 이동할 수 있습니다. 이렇게 하면 사용자가 특정 뷰포인트에서 더 자세히 항목을 검사할 수 있습니다.

![회전 집합의 이미지](/help/using/assets/spin_set.png)

회전 집합도 이미지 맵을 허용합니다. 이미지 맵은 회전 집합 내 이미지의 영역으로, 텍스트가 있는 롤오버 패널을 표시합니다. 사용자가 이미지 맵을 클릭하면 일종의 작업이 트리거됩니다. 예를 들어 사용자가 제품에 대한 자세한 정보를 확인할 수 있도록 웹 페이지가 시작됩니다. 회전 집합에서 이미지 맵을 가리키기 위해 사용자가 마우스 포인터를 회전 집합 위로 이동하면 윤곽선이 이미지 맵 자체 주위에 나타납니다.

다음을 참조하십시오 [이미지 맵 만들기](creating-image-maps.md).

다음을 참조하십시오 [이미지 및 스핀 세트: Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS) 교육 비디오입니다.

회전 집합을 만들 때 Adobe은 다음 모범 사례를 권장하며 다음 제한을 적용합니다.

| 회전 집합 제한 유형 | 우수 사례 | 제한 적용됨 |
| --- | --- | --- |
| 2D 세트당 최대 행/열 수 | 세트당 12~18개 이미지 | 1000 |

참조: [Dynamic Media 제한 사항](/help/using/limitations.md).

이 Spin Sets Quick Start는 Adobe Dynamic Media Classic의 Spin Set 기술을 통해 빠르게 시작하고 실행할 수 있도록 설계되었습니다. 1-7 단계를 수행하십시오. 각 단계가 끝날 때 항목 링크를 선택하여 자세히 알아볼 수 있습니다.

## 1. 이미지 만들기 및 업로드

최소한 1차원 스핀 세트의 경우 8-12개의 샷이 필요하고 2차원 스핀 세트의 경우 16-24개의 샷이 필요합니다. 항목을 회전하고 뒤집는 듯한 인상을 주려면 일정한 간격으로 촬영해야 합니다. 예를 들어 1차원 스핀 세트에 12개의 샷이 포함되어 있는 경우 각 샷에 대해 항목을 30°(360°/12)로 회전합니다.

전역 탐색 모음에서 를 선택합니다. **[!UICONTROL 업로드]** 컴퓨터 또는 네트워크에서 Adobe Dynamic Media Classic으로 회전 이미지를 업로드합니다.

[회전 집합 이미지 촬영에 대한 지침](creating-spin-set.md#guidelines-for-shooting-spin-set-images)을 참조하십시오.

## 2. 회전 집합 만들기

회전 집합을 만들려면 전역 탐색 막대에서 **[!UICONTROL 빌드]** > **[!UICONTROL 스핀 세트]**. [회전 집합 크기] 대화 상자에서 원하는 행과 셀의 수를 선택하고 **[!UICONTROL 확인]**. 그런 다음 이미지를 회전 집합 페이지의 격자로 드래그합니다.

다음을 참조하십시오 [회전 집합 만들기](creating-spin-set.md#creating-a-spin-set).

## 3. 회전 집합 편집

회전 집합을 편집하려면 전역 탐색 모음에서 다음 위치로 이동하십시오. **[!UICONTROL 설정]** > **[!UICONTROL 뷰어 사전 설정]**. 회전 세트를 선택한 다음 를 선택합니다 **[!UICONTROL 편집]**. 이미지를 추가 및 제거하고 위치를 변경합니다. 2차원 회전 집합에서 행의 위치를 변경할 수 있습니다.

다음을 참조하십시오 [회전 집합 편집](creating-spin-set.md#editing-a-spin-set).

## 4. 스핀 세트 뷰어 사전 설정 설정

관리자는 회전 집합 뷰어 사전 설정을 만들 수 있습니다. 이러한 사전 설정은 회전 집합 뷰어의 모양을 결정합니다. 새 회전 집합 뷰어 사전 설정을 설정하려면 전역 탐색 모음에서 다음 위치로 이동하십시오. **[!UICONTROL 설정]** > **[!UICONTROL 뷰어 사전 설정]**.

뷰어 사전 설정 페이지에서 을 선택합니다. **[!UICONTROL 추가]**&#x200B;을 선택한 다음 을 선택합니다. **[!UICONTROL 회전 집합 뷰어]** 드롭다운 목록에서 을(를) 선택한 다음 **[!UICONTROL 추가]**. 뷰어 구성 페이지에서 옵션을 선택한 다음 을 선택합니다. **[!UICONTROL 저장]**.

다음을 참조하십시오 [스핀 세트 뷰어 사전 설정 설정 설정](setting-spin-set-viewer-presets.md#setting-up-spin-set-viewer-presets).

## 5. 회전 집합 미리 보기

[찾아보기] 패널에서 회전 세트를 선택한 다음 를 선택합니다 **[!UICONTROL 미리 보기]**. 미리보기 페이지에서 마우스 버튼을 누른 채 포인터를 왼쪽 또는 오른쪽으로 드래그하여 항목을 시각적으로 &quot;회전&quot;합니다.

다음을 참조하십시오 [회전 집합 미리 보기](previewing-spin-set.md#previewing-a-spin-set).

## 6. 회전 집합 게시

회전 집합을 게시하면 해당 회전 집합이 웹 사이트 또는 애플리케이션에 동적으로 전달될 수 있도록 Adobe Dynamic Media Classic 서버에 배치됩니다. 또한 Dynamic Media 이미지 서버에서 웹 사이트 또는 애플리케이션으로 스핀 세트를 호출하는 URL 문자열을 활성화합니다.

회전 세트를 게시하려면 다음을 선택하여 게시로 표시합니다. **[!UICONTROL 게시로 표시]** [찾아보기] 패널의 이름 옆에 있는 아이콘. 전역 탐색 모음에서 를 선택합니다. **[!UICONTROL 게시]** 게시를 시작합니다. 게시 화면에서 다음을 선택합니다. **[!UICONTROL 게시 제출]**.

다음을 참조하십시오 [회전 집합 게시](publishing-spin-set.md#publishing-a-spin-set).

## 7. 스핀 세트를 웹 페이지에 연결

Adobe Dynamic Media Classic은 회전 집합에 대한 URL 콜아웃 문자열을 만들고 게시한 후 활성화합니다. 미리보기 페이지에서 이러한 URL을 복사할 수 있습니다.

회전 세트를 선택한 다음 를 선택합니다. **[!UICONTROL 미리 보기]**. 회전 집합 뷰어 사전 설정을 선택합니다. 그런 다음 을 선택합니다 **[!UICONTROL URL 복사]**.

다음을 참조하십시오 [웹 페이지에 회전 집합 연결](linking-spin-set-web-page.md#linking-a-spin-set-to-a-web-page).
