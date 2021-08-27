---
title: Adobe Analytics 보고서 구성
description: Adobe Dynamic Media Classic에서 Adobe Analytics 보고서를 구성하는 방법을 알아봅니다.
uuid: bf210f68-dcb0-4e86-be04-0a8b2117ef2a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: f4c8c2b3-cc95-416f-9a5d-da81c231dfc2
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: d9fda3b8-7da8-4a30-a5f8-9bb34ec1b43d
source-git-commit: 44045daa35052f01a26c67e0b2a0fb1405c53292
workflow-type: tm+mt
source-wordcount: '1228'
ht-degree: 30%

---

# Adobe Analytics 보고서 구성{#configuring-adobe-analytics-reports}

Adobe Analytics 보고서에 포함할 정보를 Adobe Analytics에 알려 주려면, Adobe Analytics 구성 화면으로 이동합니다. 보고서를 구성한 후 이 화면에는 원하는 각 뷰어 이벤트에 대한 해당 Adobe Analytics 변수와 Dynamic Media Classic Adobe 변수가 표시됩니다. 이러한 뷰어 이벤트-Adobe Analytics 변수-Adobe Dynamic Media Classic 변수 조합은 보고되는 정보를 결정합니다.

뷰어 이벤트를 변수와 연결 하는 것 외에, Adobe Analytics 구성 화면에서는 뷰어 이벤트를 활성화, 편집 및 삭제하는 도구를 제공합니다.

>[!NOTE]
>
>Adobe Analytics 내에서 Adobe Analytics 보고서 설정을 변경할 때마다 Adobe Dynamic Media Classic 내에서 Adobe Analytics에 다시 로그온하고 Adobe Analytics 구성 설정을 다시 저장한 다음 다시 게시해야 합니다.

[Adobe Analytics에 로그인](log-analytics.md#log_in_to_adobe_analytics)을 참조하십시오.

[구성 정보 게시](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information)를 참조하십시오.

## Dynamic Media Classic 뷰어 이벤트 및 변수에 Adobe Analytics 변수 할당 {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

Adobe Analytics 구성 화면을 사용하여 뷰어 이벤트를 Adobe Analytics 변수와 연결하고 Dynamic Media Classic 변수를 Adobe 할 수 있습니다. 각 뷰어 이벤트에 대해 하나의 Adobe Analytics 변수와 하나의 Adobe Dynamic Media Classic 변수를 선택합니다. Adobe Analytics 구성 화면을 여는 방법에 대한 지침은 [Adobe Analytics에 로그인](log-analytics.md#log_in_to_adobe_analytics)을 참조하십시오.

**Dynamic Media Classic 뷰어 이벤트 및 변수에 Adobe Analytics 변수를 할당하려면 다음을 수행하십시오.**

1. Adobe Dynamic Media Classic 내에서 Adobe Analytics에 로그인하고 보고서 세트를 선택한 후 Adobe Analytics 구성 페이지의 오른쪽 테이블 열에서 **[!UICONTROL 활성화]**&#x200B;를 선택하여 뷰어 이벤트를 활성화합니다.
1. 변수 열 아래에 원하는 뷰어 이벤트에 대한 화살표 단추를 선택하여 변수 쌍 선택기를 표시합니다.

   [뷰어 이벤트](configuring-analytics-reports.md#viewer_events)를 참조하십시오.

1. Adobe Dynamic Media Classic 변수를 추가합니다.

   [Dynamic Media Classic 변수 Adobe](configuring-analytics-reports.md#scene7_variables)를 참조하십시오.

1. Adobe Analytics 변수를 추가합니다.
1. (선택 사항) 다른 변수 쌍을 추가하려면 **[!UICONTROL 추가]**&#x200B;를 선택합니다.
1. **[!UICONTROL 저장]**&#x200B;을 선택합니다.

   **[!UICONTROL 저장]**&#x200B;을 선택하면 뷰어 이벤트, 해당 Adobe Analytics 변수 및 해당 Adobe Dynamic Media Classic 변수가 Adobe Analytics 구성 화면에 나열됩니다.

1. 오른쪽 아래 모서리에서 **[!UICONTROL 닫기]**&#x200B;를 선택합니다.
1. **[!UICONTROL 게시]** > **[!UICONTROL 게시]**&#x200B;로 이동하여 이미지 제공 게시를 실행합니다.

   뷰어에 포함된 정보를 Adobe Dynamic Media Classic 서버에서 사용할 수 있도록 게시해야 합니다.

### 뷰어 이벤트 {#viewer-events}

뷰어 이벤트는 사용자가 Dynamic Media Classic 뷰어로 수행하는 작업을 설명합니다. 사용자가 축소판 선택 또는 비디오 시작 또는 중지 등의 특정 작업을 시작하면 뷰어는 해당 이벤트와 연관된 데이터와 함께 이벤트를 웹 페이지에 &quot;브로드캐스트&quot;합니다.

다음 표에서는 [Adobe Analytics 구성] 화면에 추가할 수 있는 뷰어 이벤트에 대해 설명합니다.

| 뷰어 이벤트 | HTML5 뷰어 플랫폼 지원 및 뷰어 | 설명 |
| --- | --- | --- |
| LOAD | **X**(전자 카탈로그, 플라이아웃, 회전 집합, 비디오, 확대/축소) | 사용자가 뷰어를 시작할 때 |
| PAGE | **X**(전자 카탈로그) | eCatalog에서 사용자가 페이지를 반환하는 경우 타깃팅된 확대/축소 뷰어에서 사용자가 다른 대상 또는 색상 견본을 선택하면 됩니다. |
| SWAP | **X**(전자 카탈로그, 플라이아웃, 회전 집합, 비디오, 확대/축소) | 사용자가 다른 축소판을 선택하여 다른 이미지를 볼 때 |
| 항목 | **X**(전자 카탈로그) | 롤오버가 정의된 이미지 맵을 지원하는 뷰어에서는 사용자가 포인터를 이미지 맵 위로 이동하여 롤오버 텍스트를 읽을 때 발생합니다. |
| HREF | **X**(전자 카탈로그) | 이미지 맵을 지원하는 뷰어에서 사용자가 이미지 맵에서 URL을 선택할 때. |
| TARGET |  | 타깃팅된 확대/축소 뷰어에서 사용자가 이미지의 일부로 확대/축소 대상을 선택하면 됩니다. |
| SEARCH |  | eCatalog에서는 사용자가 단어 검색을 수행할 때 발생합니다. |
| PLAY | **X**(비디오) | 비디오 뷰어에서 사용자가 재생 을 선택하여 비디오 재생을 시작할 때.<br><br>**참고:**  Adobe Analytics 하트비트 기반 비디오 보고를 사용하는 경우, Adobe Dynamic Media Classic에서 Adobe Analytics을 구성할 때 이 뷰어 이벤트에 변수를 매핑할 필요가 없습니다. 비디오 하트비트는 곧바로 사용할 수 있는 Adobe Dynamic Media Classic HTML5 비디오 및 MixedMedia 뷰어에서 작동합니다. 비디오 플레이어는 Adobe Analytics 비디오 보고서 내에서 보기 위한 추적 데이터를 생성합니다. [Adobe Analytics 비디오 보고서 활성화](enabling-analytics-video-reports.md)를 참조하십시오. |
| PAUSE | **X**(비디오) | 비디오 뷰어에서 사용자가 **[!UICONTROL 일시 중지]**&#x200B;를 선택하여 비디오를 고정하면&#x200B;<br><br>**참고:**  Adobe Analytics 하트비트 기반 비디오 보고를 사용하는 경우, Adobe Dynamic Media Classic에서 Adobe Analytics을 구성할 때 이 뷰어 이벤트에 변수를 매핑할 필요가 없습니다. 비디오 하트비트는 곧바로 사용할 수 있는 Adobe Dynamic Media Classic HTML5 비디오 및 MixedMedia 뷰어에서 작동합니다. 비디오 플레이어는 Adobe Analytics 비디오 보고서 내에서 보기 위한 추적 데이터를 생성합니다. [Adobe Analytics 비디오 보고서 활성화](enabling-analytics-video-reports.md)를 참조하십시오. |
| STOP | **X**(비디오) | 비디오 뷰어에서 사용자가 **[!UICONTROL Stop]**&#x200B;을 선택하여 비디오 재생을 중지할 때&#x200B;<br><br>**참고:**  Adobe Analytics 하트비트 기반 비디오 보고를 사용하는 경우, Adobe Dynamic Media Classic에서 Adobe Analytics을 구성할 때 이 뷰어 이벤트에 변수를 매핑할 필요가 없습니다. 비디오 하트비트는 곧바로 사용할 수 있는 Adobe Dynamic Media Classic HTML5 비디오 및 MixedMedia 뷰어에서 작동합니다. 비디오 플레이어는 Adobe Analytics 비디오 보고서 내에서 보기 위한 추적 데이터를 생성합니다. [Adobe Analytics 비디오 보고서 활성화](enabling-analytics-video-reports.md)를 참조하십시오. |
| MILESTONE | **X**  (비디오) | 비디오 뷰어에서는 사용자가 비디오를 0, 25, 50, 75 또는 100% 시청할 때 중대한 이벤트가 생성됩니다.<br><br>**참고:**  Adobe Analytics 하트비트 기반 비디오 보고를 사용하는 경우, Adobe Dynamic Media Classic에서 Adobe Analytics을 구성할 때 이 뷰어 이벤트에 변수를 매핑할 필요가 없습니다. 비디오 하트비트는 곧바로 사용할 수 있는 Adobe Dynamic Media Classic HTML5 비디오 및 MixedMedia 뷰어에서 작동합니다. 비디오 플레이어는 Adobe Analytics 비디오 보고서 내에서 보기 위한 추적 데이터를 생성합니다. [Adobe Analytics 비디오 보고서 활성화](enabling-analytics-video-reports.md)를 참조하십시오. |
| 견본 | **X**(플라이아웃, 확대/축소) | 이 뷰어 이벤트는 Adobe Dynamic Media Classic의 PAGE 뷰어 이벤트에 매핑됩니다. |
| 확대/축소 | **X**(전자 카탈로그, 회전 집합, 확대/축소) | Adobe Analytics에서 추적하지 않습니다. |
| 패닝 | **X**(전자 카탈로그, 회전 집합, 확대/축소) | Adobe Analytics에서 추적하지 않습니다. |
| 회전 | **X**(회전 집합) | Adobe Analytics에서 추적하지 않습니다. |

### Dynamic Media Classic 변수 Adobe {#scene-variables}

Adobe Analytics 구성 화면의 각 뷰어 이벤트에 대해 Adobe Analytics 변수와 *Adobe Dynamic Media Classic 변수*&#x200B;를 선택합니다. Adobe Dynamic Media Classic 변수는 보고서에 사용할 수 있는 데이터를 나타냅니다. 예를 들어 `searchTerm` 변수는 eCatalog 검색에 사용되는 키워드를 나열합니다.

다음 표에서는 Dynamic Media Classic Adobe 변수에 대해 설명합니다.

| Dynamic Media Classic 변수 Adobe | 설명 |
| --- | --- |
| asset | Adobe Dynamic Media Classic 자산 ID 또는 비디오 경로 파일. |
| viewerId | 각기 다른 뷰어 유형에 지정된 임의 번호입니다. |
| pageLabel | eCatalog에서는 뷰어에 표시되는 페이지입니다. |
| 레이블 | 레이블 값(문자열)입니다. |
| frame | 이미지 집합의 페이지 또는 페이지 참조입니다. |
| rollover_keyRaw | 처리된 부분만이 아니라 전체 HREF 값입니다. |
| rollover_keyProc | 이미지 맵에 참조된 항목의 ID입니다(href 및 항목 이벤트에 유효함). |
| searchTerm | eCatalog 검색에 사용되는 단어입니다. |
| timeStamp | 비디오 뷰어에서 선택한 재생, 중지 및 일시 중단입니다. |
| progress | 완료된 중대한 이벤트의 비율입니다. |
| targetId | ID 값(숫자)입니다. |

## 뷰어 이벤트 활성화, 편집 및 삭제 {#activating-editing-and-deleting-viewer-events}

[Adobe Analytics 구성] 화면에서 뷰어 이벤트를 활성화, 편집 및 삭제할 수 있습니다.

* **활성화**  -  **** 활성화 또는 비활성화하려면  **** 을 선택합니다. 선택한 뷰어 이벤트를 비활성화하려면 를 선택합니다.

* **편집**  - 뷰어 이벤트를 선택하고  **[!UICONTROL 보기/]** 변수 편집 회색 단추를 선택합니다. Adobe Dynamic Media Classic 변수 및 Adobe Analytics 변수 드롭다운 목록에서 각 목록에서 다른 변수를 선택합니다. 자세한 내용은 [Adobe Analytics 변수를 Adobe Dynamic Media Classic 뷰어 이벤트 및 변수에 지정](#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables)을 참조하십시오.

* **삭제**  - 뷰어 이벤트를 선택하고 보기/ **[!UICONTROL 편집]** 변수 회색 단추를 선택합니다. **[!UICONTROL 삭제]**&#x200B;를 선택합니다.
