---
title: 애플리케이션 설정
description: Adobe Dynamic Media Classic의 애플리케이션 영역을 설정하고 구성하는 방법에 대해 알아봅니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin
exl-id: 3f96606e-ef5c-4c01-aa0f-3148f14e28be
topic: Administration
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '10945'
ht-degree: 30%

---

# 애플리케이션 설정{#application-setup}

[응용 프로그램 설정] 페이지에서는 일반 설정을 입력하거나, 이미지 사전 설정을 생성하거나, 비디오 인코딩 사전 설정, 뷰어 사전 설정을 생성하거나, 기본 뷰어 및 메타데이터를 정의할 수 있습니다. 2D 스핀 세트(예:), 게시 설정 및 비디오 SEO 설정 생성을 자동화하도록 일괄처리 집합 사전 설정을 설정할 수 있습니다.

>[!NOTE]
>
>Adobe Dynamic Media Classic 관리자만 애플리케이션 설정에서 설정을 변경할 수 있습니다.

## 일반 설정 {#general-settings}

응용 프로그램 일반 설정 페이지를 열려면 전역 탐색 모음에서 **[!UICONTROL 설정]** > **[!UICONTROL 응용 프로그램 설정]** > **[!UICONTROL 일반 설정]**(으)로 이동합니다.

### 서버

계정 생성 시 Adobe Dynamic Media Classic은 회사에 할당된 서버를 자동으로 제공합니다. 이러한 서버는 웹 사이트 및 응용 프로그램의 URL 문자열을 구성하는 데 사용됩니다. 이러한 URL 호출은 계정과 관련이 있습니다.

[보안 테스트 서비스 테스트](testing-assets-making-them-public.md#testing_the_secure_testing_service)도 참조하세요.

* **[!UICONTROL 게시된 서버 이름]**: 이 서버는 계정과 관련된 모든 시스템 생성 URL 호출에 사용되는 Live CDN(Content Deliver Network) 서버입니다. Adobe Dynamic Media Classic 지원 기술자가 이 서버 이름을 변경하도록 지시한 경우에만 이 서버 이름을 변경하십시오.

* **[!UICONTROL 원본 서버 이름]**: 이 서버는 품질 보증 테스트에만 사용됩니다. Adobe Dynamic Media Classic 지원 기술자가 이 서버 이름을 변경하도록 지시한 경우에만 이 서버 이름을 변경하십시오.

<!-- **AGM Server Name** This server is used for Web-to-Print templates. This server is set on a company-wide basis. Do not change this server name unless instructed to do so by an Adobe DynamicMedia Classic support technician. -->

* **[!UICONTROL Test&amp;Target 서버 이름]**: `.com`을(를) 포함하는 Test&amp;Target URL. 이 URL을 가져오는 방법에 대한 지침은 [!DNL Adobe Dynamic Media Classic]을(를) [!DNL Adobe Target Standard/Premium]과(와) 통합 을 참조하십시오.

<!-- **Test Publish Context Server Name** -->

* **[!UICONTROL iOS 스트리밍 서버 이름]**: [!DNL Adobe Dynamic Media Classic] iOS 스트리밍 서버의 URL. 이 서버는 HTTP 프로토콜을 사용하여 iOS 기반 장치에 스트리밍 비디오를 전달합니다.

* **[!UICONTROL 점진적 비디오 서버 이름]**: [!DNL Adobe Dynamic Media Classic] 점진적 비디오 서버의 URL입니다. 이 서버는 HTTP 프로토콜을 사용하여 점진적 비디오를 전달합니다.

* **[!UICONTROL 게시되지 않은 에셋의 URL 표시]**: 에셋을 미리 볼 때 게시 여부에 관계없이 [!DNL Adobe Dynamic Media Classic]에 URL을 표시하려면 이 옵션을 선택하십시오. 자산이 게시되지 않은 경우 URL이 작동하지 않지만 계획 또는 구성 용도로 URL을 사용할 수 있습니다.

<!-- **Allow AIR install** Select this option to allow users to download Adobe Dynamic Media Classic desktop version to their local hard drives. Users install the application from the Desktop Version area of the Personal Setup screen. -->

<!-- AIR users must manually uninstall their existing app and reinstall from the Web version of Adobe Dynamic Media Classic (in Personal Settings). After this one-time reinstallation, you are prompted to upgrade whenever the server has a newer version of Adobe Dynamic Media Classic AIR. Adobe Dynamic Media Classic is integrated with the Application Update Framework which streamlines the upgrade process. -->

* **[!UICONTROL CDN 무효화 템플릿]**: CDN(Content Delivery Network) 캐시를 무효화하는 데 사용되는 템플릿을 지정합니다.

  예를 들어 다음 예제와 같이 특정 이미지 ID 대신 `<ID>`을(를) 참조하는 이미지 URL(이미지 사전 설정 또는 수정자 포함)을 입력한다고 가정해 봅시다.

  `https://sample.scene7.com/is/image/Company/<ID>?$s7product$`

  템플릿에 `<ID>`이(가) 포함된 경우 Adobe Dynamic Media Classic은 `https://<server>/is/image`을(를) 채웁니다. 여기서 `<server>`은(는) 일반 설정에 정의된 게시 서버 이름입니다.

  CDN 무효화 템플릿을 설정하고 Backpack_B라는 이미지를 선택한 다음 **[!UICONTROL 파일]** > **[!UICONTROL CDN 무효화]**(으)로 이동하면 CDN 무효화 인터페이스에 다음과 같은 URL이 생성됩니다.

  `https://sample.scene7.com/is/image/Company/Backpack_B?$s7product$`

  URL 목록 상자에서 **[!UICONTROL 계속]**&#x200B;을 선택하여 특정 이미지 URL 호출에 대한 캐시를 지웁니다. URL 목록 상자에 URL을 입력하거나 붙여 넣어 추가할 수도 있습니다. 미리 템플릿을 설정할 필요가 없습니다.

  CDN 무효화 템플릿을 선택하고 무효화 CDN 요청을 수행하면 사용자 인터페이스에 표시기가 팝업됩니다. 캐시를 지우는 데 걸리는 시간을 예상할 수 있습니다.

  **[!UICONTROL 파일]** > **[!UICONTROL CDN 무효화]**&#x200B;를 클릭하면 Dynamic Media Classic에서 여러 이미지를 선택한 경우 각 이미지가 저장된 템플릿 URL에서 참조됩니다. 따라서 웹 사이트에서 참조되는 각 URL(예: 제품 세부 사항 및 검색 결과)을 참조하는 CDN 무효화 템플릿을 정의할 수 있습니다. 그런 다음 캐시에서 무효화할 이미지를 하나 이상 선택하면 URL이 인터페이스를 자동으로 채웁니다.

  [컨텐츠 캐싱](dmc-platform-overview.md#content_caching)을 참조하십시오.

  [다시 게시한 자산 및 CDN 지연](publishing-files.md#republished_assets_and_cdn_delays)을 참조하십시오.

### 찾아보기

* **[!UICONTROL 프로젝트 표시]**: Adobe Dynamic Media Classic 에셋을 구성하는 수단으로 프로젝트를 사용할 수 있는지 여부를 결정합니다. [프로젝트로 작업 구성](/help/using/organizing-projects.md)을 참조하세요.

* **[!UICONTROL 샘플 eVideo 콘텐츠 표시]**: eVideo 샘플 콘텐츠 표시를 설정하거나 해제합니다.

* **[!UICONTROL 생성된 콘텐츠 표시]**: 폴더에서 에셋에서 생성된 콘텐츠를 표시합니다. 예를 들어 PDF 파일이 업로드될 때 래스터화되면 Adobe Dynamic Media Classic에서는 원본 PDF의 각 페이지에 대해 하나의 이미지를 만듭니다. 생성된 PDF 표시 를 선택하면 원래 콘텐츠가 업로드될 때 생성된 각 이미지가 표시됩니다. PDF이 업로드된 폴더의 PDF과 함께 표시됩니다.

* **[!UICONTROL 인코딩된 비디오 표시]**: 기본적으로 선택 해제됨(해제).

  동일한 비디오의 인코딩된 다양한 파생을 탐색하지 않고도 Adobe Dynamic Media Classic에서 비디오를 빠르게 검색하고 탐색할 수 있습니다. 이 옵션을 선택 해제한 상태로 둡니다(기본값). 기본 비디오 축소판(업로드하여 파생 만들기에 사용한 소스 비디오)과 &quot;상위&quot; 응용 비디오 세트 축소판(인코딩된 비디오 세트의 &quot;하위&quot; 파생 포함)만 표시됩니다.

  그러나 기본 비디오 또는 응용 비디오 세트에서 인코딩된 개별 비디오에 계속 액세스할 수 있습니다. 이렇게 하려면 비디오 썸네일 이미지를 두 번 클릭하여 [세부 사항 보기]를 엽니다. 그런 다음 모든 &quot;하위&quot; 비디오에 액세스할 수 있도록 오른쪽 패널에서 **[!UICONTROL 인코딩된 비디오]**&#x200B;를 선택합니다.

  **[!UICONTROL 파일]** > **[!UICONTROL 재처리]**(으)로 이동하여 응용 비디오 세트에서 직접 더 많은 인코딩된 &quot;하위&quot; 비디오를 만들 수도 있습니다. Adobe Dynamic Media Classic은 응용 비디오 세트의 &quot;상위&quot; 기본 비디오를 자동으로 찾아 트랜스코딩을 위한 소스 비디오로 사용합니다. 그러나 새 개별 인코딩된 비디오를 저장할 때 검색 또는 탐색 시 해당 비디오는 표시되지 않습니다. 그러나 [세부 사항 보기]의 [인코딩된 비디오] 탭에서 여전히 액세스할 수 있습니다.

  [비디오 업로드 및 변환](uploading-encoding-videos.md#uploading_and_encoding_videos)을 참조하세요.

  검색 및 탐색 시 모든 인코딩된 비디오 파생에 액세스하는 기능을 계속 사용하려면 **[!UICONTROL [인코딩된 비디오 표시]]**&#x200B;를 선택합니다.

  [작성] 메뉴의 특정 작업은 개별 비디오에서만 작동하거나 선택적으로 작동합니다. 이 기능을 사용하려면 **[!UICONTROL [인코딩된 비디오 표시]]** 설정 방법과 관계없이 선택할 수 있는 모든 인코딩된 비디오 파생을 표시해야 합니다. **[!UICONTROL 인코딩된 비디오 표시]** 설정을 오버라이드하는 빌드 작업에는 **[!UICONTROL 응용 비디오 집합]** 및 **[!UICONTROL eCatalogs]**&#x200B;이(가) 포함됩니다.

  >[!NOTE]
  >
  >Adobe Dynamic Media Classic을 사용하여 비디오 에셋을 업로드하고 인코딩하지 않은 경우 이 옵션이 선택 취소되더라도 Adobe Dynamic Media Classic에는 개별적으로 인코딩된 모든 비디오가 표시됩니다.

* **[!UICONTROL 하위 폴더 새로 고침 단추 표시]**: 하위 폴더 새로 고침 단추 표시를 설정하거나 해제합니다.

### Adobe Dynamic Media Classic FTP 계정

* **[!UICONTROL 서버]**: FTP 계정 서버를 나열합니다.

* **[!UICONTROL 사용자 이름]**: FTP 계정 사용자 이름을 나열합니다.

### 애플리케이션에 업로드

[업로드 작업 옵션](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/569_Default%20Job%20Options_converted%20renamed_Getting%20Started-AVS) 교육 비디오도 참조하세요.

* **[!UICONTROL 이미지 덮어쓰기]**: Adobe Dynamic Media Classic에서는 두 파일의 이름이 같을 수 없습니다. 각 항목의 Adobe Dynamic Media Classic ID(이미지 이름에서 파일 이름 확장자를 뺀 값)는 고유해야 합니다. 이 규칙 때문에 [업로드] 대화 상자에는 [덮어쓰기] 선택 사항이 있습니다. 이 선택 사항의 정확한 효과는 지정한 [이미지 덮어쓰기] 선택 사항에 따라 달라집니다. 이러한 선택 사항은 대체 이미지 업로드 방법(원본 이미지를 바꾸는지, 아니면 중복 이미지가 되는지 여부)을 지정합니다. 중복 이미지의 이름은 &quot;-1&quot;로 변경됩니다(예: chair.tif의 이름은 chair-1.tif로 변경됨). 이 선택 사항은 원본과 다른 폴더에 업로드된 이미지나 원본과 다른 파일 이름 확장자(예: JPG, TIF 또는 PNG)를 가진 이미지에 영향을 줍니다. [이미지 덮어쓰기 옵션 사용](#using-the-overwrite-images-option)을 참조하십시오.

   * **[!UICONTROL 같은 기본 이미지 이름 또는 확장명으로 현재 폴더에 덮어쓰기]**: 이 옵션은 교체에 가장 엄격한 규칙입니다. 대체 이미지를 원본과 동일한 폴더에 업로드해야 하며, 대체 이미지가 원본과 동일한 파일 이름 확장자를 사용해야 합니다. 이러한 요구 사항을 충족하지 않으면 중복 항목이 만들어집니다.

   * **[!UICONTROL 확장명에 관계없이 같은 기본 자산 이름으로 현재 폴더에 덮어쓰기]**: 대체 이미지를 원본과 같은 폴더에 업로드해야 하지만 파일 이름 확장명은 원본과 다를 수 있습니다. 예를 들어 chair.tif가 chair.jpg를 대체합니다.

   * **[!UICONTROL 같은 기본 에셋 이름 또는 확장명으로 모든 폴더에 덮어쓰기]**: 대체 이미지의 파일 이름 확장명이 원본 이미지와 같아야 합니다. 예를 들어 chair.jpg는 chair.tif)가 아닌 chair.jpg를 대체해야 합니다. 그러나 대체 이미지를 원본과 다른 폴더에 업로드할 수 있습니다. 업로드한 이미지는 새 폴더에 있으며 원래 위치에서 더 이상 파일을 찾을 수 없습니다.

   * **[!UICONTROL 확장명에 상관없이 같은 기본 자산 이름으로 모든 폴더에 덮어쓰기]**: 이 옵션은 가장 포괄적인 대체 규칙입니다. 대체 이미지를 원본과 다른 폴더에 업로드하고 다른 파일 이름 확장자를 가진 파일을 업로드하여 원본 파일을 대체할 수 있습니다. 원본 파일이 다른 폴더에 있는 경우 대체 이미지는 업로드된 새 폴더에 있습니다.

* **[!UICONTROL Publish 유지]**: Adobe Dynamic Media Classic에 업로드된 대체 이미지가 대체 중인 이미지의 Publish 준비 설정을 유지하는지 여부를 지정합니다. 또는 업로드 시 설정이 지정됩니다.

* **[!UICONTROL 기본 색상 프로파일]**: CMYK 이미지를 추가할 때 기본 색상 프로파일 옵션의 일부로 적용된 색상 프로파일을 지정합니다.

* **[!UICONTROL 기본 업로드 옵션]**: 기본 업로드 옵션을 지정할 수 있는 [업로드 작업 옵션] 대화 상자를 엽니다. 이 선택 사항에 대한 자세한 내용은 [업로드 선택 사항](/help/using/uploading-files.md#upload_options)을 참조하십시오.

### 이미지 맵 편집기(응용 프로그램)

* **[!UICONTROL 기본 이미지 매핑 HREF]**: 이미지 매핑에서 HREF 열에 사용되는 기본 URL을 정의합니다. 이 URL은 이미지 맵을 만들 때 표시되는 기본 URL입니다.

* **[!UICONTROL 기본 이미지 매핑 템플릿]**: 이미지 매핑에서 HREF 템플릿에 대한 기본 JavaScript을 정의합니다. 여기서 이미지 맵을 선택할 때마다 사용자 지정 코드가 실행되도록 설정할 수 있습니다.

### 기타 설정(응용 프로그램)

* **[!UICONTROL 휴지통에서 경고를 정리합니다]**: 휴지통의 Assets이 7일 이내에 자동으로 제거됩니다. 휴지통에 있는 자산이 영구적으로 삭제될 때까지 4일 후에 회사 관리자에게 알림을 보내려면 &quot;휴지통 항목이 자동으로 삭제되기 전에 이메일 보내기&quot;를 선택하십시오. [휴지통 폴더 관리](/help/using/trash-folder.md)를 참조하십시오.

## 이미지 덮어쓰기 옵션 사용 {#using-the-overwrite-images-option}

Adobe Dynamic Media Classic에서는 두 파일의 이름이 동일하지 않습니다. 각 항목의 Adobe Dynamic Media Classic ID(이미지 이름에서 파일 이름 확장자를 뺀 값)는 고유해야 합니다. 이 규칙 때문에 [업로드] 대화 상자에는 [이미지 덮어쓰기] 선택 사항이 있습니다. 이 옵션의 정확한 효과는 각 회사의 Adobe Dynamic Media Classic 내부 설정에 대한 설정에 따라 달라집니다.

이전에 이미지를 업로드한 다음 원본 파일을 변경(또는 대체)한 경우, 선택한 덮어쓰기 옵션은 Adobe Dynamic Media Classic이 이미지를 대체하는 방법을 지정합니다. 이미지 정보는 변경되지 않고 새 이미지가 이전 이미지를 대체합니다. 폴더에 Adobe Dynamic Media Classic에 아직 없는 이미지도 포함되어 있는 경우 이러한 이미지가 추가됩니다.

업로드된 이미지가 어떤 식으로든 변경되었지만(이미지가 변경됨) 이미지에 대한 참조가 동일하게 유지되는 경우 이 옵션을 사용합니다. 덮어쓰기는 Adobe® PDF을 업로드하고 리핑할 때도 유용합니다. Adobe Dynamic Media Classic에서 이미지를 *립*&#x200B;하는 방법을 미세 조정할 수 있습니다. 업로드(Upload) 대화상자에서 ICC 색상 프로파일 옵션을 조정하고 덮어쓰기 기능을 사용하여 다시 업로드할 수도 있습니다.

프로덕션 서버의 이미지에 액세스하는 데 사용되는 Adobe Dynamic Media Classic ID는 이미지 파일 이름에서 파생됩니다. 파일 이름에 대문자와 소문자를 사용하는 것은 기존 파일을 대체하는 경우와 이미지에 액세스하는 데 사용되는 Adobe Dynamic Media Classic ID를 대체하는 경우 모두에서 중요합니다. Adobe Dynamic Media Classic에 업로드하기 전에 대문자 및 소문자가 있는 파일 이름을 사용하는 것이 올바르므로 동일한 이미지에 대해 대/소문자만 다른 Adobe Dynamic Media Classic ID가 사용되지 않도록 해야 합니다.

이 선택 사항을 선택 취소하면 기존 이미지와 동일한 파일 이름을 가진 모든 이미지가 중복 항목으로 처리되고 추가되지 않습니다.

## 이미지 사전 설정 {#image-presets}

[이미지 사전 설정] 화면은 이미지 사전 설정을 만들고 편집하는 데 사용됩니다. 이미지 사전 설정을 사용하면 Adobe Dynamic Media Classic에서 동일한 기본 이미지의 다른 크기로 이미지를 동적으로 전달할 수 있습니다. 각 이미지 사전 설정은 이미지 표시를 위한 크기 및 형식 지정 명령의 사전 정의된 모음을 나타냅니다. 이미지 사전 설정을 만들 때 이미지 제공 크기를 선택합니다. 보기 위해 이미지가 전달될 때 이미지의 모양이 최적화되도록 서식 지정 명령을 선택할 수도 있습니다.

관리자는 자산 내보내기에 대한 사전 설정을 만들 수 있습니다. 사용자는 이미지를 내보낼 때 사전 설정을 선택할 수 있으며, 이 사전 설정은 관리자가 지정하는 사양으로 이미지 형식을 다시 지정할 수도 있습니다.

이미지 사전 설정 화면을 열려면 전역 탐색 모음에서 **[!UICONTROL 설정]** > **[!UICONTROL 이미지 사전 설정]**(으)로 이동합니다.

[스마트 이미징](https://experienceleague.adobe.com/ko/docs/experience-manager-65/content/assets/dynamic/imaging-faq)을 참조하세요.

### 이미지 사전 설정 만들기 및 편집 {#creating-and-editing-image-presets}

1. **[!UICONTROL 설정]** > **[!UICONTROL 이미지 사전 설정]**(으)로 이동합니다.
1. 사전 설정을 만들거나 기존 사전 설정에서 시작합니다.

   * **이미지 사전 설정 만들기**: **[!UICONTROL 추가]**&#x200B;를 선택합니다.
   * **기존 사전 설정에서 이미지 사전 설정을 만듭니다**: 만들려는 이미지 사전 설정과 가장 유사한 이미지 사전 설정을 선택한 다음 **[!UICONTROL 편집]**&#x200B;을 선택합니다.

1. [사전 설정 추가] (또는 [편집]) 페이지에서 사전 설정 이름을 입력합니다.
1. 원하는 [사전 설정] 선택 사항을 설정합니다. 

   [이미지 사전 설정 선택 사항](application-setup.md#image_preset_options)을 참조하십시오.

1. **[!UICONTROL 저장]**&#x200B;을 선택하거나 기존 사전 설정에서 시작한 경우 **[!UICONTROL 다른 이름으로 저장]**&#x200B;을 선택합니다.
1. 사전 설정을 사용자의 이미지로 미리 보려면 **[!UICONTROL 찾아보기]**&#x200B;를 선택한 다음 이미지를 선택하십시오. 기본 이미지로 미리 보려면 **[!UICONTROL 재설정]**&#x200B;을 선택합니다.

이미지 사전 설정 화면에서 이미지 사전 설정 이름을 선택한 다음 **[!UICONTROL 편집]**&#x200B;을 선택하여 이미지 사전 설정을 편집할 수 있습니다. 이미지 사전 설정을 삭제하려면 선택한 다음 **[!UICONTROL 삭제]**&#x200B;를 선택합니다.

### 이미지 사전 설정 선택 사항 {#image-preset-options}

[사전 설정 추가] 및 [사전 설정 편집] 화면에서는 이미지 사전 설정을 만들고 편집하기 위해 다음 선택 사항을 제공합니다.

* **[!UICONTROL 사전 설정 이름]**: 공백 없이 수사적 이름을 입력하십시오. 사용자가 이 이미지 사전 설정을 식별하는 데 도움이 되도록 이름에 이미지 크기 사양을 포함하십시오.

* **[!UICONTROL 너비 및 높이]**: 이미지가 표시될 크기를 픽셀 단위로 입력하십시오.

* **[!UICONTROL 형식]**: 메뉴에서 형식을 선택합니다. GIF, JPEG, PDF 또는 TIFF 형식을 선택하면 더 많은 옵션이 표시됩니다.

   * GIF 색상 양자화 선택 사항

      * **[!UICONTROL 유형]**: 적응형(기본값), 웹 또는 Mac을 선택합니다. **[!UICONTROL Alpha이 있는 GIF]**&#x200B;을(를) 선택하면 Mac 옵션을 사용할 수 없습니다.

      * **[!UICONTROL 디더]**: [분산] 또는 [끔]을 선택합니다.

      * **[!UICONTROL 색상 수]**: 슬라이더를 드래그하여 2-255를 입력합니다.

      * **[!UICONTROL 색상 목록]**: 쉼표로 구분된 목록을 입력하십시오. 예를 들어 흰색, 회색 및 검은색은 `000000,888888,ffffff`을(를) 입력합니다.

   * JPEG 선택 사항

      * **[!UICONTROL 품질]**: JPEG 압축 수준을 제어합니다. 이 설정은 파일 크기와 이미지 품질에 모두 영향을 줍니다. JPEG 품질 범위는 1에서 100 사이입니다.

      * **[!UICONTROL JPG 색차 다운샘플링 사용]**: 눈은 고주파 광도보다 고주파 색상 정보에 덜 민감하므로 JPEG 이미지는 이미지 정보를 광도와 색상 구성 요소로 나눕니다. JPEG 이미지가 압축된 경우 광도 구성 요소는 전체 해상도로 유지되고 색상 구성 요소는 픽셀 그룹을 평균화하여 다운샘플링됩니다. 다운샘플링은 체감 품질에 거의 영향을 미치지 않으면서 데이터 양을 1/2 또는 1/3로 줄입니다. 회색 음영 이미지에는 다운샘플링을 적용할 수 없습니다. 이 기술은 고대비 이미지(예: 오버레이된 텍스트가 있는 이미지)에 유용한 압축 양을 줄입니다.

   * PDF 및 TIFF 선택 사항

      * **[!UICONTROL 압축]**: 압축 알고리즘을 선택하십시오.

* **[!UICONTROL 색상 공간]**: 색상 공간을 선택하십시오.

* **[!UICONTROL 선명하게 하기]**: 모든 크기 조절 후 기본 선명하게 하기 필터를 이미지에 적용하려면 [단순 선명 활성화] 옵션을 선택합니다. 선명하게 하기는 이미지를 다른 크기로 표시할 때 발생할 수 있는 흐림을 보상하는 데 도움이 됩니다. 

  선명하게 하기, 재샘플링 모드 및 언샵 마스킹에 대한 자세한 내용은 [이미지 선명하게](sharpening-image.md#sharpening_an_image)를 참조하십시오. [선명하게 하기](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/547_sharpening1_converted%20renamed_Done-AVS) 교육 비디오도 참조하세요.

* **[!UICONTROL 리샘플링 모드]**: 리샘플링 모드 옵션을 선택하십시오. 이미지를 다운샘플링할 때 다음 선택 사항은 이미지를 선명하게 합니다.

* **[!UICONTROL B-Linear]**: 가장 빠른 리샘플링 방법으로 일부 앨리어싱 아티팩트가 눈에 띕니다.

* **[!UICONTROL 쌍입방]**: 이미지 서버의 CPU 사용량이 증가하지만 덜 눈에 띄는 앨리어싱 아티팩트로 더 선명한 이미지를 만듭니다.

* **[!UICONTROL `Sharp 2`]**: 쌍입방 옵션보다 약간 더 선명한 결과를 만들 수 있지만 이미지 서버에서 더 높은 CPU 비용이 듭니다.

* **[!UICONTROL 삼선형]**: 사용 가능한 경우 더 높은 해상도와 더 낮은 해상도를 모두 사용합니다. 앨리어싱이 문제가 될 때만 사용하는 것이 좋습니다. 이 방법을 사용하면 고주파수 데이터가 감소하기 때문에 JPEG 크기가 줄어듭니다.

* **[!UICONTROL 언샵 마스킹]**: 선명하게 하기를 미세 조정하려면 다음 옵션을 선택하십시오.

* **[!UICONTROL 양]**: 가장자리 픽셀에 적용된 대비의 양을 제어합니다. 기본값은 1.0입니다. 고해상도 이미지의 경우 5.0만큼 높게 늘릴 수 있습니다. 이 양을 필터 강도의 측정값으로 간주합니다.

* **[!UICONTROL 반경]**: 선명하게 하기가 적용되는 가장자리 픽셀 주위의 픽셀 수를 결정합니다. 고해상도 이미지의 경우 1에서 2 사이의 값을 입력합니다. 값이 작으면 가장자리 픽셀만 선명하게 되고 값이 크면 넓은 범위의 픽셀이 선명하게 됩니다. 올바른 값은 이미지 크기에 따라 달라집니다.

* **[!UICONTROL 임계값]**: 언샵 마스크 필터가 적용될 때 무시할 대비 범위를 결정합니다. 즉, 가장자리 픽셀로 간주하여 선명하게 되기 전에 선명하게 된 픽셀이 주변 영역과 얼마나 달라야 하는지 해결하는 데 도움이 될 수 있습니다. 잡음이 발생하지 않도록 하려면 `.02`과(와) `0.2` 사이의 값으로 실험하십시오. 기본값인 6은 이미지의 모든 픽셀을 선명하게 합니다.

* **[!UICONTROL 색상 공간]**: 이미지가 만들어지는 공간(일반적으로 RGB(원본) 또는 광도 공간(강도))을 이미지에 사용할지 여부를 결정합니다.

* **[!UICONTROL 색상]** 다음 옵션을 선택하십시오.

* **[!UICONTROL 출력 색 프로필]**: **[!UICONTROL 기본 사용]** 또는 Adobe Dynamic Media Classic에서 사용할 수 있는 ICC 색 프로필 중 하나를 선택하십시오.

  [ICC 프로필](icc-profiles.md#icc_profiles)을 참조하십시오.

* **[!UICONTROL 렌더링 의도]**: 색상 프로필의 기본 렌더링 의도를 재정의하려면 옵션을 선택합니다. 기본 ICC 프로파일 중 하나가 색상 변환의 대상 색상 공간인 경우 이 옵션을 사용합니다. 또는 이 프로필은 출력 장치(프린터 또는 모니터)를 특성화하며 지정된 렌더링 의도가 이 프로필에 유효합니다.

* **[!UICONTROL 프로필 포함]**: Adobe® Photoshop®에서 이 이미지를 여는 경우 이 프로필이 사용되도록 하려면 이 옵션을 선택하십시오.

* **[!UICONTROL 인쇄 해상도]**: 이 이미지를 인쇄할 해상도를 선택합니다. 기본값은 72픽셀입니다.

* **[!UICONTROL URL 수정자]**: 설정이 아니라 이미지 사전 설정을 정의하는 URL 수정자를 지정하려면 여기에 수정자를 입력하십시오.

* **[!UICONTROL 샘플 이미지 URL]**: 추가 또는 편집 중인 이미지 사전 설정으로 이미지를 전달하는 데 Dynamic Media 이미지 서버에서 사용하는 &quot;원시&quot; URL 문자열을 나열합니다. 이 URL 문자열은 사전 설정 추가 또는 사전 설정 편집 화면에서 선택한 모든 형식 설정을 인코딩합니다.

### 이미지 사전 설정 편집, 제거 또는 비활성화 {#editing-removing-or-deactivating-an-image-preset}

1. **[!UICONTROL 설정]** > **[!UICONTROL 이미지 사전 설정]**(으)로 이동합니다.
1. [이미지 사전 설정] 화면의 테이블에서 사전 설정을 선택하고 다음 중 하나를 수행합니다.

   * **[!UICONTROL 편집]**&#x200B;을 선택한 다음 [사전 설정 편집] 대화 상자에서 새 옵션을 지정하십시오.
   * 목록에서 사전 설정을 제거하려면 **[!UICONTROL 삭제]**&#x200B;를 선택하십시오.
   * MediaPortal 사용자를 위한 전체 Adobe Dynamic Media Classic 사용자 인터페이스에서 사전 설정 이름 옆의 **[!UICONTROL 활성]** 확인란을 선택 취소합니다.

## 응용 비디오 사전 설정 활성화 또는 비활성화 {#activating-or-deactivating-adaptive-video-presets}

Adobe Dynamic Media Classic에서는 응용 비디오 인코딩 사전 설정을 제공합니다. 16:9 응용 비디오 사전 설정과 4:3 응용 비디오 사전 설정을 모두 하나의 그룹으로 결합하는 기본 사전 설정 목록입니다. 이 사전 정의된 사전 설정은 가장 일반적인 인코딩 설정을 반영하며 타겟 모바일 장치, 태블릿 및 데스크톱의 재생에 최적화되어 있습니다.

기본적으로 &quot;응용 비디오&quot; 인코딩 사전 설정만 활성화됩니다(활성화 또는 &quot;켜짐&quot;). 원할 경우, 비활성화할 수 있습니다. 비활성 적응형 비디오 사전 설정은 [업로드 작업 선택 사항] 대화 상자의 [eVideo] 섹션에 선택 가능한 선택 사항으로 표시되지 않습니다.

[비디오 업로드 및 인코딩](uploading-encoding-videos.md#uploading_and_encoding_videos)을 참조하세요.

[비디오 사전 설정](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) 교육 비디오도 참조하세요.

**응용 비디오 사전 설정을 활성화하거나 비활성화하려면:**

1. Adobe Dynamic Media Classic 오른쪽 상단 모서리에서 **[!UICONTROL 설정]** > **[!UICONTROL 응용 프로그램 설정]** > **[!UICONTROL 비디오 사전 설정]** > **[!UICONTROL 응용 비디오 사전 설정]**(으)로 이동합니다.
1. 적응형 비디오 사전 설정 페이지에서 사전 설정 이름 옆에 있는 확인란을 선택 취소하여 [업로드 작업 옵션] 대화 상자의 [EVIDEO 옵션] 목록에서 사전 설정을 제거합니다.
1. **[!UICONTROL 닫기]**&#x200B;를 선택합니다.

## 비디오 파일 인코딩을 위한 비디오 사전 설정 {#video-presets-for-encoding-video-files}

인코딩 사전 설정을 선택하려면 [업로드] 페이지의 오른쪽 아래 모서리에서 **[!UICONTROL 작업 옵션]**&#x200B;을 선택합니다. 업로드 작업 옵션 대화 상자에서 eVideo Options를 확장하고 원하는 비디오 인코딩 사전 설정을 선택합니다.

>[!NOTE]
>
>기본적으로 활성화되어 있는 &quot;응용 비디오&quot;를 제외하고, 업로드 작업 옵션 대화 상자에 다른 모든 응용 비디오 또는 단일 비디오 인코딩 사전 설정이 표시되지 않습니다. Adobe Dynamic Media Classic 관리자는 업로드 작업 옵션 대화 상자에 표시되는 비디오 인코딩 사전 설정을 결정합니다.

* 다음 응용 비디오 인코딩 또는 단일 인코딩 사전 설정 중에서 선택합니다.

   * **[!UICONTROL 16:9 응용 비디오]**: 데스크톱, 모바일(iPhone, iPad, Android™) 및 태블릿(iPad, Android™)에 전송할 16:9 화면 비율의 비디오를 만드십시오. 이 비디오는 뷰어의 연결 속도와 가장 일치하는 해상도 및 비트 전송률로 최적화되었습니다.

   * **[!UICONTROL 4:3 응용 비디오]**: 데스크톱, 모바일(iPhone, iPad, Android™) 및 태블릿(iPad, Android™)에 전송할 4:3 화면 비율의 비디오를 만드십시오. 이 비디오는 뷰어의 연결 속도와 가장 일치하는 해상도 및 비트 전송률로 최적화되었습니다.

   * **[!UICONTROL 응용 비디오]**: 모바일, 태블릿 및 데스크톱에 전송할 비디오를 만드는 데 사용되는 모든 종횡비의 단일 인코딩 사전 설정입니다. 이 사전 설정으로 인코딩된 업로드된 소스 비디오는 고정 높이로 설정됩니다. 그러나 비디오의 종횡비를 유지하기 위해 너비가 자동으로 조절됩니다.

     이렇게 유연한 &quot;자동 크기 조정&quot;은 사용자 지정 비디오 인코딩 사전 설정을 만들 때도 기본적으로 사용할 수 있습니다.

     [비디오 인코딩 사전 설정 추가 또는 편집](uploading-encoding-videos.md#adding_or_editing_a_video_encoding_preset)을 참조하세요.

   * **[!UICONTROL 응용 비디오 인코딩(16:9 또는 4:3)]**: 데스크톱, 모바일(iPhone, iPad, Android™) 및 태블릿(iPad, Android™)에 전송할 16:9 및 4:3 화면 비율의 비디오를 모두 만듭니다. 모두 뷰어의 연결 속도와 가장 일치하는 해상도 및 비트 전송률로 최적화되었습니다.

     [적응형 비디오 인코딩(16:9 또는 4:3) 비디오 사전 설정](application-setup.md#adaptive_video_encoding_16_9_or_4_3_video_presets)을 참조하십시오.

   * **[!UICONTROL 단일 인코딩 사전 설정]**

     >[!NOTE]
     >
     >iPads에 비디오를 전달하려면 모바일 인코딩 사전 설정 또는 태블릿 인코딩 사전 설정을 선택할 수 있습니다. 태블릿 사전 설정은 특히 iPad용으로 디자인되었으며, 일반적으로 큰 화면 크기와 대역폭 연결을 활용하기 위해 고해상도와 품질을 지정합니다. 태블릿 사전 설정으로 인코딩된 비디오 파일을 제공하려면 모바일 사이트나 애플리케이션에 장치 검색 코드를 포함해야 합니다. 이 코드는 재생 장치에 따라 iPhone 또는 iPad 비디오 환경을 전환합니다. 비디오 파일을 iPad에 제공하기 위한 모바일 사전 설정 선택이 보다 간소화됩니다. iPhone과 iPad에 동일한 비디오 파일을 사용할 수 있기 때문입니다. 그러나 품질은 더 낮은 해상도의 iPhone 환경으로 표준화됩니다.

      * [인코딩 사전 설정] 그룹의 [인코딩 사전 설정 정렬] 드롭다운 목록에서 [이름] 또는 [크기]를 선택하여 이름 또는 해상도 크기별로 사전 설정을 정렬합니다.
      * 비디오를 재생할 해상도 크기 및 대역폭을 기준으로 인코딩 사전 설정을 선택합니다.
      * 응용 비디오 인코딩과 비디오당 하나 이상의 인코딩 사전 설정을 선택할 수 있습니다. 예를 들어 하나의 업로드 작업에서 데스크톱과 모바일용 파일을 모두 인코딩할 수 있습니다.

**[!UICONTROL 업로드 시작]**&#x200B;을 선택하면 원본 기본 비디오 파일이 업로드되고 기본 파일에서 인코딩된 파일이 생성됩니다.

### 인코딩 사전 설정 선택 사항 정보 {#about-encoding-preset-options}

인코딩 사전 설정 선택 사항의 매개 변수는 다음과 같습니다.

* **[!UICONTROL 대상 연결 속도]**: 대상 최종 사용자의 인터넷 연결 속도입니다.

* **[!UICONTROL 인코딩된 파일 접미사]**: 식별을 위해 인코딩된 비디오 파일에 첨부된 접미사입니다.

* **[!UICONTROL 비디오 비트 전송률(데이터 전송률)]**: 비디오 재생의 1초를 구성하기 위해 인코딩되는 데이터의 양(초당 킬로비트)입니다.

* **[!UICONTROL 픽셀 너비/높이]**: 화면 이미지의 너비 차원(픽셀), 화면 이미지의 높이 차원(픽셀).

* **[!UICONTROL 초당 프레임(fps)]**: 비디오의 각 초 당 프레임 수 또는 스틸 이미지입니다. 미국과 일본에서는 대부분의 비디오가 29.97fps로 촬영되고, 유럽 및 아시아(일본 제외)에서는 대부분의 비디오가 25fps로 촬영됩니다. 그 필름은 24fps로 촬영된다.

* **[!UICONTROL 오디오 비트 전송률]**: 오디오 재생의 1초를 구성하기 위해 인코딩되는 데이터의 양(초당 킬로비트)입니다.

다음 표에서는 인코딩된 파일을 지정하는 데 사용되는 이름 지정 규칙과 비디오 사전 설정을 선택하는 권장 우수 사례를 보여 줍니다.

### 적응형 비디오(기본값) {#adaptive-video-default}

모바일, 태블릿 및 데스크톱 제공용 비디오를 만들 수 있도록 모든 종횡비에서 작동하는 인코딩 사전 설정. 이 사전 설정(기본값 및 모범 사례)으로 인코딩된 업로드된 소스 비디오는 고정된 높이로 설정되지만 비디오의 종횡비를 유지하기 위해 너비가 자동으로 조절됩니다.

**응용 비디오(기본값)**

|  | 인코딩 사전 설정 이름/도구 설명 텍스트 | 인코딩된 파일 접미어 | 비디오 데이터 속도(Kbps) | 너비/높이(픽셀) | FPS | 오디오 비트 전송률(Kbps) | 권장 사항 |
|--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 자동 × 360, 800Kbps | _Mobile_Auto×360p_800K | 800 | Auto×360 | 소스와 동일 | 64 | 모바일용(iPhone, iPad, Android™) |
| 2 | 자동 × 480, 1400Kbps | _Tablet_Auto×480p_1400K | 1400 | Auto×480 | 소스와 동일 | 96 | 태블릿용(iPad, Android™) |
| 3 | 자동 × 720, 2600Kbps | _Desktop_Auto×720p_2600K | 2600 | Auto×720 | 소스와 동일 | 128 | 데스크톱용 |

### 응용 비디오 인코딩(16:9 또는 4:3) 사전 설정 {#adaptive-video-encoding-or-video-presets}

이러한 응용 비디오 인코딩 사전 설정은 업로드한 비디오의 종횡비에 따라 자동으로 선택되는 일련의 개별 인코딩 사전 설정을 결합합니다. 예를 들어 4:3 비디오를 업로드하는 경우 **응용 비디오 인코딩(16:9 또는 4:3)** 옵션의 기본 사전 설정 목록에 있는 5개의 4:3 사전 설정을 모두 사용하여 자동으로 인코딩됩니다.

인코딩 옵션 매개 변수에 대한 자세한 내용은 [인코딩 사전 설정 옵션 정보](application-setup.md#about_encoding_preset_options)를 참조하십시오.

**응용 비디오 인코딩(16:9 또는 4:3) 사전 설정**

|  | 인코딩 사전 설정 이름/도구 설명 텍스트 | 타겟 연결 속도(Kbps) | 인코딩된 파일 접미어 | 비디오 데이터 속도(Kbps) | 너비/높이(픽셀) | FPS | 오디오 비트 전송률(Kbps) | 권장 사항 |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | `16:9, 512x288, Mobile (iPhone, iPad, Android&trade;), (400 Kbps)` | 500 | _Mobile_512x288_400K | 400 | 512x288 | 소스와 동일 | 64 | 저해상도, 3G |
| 2 | `4:3, 384x288px, Mobile (iPhone, iPad, Android&trade;), (400 Kbps)` | 500 | _Mobile_384x288_400K | 400 | 384x288 | 소스와 동일 | 64 | 저해상도, 3G |
| 3 | `16:9, 512x288, Mobile (iPhone, iPad, Android&trade;), (600 Kbps)` | 700 | _Mobile_512x288_600K | 600 | 512x288 | 소스와 동일 | 64 | 중해상도, 3G |
| 4 | `4:3, 384x288, Mobile (iPhone, iPad, Android&trade;), (600 Kbps)` | 700 | _Mobile_384x288_600 | 600 | 384x288 | 소스와 동일 | 64 | 중해상도, 3G |
| 5 | `16:9, 640x360, Tablet (iPad, Android&trade;), (800 Kbps)` | 900 | _iPad_640x360_800K | 800 | 640x360 | 소스와 동일 | 80 | 중해상도, WiFi |
| 6 | `4:3, 640x480, Tablet (iPad, Android&trade;), (800 Kbps)` | 900 | _iPad_640x480_800K | 800 | 640x480 | 소스와 동일 | 80 | 중해상도, WiFi |
| 7 | `16:9, 768x432, Tablet (iPad, Android&trade;), (1200 Kbps)` | 1.5Mbps | _iPad_768x432_1200K | 1200 | 768x432 | 소스와 동일 | 96 | 고해상도, WiFi |
| 8 | `4:3, 768x576, Tablet (iPad, Android&trade;), (1200 Kbps)` | 1.5Mbps | _iPad_768x576_1200K | 1200 | 768x576 | 소스와 동일 | 96 | 고해상도, WiFi |
| 9 | `16:9, 1280x720, Desktop, (2000 Kbps)` | 3.0Mbps | _1280x720_2000K | 2000 | 1280x720 | 소스와 동일 | 128 | 고화질, 와이드스크린 |
| 10 | `4:3, 1280x960, Desktop, (2000 Kbps)` | 3.0Mbps | _1280x960_2000K | 2000Kbps | 1280x960 | 소스와 동일 | 128 | 고화질 |

### 데스크톱 비디오 인코딩 사전 설정 {#desktop-video-encoding-presets}

데스크톱 컴퓨터에서 MP4 및 OGV를 위한 비디오 인코딩 사전 설정입니다.

인코딩 선택 사항 매개 변수에 대한 자세한 내용은 [인코딩 사전 설정 선택 사항 정보](application-setup.md#about_encoding_preset_options)를 참조하십시오.

**H264 Main 3.2: 오디오 AAC, MP4 파일 확장명**

|  | 인코딩 사전 설정 이름/도구 설명 텍스트 | 타겟 연결 속도(Kbps) | 인코딩된 파일 접미어 | 비디오 데이터 속도(Kbps) | 너비/높이(픽셀) | FPS | 오디오 비트 전송률(Kbps) | 권장 사항 |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 480x270 (400Kbps) | 500 | _480x270_400K | 400 | 480x270 | 소스와 동일 | 64 | 저해상도 와이드스크린 |
| 2 | 16:9, 640x360 (800Kbps) | 900 | _640x360_800K | 800 | 640x360 | 소스와 동일 | 80 | 중해상도 와이드스크린 |
| 3 | 16:9, 800x450 (1200Kbps) | 1.5Mbps | _800x450_1200K | 1200 | 800x450 | 소스와 동일 | 96 | 중-고해상도 |
| 4 | 16:9, 1280x720(2000Kbps) | 3.0Mbps | _1280x720_2000K | 2000 | 1280x720 | 소스와 동일 | 128 | 고화질, 와이드스크린 |
| 5 | 4:3, 320x240 (400Kbps) | 500 | _320X240_400K | 400 | 320x240 | 소스와 동일 | 64 | 저해상도 |
| 6 | 4:3, 480x360 (800Kbps) | 900 | _480x360_800K | 800 | 480x360 | 소스와 동일 | 80 | 중해상도 |
| 7 | 4:3, 640x480 (1200Kbps) | 1.5Mbps | _640x480_1200K | 1200 | 640x480 | 소스와 동일 | 96 | 중-고해상도 |
| 8 | 4:3, 1280x960(2000Kbps) | 3.0Mbps | _1280x960_2000K | 2000 | 1280x960 | 소스와 동일 | 128 | 고화질 |

**OGG Theora Vorbis: OGV 파일 확장명**

|  | 인코딩 사전 설정 이름/도구 설명 텍스트 | 타겟 연결 속도(Kbps) | 인코딩된 파일 접미어 | 비디오 데이터 속도(Kbps) | 너비/높이(픽셀) | FPS | 오디오 비트 전송률(Kbps) | 권장 사항 |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 480x270(400Kbps), OGG | 500 | _OGG_480x270_400K | 400 | 480x270 | 소스와 동일 | 64 | 저해상도 와이드스크린 |
| 2 | 16:9, 640x360(800Kbps), OGG | 900 | _OGG_640x360_800K | 800 | 640x360 | 소스와 동일 | 80 | 중해상도 와이드스크린 |
| 3 | 16:9, 800x450(1200Kbps), OGG | 1.5Mbps | _OGG_800x450_1200K | 1200 | 800x450 | 소스와 동일 | 96 | 중-고해상도 |
| 4 | 16:9, 1280x720(2000Kbps), OGG | 3.0Mbps | _OGG_1280x720_2000K | 2000 | 1280x720 | 소스와 동일 | 128 | 고화질, 와이드스크린 |
| 5 | 4:3, 320x240(400Kbps), OGG | 500 | _OGG_320X240_400K | 400 | 320x240 | 소스와 동일 | 64 | 저해상도 |
| 6 | 4:3, 480x360(800Kbps), OGG | 900 | _OGG_480x360_800K | 800 | 480x360 | 소스와 동일 | 80 | 중해상도 |
| 7 | 4:3, 640x480(1200Kbps), OGG | 1.5Mbps | _OGG_640x480_1200K | 1200 | 640x480 | 소스와 동일 | 96 | 중-고해상도 |
| 8 | 4:3, 1280x960(2000Kbps), OGG | 3.0Mbps | _OGG_1280x960_2000K | 2000 | 1280x960 | 소스와 동일 | 128 | 고화질 |

### 모바일 비디오 인코딩 사전 설정 {#mobile-video-encoding-presets}

소스 fps와 같습니다. iPhone, iPad 및 Android™ 모바일 장치용 비디오 인코딩 사전 설정입니다.

인코딩 선택 사항 매개 변수에 대한 자세한 내용은 [인코딩 사전 설정 선택 사항 정보](application-setup.md#about_encoding_preset_options)를 참조하십시오.

**H264 기본 2.1: 오디오 AAC, MP4 파일 확장명**

|  | 인코딩 사전 설정 이름/도구 설명 텍스트 | 타겟 연결 속도(Kbps) | 인코딩된 파일 접미어 | 비디오 비트 전송률(Kbps) | 픽셀 너비/높이 | FPS | 오디오 비트 전송률(Kbps) | 권장 사항 |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 512x288, 모바일(400Kbps) | 500 | _Mobile_512x288_400K | 400 | 512x288 | 소스와 동일 | 64 | 저해상도, 3G |
| 2 | 16:9, 512x288, 모바일(600Kbps) | 700 | _Mobile_512x288_600K | 600 | 512x288 | 소스와 동일 | 64 | 중해상도, 3G |
| 3 | 16:9, 512x288, 모바일(800Kbps) | 900 | _Mobile_512x288_800K | 800 | 512x288 | 소스와 동일 | 80 | 중해상도, Wi-Fi |
| 4 | 16:9, 512x288, 모바일(1000Kbps) | 1.2Mbps | _Mobile_512x288_1000K | 1000 | 512x288 | 소스와 동일 | 80 | 고해상도, Wi-Fi |
| 5 | 16:9, 512x288, 모바일(1200Kbps) | 1.5Mbps | _Mobile_512x288_1200K | 1200 | 512x288 | 소스와 동일 | 96 | 고해상도, Wi-Fi |
| 6 | 4:3, 384x288, 모바일(400Kbps) | 500 | _Mobile_384x288_400K | 400 | 384x288 | 소스와 동일 | 64 | 저해상도, 3G |
| 7 | 4:3, 384x288, 모바일(600Kbps) | 700 | _Mobile_384x288_600K | 600 | 384x288 | 소스와 동일 | 64 | 중해상도, 3G |
| 8 | 4:3, 448x336, 모바일(800Kbps) | 900 | _Mobile_448x336_800K | 800 | 448x336 | 소스와 동일 | 80 | 중해상도, Wi-Fi |
| 9 | 4:3, 448x336, 모바일(1000Kbps) | 1.2Mbps | _Mobile_448x336_1000K | 1000 | 448x336 | 소스와 동일 | 80 | 고해상도, Wi-Fi |
| 10 | 4:3, 448x336, 모바일(1200Kbps) | 1.5Mbps | _Mobile_448x336_1200K | 1200 | 448x336 | 소스와 동일 | 96 | 고해상도, Wi-Fi |

## 뷰어 사전 설정 {#viewer-presets}

>[!NOTE]
>
>**Flash 뷰어 지원 중단 알림**: 2017년 1월 31일부터 Adobe Dynamic Media Classic에서 Flash 뷰어 플랫폼에 대한 지원을 공식적으로 종료했습니다.

*뷰어 사전 설정*&#x200B;은 사용자가 컴퓨터 화면과 모바일 장치에서 리치 미디어 자산을 보는 방법을 결정하는 설정 모음입니다. 관리자는 뷰어 사전 설정을 만들 수 있습니다. 뷰어 구성 선택 사항 배열에 대한 설정을 사용할 수 있습니다. 예를 들어 뷰어 표시 크기, 확대/축소 동작, 색상 구성표, 테두리 및 글꼴을 변경할 수 있습니다.

가장 좋은 방법은 Adobe Dynamic Media Classic HTML5 비디오 뷰어를 사용하는 것입니다. HTML5 비디오 뷰어에 사용되는 사전 설정은 강력한 비디오 플레이어입니다.

를 단일 플레이어로 결합하여 다음을 수행합니다.

* HTML5 및 CSS를 사용하여 재생 구성 요소를 디자인하는 기능.
* 포함된 재생 있음.
* 브라우저의 기능에 따라 적응형 및 점진적 스트리밍을 사용합니다.

리치 미디어 콘텐츠의 범위를 데스크탑, 태블릿 및 모바일 사용자까지 확장하고 간소화된 비디오 환경을 제공합니다.

Adobe 뷰어 참조 안내서에서 [HTML 5 뷰어 정보](https://experienceleague.adobe.com/ko/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers#viewers-for-aem-assets-only)를 참조하십시오.

[Adobe Dynamic Media Classic 뷰어 사전 설정 호환성 매트릭스](application-setup.md#scene7_viewer_preset_compatibility_matrix)를 참조하십시오.

[우수 사례: HTML5 비디오 뷰어 사용](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer)을 참조하십시오.

뷰어에 따라 커뮤니티 기능을 추가할 수 있습니다. 커뮤니티 기능에는 [포함] 단추, [이메일] 단추, [링크] 단추 및 [사이트 방문] 단추가 포함됩니다. 이 단추를 사용하면 뷰어를 사용하는 사람이 다른 사람과 뷰어를 공유하거나 Adobe Dynamic Media Classic 웹 사이트를 열 수 있습니다.

[Adobe 뷰어 참조 라이브러리 예](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html)도 참조하세요.

### 응답형 디자인 웹 페이지에 대한 뷰어 지원 {#viewer-support-for-responsive-designed-web-pages}

웹 페이지마다 요구 사항이 다릅니다. 경우에 따라 별도의 브라우저 창에서 HTML 5 뷰어를 여는 링크를 제공하는 웹 페이지가 필요할 수 있습니다. 다른 경우에는 호스팅 페이지에 HTML5 뷰어를 직접 임베드해야 합니다. 후자의 경우 웹 페이지에 정적 레이아웃이 있을 수 있습니다. 또는 &quot;응답형&quot;이며 디바이스마다 또는 브라우저 창 크기마다 다르게 표시됩니다. 이러한 요구 사항을 수용하기 위해 Adobe Dynamic Media Classic과 함께 제공되는 HTML5 뷰어는 정적 웹 페이지와 반응형 디자인 웹 페이지를 모두 지원합니다.

웹 페이지에 응답형 뷰어를 포함하는 방법에 대한 자세한 내용은 [응답형 이미지 라이브러리 정보](https://experienceleague.adobe.com/ko/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/c-about-responsive-static-image-library#image-serving-api), [응답형 이미지 라이브러리 사용](https://experienceleague.adobe.com/ko/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library#image-serving-api) 및 [명령 참조: 명령 특성](https://experienceleague.adobe.com/ko/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library#responsive-static-image-library)을 참조하세요.

### 뷰어 사전 설정 유형 {#viewer-preset-types}

관리자는 다음 유형의 뷰어 사전 설정을 만들고 사용자 지정할 수 있습니다.

* **[!UICONTROL eCatalog 뷰어]**: 인쇄된 카탈로그를 읽는 환경을 시뮬레이션합니다. 페이지에서 페이지로 이동하거나, 페이지의 항목을 확대/축소하거나, 이미지 맵을 사용하여 페이지의 항목에 대한 자세한 정보를 보거나, 카탈로그를 검색할 수 있습니다. 맵 영역에 유효한 rollover_key 특성이 있는 경우 세부 정보와 이미지 매핑 항목을 표시하는 정보 패널을 포함할 수도 있습니다. 정보 패널을 포함하려면 eCatalog 뷰어 사전 설정 창의 정보 패널 설정 패널에서 정보 서버 URL을 지정합니다.

* **[!UICONTROL 견본 집합 뷰어]**: 다른 색상, 재질, 질감, 마무리 또는 패브릭으로 이미지를 표시합니다. 사용자는 썸네일을 선택하여 이미지의 변형을 확인합니다.

* **[!UICONTROL 혼합 미디어 집합 뷰어]**: 하나의 뷰어에 서로 다른 유형의 미디어를 표시합니다. 견본 집합, 회전 집합, 이미지 및 비디오를 포함할 수 있습니다. 이미지 세트의 탭 및 비디오의 탭과 같이 다양한 유형의 콘텐츠를 포함하도록 탭을 설정할 수 있습니다. 혼합 미디어 집합에서 재생되는 비디오는 타임라인과 중지, 일시 중지, 되감기 및 재생과 같은 비디오 컨트롤이 있는 표준 비디오 뷰어를 사용합니다. 혼합 미디어 세트 뷰어 사전 설정을 설정할 때 혼합 미디어 세트의 다양한 자산 유형에 사용할 뷰어를 지정합니다. [그리드 뷰어] 또는 [회전식 뷰어]를 사용하여 혼합 미디어 집합을 볼 수도 있습니다.

* **[!UICONTROL 회전 집합 뷰어]**: 사용자가 개체를 돌려 서로 다른 변과 각도를 검사할 수 있도록 여러 이미지 보기를 제공합니다.

* **비디오 뷰어**: 원본 파일의 해상도 크기 또는 사용자 지정 크기를 사용하여 비디오를 표시합니다. Adobe Dynamic Media Classic에는 비디오 재생을 위해 사전 정의된 많은 뷰어 사전 설정이 포함되어 있으며 관리자인 경우 사용자 지정 비디오 뷰어 사전 설정을 만들 수 있습니다. 비디오 뷰어를 구성하는 데 12개 이상의 설정이 있습니다. 다음을 구성할 수 있습니다.

   * 크기
   * 전경색과 배경색
   * 비디오 및 오디오 컨트롤
   * 진행률 표시줄
   * 사용자 인터페이스 스킨
   * 소셜 기능
   * 및 도움말

* **[!UICONTROL 확대/축소 뷰어]**: 다음 세 가지 확대/축소 뷰어 유형 중 하나를 선택할 수 있습니다.

* **[!UICONTROL 확대/축소 뷰어]**: 사용자가 영역을 선택하여 확대할 수 있습니다. 이미지를 확대 및 축소하고 기본 크기로 재설정할 컨트롤을 선택할 수 있습니다.

* **[!UICONTROL 확대/축소 뷰어: 플라이아웃]**: 원본 이미지 옆에 확대/축소된 영역의 두 번째 이미지를 표시합니다. 사용할 컨트롤은 없습니다. 사용자가 보려는 영역으로 선택을 이동하면 됩니다.

이 뷰어의 전체 대역폭 사용을 결정하는 경우 기본 이미지와 플라이아웃 이미지가 뷰어에 모두 제공된다는 것을 고려합니다. 기본 이미지 크기(단계 [너비] 및 [높이])와 확대/축소 비율에 의해 플라이아웃 이미지 크기가 결정됩니다. 플라이아웃 파일 크기가 너무 커지지 않도록 하려면 이러한 두 값의 균형을 조정합니다. 기본 이미지가 크면 확대/축소 비율 값을 줄입니다. [플라이아웃 너비] 및 [플라이아웃 높이]는 뷰어에 제공되는 플라이아웃 이미지의 크기가 아니라 플라이아웃 창의 크기를 결정합니다.

예를 들어 기본 이미지 크기가 350x350 픽셀이고 확대/축소 비율이 3이면 결과 플라이아웃 이미지는 1050x1050 픽셀이 됩니다. 기본 이미지 크기가 300x300 픽셀이고 확대/축소 비율이 4이면 플라이아웃 이미지는 1200x1200 픽셀이 됩니다. JPEG 품질 설정(권장 설정은 80-90 사이임)에 따라 파일 크기를 훨씬 줄일 수 있습니다. 기본 이미지 크기에 따라 권장되는 확대/축소 비율은 2.5에서 4 사이입니다.

### Adobe Dynamic Media Classic 뷰어 사전 설정 호환성 매트릭스 {#scene-viewer-preset-compatibility-matrix}

**Flash 뷰어 지원 중단 알림**: 2017년 1월 31일부터 Adobe Dynamic Media Classic에서 Flash 뷰어 플랫폼에 대한 지원을 공식적으로 종료했습니다.

다음 표는 현재 사용 가능한 Adobe Dynamic Media Classic 뷰어 사전 설정을 식별합니다. 또한 이 표에서는 뷰어가 데스크탑 및 모바일 장치와 호환되는지 여부와 지정된 각 뷰어에 사용되는 기술을 지정합니다.

[Adobe 뷰어 참조 라이브러리 예](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html)도 참조하세요.

뷰어에 대해 지원되는 웹 브라우저 및 운영 체제 버전에 대한 자세한 내용은 뷰어 릴리스 정보 를 참조하십시오.

[Adobe 뷰어 참조 릴리스 정보](https://experienceleague.adobe.com/ko/docs/dynamic-media-developer-resources)를 참조하세요.

|  | 뷰어 기술 | 데스크톱 | Apple iPhone | Apple iPad | Android™ Smartphone | Android™ 태블릿 |
|--- |--- |--- |--- |--- |--- |--- |
| 확대/축소 뷰어 |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_inline | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_light | HTML5 | X | X | X | X | X |


|  | 뷰어 기술 | 데스크톱 | Apple iPhone | Apple iPad | Android™ Smartphone | Android™ 태블릿 |
|--- |--- |--- |--- |--- |--- |--- |
| 이미지 집합 뷰어 |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

|  | 뷰어 기술 | 데스크톱 | Apple iPhone | Apple iPad | Android™ Smartphone | Android™ 태블릿 |
|--- |--- |--- |--- |--- |--- |--- |
| 견본 집합 뷰어 |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_light | HTML5 | X | X | X | X | X |

|  | 뷰어 기술 | 데스크톱 | Apple iPhone | Apple iPad | Android™ Smartphone | Android™ 태블릿 |
|--- |--- |--- |--- |--- |--- |--- |
| eCatalog 뷰어 |  |  |  |  |  |  |
| Universal_Media5_eCatalog_Adv(소셜 HTML 및 카탈로그 검색에 대한 지원이 포함됩니다.) | HTML5 | X | X | X | X | X |
| Universal_Media5_eCatalog(소셜 HTML 및 카탈로그 검색 지원 포함) | HTML5 | X | X | X | X | X |

|  | 뷰어 기술 | 데스크톱 | Apple iPhone | Apple iPad | Android™ Smartphone | Android™ 태블릿 |
|--- |--- |--- |--- |--- |--- |--- |
| 회전 뷰어 |  |  |  |  |  |  |
| Universal_HTML5_SpinSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SpinSet_light | HTML5 | X | X | X | X | X |

**eVideo 뷰어**

Adobe Dynamic Media Classic은 MP4 H.264 비디오용 모바일 비디오 재생을 지원합니다.

* 다음 위치에서 이 비디오 형식을 지원하는 BlackBerry® 장치를 찾을 수 있습니다. [BlackBerry에서 지원되는 비디오 형식®](https://developers.blackberry.com/us/en)
* 또한 이 비디오 형식을 지원하는 Windows® 장치는 [Windows® Phone에서 지원되는 비디오 형식](https://learn.microsoft.com/en-us/windows/uwp/audio-video-camera/supported-codecs)에 있습니다.

|  | 뷰어 기술 | 데스크톱 | Apple iPhone | Apple iPad | Android™ Smartphone | Android™ 태블릿 | BlackBerry® 스마트폰 | Windows® Phone |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| HTML Universal_Captivate5_Video(자막 지원 포함) [우수 사례: 범용 HTML 5 비디오 뷰어 사용](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer)을 참조하세요. | HTML5 | X | X | X | X | X | X | X |
| HTML Universal_Media5_Video_social(자막 및 소셜 미디어에 대한 지원 포함) | HTML5 | X | X | X | X | X | X | X |

|  | 뷰어 기술 | 데스크톱 | Apple iPhone | Apple iPad | Android™ Smartphone | Android™ 태블릿 |
|--- |--- |--- |--- |--- |--- |--- |
| 혼합 미디어 집합 뷰어 |  |  |  |  |  |  |
| Universal_HTML5_MixedMedia_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_MixedMedia_light | HTML5 | X | X | X | X | X |

### 지원되는 모바일 뷰어 제스처 매트릭스 {#supported-mobile-viewers-gestures-matrix}

다음 표에서는 iOS, Android™ 2.x 및 Android™ 3.x 장치에서 지원되는 모바일 뷰어 제스처를 식별합니다.

|  | 뷰어 기술 | 데스크톱 | Apple iPhone | Apple iPad | Android™ Smartphone | Android™ 태블릿 |
|--- |--- |--- |--- |--- |--- |--- |
| 이미지 집합 뷰어 |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

### [뷰어 사전 설정] 화면 정보 {#about-the-viewer-preset-screen}

[뷰어 사전 설정] 화면에서 뷰어 사전 설정을 만들고 관리합니다. 이 화면을 열려면 **[!UICONTROL 설정]** > **[!UICONTROL 뷰어 사전 설정]**(으)로 이동합니다.

[뷰어 사전 설정] 화면에서는 다음 작업을 위한 도구를 제공합니다.

* **사전 설정 추가**: **[!UICONTROL 추가]**&#x200B;를 선택하고 [뷰어 사전 설정 추가] 대화 상자에서 선택하십시오.

      [뷰어 사전 설정 추가 및 편집](application-setup.md#adding_and_editing_viewer_presets)을 참조하십시오.
  
* **사전 설정 편집**: 사전 설정을 선택한 다음 **[!UICONTROL 편집]**&#x200B;을 선택합니다.

      [뷰어 사전 설정 추가 및 편집](application-setup.md#adding_and_editing_viewer_presets)을 참조하십시오.
  
* **사전 설정 삭제**: 사전 설정을 선택한 다음 **[!UICONTROL 삭제]**&#x200B;를 선택합니다.

* **사전 설정 내보내기**: HTML5 뷰어 사전 설정을 선택합니다. 그런 다음 **[!UICONTROL 내보내기]**&#x200B;를 클릭하여 뷰어 스킨을 다운로드하여 다른 뷰어 사전 설정을 만들고 추가하는 기준으로 사용할 수 있습니다.

      HTML 5 뷰어 사전 설정 내보내기&rbrack;(application-setup.md#exporting_an_html5_viewer_preset)를 참조하십시오.
  
* **뷰어 사전 설정 목록 필터링**: 다음 도구를 사용하여 목록을 필터링합니다.

      * **활성/비활성** 드롭다운 목록을 열고 활성 사전 설정, 비활성 사전 설정 또는 모든 사전 설정을 표시하는 옵션을 선택합니다.
     * **뷰어** 드롭다운 목록을 열고 특정 종류의 뷰어만 볼 수 있는 옵션을 선택합니다. 모든 **를 보려면 모든 뷰어**&#x200B;1&rbrace;를 선택하십시오.
&rbrack;  
* **사전 설정 정렬**: 열에서 목록을 정렬할 열 제목(**[!UICONTROL Active]**, **[!UICONTROL Type]**, **[!UICONTROL Preset]** 또는 **[!UICONTROL Platform]**)을 선택합니다. 목록을 내림차순(또는 오름차순)으로 정렬하려면 열 제목을 한 번 더 선택합니다.

* **사전 설정 활성화 및 비활성화**: 사전 설정을 선택한 다음 활성화 또는 비활성화할 수 있도록 해당 [활성] 옵션을 선택합니다.

      뷰어 사전 설정 활성화 또는 비활성화&rbrack;(application-setup.md#activating_or_deactivating_viewer_presets)를 참조하십시오.
  
>[!NOTE]
>
>선택한 뷰어 사전 설정에서 에셋의 모양을 확인할 수 있도록 뷰어 사전 설정 페이지의 오른쪽에 있는 **[!UICONTROL 미리 보기]**&#x200B;를 선택합니다. 다른 에셋을 보려면 [뷰어 사전 설정] 페이지에서 **[!UICONTROL 찾아보기]**&#x200B;를 선택하고 [에셋 미리 보기 선택] 대화 상자에서 다른 에셋을 선택하십시오.

### 뷰어 사전 설정 추가 및 편집 {#adding-and-editing-viewer-presets}

사용자 인터페이스에서 **[!UICONTROL 추가]**&#x200B;를 사용하여 뷰어 사전 설정을 추가하는 것 외에 **[!UICONTROL 내보내기]**&#x200B;를 사용하여 뷰어 사전 설정을 추가할 수도 있습니다. 기존 HTML5 뷰어 사전 설정을 내보낸 다음 새 사전 설정의 기준으로 사용하면 됩니다.

[HTML5 뷰어 사전 설정 내보내기](application-setup.md#exporting_an_html5_viewer_preset)를 참조하세요.

[뷰어 사전 설정](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) 교육 비디오도 참조하세요.

**뷰어 사전 설정을 추가하고 편집하려면:**

1. Adobe Dynamic Media Classic 오른쪽 상단 모서리에서 **[!UICONTROL 설정]** > **[!UICONTROL 뷰어 사전 설정]**(으)로 이동합니다.

   사전 설정 목록에서 필터링할 수 있습니다. 예를 들어 비디오 뷰어의 사전 설정만 표시하려면 테이블 바로 위의 도구 모음에 있는 [뷰어] 드롭다운 메뉴에서 [비디오 뷰어]를 선택합니다.

1. 뷰어 사전 설정 페이지의 뷰어 사전 설정 화면에서 뷰어 사전 설정을 추가하거나 편집합니다.

   * **추가**: 도구 모음에서 **[!UICONTROL 추가]**&#x200B;를 선택합니다. 뷰어 사전 설정 추가 대화 상자에서 플랫폼을 선택하고 리치 미디어 자산 유형을 선택합니다.

     뷰어 사전 설정 **&#x200B; 만들었으면     [!UICONTROL 다른 이름으로 저장]**&#x200B;을 선택합니다.
     
   * **기존 뷰어 사전 설정에서 시작하여 추가**: 테이블에서 비디오 뷰어 사전 설정을 선택한 다음 도구 모음에서 **[!UICONTROL 편집]**&#x200B;을 선택합니다.

         비디오 뷰어를 다시 구성한 후 **[!UICONTROL 다른 이름으로 저장]**&#x200B;을 선택하여 [사전 설정 이름] 텍스트 필드에 다른 이름을 사용하여 사전 설정을 저장합니다.
     
   * **편집**: 기존 뷰어 사전 설정을 선택한 다음 **[!UICONTROL 편집]**&#x200B;을 선택합니다.

1. [뷰어 구성] 페이지의 [사전 설정 이름] 필드에 사전 설정 이름을 입력하거나 편집합니다.
1. 원하는 나머지 선택 사항을 설정합니다.

   >[!NOTE]
   >
   >인코딩된 비디오 자체의 해상도 크기로 비디오 뷰어의 크기를 자동으로 조정하려면 **[!UICONTROL Source과 동일]**&#x200B;을 선택합니다. 이 옵션을 선택하면 스테이지 너비와 스테이지 높이를 입력할 수 없습니다. 대신 비디오 자체에서 이 선택 사항이 제공됩니다. **[!UICONTROL Source과 동일]**&#x200B;을 선택한 경우 여백 크기 옵션을 설정하여 비디오 재생 영역 외부의 스킨 차원을 반영합니다. 이 여백 크기는 비디오 컨트롤의 픽셀 높이와 너비입니다. 다음 이미지를 사용하여 사용할 여백 크기를 결정할 수 있습니다.*

   비디오 뷰어의 ![여백 구성](assets/vs_video_viewer_configure_margin.png)

1. 다음 중 하나를 수행하십시오.

   * 기존 사전 설정에서 시작하여 뷰어 사전 설정을 추가한 경우 **[!UICONTROL 다른 이름으로 저장]**&#x200B;을 선택합니다.
   * 뷰어 사전 설정을 추가하거나 편집한 경우 **[!UICONTROL 저장]**&#x200B;을 선택합니다.

### HTML5 뷰어 사전 설정 내보내기 {#exporting-an-html-viewer-preset}

기존 HTML5 뷰어 사전 설정을 내보내어 HTML5 뷰어 사전 설정을 만드는 기준으로 사용할 수 있습니다. 이 내보내기 선택 사항은 뷰어를 처음부터 만들 필요가 없기 때문에 유용합니다. 대신, 원하는 사전 설정과 모양 및 동작이 비슷한 사전 설정을 내보내며, 이 사전 설정을 디자인 조정의 시작 지점으로 사용할 수 있습니다.

Adobe Dynamic Media Classic의 모든 기본 기본 뷰어 사전 설정 CSS 파일은 `Scene7SharedAssets`의 자산을 가리키는 상대 이미지 제공 경로를 사용합니다. 예를 들어 다음은에 있는 뷰어 사전 설정 CSS 파일의 이미지 에셋에 대한 상대 경로입니다

`Scene7SharedAsset`: `.s7videoviewer .s7fullscreenbutton[state][selected] { background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }`

그러나 사용자 사이트에서 뷰어 CSS 파일을 호스팅하는 경우 사용자 환경의 이미지 서버에 대한 명시적 경로를 사용하여 이러한 상대 이미지 경로를 확인해야 합니다. 예를 들어 위의 상대 경로를 명시적 경로로 업데이트한 경우 다음과 같이 표시될 수 있습니다. 여기서 `https://s7d1.scene7.com`은(는) 이미지 서버에 대한 직접 경로입니다. `https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha`

**HTML5 뷰어 사전 설정을 내보내려면:**

```as3
.s7videoviewer .s7fullscreenbutton[state][selected] 
{ background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }
```

```as3
https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha
```

1. **[!UICONTROL 설정]** > **[!UICONTROL 뷰어 사전 설정]**(으)로 이동합니다.
1. 뷰어 사전 설정 도구 모음의 왼쪽에서 두 번째 드롭다운 목록에서 **[!UICONTROL HTML5]**&#x200B;을(를) 선택합니다.
1. 왼쪽 세 번째 드롭다운 목록에서 **[!UICONTROL [모든 뷰어]]**&#x200B;를 선택합니다.
1. 새 Viewer5 뷰어 사전 설정의 기반으로 사용할 HTML 사전 설정을 선택합니다.
1. 도구 모음에서 **[!UICONTROL 내보내기]**&#x200B;를 선택합니다.
1. 선택한 Assets 내보내기 대화 상자에서 **[!UICONTROL 내보내기 제출]**&#x200B;을 선택합니다.

   내보내기를 수행하면 CSS 파일이 만들어집니다. 파일을 다운로드하고 압축을 풉니다.

1. CSS 편집기에서 CSS 파일을 열고 변경한 다음 파일을 저장합니다.
1. CSS 파일을 Adobe Dynamic Media Classic에 업로드합니다.

   [파일 업로드](uploading-files.md#uploading_files)를 참조하십시오.

1. Dynamic Media 이미지 서버에 CSS 파일을 Publish 합니다.

   [Publish 파일](publishing-files.md#publishing_files)을 참조하세요.

1. 평소와 같이 새 뷰어 사전 설정을 추가합니다. 업로드한 뷰어 CSS 파일을 선택합니다.

   [뷰어 사전 설정 추가 및 편집](application-setup.md#adding_and_editing_viewer_presets)을 참조하십시오.

### 뷰어 사전 설정 활성화 또는 비활성화 {#activating-or-deactivating-viewer-presets}

에셋을 표시하는 URL을 만들려면 사용자는 미리 보기 대화 상자에서 사전 설정 드롭다운 목록을 열고 뷰어 사전 설정을 선택한 다음 **[!UICONTROL URL 복사]**&#x200B;를 선택합니다([뷰어 사전 설정의 URL 복사](application-setup.md#copying_the_url_of_a_viewer_preset) 참조). 이 [사전 설정] 목록은 관리자가 [뷰어 사전 설정] 화면에서 추가하고 관리하는 뷰어 사전 설정을 제공합니다. 예를 들어, 사용자가 eCatalog를 미리 볼 때 모든 활성 eCatalog 뷰어 사전 설정은 미리 보기 대화 상자의 사전 설정 드롭다운 목록에 나타납니다.

[뷰어 사전 설정] 화면에서 뷰어 사전 설정을 비활성화하지 않으면 [미리 보기] 대화 상자의 [사전 설정] 드롭다운 목록이 가득 찰 수 있습니다.

**뷰어 사전 설정을 활성화하거나 비활성화하려면:**

1. **[!UICONTROL 설정]** > **[!UICONTROL 뷰어 사전 설정]**(으)로 이동합니다.
1. 뷰어 사전 설정 페이지에서 **[!UICONTROL 활성]** 옵션을 선택하거나 선택 해제하여 뷰어 사전 설정을 활성화하거나 비활성화합니다.

### 뷰어 사전 설정 URL 복사 {#copying-the-url-of-a-viewer-preset}

자산을 게시하면 뷰어 사전 설정의 설정으로 자산을 표시하는 데 사용할 URL을 복사할 수 있습니다.

URL이 클립보드로 복사됩니다. 웹 페이지, 모바일 장치 또는 애플리케이션의 HTML 코드에서 필요에 따라 사용할 수 있습니다.

**뷰어 사전 설정의 URL을 복사하려면:**

1. 찾아보기 패널에서 에셋을 선택합니다.
1. [자산 찾아보기] 패널 위의 도구 모음 오른쪽에서 다음 중 하나를 수행합니다.

   * **[!UICONTROL 눈금 보기]**&#x200B;를 선택합니다. [자산 찾아보기] 패널에서 단일 자산을 두 번 클릭하여 [세부 사항 보기]에서 엽니다. 오른쪽의 URL 및 포함 코드 패널에서 원하는 뷰어의 오른쪽에 있는 **[!UICONTROL URL 복사]**&#x200B;를 선택합니다.
   * **[!UICONTROL 눈금 보기]**&#x200B;를 선택합니다. [에셋 찾아보기] 패널에서 단일 에셋을 선택한 다음 썸네일 이미지 아래에서 **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**(으)로 이동합니다.

   뷰어 목록 페이지의 표에 있는 작업 열에서 **[!UICONTROL URL 복사]**&#x200B;를 선택합니다.

   * **[!UICONTROL 목록 보기]**&#x200B;를 선택합니다. [에셋 찾아보기] 패널에서 단일 에셋을 선택한 다음 썸네일 이미지의 오른쪽에 있는 **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**(으)로 이동합니다.

   뷰어 목록 페이지의 표에 있는 작업 열에서 **[!UICONTROL URL 복사]**&#x200B;를 선택합니다.

   * **[!UICONTROL 눈금 보기]**, **[!UICONTROL 목록 보기]** 또는 **[!UICONTROL 자세히 보기]**&#x200B;를 선택하십시오. 같은 도구 모음에서 **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**(으)로 이동합니다.

   뷰어 목록 페이지의 표에 있는 작업 열에서 **[!UICONTROL URL 복사]**&#x200B;를 선택합니다.

### 뷰어 사전 설정의 포함 코드 복사 {#copying-the-embed-code-of-a-viewer-preset}

임베드 코드 기능을 사용하면 선택한 뷰어 사전 설정의 뷰어 코드를 검토할 수 있습니다. 또한 코드를 클립보드에 복사하여 뷰어의 배포를 위해 웹 페이지에 붙여넣을 수 있습니다.

코드 편집은 [임베드 코드] 대화 상자에서 허용되지 않습니다.

**뷰어 사전 설정의 포함 코드를 복사하려면:**

1. 에셋 찾아보기 패널에서 에셋을 선택합니다.
1. [자산 찾아보기] 패널 위의 도구 모음 오른쪽에서 다음 중 하나를 수행합니다.

   * **[!UICONTROL 눈금 보기]**&#x200B;를 선택합니다. [자산 찾아보기] 패널에서 단일 자산을 두 번 클릭하여 [세부 사항 보기]에서 엽니다. 오른쪽의 URL 패널에서 **[!UICONTROL 포함 코드]**&#x200B;을(를) 선택합니다.
   * **[!UICONTROL 눈금 보기]**&#x200B;를 선택합니다. [에셋 찾아보기] 패널에서 단일 에셋을 선택한 다음 썸네일 이미지 아래에서 **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**(으)로 이동합니다.

   뷰어 목록 페이지의 표에 있는 작업 열에서 **[!UICONTROL 포함 코드]**&#x200B;를 선택합니다.

   * **[!UICONTROL 목록 보기]**&#x200B;를 선택합니다. [에셋 찾아보기] 패널에서 단일 에셋을 선택한 다음 썸네일 이미지의 오른쪽에 있는 **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**(으)로 이동합니다.

   뷰어 목록 페이지의 표에 있는 작업 열에서 **[!UICONTROL 포함 코드]**&#x200B;를 선택합니다.

   * **[!UICONTROL 눈금 보기]**, **[!UICONTROL 목록 보기]** 또는 **[!UICONTROL 자세히 보기]**&#x200B;를 선택하십시오. 같은 도구 모음에서 **[!UICONTROL 미리 보기]** > **[!UICONTROL 뷰어 목록]**(으)로 이동합니다.

   뷰어 목록 페이지의 표에 있는 작업 열에서 **[!UICONTROL 포함 코드]**&#x200B;를 선택합니다.

1. 포함 코드 대화 상자에서 **[!UICONTROL 클립보드에 복사]**&#x200B;를 선택합니다.
1. **[!UICONTROL 닫기]**&#x200B;를 선택합니다.

## 기본 뷰어 구성 {#configure-default-viewers}

Adobe Dynamic Media Classic에서 미리 보기 를 사용할 때 기본 뷰어 를 사용하여 에셋과 연결된 기본 뷰어를 구성할 수 있습니다. 다음 자산 유형에 대해 기본 미리 보기 환경을 설정할 수 있습니다.

* 이미지
* 비디오
* 회전 집합
* 카탈로그
* 이미지 집합
* 견본 집합
* 미디어 집합

**기본 뷰어를 구성하려면:**

1. 설치 드롭다운 목록에서 **[!UICONTROL 응용 프로그램 설치]**&#x200B;를 선택합니다.
1. 설정 창의 왼쪽 창에서 **[!UICONTROL 응용 프로그램 설정]** > **[!UICONTROL 뷰어]**(으)로 이동합니다.
1. **[!UICONTROL 기본 뷰어]**&#x200B;을(를) 선택하십시오.
1. 기본 뷰어 창의 각 에셋 유형에 대한 드롭다운 목록에서 에셋의 미리 보기와 연결할 뷰어를 선택합니다.
1. 기본 뷰어 창의 오른쪽 아래 모서리에서 **[!UICONTROL 설정 저장]**&#x200B;을 선택합니다.
1. [설정] 창의 오른쪽 아래 모서리에서 **[!UICONTROL 닫기]**&#x200B;를 선택하여 [자산] 창으로 돌아갑니다.

## 메타데이터 보기 {#metadata-views}

*메타데이터*&#x200B;는 자산에 대한 표준화된 정보입니다. 메타데이터를 사용하여 워크플로를 간소화하고, 자산을 구성하고, 검색을 향상시킬 수 있습니다. Adobe Dynamic Media Classic은 IPTC(International Press Telecommunications Council) 표준과 XMP(extensible metadata platform) 표준을 지원합니다. 사용자가 세부 사항 보기에서 에셋에 대한 메타데이터를 보거나 입력하기 전에 메타데이터 보기 메뉴를 열 수 있습니다. 여기에서 보거나 자산을 설명하는 데 사용할 메타데이터 필드 집합을 선택할 수 있습니다.

Adobe Dynamic Media Classic에는 사전 정의된 메타데이터 보기가 포함되어 있으며 관리자는 사용자가 메타데이터를 입력할 때 선택할 수 있도록 고유한 메타데이터 보기를 만들 수 있습니다.

### 메타데이터 보기 만들기 {#creating-a-metadata-view}

1. **[!UICONTROL 설정]** > **[!UICONTROL 응용 프로그램 설정]** > **[!UICONTROL 메타데이터]** > **[!UICONTROL 메타데이터 보기]**&#x200B;로 이동합니다.
1. **[!UICONTROL 추가]**&#x200B;를 선택합니다.
1. [사전 설정 이름] 텍스트 필드에 보기의 이름을 입력합니다.
1. (선택 사항) 사용자가 [세부 사항 보기]에서 [메타데이터] 패널을 열 때 이 보기가 표시되도록 하려면 **[!UICONTROL 기본값으로 설정]**&#x200B;을 선택합니다.
1. (선택 사항) 보기에 사용자 정의 필드를 포함하려면 **[!UICONTROL UDF 포함]**&#x200B;을 선택합니다. 사용자 지정 필드는 [세부 사항 보기]에서 [메타데이터] 패널 상단에 표시됩니다.
1. 보기에 사용할 필드를 선택합니다(**[!UICONTROL 모두 선택]**&#x200B;을(를) 선택하여 모든 필드를 선택합니다).
1. **[!UICONTROL 저장]**&#x200B;을 선택합니다.

   보기에 대해 선택한 범주와 필드가 [미리 보기] 패널에 표시됩니다.

### 메타데이터 보기 관리 {#managing-metadata-views}

1. **[!UICONTROL 설정]** > **[!UICONTROL 응용 프로그램 설정]** > **[!UICONTROL 메타데이터]** > **[!UICONTROL 메타데이터 보기]**&#x200B;로 이동합니다.
1. 다음 중 하나를 수행합니다.

   * 보기를 미리 보려면 선택합니다. 보기의 필드가 [미리 보기] 패널에 표시됩니다.
   * 보기를 편집하려면 해당 보기를 선택한 다음 **[!UICONTROL 편집]**&#x200B;을 선택합니다. 그런 다음 [미리 보기] 패널에서 필드 이름을 선택하거나 선택 취소하고 **[!UICONTROL UDF 포함]** 옵션을 선택하거나 선택 취소합니다.
   * 보기를 삭제하려면 해당 보기를 선택한 다음 **[!UICONTROL 삭제]**&#x200B;를 선택합니다.
   * 보기를 기본값으로 설정하려면 해당 보기를 선택한 다음 **[!UICONTROL 기본값으로 설정]**&#x200B;을 선택합니다. 기본 보기는 사용자가 세부 사항 보기에서 에셋을 열고 메타데이터 패널로 이동할 때 표시되는 보기입니다.

## 메타데이터 사전 설정 {#metadata-presets}

메타데이터 사전 설정은 관리자가 에셋에 할당된 메타데이터를 제어하고 규제할 수 있는 방법을 제공합니다. 세부 정보 보기에서 사용자는 해당 용도로 제공된 필드에 에셋에 대한 메타데이터를 입력할 수 있습니다. 예를 들어 사용자는 소유자 이름, 저작권 설명 및 주소를 입력할 수 있습니다. 사용자가 이 정보를 정확하고 완전하게 입력하도록 하려면 메타데이터 사전 설정을 만들 수 있습니다. 세부 사항 보기의 메타데이터 사전 설정을 선택하면 메타데이터 필드가 사전 정의된 값으로 채워집니다. 예를 들어 소유자 이름, 저작권 설명 및 주소가 자동으로 입력됩니다.

사용자가 세부 사항 보기에 자동으로 입력하여 자산을 설명할 수 있도록 하려는 각 메타데이터 값 집합에 대한 메타데이터 사전 설정을 만듭니다.

### 메타데이터 사전 설정 만들기 또는 편집 {#creating-or-editing-a-metadata-preset}

1. **[!UICONTROL 설정]** > **[!UICONTROL 응용 프로그램 설정]** > **[!UICONTROL 메타데이터]** > **[!UICONTROL 메타데이터 사전 설정]**(으)로 이동합니다.
1. [메타데이터 사전 설정] 화면에서 다음 중 하나를 수행합니다.

   * 사전 설정을 만들려면 **[!UICONTROL 추가]**&#x200B;를 선택합니다. 메타데이터 템플릿 이름 텍스트 필드에 사전 설정의 이름을 입력합니다. **[!UICONTROL 메타데이터 보기]**&#x200B;를 선택한 다음 드롭다운 목록에서 보기를 선택하십시오([메타데이터 보기](application-setup.md#metadata_views) 참조).
   * 기존 사전 설정을 편집하려면 [메타데이터 사전 설정] 목록에서 사전 설정을 선택한 다음 **[!UICONTROL 편집]**&#x200B;을 선택합니다.

1. 사전 설정에 포함할 머리글을 확장하고 사전 설정에 포함할 다른 필드에 값을 입력합니다.
1. **[!UICONTROL 저장]**&#x200B;을 선택합니다.

   사전 설정에 대해 선택한 범주와 필드가 [미리 보기] 패널에 표시됩니다.

### 메타데이터 사전 설정 관리 {#managing-metadata-presets}

1. **[!UICONTROL 설정]** > **[!UICONTROL 응용 프로그램 설정]** > **[!UICONTROL 메타데이터]** > **[!UICONTROL 메타데이터 사전 설정]**(으)로 이동합니다.
1. 다음 중 하나를 수행합니다.

   * 사전 설정을 미리 보려면 미리 보려는 사전 설정을 선택합니다. 사전 설정 정보(범주와 필드)가 [미리 보기] 화면에 표시됩니다.
   * 사전 설정을 삭제하려면 사전 설정을 선택한 다음 **[!UICONTROL 삭제]**&#x200B;를 선택합니다.

## 사용자 지정 필드 {#user-defined-fields}

미디어 포털 관리자 또는 회사 관리자는 사용자 지정, 사용자 지정 메타데이터 필드를 만들 수 있습니다. 사용자 정의 필드는 Adobe Dynamic Media Classic에서 에셋을 구성하는 데 도움이 될 수 있습니다. 필요에 따라 필드를 활성으로 표시할 수 있습니다. 활성화되면 이러한 사용자 지정 메타데이터 필드의 이름이 [상세 보기]의 [메타데이터] 패널에 표시됩니다. 사용자는 자산을 설명하기 위해 사용자 지정 메타데이터 필드에 정보를 입력할 수 있습니다. 또한 사용자 지정 메타데이터 필드를 검색 기준으로 설정할 수도 있습니다.

사용자 지정 메타데이터 필드의 효과적인 한 가지 사용 예는 특정 출시 또는 판매용 자산의 활성화 시간을 지연하는 것입니다. *날짜* 형식을 기준으로 &quot;활성화&quot; 필드를 정의합니다. 그런 다음 세부 사항 보기의 **[!UICONTROL 메타데이터]** 패널 또는 **[!UICONTROL 파일]** > **[!UICONTROL 정보 편집]**&#x200B;을 사용하여 에셋이 활성화되는 시기를 지정할 수 있습니다. Adobe Dynamic Media Classic은 에셋의 게시된 상태와 게시 내역을 확인합니다. 활성화 시간 내에 있지 않으면 게시 상태가 &quot;게시되지 않음&quot;으로 표시됩니다.

>[!NOTE]
>
>세부 사항 보기의 [메타데이터] 패널에 사용자 정의 필드가 표시되도록 하려면 메타데이터 보기에 사용자 정의 필드를 포함하십시오. [메타데이터 보기] 화면에서 [UDF(사용자 지정 필드) 포함] 선택 사항을 선택합니다. 자세한 내용은 [메타데이터 보기](application-setup.md#metadata_views)를 참조하십시오.

>[!NOTE]
>
>사용자 지정 사용자 정의 필드를 사용하여 자산을 검색하려면 **[!UICONTROL 설정]** > **[!UICONTROL 개인 설정]**(으)로 이동한 다음 **[!UICONTROL 검색에 UDF 포함]**&#x200B;을 선택합니다. [개인 설정](personal-setup.md#personal_setup)을 참조하십시오.

### 사용자 정의 메타데이터 필드 만들기 {#creating-a-user-defined-metadata-field}

1. **[!UICONTROL 설정]** > **[!UICONTROL 응용 프로그램 설정]** > **[!UICONTROL 메타데이터]** > **[!UICONTROL 사용자 정의 필드]**&#x200B;로 이동합니다.
1. **[!UICONTROL 추가]** 선택
1. [사용자 지정 필드] 대화 상자에서 원하는 선택 사항을 설정합니다.

   * **[!UICONTROL 이름]**: 메타데이터 필드의 이름을 입력하십시오.

   * **[!UICONTROL 유형]**: 사용자가 메타데이터 필드에 입력할 수 있는 정보 유형을 정의하는 옵션을 선택하십시오.

   * **[!UICONTROL 문자열]**: 텍스트 문자열입니다.

   * **[!UICONTROL Int]**: 정수입니다.

   * **[!UICONTROL 부동 소수점]**: 부동 소수점 수입니다.

   * **[!UICONTROL 예/아니요]**: 예/아니요 부울 값입니다.

   * **[!UICONTROL 날짜]**: 날짜. MM/DD/YYYY 형식을 사용할 수 있습니다.

   * **[!UICONTROL 파일 이름]**: 파일 이름입니다.

   * **[!UICONTROL 색상]**: 색상 이름입니다.

   * **[!UICONTROL Dimension]**: 에셋의 너비와 높이입니다.

   * **[!UICONTROL 형식화되지 않음]**: 이전 버전과의 호환성을 위한 것입니다. 이 선택 사항을 선택하지 마십시오.

   * **[!UICONTROL 기본값]**: 선택 사항입니다. 사용자가 필드에 입력할 가능성이 가장 높은 값을 입력합니다. 입력한 값은 만든 필드의 기본값이 됩니다.

   * **[!UICONTROL 적용 대상]**: 선택 사항입니다. 메타데이터 필드를 특정 자산 유형에만 적용하려면 자산 유형을 선택합니다.

     >[!NOTE]
     >
     >사용자 정의 필드를 만든 후에는 **[!UICONTROL 적용 대상]** 옵션을 변경할 수 없으므로 **[!UICONTROL 적용 대상]** 옵션을 신중하게 선택하십시오. Adobe Dynamic Media Classic을 사용하면 사용자 정의 필드의 이름, 유형 및 기본값을 편집할 수 있지만 **[!UICONTROL 적용 대상]** 설정은 편집할 수 없습니다. *

1. 메타데이터 필드 만들기를 마치면 **[!UICONTROL 저장]**&#x200B;을(를) 선택합니다.

### 사용자 지정 필드 관리 {#manage-user-defined-fields}

[사용자 지정 필드] 화면에서는 사용자 지정 메타데이터 필드를 관리하기 위한 명령을 제공합니다. 

Media Portal 관리자 또는 회사 관리자만 사용자 지정 필드를 관리할 수 있습니다.

이 화면을 열려면 **[!UICONTROL 설정]** > **[!UICONTROL 응용 프로그램 설정]** > **[!UICONTROL 메타데이터]** > **[!UICONTROL 사용자 정의 필드]**&#x200B;로 이동합니다.

* **필드 편집**: 필드를 선택한 다음 **[!UICONTROL 편집]**&#x200B;을 선택합니다.

* **필드 삭제**: 필드를 선택한 다음 **[!UICONTROL 삭제]**&#x200B;를 선택합니다.

* **필드 활성화**: 필드 이름 옆에 있는 **[!UICONTROL 활성]** 옵션을 선택하거나 선택 취소합니다. 회사 관리 역할에 있는 경우 이 옵션은 표시되지 않습니다. 이 옵션은 MediaPortal과 관련되어 있으므로 활성화된 필드를 보려면 [개인 설정]에서 [MediaPortal 기능 표시]를 선택(켜기)해야 합니다.

## 파일 최적화 {#optimize-files}

Adobe Dynamic Media Classic에 파일을 업로드하면 시스템이 저장 및 게시용으로 파일을 최적화합니다. 그러나 업로드 프로세스가 중단되면 일부 이미지를 최적화할 수 없습니다. 이 경우 &quot;이미지가 아직 최적화되지 않음&quot; 메시지가 표시됩니다. 관리자는 이러한 파일을 최적화할 수 있습니다.

Adobe Dynamic Media Classic은 파일을 검색하고 이전에 완전히 최적화되지 않은 이미지만 최적화합니다.

1. **[!UICONTROL 설치]** > **[!UICONTROL 응용 프로그램 설치]**(으)로 이동한 다음 **[!UICONTROL 파일 최적화]**&#x200B;를 선택합니다.
1. 최적화 작업에 대한 정보를 입력하고 **[!UICONTROL 제출]**&#x200B;을(를) 선택합니다.

   여러 회사에서 작업하는 경우 각 회사에 속하는 파일을 별도로 최적화합니다.

## 배치 집합 사전 설정 {#batch-set-presets}

Adobe Dynamic Media Classic에 에셋을 업로드하는 작업이 실행되는 동안 이미지 세트 또는 스핀 세트를 자동으로 만들 수 있도록 일괄처리 세트 사전 설정을 사용하십시오.

회사 관리자는 먼저 세트에서 그룹화할 에셋에 대한 이름 지정 규칙을 정의합니다. 그런 다음 일괄처리 집합 사전 설정을 만들어 이러한 이미지를 참조할 수 있습니다. 각 사전 설명은 고유한 이름이 지정된 독립된 지침 집합으로, 사전 설명 레서피에 정의된 이름 지정 규칙과 일치하는 이미지를 사용하여 집합을 구성하는 방법을 정의합니다.

회사에 대한 모든 활성 일괄처리 집합 사전 설정은 [업로드 작업 옵션] 대화 상자에 나열되므로 각 업로드 세션 중에 적용할 사전 설정을 지정할 수 있습니다. 회사 관리자는 모든 활성 및 비활성 일괄처리 집합 사전 설정을 볼 수 있습니다. 파일을 업로드할 때 Adobe Dynamic Media Classic은 활성 사전 설정에서 정의된 명명 규칙과 일치하는 모든 파일을 사용하여 자동으로 세트를 만듭니다.

### 기본 이름 지정 {#default-naming}

회사 관리자는 일괄처리 집합 사전 설정 레시피에 사용되는 기본 명명 규칙을 만듭니다. 일괄처리 집합 사전 설정 정의에서 선택한 기본 명명 규칙은 회사에서 모든 웹 사이트에 대해 일괄처리 집합을 생성해야 하는 모든 것일 수 있습니다. 사용자가 정의하는 기본 명명 규칙을 사용하도록 일괄처리 집합 사전 설정이 만들어집니다. 회사 정의 기본 이름 지정에 예외가 있는 경우 특정 콘텐츠 세트에 필요한 대체 사용자 지정 이름 지정 규칙을 사용하여 일괄처리 집합 사전 설정을 최대한 만들 수 있습니다.

일괄처리 집합 사전 설정 기능을 사용하려면 기본 이름 지정 규칙을 설정할 필요가 없습니다. 그러나 Adobe 우수 사례에서는 기본 명명 규칙을 사용하여 집합에 그룹화할 명명 규칙의 요소를 여러 개 정의하는 것이 좋습니다. 이렇게 하면 일괄처리 집합 생성을 간소화할 수 있습니다.

1. **[!UICONTROL 설정]** > **[!UICONTROL 응용 프로그램 설정]** > **[!UICONTROL 일괄처리 집합 사전 설정]** > **[!UICONTROL 기본 이름 지정]**(으)로 이동합니다.
1. **[!UICONTROL 양식 보기]** 또는 **[!UICONTROL 코드 보기]**&#x200B;를 선택하여 각 요소에 대한 정보를 보거나 입력하는 방법을 지정합니다.

   **[!UICONTROL 코드 보기]** 확인란을 선택하여 양식 선택과 함께 정규식 값 빌드를 볼 수 있습니다. 양식 보기에서 어떤 이유로든 제한한다면 이러한 값을 입력하거나 변경하여 명명 규칙의 요소를 정의할 수 있습니다. 값을 양식 보기에서 구문 분석할 수 없으면 양식 필드가 비활성화됩니다.

   >[!NOTE]
   >
   >비활성화된 양식 필드가 잘못된 정규 표현식을 나타내는 것은 아닙니다. 정규 표현식이 올바른지 확인되지 않습니다. 결과 줄 다음에 각 요소에 대해 작성하고 있는 정규 표현식의 결과가 표시됩니다. 전체 정규 표현식은 페이지 하단에 표시됩니다.

1. 필요한 경우 각 요소를 확장하고 사용하려는 이름 지정 규칙을 입력합니다.
1. 필요에 따라 요소에 다른 명명 규칙을 추가하려면 **[!UICONTROL 추가]**&#x200B;를 선택하십시오. 또는 **[!UICONTROL 제거]**&#x200B;를 선택하여 요소에 대한 명명 규칙을 삭제합니다.
1. **[!UICONTROL 다른 이름으로 저장]**&#x200B;을 선택하고 사전 설정 이름을 입력하세요. 또는 기존 사전 설정을 편집하는 경우 **[!UICONTROL 저장]**&#x200B;을 선택합니다.

또는 사용 가능한 양식 필드 없이 [코드 보기]를 사용할 수 있습니다. 이 뷰에서는 이름 지정 규칙 정의를 완전히 정규 표현식을 사용하여 만듭니다.

[일치] 및 [기본 이름]이라는 두 가지 요소를 정의에 사용할 수 있습니다. 이러한 필드는 명명 규칙에 대해 정의한 모든 요소입니다. 이러한 콜론은 해당 콜론이 포함된 세트의 이름을 지정하는 데 사용되는 규칙 부분을 식별하는 데 도움이 될 수 있습니다. 회사의 개별 명명 규칙은 이러한 각 요소에 대해 하나 이상의 정의 라인을 사용할 수 있습니다. 고유한 정의에 대해 여러 줄을 사용하고 주 이미지, 색상 요소, 대체 보기 요소 및 견본 요소와 같은 고유한 요소로 그룹화할 수 있습니다.

### 일괄처리 집합 사전 설정 만들기 {#creating-a-batch-set-preset}

Adobe Dynamic Media Classic은 일괄처리 집합 사전 설정을 사용하여 몇 가지 공통 정보나 콘텐츠를 공유하는 에셋을 뷰어에 표시할 이미지 세트로 구성합니다. Adobe Dynamic Media Classic에서 예약한 자산 가져오기 작업과 함께 일괄처리 집합 사전 설정 레시피가 자동으로 실행됩니다.

일괄처리 집합 사전 설정을 사용하여 일괄처리 집합 사전 설정을 만들고, 편집하고, 관리합니다. 필요한 모든 에셋 수집 작업을 처리하기 위해 필요한 만큼 사전 설정을 만들 수 있습니다. 배치 집합 사전 설정 정의에는 두 가지 형태가 있습니다. 하나는 설정한 기본 이름 지정 규칙에 대한 것이고 다른 하나는 즉석에서 생성하는 사용자 지정 이름 지정 규칙에 대한 것입니다.

양식 필드 메소드를 사용하여 일괄처리 집합 사전 설정을 정의하거나, 정규 표현식을 사용할 수 있는 코드 메소드를 사용할 수 있습니다. **[!UICONTROL 기본 이름 지정]**&#x200B;에서와 같이, 양식 보기에서 정의하고 정규식을 사용하여 정의를 빌드하는 동시에 **[!UICONTROL 코드 보기]**&#x200B;를 선택할 수 있습니다. 또는 하나의 보기만 사용하기 위해 두 보기 중 하나를 선택 취소할 수 있습니다.

[2D 회전 집합의 자동 생성을 위한 일괄처리 집합 사전 설정 만들기](application-setup.md#creating_a_batch_set_preset_for_the_auto_generation_of_a_2d_spin_set)도 참조하십시오.

[2D 회전 집합](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/537_2d-spin_converted%20renamed_Done-AVS) 교육 비디오도 참조하세요.

**일괄처리 집합 사전 설정을 만들려면:**

1. **[!UICONTROL 설정]** > **[!UICONTROL 응용 프로그램 설정]** > **[!UICONTROL 일괄처리 집합 사전 설정]** > **[!UICONTROL 일괄처리 집합 사전 설정]**(으)로 이동합니다. [세부 사항] 페이지의 오른쪽 상단에서 설정되는 **[!UICONTROL 보기 양식]**&#x200B;은 기본 보기입니다.
1. [사전 설정 목록] 패널에서 **[!UICONTROL 추가]**&#x200B;를 선택하여 페이지 오른쪽의 [세부 정보] 패널에 있는 정의 필드를 활성화합니다.
1. [세부 사항] 패널의 사전 설정 이름 필드에서 사전 설정 이름을 입력합니다.
1. [일괄처리 집합 유형] 드롭다운 메뉴에서, 사전 설정 유형을 선택합니다.

   2D 회전 집합을 자동 생성하려면 [배치 집합 유형] 드롭다운 목록에서 **[!UICONTROL 다축 회전 집합]**&#x200B;을 선택합니다.

1. 다음 중 하나를 수행하십시오.

   * 이전에 **[!UICONTROL 응용 프로그램 설정]** > **[!UICONTROL 일괄처리 집합 사전 설정]** > **[!UICONTROL 기본 이름 지정]**&#x200B;에서 설정한 기본 이름 지정 규칙을 사용하는 경우 **[!UICONTROL 자산 이름 지정 규칙]**&#x200B;을 확장한 다음 파일 이름 지정 드롭다운 목록에서 **[!UICONTROL 기본]**&#x200B;을 선택합니다.
   * 사전 설정을 설정할 때 명명 규칙을 정의하려면 **[!UICONTROL 자산 명명 규칙]**&#x200B;을 확장한 다음 파일 명명 드롭다운 목록에서 **[!UICONTROL 사용자 지정]**&#x200B;을 선택합니다.

1. 시퀀스 순서의 경우 세트가 Adobe Dynamic Media Classic에 그룹화된 후 이미지에 대한 순서를 정의합니다. 기본적으로 자산은 영숫자 순서로 지정됩니다. 그러나 정규 표현식의 쉼표 구분 목록을 사용하여 순서를 정의할 수 있습니다.
1. 이름 지정 및 생성 규칙 설정의 경우 에셋 이름 지정 규칙에서 정의한 기본 이름에 접미사 또는 접두어를 지정합니다. Adobe Dynamic Media Classic 폴더 구조 내에서 이미지 세트가 만들어지는 위치도 정의합니다.

   많은 이미지 세트를 정의하는 경우 이러한 세트를 에셋 자체가 들어 있는 폴더와 분리하십시오. 많은 고객이 이미지 세트 폴더를 만들고 애플리케이션을 리디렉션하여 여기에 일괄처리 집합 생성 세트를 배치합니다.

1. 세부 정보 패널에서 **[!UICONTROL 저장]**&#x200B;을(를) 선택합니다.

### 2D 회전 집합의 자동 생성을 위한 일괄처리 집합 사전 설정 만들기 {#creating-a-batch-set-preset-for-the-auto-generation-of-a-d-spin-set}

일괄처리 집합 유형 **다축 회전 집합**&#x200B;을(를) 사용하여 2D 회전 집합의 생성을 자동화하는 &quot;레시피&quot;를 만들 수 있습니다. 이미지 그룹은 이미지 자산이 다차원 배열에서 해당 위치에 제대로 정렬되도록 [행] 및 [열] 정규 표현식을 사용합니다.

[일괄처리 집합 사전 설정 만들기](application-setup.md#creating_a_batch_set_preset)도 참조하세요.

다축 회전 집합에는 최소한 또는 최대 개수의 행 또는 열이 없습니다.

예를 들어 *spin-2dspin*(이)라는 다축 회전 집합을 만들려고 한다고 가정합니다. 세 개의 행을 포함하고 행당 12개의 이미지가 있는 일련의 회전 집합 이미지가 있습니다. 다음과 같이 이미지의 이름이 지정됩니다.

```as3
spin-01-01
spin-01-02
… 
spin-01-12
spin-02-01
… 
spin-03-12
```

이 정보를 사용하여 다음과 같이 배치 세트 유형 배합식을 생성할 수 있습니다.

![일괄처리 집합 레시피 이미지](assets/se_batch_set_recipe.png)

회전 집합의 공유 에셋 이름 부분에 대한 그룹화가 일치 필드에(강조 표시된 대로) 추가됩니다. 행 및 열이 포함된 에셋 이름의 변수 부분이 행 및 열 필드에 각각 추가됩니다.

회전 집합을 업로드하고 게시하면 [업로드 작업 옵션] 대화 상자의 **[!UICONTROL 일괄처리 집합 사전 설정]** 아래에 나열된 2D 회전 집합 레시피의 이름이 활성화됩니다.

**2D 회전 집합의 자동 생성을 위한 일괄처리 집합 사전 설정을 만들려면:**

1. **[!UICONTROL 설정]** > **[!UICONTROL 응용 프로그램 설정]** > **[!UICONTROL 일괄처리 집합 사전 설정]** > **[!UICONTROL 일괄처리 집합 사전 설정]**(으)로 이동합니다. [세부 사항] 페이지의 오른쪽 상단에서 설정되는 **[!UICONTROL 보기 양식]**&#x200B;은 기본 보기입니다.
1. [사전 설정 목록] 패널에서 **[!UICONTROL 추가]**&#x200B;를 선택하여 페이지 오른쪽의 [세부 정보] 패널에 있는 정의 필드를 활성화합니다.
1. [세부 사항] 패널의 사전 설정 이름 필드에서 사전 설정 이름을 입력합니다.
1. [일괄처리 집합 유형] 드롭다운 메뉴에서, **[!UICONTROL 자산 집합]**&#x200B;을 선택합니다.
1. 하위 유형 드롭다운 목록에서 **[!UICONTROL 다축 회전 집합]**&#x200B;을 선택합니다.
1. **[!UICONTROL 자산 이름 지정 규칙]**&#x200B;을 확장한 다음 파일 이름 지정 드롭다운 목록에서 **[!UICONTROL 사용자 지정]**&#x200B;을 선택합니다.
1. **[!UICONTROL 일치]**&#x200B;를 사용하고, 원할 경우 **[!UICONTROL 기본 이름]** 특성도 사용하여 그룹을 구성하는 이미지 자산의 정규 표현식을 정의합니다.

   예를 들어 리터럴 Match 정규 표현식은 다음과 같습니다.

   `(\w+)-\w+-\w+`

1. **[!UICONTROL 행 열 위치]**&#x200B;를 확장한 다음 2D 회전 집합 배열 내의 이미지 자산 위치에 대해 이름 형식을 정의합니다.

   괄호로 파일 이름에 있는 행 또는 열 위치를 묶습니다.

   예를 들어 행의 정규 표현식은 다음과 같을 수 있습니다.

   `\w+-R([0-9]+)-\w+`

   또는

   `\w+-(\d+)-\w+`

   열 정규 표현식의 경우 다음과 같이 표시될 수 있습니다.

   `\w+-\w+-C([0-9]+)`

   또는

   `\w+-\w+-C(\d+)`

   이러한 표현식은 단지 예시일 뿐이라는 것을 기억하라. 정규 표현식을 만들 수 있지만 필요에 따라 조정할 수 있습니다.

   >[!NOTE]
   >
   >행과 열의 정규 표현식의 조합으로 다차원 스핀 세트 배열 내의 자산 위치를 결정할 수 없는 경우 해당 자산은 세트에 추가되지 않습니다. 오류가 기록됩니다.

1. 이름 지정 및 생성 규칙 설정의 경우 에셋 이름 지정 규칙에서 정의한 기본 이름에 접미사 또는 접두어를 지정합니다. Adobe Dynamic Media Classic 폴더 구조 내에서 이미지 세트가 만들어지는 위치도 정의합니다.

   많은 이미지 세트를 정의하는 경우 이러한 세트를 에셋 자체가 들어 있는 폴더와 분리하십시오. 많은 고객이 이미지 세트 폴더를 만들고 애플리케이션을 리디렉션하여 여기에 일괄처리 집합 생성 세트를 배치합니다.

1. 세부 정보 패널에서 **[!UICONTROL 저장]**&#x200B;을(를) 선택합니다.
1. 스핀 세트를 평소와 같이 업로드하고 게시하면 [작업 로드 옵션] 대화 상자의 [일괄처리 집합 사전 설정]에서 2D 스핀 세트의 이름을 활성화할 수 있습니다.

>[!MORELIKETHIS]
>
>* [에셋 미리 보기](previewing-asset.md#previewing_an_asset)
>* [이미지 사전 설정 설정](setting-image-presets.md#setting_up_image_presets)
>* [메타데이터 보기, 추가 및 내보내기](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
>* [작업 파일 확인](checking-job-files.md#checking_job_files)
