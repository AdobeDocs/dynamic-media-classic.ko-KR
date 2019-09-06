---
title: Ecatalog에서 정보 패널 컨텐츠 관리
seo-title: Ecatalog에서 정보 패널 컨텐츠 관리
description: 널
seo-description: Ecatalog에서 정보 패널 컨텐츠를 관리하는 방법을 알아봅니다.
uuid: 5 AA 634 F 9-0874-4 BB 5-A 3 D 9-8 CE 4 D 5577941
contentOwner: 관리
content-type: 참조
products: sg_ Experiencemanager/dynamic-media-scene -7
geptopics: sg_ scenesevenondemand_ pk/categories/ecatalogs
discoiquuid: BE 277831-77 CC -4011-AE 30-E 75 C 18 EEC 99 B
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Ecatalog에서 정보 패널 컨텐츠 관리{#managing-info-panel-content-in-ecatalogs}

eCatalog에 롤오버의 이미지 맵 텍스트를 사용하는 것은 물론 정보 패널을 사용하여 링크를 비롯한 많은 롤오버 텍스트를 추가할 수도 있습니다. 시간 지정 캐싱과 컨텐츠 업데이트 예약을 사용하여 정보 패널을 관리할 수도 있습니다.

Dynamic Media Classic의 다음 기능을 사용하여 infopanel 설정 및 데이터를 관리할 수 있습니다.

* [정보 패널 설정] 패널에서는 정보 패널 텍스트, 오류에 대한 기본 응답 및 정보가 캐싱되는 시간 수를 표시하는 데 사용되는 템플릿을 지정할 수 있습니다. 또한 eCatalog를 자동으로 게시할지 여부를 지정할 수 있습니다.
* [정보 패널 데이터 피드] 패널에서는 정보 패널 롤오버 텍스트에 표시할 텍스트가 포함된 CSV 파일을 지정하고 정보 업데이트 시간을 예약할 수 있습니다.
* [메타데이터 가져오기] 대화 상자([맵 페이지] 보기에서 액세스함)에서는 롤오버 텍스트 정보가 포함된 탭으로 구분된 TXT 파일을 가져올 수 있습니다. 이 TXT 선택 사항이나 [데이터 피드] 패널 및 CSV 파일 선택 사항을 롤오버 텍스트에 사용할 수 있습니다.
* [맵 페이지] 보기에서는 특정 이미지 맵에 대해 표시되는 xml을 미리 보는 선택 사항을 제공합니다.

## Ecatalog에 대한 응답 템플릿 설정 {#set-up-a-response-template-for-ecatalogs}

정보 패널에 텍스트를 표시하기 위해 세 가지 사전 설정 응답 템플릿 중 하나를 선택할 수 있습니다. 이러한 사전 설정 응답 템플릿은 열과 행 수, 서체 크기, 글꼴 등 정보 패널에 정보를 표시하는 방법을 결정합니다. 사전 설정 응답 템플릿을 선택하거나 고유한 템플릿 중 하나를 만들 수 있습니다.

>[!NOTE]
>
>[뷰어 사전 설정]에서 응답 템플릿을 설정할 수도 있습니다. To use the Response Template in the Viewer Preset instead, add `fmt=1` to the end of the Information Server URL in the Viewer Preset.
>
>[eCatalog 뷰어 사전 설정 지정](setting-ecatalog-viewer-presets.md#setting_up_ecatalog_viewer_presets)을 참조하십시오.

1. eCatalog를 두 번 클릭하여 [세부 사항 보기]에서 엽니다.
1. [정보 패널 설정] 패널을 클릭하여 엽니다.
1. 응답 템플릿을 선택합니다.

   * [응답 템플릿] 메뉴에서 사전 설정을 선택합니다. 템플릿 디자인의 XML이 [사용자 템플릿] 상자에 표시됩니다.
   * [사용자 지정]을 선택하여 고유한 응답 템플릿을 만듭니다. [사용자 템플릿] 상자에 템플릿 XML 정의를 입력합니다. 사전 설정 템플릿을 고유한 템플릿의 기초로 사용할 수 있습니다.

1. (선택 사항) 기본 응답 상자에, Dynamic Media Classic에서 이미지 맵에 대한 정보를 검색하는 동안 오류가 발생하는 경우 표시할 텍스트를 입력합니다. 예를 들어 시스템에 회사 이름과 eCatalog 이름이 수신되었지만 롤오버 식별자가 수신되지 않은 경우 이 메시지가 사용자에게 표시됩니다.
1. [응답 TTL] 상자에 데이터 캐싱 전에 대기할 시간 수를 입력합니다.

   * 하루 종일 데이터가 자주 업데이트되는 경우 더 작은 숫자를 설정합니다.
   * 데이터가 비교적 안정적이며 하루 종일 자주 업데이트할 필요가 없는 경우 더 큰 숫자를 설정합니다. 기본값은 10시간입니다.

1. **게시를**&#x200B;클릭합니다.

## Import source content for the Info Panel in eCatalogs {#import-source-content-for-the-info-panel-in-ecatalogs}

eCatalog의 정보 패널 소스 텍스트에 쉼표로 구분된 값 파일(CSV)이나 탭으로 구분된 파일(TXT)을 사용할 수 있습니다. 탭으로 구분된 파일은 UTF16(유니코드) 인코딩을 사용해야 합니다. 각 파일 유형을 서로 다른 방법으로 가져옵니다.

소스 컨텐츠 형식을 지정할 때는 다음 지침에 주의하십시오.

* 탭으로 구분된 데이터와 쉼표로 구분된 데이터가 롤오버 템플릿에 필요한 개수만큼 열을 포함하고 있는지 확인합니다.
* 데이터의 첫 번째 항목이나 열이 이미지 맵 URL의 rollover_key 값과 연결된 롤오버 식별자인지 확인합니다.
* 식별자 뒤의 탭으로 구분된 항목이나 쉼표로 구분된 항목이 응답 템플릿에 대체할 항목인지 확인합니다(첫 번째 열은 $1$에 대체되고, 두 번째 열은 $2$에 대체됨).

### Import CSV content into eCatalogs from an externally hosted location {#import-csv-content-into-ecatalogs-from-an-externally-hosted-location}

1. eCatalog를 두 번 클릭하여 [세부 사항 보기]에서 엽니다.
1. [정보 패널 데이터 피드] 패널을 클릭하여 엽니다.
1. [외부 호스팅된 CSV 파일 위치] 상자에 CSV 파일의 URL을 입력합니다. 이 필드에 URL을 붙여 넣거나 직접 입력할 수 있습니다.
1. (선택 사항) [업데이트 예약] 메뉴를 사용하여 컨텐츠 업데이트 시간을 지정하고 [추가]를 클릭합니다. 업데이트 시간을 여러 개 선택할 수 있습니다. 각 업데이트 시간이 [시간 업데이트] 상자에 표시됩니다. 시간을 제거하려면 시간을 선택하고 [삭제]를 클릭합니다.
1. (선택 사항) [지금 업데이트 실행]을 클릭하여 컨텐츠를 즉시 업데이트합니다.

### 탭으로 구분된 파일 또는 CSV 파일 가져오기 {#import-a-tab-delimited-or-csv-file}

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>SR changed this section 10/23/2012</p>

 -->

1. eCatalog를 두 번 클릭하여 [세부 사항 보기]에서 엽니다.
1. [정보 패널 설정] 패널을 클릭하여 엽니다.
1. **S 7 정보 컨텐츠 업로드를 클릭합니다**.
1. **[탐색**] 를 클릭하고 사용할 탭으로 구분된 TXT 파일, CSV 또는 SSV 파일을 선택한 다음 [ **열기**] 를 클릭합니다.
1. **업로드**&#x200B;를 클릭합니다.

Dynamic Media Classic는 업로드가 성공했는지 여부를 알려주는 전자 메일 메시지를 보냅니다.

## 이미지 맵의 롤오버 키 텍스트 미리 보기 {#preview-rollover-key-text-for-an-image-map}

[맵 페이지] 화면을 사용하여 eCatalog의 특정 페이지에 있는 이미지 맵의 정보 패널 텍스트를 쉽고 빠르게 볼 수 있습니다.

1. eCatalog의 롤오버 [편집] 단추를 클릭합니다.
1. [맵 페이지]를 클릭합니다.
1. 화면 오른쪽의 테이블 상단에 있는 [표시] 메뉴에서 [정보 패널]을 선택합니다.

   정보 패널 텍스트가 포함된 각 이미지 맵 옆에 롤오버 키 텍스트가 표시됩니다.
