---
title: "빠른 시작: 이미지 크기 조정"
description: Adobe Dynamic Media Classic의 이미지 크기 조정 기술을 사용하여 빠르게 시작하고 실행할 수 있도록 해주는 이미지 크기 조정 소개 및 빠른 시작
uuid: 6c4ad4b7-549d-4daa-b6b9-5997a8427af8
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: dcaa9b21-b925-4dbb-865e-7918cdbda50c
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: f1d46f03-57a1-43d8-a0ee-74b92b590736
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 22%

---

# 빠른 시작: 이미지 크기 조정{#quick-start-image-sizing}

이미지 크기 조절은 Adobe Dynamic Media Classic에서 단일 고해상도 이미지를 기반으로 여러 파생 이미지를 만들 수 있는 기능을 의미합니다. 웹 사이트나 애플리케이션에 대해 축소판이나 확대된 뷰 이미지와 같은 여러 이미지를 수동으로 생성하는 대신 하나의 1차 이미지를 제공합니다. Adobe Dynamic Media Classic은 사용자가 요청하는 대로 수정된 모든 이미지를 생성합니다. 단일 1차 이미지에서 동적으로 이미지를 제공할 수 있다는 것은 다음과 같은 많은 이점이 있습니다.

* 각기 다른 크기로 여러 이미지를 수동으로 만들지 않아도 됩니다. 1차 이미지 하나를 Adobe Dynamic Media Classic에 제공하면 Adobe Dynamic Media Classic에서 1차 이미지에서 서로 다른 크기의 파생물을 생성합니다.
* 웹 사이트나 애플리케이션 전체에서 이미지 유형의 크기를 신속하게 변경할 수 있습니다. 예를 들어 모든 썸네일 이미지를 변경하려면 &quot;썸네일&quot; 이미지 사전 설정을 수정할 수 있습니다. 매크로와 비슷한 이미지 사전 설정은 크기 및 형식 지정 특성 모음입니다. &quot;썸네일&quot; 이미지 사전 설정을 수정하여 웹 사이트나 애플리케이션 전체에서 모든 썸네일 이미지의 크기를 변경할 수 있습니다.
* 컨텐츠 또는 자산 관리 시스템의 내부 또는 외부에서 기본 파일 및 모든 다양한 파생물을 관리할 필요가 없습니다.

![동일한 고해상도 기본 파일과 다른 크기의 여러 파생 이미지를 만들 수 있습니다.](/help/assets/is_derivative_sizes_popup.png)

자세한 내용은 [이미지 크기 조정: Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/557_Image%20Sizing_converted%20renamed_Dynamic%20Imaging-AVS) 교육 비디오.

다음 이미지 크기 조정 빠른 시작 은 Adobe Dynamic Media Classic에서 이미지 크기 조정 기술을 사용하여 빠르게 시작하고 실행할 수 있도록 설계되었습니다. 1-5단계를 수행합니다. 각 단계 후에 필요한 경우 추가 정보를 찾을 수 있는 상호 참조가 있습니다.

## 1. 기본 이미지 업로드

먼저 기본 이미지를 Adobe Dynamic Media Classic에 업로드합니다. 크기는 웹 사이트 또는 애플리케이션에서 사용할 것으로 예상되는 가장 큰 크기를 사용하는 것이 좋습니다. 예를 들어 뷰어에서 이미지를 확대/축소하려면 가장 큰 크기의 2,000픽셀 이상의 이미지를 업로드합니다. Adobe Dynamic Media Classic에서는 많은 이미지 파일 형식을 지원하지만, 무손실 TIFF 및 PNG 이미지가 좋습니다.

전역 탐색 모음에서 를 선택합니다 **[!UICONTROL 업로드]** 컴퓨터의 파일을 Adobe Dynamic Media Classic의 폴더로 업로드합니다. 자세한 내용은 [기본 이미지 업로드](uploading-master-images.md#uploading_master_images).

## 2. 이미지 사전 설정 설정

매크로와 마찬가지로 이미지 사전 설정은 특정 이름으로 저장된 사전 정의된 크기 및 형식 지정 명령 모음입니다. 이미지 사전 설정은 Dynamic Media 이미지 서버에서 전달되는 이미지의 크기 및 형식을 제어합니다. 회사 관리자 상태인 경우 고유한 이미지 사전 설정을 지정할 수 있습니다. Adobe Dynamic Media Classic에도 기본 이미지 사전 설정이 포함되어 있으며 이 사전 설정을 사용하여 이미지를 동적으로 전달할 수 있습니다.

이미지 사전 설정을 만들려면(관리자의 경우) 전역 탐색 표시줄에서 **[!UICONTROL 설정]** > **[!UICONTROL 애플리케이션 설정]** > **[!UICONTROL 이미지 사전 설정]**. 그런 다음 을(를) 선택합니다 **[!UICONTROL 추가]** 이미지 사전 설정을 만들려면 또는 **[!UICONTROL 편집]** 기존 이미지 사전 설정을 변경하려면 다음을 수행하십시오.

만드는 이미지 사전 설정이 미리 보기 페이지의 이미지 사전 설정 메뉴에 추가됩니다. 새 이미지 사전 설정을 사용하여 웹 사이트와 애플리케이션에 이미지를 동적으로 표시할 수 있습니다. 자세한 내용은 [이미지 사전 설정 설정](setting-image-presets.md#setting_up_image_presets).

## 3. 이미지 사전 설정 미리 보기

다음 단계에서는 관리자가 각기 다른 사전 설정 크기로 설정한 이미지 사전 설정을 미리 봅니다.

이미지 사전 설정을 탐색하려면 전역 탐색 막대에서 **[!UICONTROL 설정]** > **[!UICONTROL 이미지 사전 설정]**&#x200B;로 이동한 다음 이미지 사전 설정으로 이동합니다.

여러 이미지 사전 설정으로 실험합니다. 이미지가 다양한 크기로 웹 사이트나 애플리케이션에 동적으로 전달될 때 어떻게 나타나는지 확인하십시오.

자세한 내용은 [이미지 사전 설정을 기반으로 이미지 자산 미리 보기](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

## 4. 기본 이미지 게시

기본 이미지 파일을 게시하면 두 가지 중요한 목적이 있습니다.

* 웹 사이트 및 애플리케이션에 이미지를 동적으로 전달할 수 있도록 기본 이미지를 Dynamic Media 이미지 서버에 게시합니다.
* 게시를 사용하면 Dynamic Media 이미지 서버에서 웹 사이트 또는 응용 프로그램으로 이미지를 호출하기 위한 URL 문자열이 활성화됩니다. 게시 후 웹 사이트 또는 애플리케이션에서 필요한 경우 Adobe Dynamic Media Classic 생성 URL을 복사하여 배치할 수 있습니다.

전역 탐색 모음에서 를 선택합니다 **[!UICONTROL 게시]** 게시 작업을 시작하려면 다음을 수행하십시오. 게시 대화 상자에서 를 선택합니다 **[!UICONTROL 게시 제출]**. 자세한 내용은 [기본 이미지 게시](publishing-master-images.md#publishing_master_images).

## 5. 웹 애플리케이션에 URL 연결

Adobe Dynamic Media Classic은 이미지에 대한 URL 콜아웃 문자열을 생성합니다. Dynamic Media 이미지 서버에 이미지를 게시하면 URL이 활성화됩니다. [검색] 패널([세부 사항 보기])이나 [미리 보기] 화면에서 이러한 URL 문자열을 복사할 수 있습니다. URL 문자열을 복사한 후 웹 사이트와 애플리케이션에서 사용할 수 있습니다. 이미지 크기 조정 URL이 웹 페이지 코드의 정적 이미지 이름 참조를 바꿉니다. 이 URL은 표시할 각 새 이미지에 대해 데이터베이스로 대체되는 기본 이미지 이름을 참조합니다.

이미지 사전 설정을 사용하여 생성된 URL 문자열에는 이미지 사전 설정 이름이 포함됩니다. 이 이름은 달러 기호(`$`). 예, `$thumbnail$` 는 축소판 크기로 기본 이미지를 표시하도록 설계된 이미지 사전 설정일 수 있습니다. 자세한 내용은 [웹 애플리케이션에 URL 연결](linking-urls-web-application.md#linking_urls_to_your_web_application).
