---
title: Publish 파일
description: Dynamic Media 이미지 서버에 자산을 게시하는 방법을 알아봅니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 91b73a09-c5b5-4001-b36f-6bebe65717ff
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '1674'
ht-degree: 21%

---

# Publish 파일{#publishing-files}

자산을 Dynamic Media 이미지 서버에 게시합니다. 자산을 한 번만 게시하거나 Adobe Dynamic Media Classic에서 반복 일정에 자산을 게시하도록 예약할 수 있습니다. 자산이 게시되면 제공할 수 있습니다. Adobe Dynamic Media Classic에서 URL 호출을 복사하여 웹 사이트 또는 애플리케이션에 추가할 수 있습니다.

Adobe Dynamic Media Classic은 이제 HTTP/2를 통해 모든 이미지 및 비디오의 전달을 지원합니다. 즉, 이미지 또는 비디오에 대한 게시된 URL 또는 포함 코드는 호스팅된 에셋을 수락하는 모든 애플리케이션과 통합할 수 있습니다. 게시된 해당 자산은 HTTP/2 프로토콜을 사용하여 전달됩니다. 이 전달 방법은 브라우저와 서버의 통신 방식을 개선하여 모든 Adobe Dynamic Media Classic 에셋의 응답 및 로드 시간을 향상시킵니다. [HTTP2 콘텐츠 배달 FAQ](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/dynamic/http2)를 참조하십시오.

## 업로드 후 게시 {#publish-after-uploading}

게시 또는 게시 취소 상태의 자산. 기본적으로 Adobe Dynamic Media Classic에 업로드하는 모든 자산은 게시용으로 자동으로 표시됩니다.

자세한 내용은 [빠른 Publish 알림 PDF](/help/using/assets/rendering-instant-publish-notification.pdf)를 참조하세요.

게시할 자산을 표시하려면 다음 기술을 사용하십시오.

* **[!UICONTROL 업로드 후 Publish]**: 맨 아래의 [업로드] 페이지에서 **[!UICONTROL 업로드 후 Publish]**&#x200B;을 선택합니다. 기본값은 선택된 상태입니다.

* **[!UICONTROL 업로드 후 Publish]**: [작업 옵션] 대화 상자에서 **[!UICONTROL 업로드 후 Publish]**&#x200B;을 선택합니다. 기본값은 선택된 상태입니다.

일부 &quot;하위&quot; 자산은 상위 자산을 게시로 표시할 때 자동으로 게시로 표시됩니다. 이 표에는 게시로 표시된 하위 자산이 자동으로 나열됩니다.

| 상위(그룹) 항목 | 하위(구성원) 항목 |
| --- | --- |
| 이미지 집합 | 세트 내 이미지. |
| 견본 집합 | 세트 내 견본. |
| 회전 집합 | 세트 내 이미지. |
| 템플릿 | 템플릿 파일, 페이지 및 이미지 |

파생 이미지는 상위 이미지가 게시되는 동안 자동으로 게시용으로 표시됩니다. 파생 이미지에는 이미지 편집 선택 사항으로 조정한 이미지도 포함됩니다. 기본 및 파생 아래의 세부 사항 보기에서 이러한 파생된 이미지를 볼 수 있습니다.

## 게시 작업 만들기 {#creating-a-publish-job}

Adobe Dynamic Media Classic 서버에 업로드했지만 아직 자동으로 게시하지 않으려는 자산을 게시하기 위한 게시 작업을 만듭니다. 1회 게시 작업을 수행하거나 작업이 정기적으로 반복되도록 예약할 수 있습니다. Adobe Dynamic Media Classic은 특정 서버에 게시하기 위한 고급 게시 옵션과 이미 게시된 에셋을 다시 게시하기 위한 옵션을 제공합니다.

**게시 작업을 만들려면:**

1. 전역 탐색 모음에서 **[!UICONTROL Publish]**&#x200B;을(를) 선택합니다.
1. 게시 대화 상자에서 1회 게시 작업을 원하는지 반복 게시 작업을 원하는지 선택합니다.

   [1회 게시 작업 만들기](publishing-files.md#creating_a_one_time_publish_job) 및 [반복 게시 작업 만들기](publishing-files.md#creating_a_recurring_publish_job)를 참조하십시오.

1. 작업 이름을 입력합니다.
1. 선택적으로 [고급] 선택 사항을 표시하고 이러한 선택 사항을 선택합니다. 

   [[고급] 게시 선택 사항](publishing-files.md#advanced_publish_options)을 참조하십시오.

1. **[!UICONTROL Publish 제출]**&#x200B;을 선택합니다.

Adobe Dynamic Media Classic은 작업 페이지에서 게시 작업을 추적합니다. 이 페이지에서 게시 작업을 검토할 수 있습니다.

>[!NOTE]
>
>다시 게시한 Assets(이전에 게시한 적이 있음)는 CDN(content delivery network)의 웹 캐싱 메커니즘 때문에 웹 사이트에 즉시 표시되지 않습니다. [다시 게시한 자산 및 CDN 지연](publishing-files.md#republished_assets_and_cdn_delays)을 참조하십시오.

### 1회 게시 작업 만들기 {#creating-a-one-time-publish-job}

게시 페이지에서 **[!UICONTROL 1회]** 옵션을 선택하여 1회 게시 작업을 만듭니다.

게시 작업을 나중에 수행하려면 게시 페이지에서 **[!UICONTROL 한 번]**&#x200B;을 선택하십시오. 드롭다운 목록에서 **[!UICONTROL 나중에 예약]**&#x200B;을 선택합니다. [달력] 및 [시간] 슬라이더를 사용하여 게시 작업을 실행할 날짜와 시간을 선택합니다.

### 반복 게시 작업 만들기 {#creating-a-recurring-publish-job}

게시 페이지에서 **[!UICONTROL 반복]**&#x200B;을(를) 선택하여 반복 게시 작업을 만듭니다.

그런 다음 **[!UICONTROL 일별]**, **[!UICONTROL 주별]**, **[!UICONTROL 월별]** 또는 **[!UICONTROL 사용자 지정]**&#x200B;의 반복 옵션을 선택한 다음 게시 작업을 다시 실행할 시기를 지정하십시오. Adobe Dynamic Media Classic은 반복 게시 작업 일정을 조정하는 캘린더 도구를 제공합니다. **[!UICONTROL 사용자 지정]** 옵션을 선택하고 규칙 텍스트 필드에 규칙을 입력하여 사용자 지정 작업 간격을 설명할 수 있습니다.

[사용자 지정 업로드 또는 게시 작업 시간 간격 만들기](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval)를 참조하십시오.

>[!NOTE]
>
>작업 페이지에 반복 게시(및 업로드) 작업이 나열됩니다. 작업 페이지의 [예약됨] 탭으로 이동하여 예약된 작업을 편집하거나 삭제할 수 있습니다.

### [고급] 게시 선택 사항 {#advanced-publish-options}

게시 페이지에 고급 옵션을 표시하고 게시 작업을 처리하기 위해 다음 옵션을 선택할 수 있습니다.

* **[!UICONTROL Publish 받는 사람]**: 에셋을 특정 서버에만 게시하려면 서버 형식을 선택하십시오.

* **[!UICONTROL Publish]**: 기본적으로 Adobe Dynamic Media Classic은 새로운 에셋만 게시하며 이전에 게시되지 않았습니다(마지막 Publish 이후 새로운 옵션). 그러나 **[!UICONTROL 전체 Publish]**&#x200B;을(를) 선택하여 마지막으로 게시된 이후 업데이트 또는 변경된 에셋을 게시할 수도 있습니다. eCatalog를 게시하고 독자가 키워드로 검색할 수 있도록 하려면 **[!UICONTROL 검색 데이터를 포함한 전체]**&#x200B;을(를) 선택하십시오.

* **[!UICONTROL 다음으로 작업 실행]**: 목록에서 사용자 이름을 선택합니다. 작업 페이지에서 사용자 이름을 기준으로 작업을 정렬할 수 있습니다. 이름을 선택하여 게시 작업을 사용자와 연관시킵니다.

**[!UICONTROL HTTP 알림]**: 후속 게시 작업을 트리거할 URL을 입력하십시오.

[업로드 또는 게시 작업을 트리거로 사용](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)을 참조하십시오.)

## 게시 작업 취소 {#canceling-a-publish-job}

진행 중인 게시 작업을 취소할 수 있습니다. 관리자는 회사 작업 페이지에서 진행 중인 게시 작업을 취소할 수도 있습니다.

게시 작업을 취소하려면 [작업] 페이지로 이동하여 **[!UICONTROL 취소]**&#x200B;를 선택하십시오. 작업 페이지의 [일정이 잡힘] 탭에서는 작업의 [활성] 열에서 확인란을 선택 취소하거나 선택하여 작업을 일시 중지하거나 다시 시작할 수 있습니다.

>[!NOTE]
>
>게시 작업을 취소하면 작업이 안전하게 중지될 수 있는 지점에 도달할 때까지 상태가 &quot;중지 중&quot;으로 변경됩니다. 데이터베이스에서 데이터를 가져오는 중인 경우 게시 작업을 중지하는 데 시간이 걸릴 수 있습니다.

## Publish assets 수동으로 {#manually-publishing-assets}

게시 작업을 만드는 대신 개별 자산을 수동으로 게시할 수 있습니다. 이미지 세트 또는 응용 비디오 세트와 같은 세트를 게시하면 해당 세트 내의 세트(또는 &quot;상위&quot;) 및 모든 멤버(또는 &quot;하위&quot;)가 게시됩니다.

게시되지 않은 에셋은 에셋 이름 왼쪽에 슬래시가 있는 회색 원형 아이콘(게시되지 않은 상태)으로 사용자 인터페이스에 표시됩니다. 자산이 게시되면 이 아이콘은 녹색으로 변하고 중앙에 흰색 확인 표시(게시된 상태)가 생깁니다.

**자산을 수동으로 게시하려면:**

1. 다음 중 하나를 수행하십시오.

   * [격자 보기], [목록 보기] 또는 [상세 보기]에서 표준 파일 선택 방법을 사용하여 자산을 하나 이상 선택합니다.

     전역 탐색 모음에서 **[!UICONTROL 파일]** > **[!UICONTROL Publish]**(으)로 이동합니다.

   * 그리드 보기, 목록 보기 또는 세부 사항 보기에서 에셋 이름 왼쪽에 슬래시가 있는 회색의 라운드 아이콘을 선택합니다.

## 수동으로 자산 게시 취소 {#manually-unpublishing-assets}

개별 자산을 수동 게시 취소할 수 있습니다. 견본 세트 또는 eCatalog와 같은 세트를 게시 취소하면 세트(또는 &quot;상위&quot;) 자체가 게시 취소 상태로 전환됩니다. 그러나 해당 집합 내의 멤버(또는 &quot;하위&quot;)는 영향을 받지 않습니다. 대신 각 멤버는 기존의 게시 또는 게시 취소 상태를 유지합니다.

게시된 에셋은 에셋 이름 왼쪽에 중앙(게시된 상태)에 흰색 확인 표시가 있는 둥근 녹색 아이콘으로 사용자 인터페이스에 표시됩니다. 에셋의 게시가 취소되면 아이콘이 회색으로 바뀌고 그 사이에 슬래시가 표시됩니다(게시되지 않은 상태).

**자산 게시를 수동으로 취소하려면:**

1. 다음 중 하나를 수행하십시오.

   * 그리드 보기, 목록 보기 또는 세부 사항 보기에서 게시된 에셋을 하나 이상 선택합니다.

     전역 탐색 모음에서 **[!UICONTROL 파일]** > **[!UICONTROL 게시 취소]**(으)로 이동합니다.

   * 그리드 보기, 목록 보기 또는 세부 사항 보기에서 에셋 이름의 왼쪽에 있는 둥근 녹색 확인 표시 아이콘을 선택합니다.

## 에셋의 게시 내역 가져오기 {#getting-an-asset-s-publish-history}

에셋이 마지막으로 게시된 날짜가 패널 상단에 세부 사항 보기에 표시됩니다. 세부 사항 보기의 내역 및 게시된 서버 패널을 열어 게시 내역에 대한 자세한 내용을 볼 수 있습니다. 여기서 자산이 게시된 시기와 자산이 게시된 서버를 확인할 수 있습니다.

## 다시 게시한 자산 및 CDN 지연 {#republished-assets-and-cdn-delays}

Adobe Dynamic Media Classic 자산은 CDN(content delivery network)에서 배포됩니다. CDN은 컨텐츠, 특히 큰 미디어 컨텐츠를 최종 사용자에게 제공하기 위해 투명하게 조정되는, 네트워크로 연결된 컴퓨터 서버 시스템입니다. CDN 시스템에서 웹 컨텐츠는 인터넷(에지 캐시 네트워크라고 함)의 웹 캐시에 저장됩니다. 웹 콘텐츠는 더 빠른 전달을 위해 웹 캐시에서 최종 사용자에게 전달됩니다.

누군가 웹 페이지를 처음 다운로드하면 자산이 CDN 웹 캐시 서버로 전달됩니다. 이 서버는 동일한 영역의 누군가가 웹 페이지에 다음에 액세스할 때 캐시된 동일한 콘텐츠가 더 빨리 전달되도록 해당 콘텐츠를 저장합니다. 최종 사용자에 더 가까운 곳에 있기 때문에 컨텐츠가 더 빨리 제공됩니다. CDN은 웹 페이지 표시 속도를 향상시킵니다. 매번 컨텐츠가 중앙 서버에서 제공되지 않고 경계 캐시 네트워크에서 제공되므로 중앙 서버의 대역폭 요구가 감소합니다.

새로 게시된 Adobe Dynamic Media Classic 콘텐츠는 최종 사용자가 즉시 사용할 수 있으며 에지 캐시 네트워크를 빠르게 채웁니다. 그러나 새로 다시 게시된 콘텐츠, 즉 이미지 서버에 이전에 게시된 이미지와 이름이 같은 이미지는 최대 10시간 동안 CDN에서 업데이트되지 않습니다. 대신 최종 사용자는 CDN 네트워크의 웹 캐시에 있는 를 확인합니다. 이러한 이유로 Adobe Dynamic Media Classic에서 다시 게시한 에셋은 10시간 동안 최종 사용자에게 표시되지 않습니다.

새로 다시 게시된 이미지 자산을 10시간 지연보다 빨리 사용할 수 있도록 하려면 CDN에서 웹 캐시를 플러시할 수 있습니다. 이러한 웹 캐시를 플러시하면 CDN 웹 캐시에서 이전 콘텐츠가 제거되고 가장 최근에 게시된 자산으로 교체됩니다.

캐시를 플러시하려면 전역 탐색 모음에서 **[!UICONTROL 파일]** > **[!UICONTROL CDN 무효화]**(으)로 이동하십시오. 선택한 모든 파일이 캐시에서 제거됩니다. 게시 가능한 자산이 없는 경우 또는 회사 관리자가 아닌 경우에는 [CDN에서 제거] 선택 사항을 사용할 수 없습니다.

>[!MORELIKETHIS]
>
>* [작업 파일 확인](checking-job-files.md)
>* [반복 작업 편집, 삭제, 일시 중지 및 다시 시작](checking-job-files.md#editing-deleting-pausing-and-resuming-recurring-jobs)
