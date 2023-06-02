---
title: 파일 게시
description: "Dynamic Media 이미지 서버에 자산을 게시하는 방법을 알아봅니다. 자산을 한 번만 게시하거나 Adobe Dynamic Media Classic에서 반복 일정에 자산을 게시하도록 예약할 수 있습니다. 자산이 게시되면 제공할 수 있습니다. Adobe Dynamic Media Classic에서 URL 호출을 복사하여 웹 사이트 또는 애플리케이션에 추가할 수 있습니다."
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 91b73a09-c5b5-4001-b36f-6bebe65717ff
source-git-commit: 358284e6c9888e5188bec35eb7b5408563a71bad
workflow-type: tm+mt
source-wordcount: '1729'
ht-degree: 45%

---

# 파일 게시{#publishing-files}

자산을 Dynamic Media 이미지 서버에 게시합니다. 자산을 한 번만 게시하거나 Adobe Dynamic Media Classic에서 반복 일정에 자산을 게시하도록 예약할 수 있습니다. 자산이 게시되면 제공할 수 있습니다. Adobe Dynamic Media Classic에서 URL 호출을 복사하여 웹 사이트 또는 애플리케이션에 추가할 수 있습니다.

Adobe Dynamic Media Classic은 이제 HTTP/2를 통해 모든 이미지 및 비디오의 전달을 지원합니다. 즉, 이미지 또는 비디오에 대한 게시된 URL 또는 포함 코드를 호스팅된 에셋을 허용하는 모든 애플리케이션과 통합할 수 있습니다. 그런 다음 게시된 에셋은 HTTP/2 프로토콜을 통해 전달됩니다. 이 전달 방법은 브라우저와 서버의 통신 방식을 개선하여 모든 Adobe Dynamic Media Classic 에셋의 응답 및 로드 시간을 향상시킵니다. 다음을 참조하십시오 [컨텐츠의 HTTP2 전달 FAQ](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/http2.html#dynamic).

## 업로드 후 게시 {#publish-after-uploading}

게시 또는 게시 취소 상태의 자산. 기본적으로 Adobe Dynamic Media Classic에 업로드하는 모든 자산은 게시용으로 자동으로 표시됩니다.

자세한 내용은 [즉시 게시 알림 PDF](/help/assets/rendering-instant-publish-notification.pdf).

다음 기술을 사용하여 자산을 게시로 표시합니다.

* **[!UICONTROL 업로드 후 게시]** - 업로드 페이지의 맨 아래에서 **[!UICONTROL 업로드 후 게시]**. 기본값은 선택된 상태입니다.

* **[!UICONTROL 업로드 후 게시]** - [작업 옵션] 대화 상자에서 **[!UICONTROL 업로드 후 게시]**. 기본값은 선택된 상태입니다.

일부 &quot;하위&quot; 자산은 상위 자산을 게시로 표시할 때 자동으로 게시로 표시됩니다. 이 표에서는 자동으로 게시로 표시되는 하위 자산을 보여 줍니다.

| 상위(그룹) 항목 | 하위(구성원) 항목 |
| --- | --- |
| 이미지 집합 | 세트 내 이미지. |
| 견본 집합 | 세트 내 견본. |
| 회전 집합 | 세트 내 이미지. |
| 템플릿 | 템플릿 파일, 페이지 및 이미지. |

파생된 이미지의 상위 이미지가 게시될 때 파생된 이미지도 자동으로 게시용으로 표시됩니다. 파생 이미지에는 이미지 편집 선택 사항으로 조정한 이미지도 포함됩니다. 기본 및 파생 아래의 세부 사항 보기에서 이러한 파생된 이미지를 볼 수 있습니다.

## 게시 작업 만들기 {#creating-a-publish-job}

Adobe Dynamic Media Classic 서버에 업로드했지만 아직 자동으로 게시하지 않으려는 자산을 게시하기 위한 게시 작업을 만듭니다. 1회 게시 작업을 수행하거나 작업이 정기적으로 반복되도록 예약할 수 있습니다. Adobe Dynamic Media Classic은 특정 서버에 게시하기 위한 고급 게시 옵션과 이미 게시된 에셋을 다시 게시하기 위한 옵션을 제공합니다.

**게시 작업을 만들려면:**

1. 전역 탐색 모음에서 를 선택합니다. **[!UICONTROL 게시]**.
1. [게시] 대화 상자에서, 게시 작업이 일회성인지 아니면 반복 게시 작업인지 선택합니다.

   다음을 참조하십시오 [1회 게시 작업 만들기](publishing-files.md#creating_a_one_time_publish_job) 및 [반복 게시 작업 만들기](publishing-files.md#creating_a_recurring_publish_job).

1. 작업 이름을 입력합니다.
1. 선택적으로 [고급] 선택 사항을 표시하고 이러한 선택 사항을 선택합니다. 

   [[고급] 게시 선택 사항](publishing-files.md#advanced_publish_options)을 참조하십시오.

1. 선택 **[!UICONTROL 게시 제출]**.

Adobe Dynamic Media Classic은 작업 페이지에서 게시 작업을 추적합니다. 이 페이지에서 게시 작업을 검토할 수 있습니다.

>[!NOTE]
>
>다시 게시하는 자산(전에 게시한 자산)은 CDN(Content Delivery Network)의 웹 캐싱 메커니즘 때문에 웹 사이트에 즉시 표시되지 않습니다. [다시 게시한 자산 및 CDN 지연](publishing-files.md#republished_assets_and_cdn_delays)을 참조하십시오.

### 1회 게시 작업 만들기 {#creating-a-one-time-publish-job}

다음을 선택하여 1회 게시 작업 만들기 **[!UICONTROL 일회]** 옵션을 선택할 수 있습니다.

게시 작업을 나중에 수행하려면 게시 페이지에서 을 선택합니다. **[!UICONTROL 일회]**&#x200B;을 선택한 다음 을 선택합니다. **[!UICONTROL 나중으로 예약]** 드롭다운. [달력] 및 [시간] 슬라이더를 사용하여 게시 작업을 실행할 날짜와 시간을 선택합니다.

### 반복 게시 작업 만들기 {#creating-a-recurring-publish-job}

을(를) 선택하여 반복 게시 작업 만들기 **[!UICONTROL 반복]** 게시 페이지에서 참조할 수 있습니다.

그런 다음 [반복] 옵션을 선택합니다. **[!UICONTROL 매일]**, **[!UICONTROL 매주]**, **[!UICONTROL 월별]**, 또는 **[!UICONTROL 사용자 정의]**&#x200B;그런 다음 게시 작업이 반복될 시기를 지정합니다. Adobe Dynamic Media Classic은 반복 게시 작업을 예약하기 위한 캘린더 도구를 제공합니다. 다음을 선택할 수 있습니다. **[!UICONTROL 사용자 정의]** 옵션을 선택하고 규칙 텍스트 필드에 규칙을 입력하여 사용자 정의 작업 간격을 설명합니다.

다음을 참조하십시오 [사용자 지정 업로드 또는 게시 작업 시간 간격 만들기](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

>[!NOTE]
>
>작업 페이지에 반복 게시(및 업로드) 작업이 나열됩니다. 작업 페이지의 [예약됨] 탭으로 이동하여 예약된 작업을 편집하거나 삭제할 수 있습니다.

### [고급] 게시 선택 사항 {#advanced-publish-options}

게시 페이지의 [고급] 옵션을 표시하고 다음과 같은 게시 작업 처리 옵션을 선택합니다.

* **[!UICONTROL 게시 위치]** - 특정 서버에만 자산을 게시하려면 서버 유형을 선택합니다.

* **[!UICONTROL 게시]** - 기본적으로 Adobe Dynamic Media Classic은 이전에 게시되지 않은 새 자산(마지막 게시 이후 새로 만들기 옵션)만 게시합니다. 그러나 다음을 선택할 수 있습니다. **[!UICONTROL 전체 게시]** 마지막으로 게시된 이후 업데이트 또는 변경된 에셋도 게시합니다. 선택 **[!UICONTROL 검색 데이터를 포함한 전체]** eCatalog를 게시하고 독자가 키워드로 검색할 수 있도록 하려는 경우.

* **[!UICONTROL 다음으로 작업 실행]** - 목록에서 사용자 이름을 선택합니다. 작업 페이지에서 사용자 이름을 기준으로 작업을 정렬할 수 있습니다. 이름을 선택하여 게시 작업을 사용자에 연결합니다.

**[!UICONTROL HTTP 알림]** - 후속 게시 작업을 트리거할 URL을 입력합니다.

다음을 참조하십시오 [업로드 또는 게시 작업을 트리거로 사용](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger).)

## 게시 작업 취소 {#canceling-a-publish-job}

진행 중인 게시 작업을 취소할 수 있습니다. 관리자는 회사 작업 페이지에서 진행 중인 게시 작업을 취소할 수도 있습니다.

게시 작업을 취소하려면 [작업] 페이지로 이동하여 **[!UICONTROL 취소]**. 작업 페이지의 [예약됨] 탭에서 작업의 [활성] 열에 있는 확인란을 선택 취소하거나 선택하여 작업을 일시 중단하거나 재시작할 수 있습니다.

>[!NOTE]
>
>게시 작업을 취소하면 작업이 안전하게 중지될 수 있는 지점에 도달할 때까지 해당 상태가 &quot;중지 중&quot;으로 변경됩니다. 게시 작업이 데이터베이스에서 데이터를 가져오는 중인 경우 게시 작업을 중지하는 데 시간이 걸릴 수 있습니다.

## 자산 수동 게시 {#manually-publishing-assets}

게시 작업을 만드는 대신 개별 자산을 수동으로 게시할 수 있습니다. 이미지 세트나 적응형 비디오 집합과 같은 세트를 게시하면, 세트(또는 &quot;상위&quot;)와 해당 세트 내의 모든 구성원(또는 &quot;하위&quot;)이 게시됩니다.

게시되지 않은 에셋은 에셋 이름 왼쪽에 슬래시가 있는 회색 원형 아이콘(게시되지 않은 상태)으로 사용자 인터페이스에 표시됩니다. 자산이 게시되면 이 아이콘은 녹색으로 변하고 중앙에 흰색 확인 표시(게시된 상태)가 생깁니다.

**수동 자산 게시:**

1. 다음 중 하나를 수행하십시오.

   * [격자 보기], [목록 보기] 또는 [상세 보기]에서 표준 파일 선택 방법을 사용하여 자산을 하나 이상 선택합니다.

      전역 탐색 모음에서 다음 위치로 이동합니다. **[!UICONTROL 파일]** > **[!UICONTROL 게시]**.

   * 그리드 보기, 목록 보기 또는 세부 사항 보기에서 에셋 이름 왼쪽에 슬래시가 있는 회색 원형 아이콘을 선택합니다.

## 수동으로 자산 게시 취소 {#manually-unpublishing-assets}

개별 자산을 수동 게시 취소할 수 있습니다. 견본 집합이나 전자 카탈로그와 같은 세트의 게시를 취소하면, 세트(또는 &quot;상위&quot;) 자체는 게시 취소 상태가 됩니다. 하지만 삭제된 세트 내의 구성원(또는 &quot;하위&quot;)은 휴지통으로 이동하지 않고, 각각 기존의 게시된 상태나 게시 취소된 상태를 유지합니다.

게시된 자산은 사용자 인터페이스에서 자산 이름의 왼쪽에, 중앙에 흰색 확인 표시가 있는 둥근 녹색 아이콘(게시된 상태)으로 표시됩니다. 에셋의 게시가 취소되면 아이콘이 회색으로 바뀌고 그 사이에 슬래시가 표시됩니다(게시되지 않은 상태).

**수동 자산 게시 취소:**

1. 다음 중 하나를 수행하십시오.

   * 그리드 보기, 목록 보기 또는 세부 사항 보기에서 게시된 에셋을 하나 이상 선택합니다.

      전역 탐색 모음에서 다음 위치로 이동합니다. **[!UICONTROL 파일]** > **[!UICONTROL 게시 취소]**.

   * 그리드 보기, 목록 보기 또는 세부 사항 보기에서 에셋 이름의 왼쪽에 있는 둥근 녹색 확인 표시 아이콘을 선택합니다.

## 에셋의 게시 내역 가져오기 {#getting-an-asset-s-publish-history}

에셋이 마지막으로 게시된 날짜가 패널 상단에 세부 사항 보기에 표시됩니다. 세부 사항 보기의 내역 및 게시된 서버 패널을 열어 게시 내역에 대한 자세한 내용을 볼 수 있습니다. 여기서 자산이 게시된 시기와 자산이 게시된 서버를 확인할 수 있습니다.

## 다시 게시한 자산 및 CDN 지연 {#republished-assets-and-cdn-delays}

Adobe Dynamic Media Classic 자산은 CDN(content delivery network)에서 배포됩니다. CDN은 컨텐츠, 특히 큰 미디어 컨텐츠를 최종 사용자에게 제공하기 위해 투명하게 조정되는, 네트워크로 연결된 컴퓨터 서버 시스템입니다. CDN 시스템에서는 웹 컨텐츠가 인터넷을 통해 웹 캐시에 저장됩니다(경계 캐시 네트워크라고 함). 웹 콘텐츠는 더 빠른 전달을 위해 웹 캐시에서 최종 사용자에게 전달됩니다.

웹 페이지를 처음 다운로드하면 자산이 CDN 웹 캐시 서버로 제공됩니다. 다음에 동일한 영역의 다른 사용자가 웹 페이지에 액세스할 때 캐시된 동일한 컨텐츠가 더 빨리 제공될 수 있도록 이 서버에 자산이 저장됩니다. 최종 사용자에 더 가까운 곳에 있기 때문에 컨텐츠가 더 빨리 제공됩니다. CDN을 사용하면 웹 페이지가 더 빨리 표시됩니다. 매번 컨텐츠가 중앙 서버에서 제공되지 않고 경계 캐시 네트워크에서 제공되므로 중앙 서버의 대역폭 요구가 감소합니다.

새로 게시된 Adobe Dynamic Media Classic 콘텐츠는 최종 사용자가 즉시 사용할 수 있으며 에지 캐시 네트워크를 빠르게 채웁니다. 그러나 새로 다시 게시한 컨텐츠(이전에 이미지 서버에 게시한 이미지와 동일한 이름을 가진 이미지)는 최대 10시간 동안 CDN에서 업데이트되지 않습니다. 대신 최종 사용자에게 CDN 네트워크의 웹 캐시에 있는 내용이 표시됩니다. 이러한 이유로 Adobe Dynamic Media Classic에서 다시 게시한 에셋은 10시간 동안 최종 사용자에게 표시되지 않습니다.

새로 다시 게시한 이미지 자산을 10시간 지연보다 빨리 사용할 수 있게 하려면 CDN의 웹 캐시를 비울 수 있습니다. 이러한 웹 캐시를 비우면 CDN 웹 캐시에서 이전 컨텐츠가 제거되고 최근에 게시한 자산으로 바뀝니다.

캐시를 플러시하려면 전역 탐색 모음에서 다음 위치로 이동하십시오. **[!UICONTROL 파일]** > **[!UICONTROL CDN 무효화]**. 선택한 모든 파일이 캐시에서 제거됩니다. 게시 가능한 자산이 없는 경우 또는 회사 관리자가 아닌 경우에는 [CDN에서 제거] 선택 사항을 사용할 수 없습니다.

>[!MORELIKETHIS]
>
>* [작업 파일 확인](checking-job-files.md)
>* [반복 작업 편집, 삭제, 일시 중지 및 다시 시작](checking-job-files.md#editing-deleting-pausing-and-resuming-recurring-jobs)

