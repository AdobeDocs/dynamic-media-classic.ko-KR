---
title: eCatalog 뷰어 사전 설정 지정
seo-title: eCatalog 뷰어 사전 설정 지정
description: 널
seo-description: Ecatalog 뷰어 사전 설정을 설정하는 방법을 알아봅니다.
uuid: ACA 66 BC 5-8491-4 D 81-9 A 06-1 D 3531860 A 14
contentOwner: 관리
content-type: 참조
products: sg_ Experiencemanager/dynamic-media-scene -7
discoiquuid: 6 c 123 f 85-3 bc 4-4392-a 7 fb -55618127 c 65 e
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# eCatalog 뷰어 사전 설정 지정{#setting-up-ecatalog-viewer-presets}

eCatalog 뷰어 사전 설정은 eCatalog 뷰어의 스타일, 동작 및 모양을 결정합니다. Dynamic Media Classic는 ecatalog 뷰어 사전 설정을 제공하며, 관리자인 경우 고유한 ecatalog 뷰어 사전 설정을 만들 수 있습니다.

새 사전 설정을 만들려면 처음부터 시작하거나 Dynamic Media Classic에서 제공하는 ecatalog 뷰어 사전 설정에서 시작하여 새 이름으로 저장할 수 있습니다. 고유한 eCatalog 뷰어 사전 설정을 만들어 회사 색상으로 인쇄물을 표시하고 톤을 설정할 수 있습니다.

eCatalog 뷰어 사전 설정은 페이지 간 이동, 확대/축소, 검색 및 "스킨" 선택을 위한 다양한 설정을 제공합니다. 이러한 컨트롤의 모양과 뷰어 자체의 모양은 eCatalog 뷰어 사전 설정의 선택 항목에 따라 달라집니다.

eCatalog 뷰어 사전 설정을 만들려면 다음 단계를 수행합니다(관리자여야 함).

1. **[설정]** &gt; **[뷰어 사전 설정]**&#x200B;을 클릭합니다.
1. [뷰어 사전 설정] 화면에서 새로 시작하거나 기존 eCatalog 뷰어 사전 설정에서 시작하여 eCatalog 뷰어 사전 설정을 만듭니다.

   **Ecatalog 뷰어 사전 설정** 만들기를 클릭합니다. In the Add Viewer Preset dialog box, choose a platform, choose eCatalog Viewer, then click **Add**.

   **Ecatalog 뷰어 사전 설정** 편집 ecatalog 뷰어 사전 설정을 선택한 다음 편집을 클릭합니다. Click **Save As** after you finish creating the preset.

1. [뷰어 구성] 화면에서 eCatalog 뷰어 사전 설정의 이름을 입력합니다.
1. [뷰어 구성] 화면에서 원하는 선택 사항을 설정합니다.

   해당 설명을 보려면 선택 사항에 인접한 [정보 팁] 아이콘 을 클릭합니다.

   설정을 업데이트하고 변경하면 [미리 보기] 화면에 뷰어가 표시됩니다.

1. (선택 사항) [정보 패널 설정]의 [정보 서버 URL] 선택 사항에는 뷰어가 대체하는 다음 특수 토큰이 포함될 수 있습니다.

   | 토큰 | 대체 값 | 주의 |
   |--- |--- |--- |
   | `$1$` | rollover_key 값 | The item identifier from the `<area>` element of the map. |
   | `$2$` | frame | 이미지 집합에 현재 표시된 프레임의 일련번호입니다. |
   | `$3$` | imageroot | 이미지 명령에 지정된 첫 번째 항목의 첫 번째 경로 요소(일반적으로 이미지 집합을 지정하는 카탈로그 항목의 이미지 카탈로그 ID)입니다. |

1. (선택 사항) [응답 템플릿] 설정에서 [응답 템플릿] 상자에 Dynamic Media Classic에서 이미지 맵에 대한 정보를 검색하는 동안 오류가 발생하는 경우 표시할 텍스트를 입력합니다. 예를 들어 시스템에 회사 이름과 eCatalog 이름이 수신되었지만 롤오버 식별자가 수신되지 않은 경우 이 메시지가 사용자에게 표시됩니다.

>[!NOTE]
>
>eCatalog 자체에 정의된 템플릿 대신 이 응답 템플릿을 사용하려면 [정보 서버 URL] 끝에 "fmt=1"을 추가합니다. 예: `https://.../$3$/$4$/$1$/?FMT=1`.

1. **[저장]**&#x200B;을 클릭합니다.
1. 직접 만든 eCatalog 뷰어 사전 설정을 웹 페이지에 eCatalog를 표시하는 데 사용하려면 [기본값]을 클릭합니다.

To delete an eCatalog Viewer Preset, select it on the Viewer Presets screen and click **Delete**.

>[!MORELIKETHIS]
>
>* [Viewer Presets](application-setup.md#viewer_presets)
