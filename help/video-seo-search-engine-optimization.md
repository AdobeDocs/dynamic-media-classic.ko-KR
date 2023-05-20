---
title: 비디오 SEO(검색 엔진 최적화)
description: Adobe Dynamic Media Classic에서 비디오 SEO 설정을 구성하는 방법에 대해 알아봅니다.
uuid: bac2c6a9-8466-4b8f-b835-6cb0b4168513
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 34ecd868-775f-452b-b26e-d139f0e280ae
feature: Dynamic Media Classic
role: Admin
exl-id: f76b0e09-f148-46aa-b710-ec35bfebcb37
source-git-commit: cb55e09a997b9d36002c4ac429603576d52fb8bd
workflow-type: tm+mt
source-wordcount: '1037'
ht-degree: 37%

---

# 비디오 SEO(검색 엔진 최적화){#video-seo-search-engine-optimization}

SEO는 검색 엔진에서 웹 사이트로의 트래픽 볼륨을 향상시키는 프로세스입니다. 검색 엔진은 텍스트 기반 컨텐츠에서 정보를 수집하는 기능은 우수하지만 정보가 제공되지 않은 경우 비디오 정보를 제대로 가져올 수 없습니다.

Adobe Dynamic Media Classic 비디오 SEO를 사용하여 비디오 메타데이터를 적용하여 검색 엔진에 비디오 설명을 제공할 수 있습니다. Adobe Dynamic Media Classic은 비디오 사이트 맵 및 mRSS 피드를 만드는 기능을 제공합니다. 이러한 표준 XML 파일은 비디오 정보를 검색 엔진에 제출하는 데 사용됩니다.

* **비디오 사이트 맵** - Google에 비디오 컨텐츠가 사이트에서 어디에 있는지 정확하게 알려줍니다. 따라서 Google에서 비디오를 완전히 검색할 수 있습니다. 예를 들어 비디오 사이트 맵은 비디오의 실행 시간과 범주를 지정할 수 있습니다. 비디오 사이트 맵에 대한 자세한 내용은 [비디오 사이트 맵 및 비디오 사이트 맵 대체 요소](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

* **mRSS(Media Really Simple Syndication) 피드** - 콘텐츠 게시자가 미디어 파일을 Yahoo!에 피드하는 데 사용됨 사용합니다. mRSS 피드에 대한 자세한 내용은 [비디오 사이트 맵 및 비디오 사이트 맵 대체 요소](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

>[!NOTE]
>
>Google은 검색 엔진에 정보 전송 시 비디오 사이트 맵과 mRSS 피드 프로토콜을 모두 지원합니다.

Adobe Dynamic Media Classic은 각 비디오와 함께 저장된 메타데이터에서 비디오 사이트 맵 및 mRSS 피드를 생성할 수 있습니다. 비디오 사이트 맵과 mRSS 피드를 만드는 경우 비디오 파일에서 포함할 메타데이터 필드를 결정합니다. 이런 방식으로 각 엔진이 트래픽을 웹 사이트의 비디오로 보다 정확하게 보낼 수 있도록 검색 엔진에 비디오를 설명합니다.

>[!NOTE]
>
>비디오 사이트 맵이나 mRSS 피드를 만들기 전에 XML 파일에서 검색 엔진에 필요한 필드와 이러한 필드의 구성 방법을 확인합니다. 성공적인 비디오 사이트 맵이나 mRSS 피드를 만들려면 검색 엔진의 요구 사항을 충족해야 합니다.

Adobe Dynamic Media Classic은 사용자가 비디오 사이트 맵 및 mRSS 피드를 생성한 후 이에 대한 보고서를 생성합니다. 이러한 보고서는 비디오 SEO 보고서 페이지에서 사용할 수 있습니다.

>[!NOTE]
>
>비디오 사이트 맵 및 mRSS 피드의 경우 Adobe Dynamic Media Classic은 게시로 표시된 비디오에서만 메타데이터를 캡처합니다. 비디오를 게시로 표시하여 해당 메타데이터를 비디오 사이트 맵과 mRSS 피드에 포함하십시오.

## 비디오 SEO 설정 선택 {#choosing-video-seo-settings}

에서 비디오 사이트 맵 및 mRSS 피드에 대한 비디오 SEO 설정을 선택합니다. **[!UICONTROL 비디오 검색 엔진 최적화 설정]** 페이지를 가리키도록 업데이트하는 중입니다. 이 페이지를 열려면 전역 탐색 모음에서 다음 위치로 이동합니다. **[!UICONTROL 설정]** > **[!UICONTROL 응용 프로그램 설정]** > **[!UICONTROL 비디오 SEO]** > **[!UICONTROL 설정]**.

다음에서 **[!UICONTROL 일반 설정]** 영역에서 비디오 사이트 맵, mRSS 피드 또는 둘 다를 생성할지 여부를 선택합니다. 다음에서 **[!UICONTROL 생성 설정]** 영역, 메타데이터 필드를 입력 필드에 매핑합니다.

설정을 선택한 후 다음을 선택합니다 **[!UICONTROL 저장]** (또는 **[!UICONTROL 저장 및 생성]**)을 클릭하여 비디오 사이트 맵, mRSS 피드 또는 둘 다를 만듭니다.

### 일반 설정 {#choosing-general-settings}

다음에서 **[!UICONTROL 생성 모드]** 드롭다운 목록에서 보고서 모드를 선택합니다.

* **비디오 사이트 맵** - 비디오 사이트 맵을 만듭니다.

* **mRSS 피드** - 미디어 RSS(mRSS) 피드를 만듭니다.

* **모두** - 두 가지 유형의 XML 파일을 모두 만듭니다.

* **끔** - 비디오 사이트 맵 및 미디어 RSS(mRSS) 피드 생성을 중지하려면 이 옵션을 선택합니다.

다음에서 **[!UICONTROL 자동/수동 모드]** 드롭다운 목록에서 자동 또는 수동 생성 여부를 선택합니다.

* **자동 모드** - Adobe Dynamic Media Classic은 매일 비디오 사이트 맵, 미디어 RSS(mRSS) 피드 또는 두 피드를 모두 자동으로 생성합니다. 다음 항목 선택 **[!UICONTROL 게시로 표시]** Adobe Dynamic Media Classic에서 생성하는 XML 파일을 게시용으로 자동으로 표시하는 옵션입니다.

   * **게시로 표시** 생성된 XML 파일을 게시하기 위해 표시합니다.

* **수동 모드** - Adobe Dynamic Media Classic은 사용자가 선택하면 비디오 사이트 맵, 미디어 RSS(mRSS) 피드 또는 둘 다 생성합니다. **[!UICONTROL 생성]** 또는 **[!UICONTROL 저장 및 생성]** 비디오 검색 최적화 설정 화면에서 다음을 수행합니다. 다음 선택 사항도 선택합니다.

   * **추가 설정 없음** - 생성된 XML 파일을 게시하도록 표시하지 않습니다.

   * **게시로 표시** - 생성된 XML 파일을 게시하기 위해 표시합니다.

   * **부분 생성 허용** - 모든 비디오에 대한 전체 메타데이터 정보가 포함되지 않은 XML 파일은 검색 엔진에서 거부할 수 있습니다. 이 옵션은 일부 비디오에 메타데이터를 사용할 수 없는 경우에도 XML 파일을 생성합니다. [보고서] 화면에 경고가 생성됩니다. XML 파일을 내보내고 누락된 정보를 수동으로 처리하려는 경우 이 선택 사항을 선택합니다.

### 생성 설정 선택 {#choosing-generation-settings}

[생성 설정] 영역에는 비디오 사이트 맵이나 mRSS 피드 또는 둘 다에 대한 입력 필드가 나열되고 [메타데이터] 패널에는 메타데이터 필드의 이름이 나열됩니다. [일반 설정] 영역을 사용하여 입력 필드를 메타데이터 필드에 매핑합니다. 이렇게 하면 Adobe Dynamic Media Classic에 비디오 사이트 맵 및/또는 mRSS 피드에 대한 메타데이터를 가져올 위치를 알려 줍니다.

1. [메타데이터 보기] 메뉴에서 메타데이터 보기를 선택합니다. 보기를 선택하면 메타데이터 필드 이름이 [메타데이터] 패널에 표시됩니다.
[메타데이터 보기](application-setup.md#metadata_views)를 참조하십시오.
1. [메타데이터] 패널에서 [랜딩 페이지], [제목], [설명], [태그] 및 [범주] 입력 필드로 메타데이터 필드 이름을 드래그합니다. [랜딩 페이지], [제목] 및 [설명] 필드는 필수입니다.

   >[!NOTE]
   >
   >입력 필드에 수동으로 데이터를 입력할 수도 있습니다.

1. 다음 중 하나를 수행하십시오.

   * XML 파일을 생성하지 않고 설정을 저장하려면 **[!UICONTROL 저장]**.
   * 파일을 저장하고 생성하려면 다음을 선택합니다. **[!UICONTROL 저장 및 생성]**.

      XML 파일이 생성되고 작업 로그에 기록됩니다. 비디오 사이트 맵(video-sitemap) 및 미디어 RSS(mRSS) 피드(mrss-feed) 파일은 회사의 루트 폴더에 저장됩니다.

>[!NOTE]
>
>검색 엔진에 제출하기 전에 비디오 사이트 맵 또는 mRSS 피드를 게시합니다. 비디오 사이트 맵과 미디어 RSS(mRSS) 피드 파일은 회사의 루트 폴더에 저장됩니다. 필요한 경우 이러한 XML 파일을 게시용으로 표시하고 을 선택합니다. **[!UICONTROL 게시]**.

## 검색 엔진에 비디오 사이트 맵 및 mRSS 피드 파일 제출 {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

비디오 사이트 맵과 미디어 RSS(mRSS) 피드 파일은 회사의 루트 폴더에 저장됩니다.

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

이러한 URL 중 하나를 검색 엔진의 웹 마스터 도구에 복사하여 비디오 사이트 맵이나 미디어 RSS(mRSS) 피드 파일을 검색 엔진으로 전송합니다.

## 비디오 SEO 보고서 보기 {#viewing-video-seo-reports}

비디오 검색 엔진 최적화 보고서 페이지에서 비디오 SEO 보고서 보기 이 페이지를 열려면 전역 탐색 모음에서 다음 위치로 이동합니다. **[!UICONTROL 설정]** > **[!UICONTROL 응용 프로그램 설정]** > **[!UICONTROL 비디오 SEO]** > **[!UICONTROL 보고서]**.

보고서가 생성될 때 오류가 발생하면 보고서 페이지에 오류가 표시됩니다.
