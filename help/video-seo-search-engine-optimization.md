---
title: 비디오 SEO(검색 엔진 최적화)
seo-title: 비디오 SEO(검색 엔진 최적화)
description: 널
seo-description: 비디오 SEO 설정을 구성하는 방법을 알아봅니다.
uuid: bac 2 c 6 a 9-8466-4 b 8 f-b 835-6 cb 0 b 4168513
contentOwner: 관리
content-type: 참조
products: sg_ Experiencemanager/dynamic-media-scene -7
geptopics: sg_ scenesevenondemand_ pk/categories/setup
discoiquuid: 34 ECD 868-775 F -452 B-B 26 E-D 26 E-D 139 F 0 E 280 AE
translation-type: tm+mt
source-git-commit: de7d2608f94935f238a11d8310b97dddc5476f57

---


# 비디오 SEO(검색 엔진 최적화){#video-seo-search-engine-optimization}

SEO는 검색 엔진에서 웹 사이트로의 트래픽 볼륨을 향상시키는 프로세스입니다. 검색 엔진은 텍스트 기반 컨텐츠에서 정보를 수집하는 기능은 우수하지만 정보가 제공되지 않은 경우 비디오 정보를 제대로 가져올 수 없습니다.

Dynamic Media Classic Video SEO를 사용하여 비디오 메타데이터를 활용하여 비디오 설명을 검색 엔진에 제공할 수 있습니다. Dynamic Media Classic 에서는 비디오 사이트 맵과 mrss 피드를 만들 수 있습니다. 이러한 항목은 비디오 정보를 검색 엔진에 전송하기 위한 표준 XML 파일입니다.

**비디오 사이트맵은** 사이트에 있는 비디오의 위치와 내용을 Google에 정확하게 알려줍니다. 이 기능을 통해 Google에서 비디오를 완벽하게 검색할 수 있습니다. 예를 들어 비디오 사이트 맵은 비디오의 실행 시간과 범주를 지정할 수 있습니다. 비디오 사이트 맵에 대한 자세한 내용은 https://www.google.com/support/webmasters/bin/answer.py?answer=80471를 참조하십시오.

**컨텐츠 게시자가 Yahoo! 에 미디어 파일을 피드하기 위해** 사용하는 mrss (Media Really Simple Syndication) 피드 사용합니다. Mrss 피드에 대한 자세한 내용은 https://www.rssboard.org/media-rss를 참조하십시오.

>[!NOTE]
>
>Google은 검색 엔진에 정보 전송 시 비디오 사이트 맵과 mRSS 피드 프로토콜을 모두 지원합니다.

Dynamic Media Classic는 각 비디오와 함께 저장된 메타데이터에서 비디오 사이트 맵과 mrss 피드를 생성할 수 있습니다. 비디오 사이트 맵과 mRSS 피드를 만드는 경우 비디오 파일에서 포함할 메타데이터 필드를 결정합니다. 이런 방식으로 각 엔진이 트래픽을 웹 사이트의 비디오로 보다 정확하게 보낼 수 있도록 검색 엔진에 비디오를 설명합니다.

>[!NOTE]
>
>비디오 사이트 맵이나 mRSS 피드를 만들기 전에 XML 파일에서 검색 엔진에 필요한 필드와 이러한 필드의 구성 방법을 확인합니다. 성공적인 비디오 사이트 맵이나 mRSS 피드를 만들려면 검색 엔진의 요구 사항을 충족해야 합니다.

Dynamic Media Classic 에서는 비디오 사이트 맵과 mrss 피드에 대한 보고서를 생성한 후에 만듭니다. 이러한 보고서는 [비디오 SEO 보고서] 화면에서 사용할 수 있습니다.

>[!NOTE]
>
>비디오 사이트 맵과 Mrss 피드의 경우 Dynamic Media Classic는 게시용으로 표시된 비디오에서만 메타데이터를 캡처합니다. 비디오를 게시로 표시하여 해당 메타데이터를 비디오 사이트 맵과 mRSS 피드에 포함하십시오.

## Choosing video SEO settings {#choosing-video-seo-settings}

[비디오 검색 엔진 최적화 설정] 화면에서 비디오 사이트 맵과 mRSS 피드에 대한 비디오 SEO 설정을 선택합니다. 이 화면을 열려면 [설정] &gt; [애플리케이션 설정] &gt; [비디오 SEO] &gt; [설정]을 선택합니다.

[일반 설정] 영역에서 비디오 사이트 맵, mRSS 피드 또는 둘 다를 생성할 것인지를 선택합니다. [생성 설정] 영역에서 메타데이터 필드를 입력 필드에 매핑합니다.

설정을 선택한 후 [생성](또는 [저장 및 생성])을 클릭하여 비디오 사이트 맵, mRSS 피드 또는 둘 다를 만듭니다.

### 일반 설정 선택 {#choosing-general-settings}

[생성 모드] 드롭다운 목록에서 보고서 모드를 선택합니다.

**비디오 사이트맵비디오** 사이트 맵을 만듭니다.

**Mrss 피드미디어** RSS (mrss) 피드를 만듭니다.

**두 가지 모두 두 유형의 XML 파일을** 만듭니다.

**끄기** 비디오 사이트 맵과 미디어 RSS (mrss) 피드 생성을 중지하려면 이 옵션을 선택합니다.

[자동/수동 모드] 드롭다운 목록에서 자동 또는 수동으로 생성할지 여부를 선택합니다.

**자동 모드** Dynamic Media Classic는 매일 하나의 비디오 사이트맵, 미디어 RSS (mrss) 피드 또는 둘 다를 자동으로 생성합니다. [게시용으로 표시] 옵션을 선택하여 Dynamic Media Classic에서 생성하는 XML 파일을 자동으로 게시로 표시합니다.

**수동 모드에서는** 비디오 검색 최적화 설정 화면에서 생성 또는 저장 및 생성을 클릭하면 비디오 사이트맵, 미디어 RSS (mrss) 피드 또는 둘 다를 생성할 수 있습니다. 다음 선택 사항도 선택합니다.

**생성되는 XML** 파일이 게시용으로 표시되지 않습니다.

**생성된 XML 파일이 게시되도록** 게시용으로 표시합니다.

**부분 생성** 검색 엔진은 모든 비디오에 대한 전체 메타데이터 정보가 들어 있지 않은 경우 XML 파일을 거부할 수 있습니다. 이 선택 사항은 일부 비디오에 대한 메타데이터를 사용할 수 없는 경우에도 XML 파일을 생성합니다. [보고서] 화면에 경고가 생성됩니다. XML 파일을 내보내고 누락된 정보를 수동으로 처리하려는 경우 이 선택 사항을 선택합니다.

### 생성 설정 선택 {#choosing-generation-settings}

[생성 설정] 영역에는 비디오 사이트 맵 및/또는 mRSS 피드에 대한 입력 필드가 나열되며 [메타데이터] 패널에 메타데이터 필드 이름이 표시됩니다. [일반 설정] 영역을 사용하여 입력 필드를 메타데이터 필드에 매핑합니다. 이렇게 하면 비디오 사이트맵 및/또는 Mrss 피드에 대한 메타데이터를 얻을 수 있는 Dynamic Media Classic에 알립니다.

1. [메타데이터 보기] 메뉴에서 메타데이터 보기를 선택합니다. 보기를 선택하면 메타데이터 필드 이름이 [메타데이터] 패널에 표시됩니다. 메타데이터 보기에 대한 자세한 내용은 [메타데이터 보기](application-setup.md#metadata_views)를 참조하십시오.
1. [메타데이터] 패널에서 [랜딩 페이지], [제목], [설명], [태그] 및 [범주] 입력 필드로 메타데이터 필드 이름을 드래그합니다. [랜딩 페이지], [제목] 및 [설명] 필드는 필수입니다.

   >[!NOTE]
   >
   >입력 필드에 수동으로 데이터를 입력할 수도 있습니다.

1. [저장]을 클릭하여 XML 파일을 생성하지 않고 설정을 저장하거나, [생성]을 클릭하여 XML 파일을 생성하거나, [저장 및 생성]을 클릭하여 저장하고 파일을 생성합니다.

   XML 파일이 생성되고 작업 로그에 기록됩니다. 비디오 사이트 맵(video-sitemap) 및 미디어 RSS(mRSS) 피드(mrss-feed) 파일은 회사의 루트 폴더에 저장됩니다.

>[!NOTE]
>
>검색 엔진에 전송하려면 먼저 비디오 사이트 맵이나 mRSS 피드를 게시해야 합니다. 비디오 사이트 맵과 미디어 RSS(mRSS) 피드 파일은 회사의 루트 폴더에 저장됩니다. 필요한 경우 이러한 XML 파일을 게시로 표시하고 [게시]를 클릭합니다.

## 검색 엔진에 비디오 사이트 맵과 mRSS 피드 파일 전송 {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

비디오 사이트 맵과 미디어 RSS(mRSS) 피드 파일은 회사의 루트 폴더에 저장됩니다.

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

이러한 URL 중 하나를 검색 엔진의 웹 마스터 도구에 복사하여 비디오 사이트 맵이나 미디어 RSS(mRSS) 피드 파일을 검색 엔진으로 전송합니다.

## 비디오 SEO 보고서 보기 {#viewing-video-seo-reports}

[비디오 검색 엔진 최적화 보고서] 화면에서 비디오 SEO 보고서를 봅니다. 이 화면을 열려면 설정 &gt; 애플리케이션 설정 &gt; 비디오 SEO &gt; 보고서를 클릭합니다.

보고서를 생성할 때 오류가 발생한 경우 [보고서] 화면에 나열됩니다.
