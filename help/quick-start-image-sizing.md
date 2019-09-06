---
title: '"빠른 시작: 이미지 크기 조정"'
seo-title: '"빠른 시작: 이미지 크기 조정"'
description: 널
seo-description: 이미지 크기 조정 기법을 사용하여 빠르게 시작할 수 있는 이미지 크기 조정 소개 및 빠른 시작을 소개합니다.
uuid: 6 c 4 ad 4 b 7-549 d -4 daa-b 6 b 9-5997 a 8427 af 8
contentOwner: 관리
content-type: 참조
products: sg_ Experiencemanager/dynamic-media-scene -7
geptopics: sg_ scenesevenondemand_ pk/categories/image_ sizing
discoiquuid: DCAA 9 B 21-B 925-4 DBB -865 E -7918 CDBDA 50 C
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# 빠른 시작: 이미지 크기 조정{#quick-start-image-sizing}

이미지 크기 조정은 하나의 고해상도 이미지를 기반으로 한 여러 파생 이미지를 만들 수 있는 Dynamic Media Classic의 기능을 말합니다. 웹 사이트나 애플리케이션에 대해 썸네일 및 확대 보기 이미지 등 여러 이미지를 수동으로 만드는 대신 단일 마스터 이미지를 제공합니다. Dynamic Media Classic는 요청한 모든 이미지를 동시에 생성합니다. 단일 마스터 이미지에서 동적으로 이미지를 제공할 수 있는 경우 다음과 같은 많은 장점이 있습니다.

* 각기 다른 크기로 여러 이미지를 수동으로 만들지 않아도 됩니다. 하나의 마스터 이미지를 Dynamic Media Classic에 제공하면 Dynamic Media Classic에서 마스터 이미지에서 크기가 다른 파생물을 생성합니다.
* 웹 사이트나 애플리케이션 전체에서 이미지 유형의 크기를 신속하게 변경할 수 있습니다. 예를 들어 모든 썸네일 이미지를 변경하려면 "썸네일" 이미지 사전 설정을 수정할 수 있습니다. 매크로와 비슷한 이미지 사전 설정은 크기 및 형식 지정 특성 모음입니다. "썸네일" 이미지 사전 설정을 수정하여 웹 사이트나 애플리케이션 전체에서 모든 썸네일 이미지의 크기를 변경할 수 있습니다.
* 컨텐츠 또는 자산 관리 시스템 내부나 외부에서 마스터와 모든 파생 이미지를 관리하지 않아도 됩니다.

![동일한 고해상도 마스터 파일에서 크기가 다른 여러 파생 이미지를 만들 수 있습니다.](/help/assets/is_derivative_sizes_popup.png)

**빠른 시작**

이 이미지 크기 조정 빠른 시작은 Scene7 Publishing System에서 이미지 크기 조정 기술을 빨리 시작하고 실행하는 데 도움이 됩니다. 1-5 단계를 수행합니다. 각 단계 뒤에는 필요한 경우 자세한 정보를 확인할 수 있는 상호 참조가 있습니다.

**1. 마스터 이미지 업로드**

먼저 마스터 이미지를 Scene7 Publishing System에 업로드합니다. 크기와 같이, Dynamic Media Classic 에서는 웹 사이트나 애플리케이션에서 사용할 가장 큰 크기의 이미지를 사용할 것을 권장합니다. 예를 들어 뷰어가 이미지를 확대/축소하도록 하려면 가장 큰 치수에서 2000픽셀 이상인 이미지를 업로드합니다. Dynamic Media Classic는 많은 이미지 파일 형식을 지원하지만 손실 없는 TIFF 및 PNG 이미지를 권장합니다.

글로벌 탐색 막대에서 [업로드] 단추를 선택하여 컴퓨터에서 Scene7 Publishing System의 폴더로 파일을 업로드합니다. [마스터 이미지 업로드](uploading-master-images.md#uploading_master_images)를 참조하십시오.

**2. 이미지 사전 설정 지정**

매크로와 마찬가지로 이미지 사전 설정은 특정 이름으로 저장된 사전 정의된 크기 및 형식 지정 명령 모음입니다. 이미지 사전 설정은 다이내믹 미디어 이미지 서버로부터 이미지를 전달하는 크기 및 형식을 제어합니다. 회사 관리자 상태인 경우 고유한 이미지 사전 설정을 지정할 수 있습니다. Dynamic Media Classic 에는 기본 이미지 사전 설정이 포함되어 있으며 이를 사용하여 이미지를 동적으로 전달할 수 있습니다.

이미지 사전 설정을 만들려면(관리자인 경우) [설정] &gt; [애플리케이션 설정]을 선택합니다. [설정] 화면에서 [애플리케이션 설정] 선택 사항을 표시하고 [이미지 사전 설정]을 선택합니다. 그런 다음 **추가** 또는 **편집을** 클릭하여 이미지 사전 설정을 만듭니다.

만든 이미지 사전 설정이 [미리 보기] 화면의 [이미지 사전 설정] 메뉴에 추가됩니다. 새 이미지 사전 설정을 사용하여 웹 사이트와 애플리케이션에 이미지를 동적으로 표시할 수 있습니다. [이미지 사전 설정 지정](setting-image-presets.md#setting_up_image_presets)을 참조하십시오.

**3. 이미지 사전 설정 미리 보기**

다음 단계에서는 관리자가 각기 다른 사전 설정 크기로 설정한 이미지 사전 설정을 미리 봅니다.

To explore Image Presets, click **Setup** &gt; **Image Presets**, and then browse to an Image Preset.

여러 이미지 사전 설정으로 실험합니다. 각기 다른 크기로 웹 사이트나 애플리케이션에 동적으로 제공될 때의 이미지 모양을 확인합니다.

[이미지 사전 설정을 기준으로 이미지 자산 미리 보기](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)를 참조하십시오.

**4. 마스터 이미지 게시**

마스터 이미지 파일을 게시하는 두 가지 필수 목적은 다음과 같습니다.

* 다이내믹 미디어 이미지 서버에 마스터 이미지를 게시하여 이미지를 웹 사이트와 애플리케이션에 동적으로 제공할 수 있습니다.
* 게시하면 Dynamic Media 이미지 서버의 이미지를 웹 사이트나 애플리케이션으로 호출하는 URL 문자열이 활성화됩니다. 게시 후에는 웹 사이트나 애플리케이션에서 필요한 경우 Dynamic Media Classic에서 생성된 URL를 복사하고 배치할 수 있습니다.

글로벌 탐색 막대에서 [게시] 단추를 선택하여 게시를 시작합니다. [게시] 화면에서 [게시 시작] 단추를 선택합니다. [마스터 이미지 게시](publishing-master-images.md#publishing_master_images)를 참조하십시오.

**5. URL을 웹 애플리케이션에 연결**

Dynamic Media Classic에서 이미지에 대한 URL 설명선 문자열을 만듭니다. 이미지를 다이내믹 미디어 이미지 서버에 게시하면 URL 이 활성화됩니다. 찾아보기 패널([세부 사항 보기])이나 [미리 보기] 화면에서 이러한 URL 문자열을 복사할 수 있습니다. URL 문자열을 복사한 후 웹 사이트와 애플리케이션에서 사용할 수 있습니다. 이미지 크기 조정 URL이 웹 페이지 코드의 정적 이미지 이름 참조를 바꿉니다. URL은 표시할 각 새 이미지에 대해 데이터베이스에서 바뀌는 마스터 이미지 이름을 참조합니다.

이미지 사전 설정을 사용하여 생성된 URL 문자열에는 이미지 사전 설정 이름이 포함됩니다. This name is enclosed in dollar signs (`$`). For example, `$thumbnail$` can be the Image Preset designed to show master images at thumbnail size. [URL을 웹 애플리케이션에 연결](linking-urls-web-application.md#linking_urls_to_your_web_application)을 참조하십시오.