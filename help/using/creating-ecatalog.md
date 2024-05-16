---
title: eCatalog 만들기
description: Adobe Dynamic Media Classic에서 eCatalog를 만드는 방법을 알아봅니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 51d411b2-b4bc-4cf6-afca-dd0ed0d219a1
topic: Integrations, Development
level: Experienced
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '976'
ht-degree: 44%

---

# eCatalog 만들기 {#creating-an-ecatalog}

eCatalog를 만드는 과정에는 페이지 정렬, 페이지 레이아웃 선택, 이미지 맵을 그리고 롤오버 및 하이퍼텍스트 링크 데이터를 입력하여 페이지 연결 등의 작업이 포함됩니다. 선택적으로 eCatalog 뷰어에 페이지 번호 대신 페이지 이름이 표시되도록 TOC를 사용자 지정할 수 있습니다.

## eCatalog 만들기 {#create}

eCatalog에 이미지 파일과 PDF 파일을 포함할 수 있습니다.

전자 카탈로그를 만들 때, **[!UICONTROL 저장 후 게시]** 옵션은 다음과 같이 세트와 세트 구성원에 영향을 줍니다.

| 저장하기 전에 &quot;저장 후 게시&quot; 옵션이 선택되었습니까? | 저장 후 세트 상태 | 저장 후 세트 구성원 상태 |
| --- | --- | --- |
| 예 | 게시됨 | 게시됨 |
| 아니요 | 게시 취소됨 | 세트 구성원은 게시된 상태나 게시되지 않은 상태를 유지합니다. |

[수동 자산 게시](publishing-files.md#manually_publishing_assets) 및 [수동 자산 게시 취소](publishing-files.md#manually_unpublishing_assets)를 참조하십시오.

**eCatalog를 만들려면:**

1. 먼저 다음 기술 중 하나를 사용하여 eCatalog를 만듭니다.

   * **먼저 파일 선택**: 찾아보기 패널에서 파일을 선택하고 **[!UICONTROL 빌드]** > **[!UICONTROL 전자 카탈로그]**.

   * **eCatalog 화면에서 시작**: 다음으로 이동 **[!UICONTROL 빌드]** > **[!UICONTROL 전자 카탈로그]**. 자산 라이브러리에서 폴더를 선택하고 폴더의 파일을 전자 카탈로그 페이지의 [주문 페이지] 탭으로 드래그합니다.

     >[!NOTE]
     >
     >자산 라이브러리에서 항목을 썸네일 대신 이름으로 표시하려면 [개인 설정]의 [기본 자산 라이브러리 보기]에 대해 [이름] 선택 사항을 선택합니다.

1. eCatalog의 전체 레이아웃을 선택합니다. 선택 **[!UICONTROL 위로 1개]** 단일 페이지의 경우 **[!UICONTROL 2장 위로]** 더블 페이지 스프레드의 경우 또는 **[!UICONTROL 사용자 정의]** 두 페이지 이상의 페이지 스프레드의 경우. 다음에서 **[!UICONTROL eCatalog 레이아웃 변경]** 대화 상자에서 **[!UICONTROL 모든 스프레드]** 옵션 및 선택 **[!UICONTROL 확인]**.
1. 선택적으로 개별 페이지 또는 페이지 스프레드를 선택한 다음 선택하여 레이아웃을 변경할 수 있습니다 **[!UICONTROL 위로 1개]**, **[!UICONTROL 2장 위로]**, 또는 **[!UICONTROL 사용자 정의]** 단추를 클릭합니다. 다음에서 **[!UICONTROL eCatalog 레이아웃 변경]** 대화 상자에서 **[!UICONTROL 선택한 스프레드]** 옵션 및 선택 **[!UICONTROL 확인]**.
1. 필요한 경우 다음 기술 중 하나를 사용하여 페이지를 다시 정렬합니다.

   * **드래그**: 페이지 또는 페이지 스프레드를 새 위치로 드래그합니다. 세로 막대에 페이지가 이동되는 위치가 표시됩니다.

   * **이동 단추**: 페이지 또는 페이지 스프레드를 선택하고 **[!UICONTROL 이동 위치:]**&#x200B;을 클릭하고, 앞에 페이지를 표시할 메뉴에서 페이지를 선택합니다.

   * **시퀀스 번호**: 목록 보기에서 시퀀스 번호의 필드에 페이지 번호를 입력합니다.

1. 완료하면 페이지 오른쪽 하단에서 **[!UICONTROL 저장 후 게시]**(기본값)가 선택되어 있는지 확인합니다.
1. 선택 **[!UICONTROL 저장]**.
1. [저장] 대화 상자에서 전자 카탈로그를 저장할 폴더를 선택합니다. [파일 이름] 필드에 회전 집합 이름을 입력합니다.
1. 선택 **[!UICONTROL 저장]**.

   전자 카탈로그를 저장한 후 을(를) 선택하여 미리 볼 수 있습니다 **[!UICONTROL 미리 보기]**.

## eCatalog 편집 {#editing-an-ecatalog}

게시된 세트를 편집하든 게시되지 않은 세트를 편집하든 **[!UICONTROL 저장 후 게시]** 옵션은 다음과 같은 방법으로 세트 및 세트 멤버에 영향을 줍니다.

| 세트를 이미 게시했습니까? | 편집을 저장하기 전에 &quot;저장 후 게시&quot; 옵션이 선택되었습니까? | 저장 후 세트 상태 | 저장 후 세트 구성원 상태 |
| --- | --- | --- | --- |
| 예 | 예 | 게시됨 | 게시됨 |
| 예 | 아니요 | 게시됨 | 기존 집합 구성원은 게시된 상태를 유지합니다. 편집 중에 새로 추가한 모든 세트 구성원은 게시된 상태나 게시 취소된 상태를 유지합니다. |
| 아니요 | 예 | 게시됨 | 게시됨 |
| 아니요 | 아니요 | 게시 취소됨 | 기존 세트 구성원과 편집 중에 새로 추가한 모든 세트 구성원은 게시된 상태나 게시 취소된 상태를 유지합니다. |

[수동 자산 게시](publishing-files.md#manually_publishing_assets) 및 [수동 자산 게시 취소](publishing-files.md#manually_unpublishing_assets)를 참조하십시오.

**eCatalog를 편집하려면:**

1. 전자 카탈로그의 롤오버 선택 **[!UICONTROL 편집]** 단추를 클릭합니다.
1. 필요한 변경 작업을 수행합니다.
1. 편집을 완료하면 페이지 오른쪽 하단에서 **[!UICONTROL 저장 후 게시]**(기본값)가 선택되어 있는지 확인합니다.
1. 선택 **[!UICONTROL 저장]**&#x200B;스토리지 폴더를 선택하고 세트 이름을 입력한 다음 을 선택합니다. **[!UICONTROL 저장]**.

## eCatalog 삭제

삭제된 세트는 휴지통으로 이동합니다. 그러나 해당 집합 내의 멤버(또는 &quot;하위&quot;)는 영향을 받지 않습니다. 대신 각 멤버는 기존의 게시 또는 게시 취소 상태를 유지합니다.

[수동 자산 게시](publishing-files.md#manually_publishing_assets) 및 [수동 자산 게시 취소](publishing-files.md#manually_unpublishing_assets)를 참조하십시오.

**eCatalog를 삭제하려면**

1. [격자 보기], [목록 보기] 또는 [상세 보기]에서 전자 카탈로그를 하나 이상 선택합니다.
1. 전역 탐색 모음에서 다음 위치로 이동합니다. **[!UICONTROL 파일]** > **[!UICONTROL 삭제]** > **[!UICONTROL 삭제]**.

## 목차(TOC) 사용자 정의 {#customizing-the-table-of-contents-toc}

Adobe Dynamic Media Classic은 eCatalog 화면의 주문 페이지 탭에서 eCatalog에 기본 페이지 번호를 제공합니다. 사용자 지정 페이지 이름의 경우 TOC(목차)를 구성하는 페이지 레이블을 변경할 수 있습니다. 앞 표지와 뒤 표지의 이름을 바꾸는 것이 좋습니다. 예를 들어 앞 표지는 &quot;0-1페이지&quot; 대신 &quot;표지&quot;를 읽을 수 있습니다.

CSV(Mac 전용) 또는 XML 파일에서 페이지 이름을 가져오거나 수동으로 eCatalog에 대한 사용자 지정 목차(TOC)를 만들 수 있습니다.

>[!NOTE]
>
>기본 페이지 제목을 복원하려면 **[!UICONTROL 페이지 주문]** 탭, 선택 **[!UICONTROL 목차 레이블]**&#x200B;을 선택한 다음 을 선택합니다 **[!UICONTROL 기본값 복원(모두)]**.

### 수동으로 페이지 이름 입력 {#manually-entering-page-names}

수동으로 페이지 이름을 하나씩 입력하려면 eCatalog 화면의 [주문 페이지] 탭으로 이동합니다. 그런 다음 페이지 번호 필드에 이름을 지정할 각 페이지의 이름을 입력합니다.

### 페이지 이름 가져오기 {#importing-page-names}

많은 페이지가 포함된 eCatalog를 다루는 경우 페이지 이름을 가져오는 것이 좋습니다. 탭으로 구분된 파일이나 XML 파일에서 이름을 가져올 수 있습니다.

목차 레이블은 이미지의 사용자 데이터 필드에 저장됩니다. 이 데이터의 형식을 `name=<value>` ` pairs separated by two question marks "??" `. 예를 들어 이라는 TOC 필드에 대해 하나의 레이블을 설정하려면 다음을 수행합니다 `tocEN`를 클릭하고 이미지의 사용자 데이터를 다음으로 설정합니다.

`tocEN=&lt;EN_page_label>`

목차 필드에 대해 별도의 레이블을 설정하려면 `tocEN` 및 `tocFR`:

`tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label>`

탭으로 구분된 파일의 사용자 데이터 필드를 가져오려면 필드 사용자 데이터를 포함합니다.

| IPSID | 사용자 데이터 |
| --- | --- |
| `<image_IPS_ID>` | `tocEN=<EN_page_label>??tocFR=<FR_page_label>` |

XML 파일의 사용자 데이터 필드를 가져오려면 속성을 포함합니다 `vc_userdata`:

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

탭으로 구분된 파일 또는 XML 파일에서 페이지 이름을 가져오려면 **[!UICONTROL 목차 레이블]** 단추 및 선택 **[!UICONTROL 가져오기]**. 메타데이터 업로드 대화 상자에서 다음을 선택합니다 **[!UICONTROL 찾아보기]**&#x200B;를 가져온 다음 각 페이지를 페이지 이름과 연결하는 CSV 파일(Mac만 해당) 또는 XML 파일을 가져옵니다.
