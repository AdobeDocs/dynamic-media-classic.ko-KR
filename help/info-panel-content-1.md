---
title: 이미지 세트의 정보 패널 컨텐츠 관리
seo-title: 이미지 세트에서 정보 패널 컨텐츠 관리
description: 널
seo-description: 이미지 세트에서 정보 패널 콘텐츠를 관리하는 방법을 알아봅니다.
uuid: ed7b4344-f180-41fc-a95a-62a9767dc056
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
content-type: reference
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: ba5d1fb1-af54-471c-a471-853ace7f72fd
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# 이미지 세트의 정보 패널 컨텐츠 관리{#managing-info-panel-content-in-image-sets}

이미지 집합에 롤오버의 이미지 맵 텍스트를 사용하는 것은 물론 정보 패널을 사용하여 링크를 비롯한 많은 롤오버 텍스트를 추가할 수도 있습니다. 시간 지정 캐싱과 컨텐츠 업데이트 예약을 사용하여 정보 패널을 관리할 수도 있습니다.

Scene7 Publishing System의 다음 기능을 사용하여 정보 패널 설정과 데이터를 관리할 수 있습니다.

* [정보 패널 설정] 패널에서는 정보 패널 텍스트, 오류에 대한 기본 응답 및 정보가 캐싱되는 시간 수를 표시하는 데 사용되는 템플릿을 지정할 수 있습니다. 또한 이미지 집합을 자동으로 게시할지 여부를 지정할 수 있습니다.
* [정보 패널 데이터 피드] 패널에서는 정보 패널 롤오버 텍스트에 표시할 텍스트가 포함된 CSV 파일을 지정하고 정보 업데이트 시간을 예약할 수 있습니다.
* [메타데이터 가져오기] 대화 상자에서는 롤오버 텍스트 정보가 포함된 탭으로 구분된 TXT 파일을 가져올 수 있습니다. 이 TXT 선택 사항이나 [정보 패널 데이터 피드] 패널 및 CSV 파일 선택 사항을 롤오버 텍스트에 사용할 수 있습니다.

## 이미지 집합에 대한 응답 템플릿 설정 {#set-up-a-response-template-for-image-sets}

정보 패널에 텍스트를 표시하기 위해 세 가지 사전 설정 응답 템플릿 중 하나를 선택할 수 있습니다. 이러한 사전 설정 응답 템플릿은 열과 행 수, 서체 크기, 글꼴 등 정보 패널에 정보를 표시하는 방법을 결정합니다. 사전 설정 응답 템플릿을 선택하거나 고유한 템플릿 중 하나를 만들 수 있습니다.

**응답 템플릿을 설정하려면**

1. 이미지 집합을 두 번 클릭하여 [세부 사항 보기]에서 엽니다.
1. Click **InfoPanel Setup** to unfold the panel.
1. [응답 템플릿] 드롭다운 목록에서 다음 중 하나를 수행합니다.

   * [기본값]을 선택하여 기본 응답을 사용합니다. 템플릿 디자인의 XML이 [사용자 템플릿] 텍스트 상자에 희미하게 표시됩니다.
   * [사용자 지정]을 선택하여 고유한 응답 템플릿을 만듭니다. [사용자 템플릿] 텍스트 상자에 템플릿 XML 정의를 입력합니다. 이미 텍스트 상자에 정의된 기본 템플릿을 고유한 응답의 기초로 사용할 수 있습니다.

1. (선택 사항) Dynamic Media Classic에서 이미지 맵에 대한 정보를 검색하는 동안 오류가 발생하는 경우 표시할 텍스트를 [기본 응답] 상자에 입력합니다. 예를 들어 시스템에 회사 이름과 이미지 집합 이름이 수신되었지만 롤오버 식별자가 수신되지 않은 경우 이 메시지가 사용자에게 표시됩니다.
1. [응답 TTL] 텍스트 필드에 데이터 캐싱 전에 대기할 시간을 입력합니다.

   * 하루 종일 데이터가 자주 업데이트되는 경우 더 작은 숫자를 설정합니다.
   * 데이터가 비교적 안정적이며 하루 종일 자주 업데이트할 필요가 없는 경우 더 큰 숫자를 설정합니다. 기본값은 10시간입니다.

1. Click **Upload** to upload info panel content, based on the rollover_key values, to s7info.
1. In the S7Info Upload dialog box, browse to the file that you want to use, and then click **Upload**.

   지원되는 파일 형식은 탭으로 구분된 파일(UTF-16 인코딩) 및 CSV 파일(ASCII 인코딩)입니다. CSV 파일의 경우 ASCII 이외의 문자는 HTML로 인코딩해야 합니다.

1. In the InfoPanel Setup panel, click **Publish**.

## 이미지 세트의 정보 패널에 대한 소스 컨텐츠 가져오기 {#import-source-content-for-the-info-panel-in-image-sets}

이미지 집합의 정보 패널 소스 텍스트에 CSV(쉼표로 구분된 값) 파일(ASCII 인코딩, ASCII 이외의 문자는 HTML로 인코딩해야 함) 또는 탭으로 구분된 파일을 사용할 수 있습니다. 탭으로 구분된 파일은 UTF-16(유니코드) 인코딩을 사용해야 합니다. 각 파일 유형을 서로 다른 방법으로 가져옵니다.

소스 컨텐츠 형식을 지정할 때는 다음 지침에 주의하십시오.

* 탭으로 구분된 데이터와 쉼표로 구분된 데이터가 롤오버 템플릿에 필요한 개수만큼 열을 포함해야 합니다.
* 데이터의 첫 번째 항목이나 열이 이미지 맵 URL의 rollover_key 값과 연결된 롤오버 식별자여야 합니다.
* 식별자 뒤의 탭으로 구분된 항목이나 쉼표로 구분된 항목이 응답 템플릿에 대체할 항목인지 확인합니다(첫 번째 열은 $1$에 대체되고, 두 번째 열은 $2$에 대체됨).

### 외부에서 호스팅된 위치에서 이미지 세트로 CSV 컨텐츠 가져오기 {#import-csv-content-into-image-sets-from-an-externally-hosted-location}

1. 이미지 집합을 두 번 클릭하여 [세부 사항 보기]에서 엽니다.
1. Click **InfoPanel Datafeed** to unfold the panel.
1. [외부 호스팅된 CSV 파일 위치(HTTP)] 텍스트 필드에 CSV 파일의 URL을 입력합니다.
1. (Optional) In the Schedule Update fields, specify a time to update the content, and then click **Add**.

   업데이트 시간을 여러 개 선택할 수 있습니다. 각 업데이트 시간이 [시간 업데이트] 텍스트 상자에 표시됩니다. To remove a scheduled time, select it, and then click **Delete**.

1. (Optional) Click **Run Update** to immediately update the content.

