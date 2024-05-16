---
title: "빠른 시작: 이미지 크기 조정"
description: Adobe Dynamic Media Classic의 이미지 크기 조정 기술을 빠르게 시작하고 실행하는 데 도움이 되는 이미지 크기 조정에 대한 소개 및 빠른 시작입니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic,Asset Management
role: User
topic: Content Management
level: Beginner
exl-id: f1d46f03-57a1-43d8-a0ee-74b92b590736
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 6%

---

# 빠른 시작: 이미지 크기 조정{#quick-start-image-sizing}

이미지 크기 조정은 Adobe Dynamic Media Classic이 하나의 고해상도 이미지를 기반으로 여러 미분 이미지를 만드는 기능을 의미합니다. 웹 사이트나 애플리케이션에 대해 축소판 및 확대 보기 이미지와 같은 여러 이미지를 수동으로 만드는 대신 하나의 1차 이미지를 제공합니다. Adobe Dynamic Media Classic은 사용자가 요청한 대로 수정된 모든 이미지를 생성합니다. 하나의 운영 이미지에서 이미지를 동적으로 전달할 수 있다는 것은 다음과 같은 많은 이점을 제공합니다.

* 이미지의 여러 사본을 다양한 크기로 수동으로 만들 필요는 없습니다. Adobe Dynamic Media Classic에 1차 이미지를 제공하면 Adobe Dynamic Media Classic은 1차 이미지에서 서로 다른 크기의 파생물을 생성합니다.
* 웹 사이트 또는 애플리케이션 전체에서 이미지 유형의 크기를 빠르게 변경할 수 있습니다. 예를 들어 모든 썸네일 이미지를 변경하려면 &quot;썸네일&quot; 이미지 사전 설정을 수정할 수 있습니다. 이미지 사전 설정 - 매크로와 유사 - 크기 및 서식 특성 모음입니다. &quot;썸네일&quot; 이미지 사전 설정을 수정하여 웹 사이트 또는 애플리케이션 전체에서 모든 썸네일 이미지의 크기를 변경할 수 있습니다.
* 내부 또는 외부에서 컨텐츠 또는 자산 관리 시스템의 기본 파일과 다양한 파생물을 관리할 필요가 없습니다.

![동일한 고해상도 주 파일과는 다른 크기로 여러 개의 파생 이미지를 만들 수 있습니다.](/help/using/assets/is_derivative_sizes_popup.png)

다음을 참조하십시오 [이미지 크기 조정: Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/557_Image%20Sizing_converted%20renamed_Dynamic%20Imaging-AVS) 교육 비디오입니다.

다음 이미지 크기 조정 빠른 시작은 Adobe Dynamic Media Classic의 이미지 크기 조정 기술을 빠르게 시작하고 실행하는 데 도움이 되도록 설계되었습니다. 1~5단계를 수행합니다. 각 단계 후에는 필요한 경우 더 많은 정보를 찾을 수 있는 상호 참조가 있습니다.

## 1. 1차 이미지 업로드

Adobe Dynamic Media Classic에 1차 이미지를 업로드하는 것부터 시작하십시오. Adobe Dynamic Media Classic에서는 크기를 조정할 때 웹 사이트 또는 애플리케이션에서 사용할 것으로 예상하는 가장 큰 크기의 이미지를 사용하는 것이 좋습니다. 예를 들어 뷰어에서 이미지를 확대/축소하려면 가장 큰 크기가 2000픽셀 이상인 이미지를 업로드하십시오. Adobe Dynamic Media Classic은 다양한 이미지 파일 형식을 지원하지만 무손실 TIFF 및 PNG 이미지를 사용하는 것이 좋습니다.

전역 탐색 모음에서 를 선택합니다. **[!UICONTROL 업로드]** 컴퓨터에서 Adobe Dynamic Media Classic의 폴더로 파일을 업로드합니다. 다음을 참조하십시오 [1차 이미지 업로드](uploading-master-images.md#uploading_master_images).

## 2. 이미지 사전 설정 설정

매크로와 마찬가지로 이미지 사전 설정은 특정 이름으로 저장된 사전 정의된 크기 및 형식 지정 명령 모음입니다. 이미지 사전 설정은 Dynamic Media 이미지 서버에서 이미지가 전달되는 크기 및 형식을 제어합니다. 회사 관리자 상태인 경우 이미지 사전 설정을 직접 설정할 수 있습니다. Adobe Dynamic Media Classic과 함께 이미 제공되는 기본 이미지 사전 설정을 사용하여 이미지를 동적으로 전달할 수 있습니다.

관리자 권한이 있는 경우 이미지 사전 설정을 만들려면 전역 탐색 모음에서 다음 위치로 이동하십시오. **[!UICONTROL 설정]** > **[!UICONTROL 응용 프로그램 설정]** > **[!UICONTROL 이미지 사전 설정]**. 그런 다음 을 선택합니다 **[!UICONTROL 추가]** 이미지 사전 설정을 만들거나 **[!UICONTROL 편집]** 기존 이미지 사전 설정을 변경할 수 있습니다.

사용자가 만든 이미지 사전 설정이 [미리 보기] 페이지의 [이미지 사전 설정] 메뉴에 추가됩니다. 새 이미지 사전 설정을 사용하여 웹 사이트 및 애플리케이션에서 이미지를 동적으로 표시할 수 있습니다. 다음을 참조하십시오 [이미지 사전 설정 설정](setting-image-presets.md#setting_up_image_presets).

## 3. 이미지 사전 설정 미리 보기

다음 단계에서는 관리자가 각기 다른 사전 설정 크기로 설정한 이미지 사전 설정을 미리 봅니다.

이미지 사전 설정을 탐색하려면 전역 탐색 모음에서 다음 위치로 이동하십시오. **[!UICONTROL 설정]** > **[!UICONTROL 이미지 사전 설정]**&#x200B;을 클릭한 다음 이미지 사전 설정으로 이동합니다.

여러 이미지 사전 설정으로 실험합니다. 이미지가 다양한 크기로 웹 사이트 또는 애플리케이션에 동적으로 제공될 때 표시되는 방식을 알아봅니다.

다음을 참조하십시오 [이미지 사전 설정을 기반으로 이미지 자산 미리 보기](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

## 4. 기본 이미지 게시

1차 이미지 파일을 게시하는 것은 두 가지 중요한 목적에 도움이 됩니다.

* 이미지가 웹 사이트 및 애플리케이션에 동적으로 전달될 수 있도록 기본 이미지를 Dynamic Media 이미지 서버에 게시합니다.
* 게시를 수행하면 Dynamic Media 이미지 서버에서 웹 사이트 또는 애플리케이션으로 이미지를 호출하기 위한 URL 문자열이 활성화됩니다. 게시 후 필요한 경우 웹 사이트 또는 애플리케이션에서 Adobe Dynamic Media Classic 생성 URL을 복사하여 배치할 수 있습니다.

전역 탐색 모음에서 를 선택합니다. **[!UICONTROL 게시]** 게시 작업을 시작합니다. 게시 대화 상자에서 다음을 선택합니다. **[!UICONTROL 게시 제출]**. 다음을 참조하십시오 [1차 이미지 게시](publishing-master-images.md#publishing_master_images).

## 5. 웹 애플리케이션에 URL 연결

Adobe Dynamic Media Classic은 이미지에 대한 URL 콜아웃 문자열을 생성합니다. Dynamic Media 이미지 서버에 이미지를 게시하면 URL이 활성화됩니다. 찾아보기 패널(세부 사항 보기) 또는 미리보기 화면에서 이러한 URL 문자열을 복사할 수 있습니다. URL 문자열을 복사한 후에는 웹 사이트 및 응용 프로그램에서 사용할 수 있습니다. 이미지 크기 조정 URL은 웹 페이지 코드의 정적 이미지 이름에 대한 참조를 대체합니다. 이 URL은 표시할 새 이미지마다 데이터베이스가 대체하는 기본 이미지 이름을 참조합니다.

이미지 사전 설정을 사용하여 생성된 URL 문자열에는 이미지 사전 설정 이름이 포함됩니다. 이 이름은 달러 기호(`$`). 예를 들어, `$thumbnail$` 썸네일 크기로 기본 이미지를 표시하도록 디자인된 이미지 사전 설정일 수 있습니다. 다음을 참조하십시오 [웹 애플리케이션에 URL 연결](linking-urls-web-application.md#linking_urls_to_your_web_application).
