---
title: eCatalog 만들기
seo-title: eCatalog 만들기
description: 널
seo-description: Ecatalog를 만드는 방법을 알아봅니다.
uuid: 2 AFF 05 C 2-7052-426 C-B 61 D -7 F 9091 F 7 ACE 8
contentOwner: 관리
content-type: 참조
products: sg_ Experiencemanager/dynamic-media-scene -7
geptopics: sg_ scenesevenondemand_ pk/categories/ecatalogs
discoiquuid: 28889 C 60-596 A -40 D 2-85 D 4-F 48 A 4 F 86 B 932
translation-type: tm+mt
source-git-commit: 1941567db5c154620bb0dcd12e363d7eebc61b20

---


# eCatalog 만들기{#creating-an-ecatalog}

eCatalog를 만드는 과정에는 페이지 정렬, 페이지 레이아웃 선택, 이미지 맵을 그리고 롤오버 및 하이퍼텍스트 링크 데이터를 입력하여 페이지 연결 등의 작업이 포함됩니다. 선택적으로 eCatalog 뷰어에 페이지 번호 대신 페이지 이름이 표시되도록 TOC를 사용자 지정할 수 있습니다.

## eCatalog 만들기 {#create}

eCatalog에는 이미지 파일과 PDF 파일을 포함할 수 있습니다.

전자 카탈로그를 만들 때, **저장 후 게시** 옵션은 다음과 같이 세트와 세트 구성원에 영향을 줍니다.

| 저장하기 전에 "저장 후 게시" 옵션을 선택했습니까? | 저장 후 세트 상태 | 저장 후 세트 구성원 상태 |
|--- |--- |--- |
| 예 | 게시됨 | 게시됨 |
| 아니요 | 게시 취소됨 | 세트 구성원은 게시된 상태나 게시되지 않은 상태를 유지합니다. |

[수동 자산 게시](publishing-files.md#manually_publishing_assets) 및 [수동 자산 게시 취소](publishing-files.md#manually_unpublishing_assets)를 참조하십시오.

**전자 카탈로그 만들기**

1. 먼저 다음 기술 중 하나를 사용하여 eCatalog를 만듭니다.

   **찾아보기 패널에서 먼저** 파일을 선택하고 파일을 선택한 다음 [빌드] &gt; [Ecatalog] 를 클릭합니다.

   **Ecatalog 화면에서 시작 &gt; ecatalog를** 클릭합니다. 자산 라이브러리에서 폴더를 선택하고 폴더의 파일을 전자 카탈로그 페이지의 [주문 페이지] 탭으로 드래그합니다.

   ***note**: To view the items in the Asset Library by name instead of thumbnail, select the Name option for Default Asset Library View in Personal Setup. *

1. eCatalog의 전체 레이아웃을 선택합니다. 단일 페이지를 나타내는 [1단계 위로] 단추 , 양면 페이지 스프레드를 나타내는 [2단계 위로] 단추  또는 세 페이지 이상의 페이지 스프레드를 나타내는 [사용자 지정] 단추 를 클릭합니다. [eCatalog 레이아웃 변경] 대화 상자가 나타납니다. Select the All Spreads options and click **OK**.
1. 선택적으로 개별 페이지나 페이지 스프레드를 클릭하고 [1단계 위로] 단추, [2단계 위로] 단추 또는 [사용자 지정] 단추를 선택하여 레이아웃을 변경합니다. [eCatalog 레이아웃 변경] 대화 상자가 나타납니다. Select the Selected Spreads options and click **OK**.
1. 필요한 경우 다음 기술 중 하나를 사용하여 페이지를 다시 정렬합니다.

   **드래그하여** 페이지 또는 페이지 스프레드를 새 위치로 드래그합니다. 세로 막대에 페이지가 이동되는 위치가 표시됩니다.

   **이동 단추로 이동페이지나** 페이지 스프레드를 선택하고 이동 버튼을 클릭한 다음 페이지에 표시할 페이지를 선택합니다.

   **시퀀스 #** in 목록 보기에서 시퀀스 # 필드에 페이지 번호를 입력합니다.

1. 완료하면 페이지 오른쪽 하단에서 **저장 후 게시**(기본값)가 선택되어 있는지 확인합니다.
1. **[저장]**&#x200B;을 클릭합니다.
1. [저장] 대화 상자에서 전자 카탈로그를 저장할 폴더를 선택합니다. [파일 이름] 필드에 회전 집합 이름을 입력합니다.
1. **[저장]**&#x200B;을 클릭합니다.

   전자 카탈로그를 저장한 후 **미리 보기**&#x200B;를 클릭하여 전자 카탈로그를 미리 볼 수 있습니다.

## 전자 카탈로그 편집 {#editing-an-ecatalog}

편집 대상이 게시된 세트인지 게시 취소된 세트인지에 따라, **저장 후 게시** 옵션은 다음과 같이 세트와 세트 구성원에 영향을 줍니다.

| 세트를 이미 게시했습니까? | 편집 내용을 저장하기 전에 [저장 후 게시] 옵션을 선택했습니까? | 저장 후 세트 상태 | 저장 후 세트 구성원 상태 |
|--- |--- |--- |--- |
| 예 | 예 | 게시됨 | 게시됨 |
| 예 | 아니요 | 게시됨 | 기존 세트 구성원은 게시된 상태를 유지합니다. 편집하는 동안 추가한 모든 새로운 세트 구성원은 게시된 상태나 게시 취소된 상태를 유지합니다. |
| 아니요 | 예 | 게시됨 | 게시됨 |
| 아니요 | 아니요 | 게시 취소됨 | 기존 세트 구성원과 편집 중에 새로 추가한 모든 세트 구성원은 게시된 상태나 게시 취소된 상태를 유지합니다. |

[수동 자산 게시](publishing-files.md#manually_publishing_assets) 및 [수동 자산 게시 취소](publishing-files.md#manually_unpublishing_assets)를 참조하십시오.

**전자 카탈로그 편집**

1. 전자 카탈로그의 롤오버 **편집** 단추를 클릭합니다.
1. 필요한 변경 작업을 수행합니다.
1. 편집을 완료하면 페이지 오른쪽 하단에서 **저장 후 게시**(기본값)가 선택되어 있는지 확인합니다.
1. **저장**&#x200B;을 클릭하고 저장 폴더를 선택한 다음에 세트 이름을 입력하고 **저장**&#x200B;을 클릭합니다.

## 전자 카탈로그 삭제 {#deleting-an-ecatalog}

삭제된 세트는 휴지통으로 이동합니다. 하지만 삭제된 세트 내의 구성원(또는 "하위")은 휴지통으로 이동하지 않고, 각각 기존의 게시된 상태나 게시 취소된 상태를 유지합니다.

[수동 자산 게시](publishing-files.md#manually_publishing_assets) 및 [수동 자산 게시 취소](publishing-files.md#manually_unpublishing_assets)를 참조하십시오.

**전자 카탈로그 삭제**

1. [격자 보기], [목록 보기] 또는 [상세 보기]에서 전자 카탈로그를 하나 이상 선택합니다.
1. 글로벌 탐색 막대에서 **파일** &gt; **삭제** &gt; **삭제**&#x200B;를 클릭합니다.

## TOC(목차) 사용자 지정 {#customizing-the-table-of-contents-toc}

Dynamic Media Classic는 ecatalog 화면의 주문 페이지 탭에서 ecatalog의 기본 페이지 번호를 제공합니다. 사용자 지정 페이지 이름의 경우 TOC(목차)를 구성하는 페이지 레이블을 변경할 수 있습니다. 앞 표지와 뒤 표지의 이름을 바꾸는 것이 좋습니다. 예를 들어 앞면 표지 페이지는 "0-1 페이지" 대신 "표지" 를 읽을 수 있습니다. »

CSV(Mac에만 해당) 또는 XML 파일에서 페이지 이름을 가져오거나 수동으로 eCatalog에 대한 사용자 지정 TOC(목차)를 만들 수 있습니다.

>[!NOTE]
>
>기본 페이지 제목을 복원하려면 [주문 페이지] 탭에서 [목차 레이블] 단추를 클릭하고 [기본값 복원(모두)]을 선택합니다.

### 수동으로 페이지 이름 입력 {#manually-entering-page-names}

수동으로 페이지 이름을 하나씩 입력하려면 eCatalog 화면의 [주문 페이지] 탭으로 이동합니다. 페이지 번호 필드를 클릭하고 이름을 입력합니다. 이름을 지정하려는 각 페이지의 이름을 입력합니다.

### 페이지 이름 가져오기 {#importing-page-names}

많은 페이지가 포함된 eCatalog를 다루는 경우 페이지 이름을 가져오는 것이 좋습니다. 탭으로 구분된 파일이나 XML 파일에서 이름을 가져올 수 있습니다.

TOC 레이블은 이미지의 사용자 데이터 필드에 저장됩니다. 이 데이터의 형식을 `name=<value>`` pairs separated by two question marks “??” `목록으로 지정합니다. 예를 들어 Tocen 이라는 TOC 필드에 대한 레이블을 하나 설정하려면 이미지의 사용자 데이터를 다음으로 설정합니다.

tocEN=&lt;EN_page_label&gt;

tocEN 및 tocFR이라는 TOC 필드에 대해 별도의 레이블을 설정하려면 다음과 같이 설정합니다.

tocEN=&lt;EN_page_label&gt;??tocFR=&lt;FR_page_label&gt;

탭으로 구분된 파일의 [사용자 데이터] 필드를 가져오려면 다음과 같이 필드 사용자 데이터를 포함합니다.

| IPSID | 사용자 데이터 |
|--- |--- |
| `<image_IPS_ID>` | tocEN=&lt;EN_page_label&gt;??tocFR=&lt;FR_page_label&gt; |

XML 파일의 [사용자 데이터] 필드를 가져오려면 다음과 같이 `vc_userdata` 특성을 포함합니다.

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

탭으로 구분된 파일이나 XML 파일에서 페이지 이름을 가져오려면 [목차 레이블] 단추를 선택한 다음 [가져오기]를 선택합니다. [메타데이터 업로드] 대화 상자가 나타납니다. [찾아보기] 단추를 클릭하고 각 페이지를 페이지 이름과 연결하는 CSV 파일(Mac에만 해당) 또는 XML 파일을 가져옵니다. 