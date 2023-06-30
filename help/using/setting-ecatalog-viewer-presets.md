---
title: eCatalog 뷰어 사전 설정 설정
description: Adobe Dynamic Media Classic에서 eCatalog 뷰어 사전 설정을 설정하는 방법에 대해 알아봅니다.
uuid: aca66bc5-8491-4d81-9a06-1d3531860a14
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6c123f85-3bc4-4392-a7fb-55618127c65e
feature: Dynamic Media Classic,Viewers,Viewer Presets,eCatalog
role: User
exl-id: 4357e6b8-fbc5-4e93-9476-db92a7dc7464
topic: Integrations, Development
level: Experienced
source-git-commit: 5d8b7cb8b4616a998346675d7324b568634698fb
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 34%

---

# eCatalog 뷰어 사전 설정 설정{#setting-up-ecatalog-viewer-presets}

eCatalog 뷰어 사전 설정은 eCatalog 뷰어의 스타일, 동작 및 모양을 결정합니다. Adobe Dynamic Media Classic은 eCatalog 뷰어 사전 설정을 제공하며, 관리자는 고유한 eCatalog 뷰어 사전 설정을 만들 수도 있습니다.

사전 설정을 만들려면 처음부터 새로 만들거나 Adobe Dynamic Media Classic에서 제공한 eCatalog 뷰어 사전 설정으로 시작하여 새 이름으로 저장할 수 있습니다. 고유한 eCatalog 뷰어 사전 설정을 만들어 회사 색상으로 인쇄물을 표시하고 톤을 설정할 수 있습니다.

eCatalog 뷰어 사전 설정은 페이지 간 이동, 확대/축소, 검색 및 &quot;스킨&quot; 선택을 위한 다양한 설정을 제공합니다. 이러한 컨트롤의 모양과 뷰어 표시 방법은 선택한 eCatalog 뷰어 사전 설정에 따라 다릅니다.

eCatalog 뷰어 사전 설정을 만들 수 있도록 다음 단계를 따르십시오(관리자여야 함).

1. 전역 탐색 모음에서 다음 위치로 이동합니다. **[!UICONTROL 설정]** > **[!UICONTROL 뷰어 사전 설정]**.
1. [뷰어 사전 설정] 화면에서 새로 시작하거나 기존 eCatalog 뷰어 사전 설정에서 시작하여 eCatalog 뷰어 사전 설정을 만듭니다.

   * **eCatalog 뷰어 사전 설정 만들기** - 선택 **[!UICONTROL 추가]**. 뷰어 사전 설정 추가 대화 상자에서 플랫폼을 선택하고 eCatalog 뷰어를 선택한 다음 를 선택합니다. **[!UICONTROL 추가]**.

   * **eCatalog 뷰어 사전 설정 편집** - eCatalog 뷰어 사전 설정을 선택한 다음 선택 **[!UICONTROL 편집]**. 선택 **[!UICONTROL 다른 이름으로 저장]** 사전 설정 만들기를 완료한 후에.

1. [뷰어 구성] 화면에서 eCatalog 뷰어 사전 설정의 이름을 입력합니다.
1. [뷰어 구성] 화면에서 원하는 선택 사항을 설정합니다.

   선택 **[!UICONTROL 정보 팁]** 아이콘 옵션 옆에 있는 아이콘을 클릭하여 설명을 읽을 수 있습니다.

   미리보기 페이지에는 설정을 업데이트하고 변경할 때 뷰어가 표시됩니다.

1. (선택 사항) **[!UICONTROL 정보 패널 설정]**, **[!UICONTROL 정보 서버 URL]** 옵션에는 뷰어가 대체할 수 있는 다음과 같은 특수 토큰이 포함될 수 있습니다.

   | 토큰 | 대체 값 | 주의 |
   | --- | --- | --- |
   | `$1$` | rollover_key 값 | 의 항목 식별자 `<area>` 맵의 요소입니다. |
   | `$2$` | frame | 이미지 집합에 현재 표시된 프레임의 일련번호입니다. |
   | `$3$` | 이미지 루트 | 이미지 명령에 지정된 첫 번째 항목의 첫 번째 경로 요소(일반적으로 이미지 집합을 지정하는 카탈로그 항목의 이미지 카탈로그 ID)입니다. |

1. (선택 사항) **[!UICONTROL 정보 패널 설정]**, **[!UICONTROL 응답 템플릿]** 상자에 이미지 맵에 대한 정보를 검색하는 동안 Adobe Dynamic Media Classic에 오류가 발생할 경우 표시할 텍스트를 입력합니다. 예를 들어 시스템에 회사 이름과 eCatalog 이름이 수신되었지만 롤오버 식별자가 수신되지 않은 경우 이 메시지가 사용자에게 표시됩니다.

>[!NOTE]
>
>eCatalog 자체에 정의된 템플릿 대신 이 응답 템플릿을 사용하려면 을 추가합니다. `fmt=1` 를 입력합니다. 예: `https://.../$3$/$4$/$1$/?FMT=1`.

1. 선택 **[!UICONTROL 저장]**.
1. 선택 **[!UICONTROL 기본값]** 만든 eCatalog 뷰어 사전 설정을 웹 페이지에 eCatalogs를 표시하는 데 사용되는 것으로 하려는 경우.

eCatalog 뷰어 사전 설정을 삭제하려면 뷰어 사전 설정 화면에서 사전 설정을 선택한 다음 을 선택합니다 **[!UICONTROL 삭제]**.

>[!MORELIKETHIS]
>
>* [Viewer Presets](application-setup.md#viewer_presets)
