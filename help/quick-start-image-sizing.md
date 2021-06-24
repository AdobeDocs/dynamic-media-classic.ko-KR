---
title: '"빠른 시작: 이미지 크기 조정"'
description: 이미지 크기 조정 소개 및 빠른 시작 을 사용하면 이미지 크기 조정 기술을 사용하여 신속하게 시작하고 실행할 수 있습니다.
uuid: 6c4ad4b7-549d-4daa-b6b9-5997a8427af8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: dcaa9b21-b925-4dbb-865e-7918cdbda50c
feature: Dynamic Media Classic,자산 관리
role: Business Practitioner
exl-id: f1d46f03-57a1-43d8-a0ee-74b92b590736
source-git-commit: c5c8c4f96f18339734f4441733cdb1e7f34d3071
workflow-type: tm+mt
source-wordcount: '844'
ht-degree: 37%

---

# 빠른 시작: 이미지 크기 조정{#quick-start-image-sizing}

이미지 크기 조절은 Dynamic Media Classic에서 단일 고해상도 이미지를 기반으로 여러 파생 이미지를 만들 수 있는 기능을 의미합니다. 웹 사이트나 애플리케이션에 대해 축소판이나 확대된 뷰 이미지와 같은 여러 이미지를 수동으로 생성하는 대신 단일 마스터 이미지를 제공합니다. Dynamic Media Classic은 수정된 모든 이미지를 요청하는 대로 생성합니다. 단일 마스터 이미지에서 동적으로 이미지를 제공할 수 있는 경우 다음과 같은 많은 장점이 있습니다.

* 각기 다른 크기로 여러 이미지를 수동으로 만들지 않아도 됩니다. Dynamic Media Classic에 하나의 마스터 이미지를 제공하면 Dynamic Media Classic이 마스터 이미지에서 다른 크기의 파생물을 생성합니다.
* 웹 사이트나 애플리케이션 전체에서 이미지 유형의 크기를 신속하게 변경할 수 있습니다. 예를 들어 모든 썸네일 이미지를 변경하려면 &quot;썸네일&quot; 이미지 사전 설정을 수정할 수 있습니다. 매크로와 비슷한 이미지 사전 설정은 크기 및 형식 지정 특성 모음입니다. &quot;썸네일&quot; 이미지 사전 설정을 수정하여 웹 사이트나 애플리케이션 전체에서 모든 썸네일 이미지의 크기를 변경할 수 있습니다.
* 컨텐츠 또는 자산 관리 시스템 내부 또는 외부에서 마스터와 모든 다양한 파생물을 관리할 필요가 없습니다.

![동일한 고해상도 마스터 파일과 크기가 다른 여러 파생 이미지를 만들 수 있습니다.](/help/assets/is_derivative_sizes_popup.png)

이 이미지 크기 조정 빠른 시작은 Dynamic Media Classic에서 이미지 크기 조정 기술을 사용하여 빠르게 시작하고 실행할 수 있도록 설계되었습니다. 1-5단계를 수행합니다. 각 단계 뒤에는 필요한 경우 자세한 정보를 확인할 수 있는 상호 참조가 있습니다.

## 1. 마스터 이미지 업로드

먼저 Dynamic Media Classic에 마스터 이미지를 업로드합니다. 크기는 웹 사이트 또는 애플리케이션에서 사용할 것으로 예상되는 가장 큰 크기를 사용하는 것이 좋습니다. 예를 들어 뷰어에서 이미지를 확대/축소하려면 가장 큰 크기의 2,000픽셀 이상의 이미지를 업로드합니다. Dynamic Media Classic에서는 많은 이미지 파일 형식을 지원하지만, 무손실 TIFF 및 PNG 이미지가 권장됩니다.

전역 탐색 모음에서 **[!UICONTROL 업로드]**&#x200B;를 클릭하여 컴퓨터의 파일을 Dynamic Media Classic의 폴더로 업로드합니다. [마스터 이미지 업로드](uploading-master-images.md#uploading_master_images)를 참조하십시오.

## 2. 이미지 사전 설정 설정

매크로와 마찬가지로 이미지 사전 설정은 특정 이름으로 저장된 사전 정의된 크기 및 형식 지정 명령 모음입니다. 이미지 사전 설정은 Dynamic Media 이미지 서버에서 전달되는 이미지의 크기 및 형식을 제어합니다. 회사 관리자 상태인 경우 고유한 이미지 사전 설정을 지정할 수 있습니다. Dynamic Media Classic에도 기본 이미지 사전 설정이 포함되어 있으며 이 사전 설정을 사용하여 이미지를 동적으로 전달할 수 있습니다.

이미지 사전 설정을 만들려면(관리자의 경우) 전역 탐색 모음에서 **[!UICONTROL 설정]** > **[!UICONTROL 애플리케이션 설정]** > **[!UICONTROL 이미지 사전 설정]**&#x200B;을 클릭합니다. 그런 다음 **[!UICONTROL 추가]**&#x200B;를 클릭하여 이미지 사전 설정을 만들거나 **[!UICONTROL 편집]**&#x200B;을 클릭하여 기존 이미지 사전 설정을 변경합니다.

만드는 이미지 사전 설정이 미리 보기 페이지의 이미지 사전 설정 메뉴에 추가됩니다. 새 이미지 사전 설정을 사용하여 웹 사이트와 애플리케이션에 이미지를 동적으로 표시할 수 있습니다. [이미지 사전 설정 지정](setting-image-presets.md#setting_up_image_presets)을 참조하십시오.

## 3. 이미지 사전 설정 미리 보기

다음 단계에서는 관리자가 각기 다른 사전 설정 크기로 설정한 이미지 사전 설정을 미리 봅니다.

이미지 사전 설정을 탐색하려면 전역 탐색 막대에서 **[!UICONTROL 설정]** > **[!UICONTROL 이미지 사전 설정]**&#x200B;을 클릭한 다음 이미지 사전 설정으로 이동합니다.

여러 이미지 사전 설정으로 실험합니다. 이미지가 다양한 크기로 웹 사이트나 애플리케이션에 동적으로 전달될 때 어떻게 나타나는지 확인하십시오.

[이미지 사전 설정을 기준으로 이미지 자산 미리 보기](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)를 참조하십시오.

## 4. 마스터 이미지 게시

마스터 이미지 파일을 게시하는 두 가지 필수 목적은 다음과 같습니다.

* 이미지를 웹 사이트 및 애플리케이션에 동적으로 전달할 수 있도록 마스터 이미지를 Dynamic Media 이미지 서버에 게시합니다.
* 게시를 사용하면 Dynamic Media 이미지 서버에서 웹 사이트 또는 응용 프로그램으로 이미지를 호출하기 위한 URL 문자열이 활성화됩니다. 게시 후 웹 사이트 또는 애플리케이션에서 필요한 경우 Dynamic Media Classic에서 생성한 URL을 복사하여 배치할 수 있습니다.

전역 탐색 막대에서 **[!UICONTROL 게시]**&#x200B;를 클릭하여 게시 작업을 시작합니다. 게시 대화 상자에서 **[!UICONTROL 게시 제출]**&#x200B;을 클릭합니다. [마스터 이미지 게시](publishing-master-images.md#publishing_master_images)를 참조하십시오.

## 5. URL을 웹 애플리케이션에 연결

Dynamic Media Classic은 이미지에 대한 URL 콜아웃 문자열을 만듭니다. Dynamic Media 이미지 서버에 이미지를 게시하면 URL이 활성화됩니다. 찾아보기 패널([세부 사항 보기])이나 [미리 보기] 화면에서 이러한 URL 문자열을 복사할 수 있습니다. URL 문자열을 복사한 후 웹 사이트와 애플리케이션에서 사용할 수 있습니다. 이미지 크기 조정 URL이 웹 페이지 코드의 정적 이미지 이름 참조를 바꿉니다. URL은 표시할 각 새 이미지에 대해 데이터베이스에서 바뀌는 마스터 이미지 이름을 참조합니다.

이미지 사전 설정을 사용하여 생성된 URL 문자열에는 이미지 사전 설정 이름이 포함됩니다. 이 이름은 달러 기호(`$`)로 묶여 있습니다. 예를 들어 `$thumbnail$`은 축소판 크기로 마스터 이미지를 표시하도록 디자인된 이미지 사전 설정일 수 있습니다. [URL을 웹 애플리케이션에 연결](linking-urls-web-application.md#linking_urls_to_your_web_application)을 참조하십시오.
