---
title: '빠른 시작: 회전 집합'
description: Adobe Dynamic Media Classic에서 빠르게 시작하고 실행하는 데 도움이 되는 소개 및 빠른 스핀 세트 시작입니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 26e3cd5b-f070-4b92-af36-25631723460e
topic: Content Management
level: Beginner
autotag-review: '2026-05-13T20:10:31.990Z'
TQID: 'https://experienceleague.adobe.com/dYjjsyvPAPOS5icw4Yi6Kpo93Nh2qvnCiW5-ih2hmDk'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
source-git-commit: 1c15d2395e62ce41a298d25b973920963eef3a7a
workflow-type: tm+mt
source-wordcount: 820
ht-degree: 11%

---

# 빠른 시작: 회전 집합{#quick-start-spin-sets}

스핀 세트는 개체에 대한 360도 뷰를 제공합니다. 스핀 세트 를 사용하면 모든 각도에서 항목을 볼 수 있으므로 모든 관점에서 시각적 세부 정보를 얻을 수 있습니다. 회전 집합은 360도 보기 환경을 시뮬레이션합니다. Adobe Dynamic Media Classic에서는 뷰어가 항목을 회전할 수 있는 1차원 스핀 세트와 뷰어가 항목을 회전하고 전환할 수 있는 2차원 스핀 세트를 제공합니다. 또한 사용자는 모든 보기를 확대/축소하고 패닝할 수 있습니다. 사용자는 특정 관점에서 항목을 보다 면밀하게 검토할 수 있습니다.

회전 집합에 대한 ![이미지](/help/using/assets/spin_set.png)

회전 집합도 이미지 맵을 허용합니다. 이미지 맵은 회전 집합 내의 이미지에서 텍스트가 있는 롤오버 패널을 표시하는 영역입니다. 사용자가 이미지 맵을 선택하면 작업이 트리거됩니다. 예를 들어 사용자가 제품에 대한 자세한 정보를 확인할 수 있도록 웹 페이지가 시작됩니다. 회전 집합에서 이미지 맵을 표시하기 위해 사용자가 이미지 맵 위로 포인터를 이동하면 이미지 맵 자체 주위에 윤곽선이 나타납니다.

[이미지 맵 만들기](creating-image-maps.md)를 참조하십시오.

[이미지 및 회전 집합: Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/556_Image%20&%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS) 교육 비디오를 참조하십시오.

회전 집합을 만들 때 Adobe에서는 다음 지침을 권장하며 다음 제한을 적용합니다.

| 회전 집합 제한 유형 | 우수 사례 | 제한 적용됨 |
| --- | --- | --- |
| 2D 세트당 최대 행/열 수 | 세트당 12~18개 이미지 | 1000 |

[Dynamic Media 제한 사항](/help/using/limitations.md)도 참조하세요.

이 안내서는 Adobe Dynamic Media Classic에서 회전 집합 기술을 빠르게 사용할 수 있도록 설계되었습니다. 1-7 단계를 수행하십시오. 각 단계가 끝날 때 항목 링크를 선택하여 자세히 알아볼 수 있습니다.

## &#x200B;1. 이미지 만들기 및 업로드

최소한 1차원 스핀 세트의 경우 8-12개의 샷이 필요하고 2차원 스핀 세트의 경우 16-24개의 샷이 필요합니다. 촬영은 항목이 회전하고 플립되는 것을 보이기 위해 일정한 간격으로 촬영해야 합니다. 예를 들어 1차원 스핀 세트에 12개의 샷이 포함되어 있으면 각 샷에 대해 항목을 30°(360/12)로 회전합니다.

전역 탐색 모음에서 **[!UICONTROL 업로드]**&#x200B;를 선택하여 컴퓨터 또는 네트워크의 회전 이미지를 Adobe Dynamic Media Classic에 업로드합니다.

[회전 집합 이미지 촬영에 대한 지침](creating-spin-set.md#guidelines-for-shooting-spin-set-images)을 참조하십시오.

## &#x200B;2. 회전 집합 만들기

회전 집합을 만들려면 전역 탐색 모음에서 **[!UICONTROL 빌드]** > **[!UICONTROL 회전 집합]**(으)로 이동하십시오. 회전 집합 크기 대화 상자에서 원하는 행과 셀의 수를 선택하고 **[!UICONTROL 확인]**&#x200B;을 선택합니다. 그런 다음 이미지를 회전 집합 페이지의 격자로 드래그합니다.

[회전 집합 만들기](creating-spin-set.md#creating-a-spin-set)를 참조하세요.

## &#x200B;3. 회전 집합 편집

회전 집합을 편집하려면 전역 탐색 모음에서 **[!UICONTROL 설정]** > **[!UICONTROL 뷰어 사전 설정]**(으)로 이동하십시오. 회전 집합을 선택한 다음 **[!UICONTROL 편집]**&#x200B;을 선택합니다. 이미지를 추가 및 제거하고 위치를 변경합니다. 2차원 스핀 세트에서 행의 위치를 변경할 수 있습니다.

[회전 집합 편집](creating-spin-set.md#editing-a-spin-set)을 참조하세요.

## &#x200B;4. 스핀 세트 뷰어 사전 설정 설정 설정

관리자는 회전 집합 뷰어 사전 설정을 만들 수 있습니다. 이러한 사전 설정은 회전 집합 뷰어의 모양을 결정합니다. 새 회전 집합 뷰어 사전 설정을 설정하려면 전역 탐색 모음에서 **[!UICONTROL 설정]** > **[!UICONTROL 뷰어 사전 설정]**(으)로 이동하십시오.

뷰어 사전 설정 페이지에서 **[!UICONTROL 추가]**&#x200B;를 클릭한 다음 드롭다운 목록에서 **[!UICONTROL 회전 집합 뷰어]**&#x200B;를 선택한 다음 **[!UICONTROL 추가]**&#x200B;를 선택합니다. `Configure Viewer` 페이지에서 옵션을 선택한 다음 **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

[회전 집합 뷰어 사전 설정 설정](setting-spin-set-viewer-presets.md#setting-up-spin-set-viewer-presets)을 참조하십시오.

## &#x200B;5. 회전 집합 미리 보기

[찾아보기] 패널에서 회전 집합을 선택한 다음 **[!UICONTROL 미리 보기]**&#x200B;를 클릭합니다. 미리보기 페이지에서 버튼을 누른 채 포인터를 왼쪽이나 오른쪽으로 드래그하여 항목을 시각적으로 회전합니다.

[회전 집합 미리 보기](previewing-spin-set.md#previewing-a-spin-set)를 참조하십시오.

## &#x200B;6. 회전 집합 게시

회전 집합을 게시하면 해당 회전 집합이 웹 사이트 또는 애플리케이션에 동적으로 전달될 수 있도록 Adobe Dynamic Media Classic 서버에 배치됩니다. 또한 Dynamic Media 이미지 서버에서 웹 사이트 또는 애플리케이션으로 스핀 세트를 호출하는 URL 문자열을 활성화합니다.

회전 집합을 게시하려면 [찾아보기] 패널에서 해당 이름 옆에 있는 **[!UICONTROL 게시용으로 표시]** 아이콘을 선택하여 게시용으로 표시합니다. 전역 탐색 모음에서 **[!UICONTROL 게시]**&#x200B;를 클릭하여 게시를 시작합니다. 게시 페이지에서 **[!UICONTROL 게시 제출]**&#x200B;을 클릭합니다.

[회전 집합 게시](publishing-spin-set.md#publishing-a-spin-set)를 참조하십시오.

## &#x200B;7. 웹 페이지에 회전 집합 연결

Adobe Dynamic Media Classic은 회전 집합에 대한 URL 콜아웃 문자열을 만들고 게시한 후 활성화합니다. 미리보기 페이지에서 이러한 URL을 복사할 수 있습니다.

회전 집합을 선택한 다음 **[!UICONTROL 미리 보기]**&#x200B;를 클릭합니다. 회전 집합 뷰어 사전 설정을 선택합니다. **[!UICONTROL URL 복사]**&#x200B;를 클릭합니다.

[회전 집합을 웹 페이지에 연결](linking-spin-set-web-page.md#linking-a-spin-set-to-a-web-page)을 참조하세요.
