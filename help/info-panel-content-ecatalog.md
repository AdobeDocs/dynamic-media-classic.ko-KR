---
title: 전자 카탈로그의 정보 패널 콘텐츠 관리
description: Adobe Dynamic Media Classic의 eCatalog에서 정보 패널 컨텐츠를 관리하는 방법을 알아봅니다.
uuid: 5aa634f9-0874-4bb5-a3d9-8ce4d5577941
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: be277831-77cc-4011-ae30-e75c18eec99b
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: bfb9c5a4-5068-4adb-9fe2-a4ead8656289
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '866'
ht-degree: 59%

---

# 전자 카탈로그의 정보 패널 콘텐츠 관리{#managing-info-panel-content-in-ecatalogs}

eCatalog에 롤오버의 이미지 맵 텍스트를 사용하는 것은 물론 정보 패널을 사용하여 링크를 비롯한 많은 롤오버 텍스트를 추가할 수도 있습니다. 시간 지정 캐싱과 컨텐츠 업데이트 예약을 사용하여 정보 패널을 관리할 수도 있습니다.

Adobe Dynamic Media Classic의 다음 기능을 사용하여 InfoPanel 설정과 데이터를 관리할 수 있습니다.

* [정보 패널 설정] 패널에서는 정보 패널 텍스트, 오류에 대한 기본 응답 및 정보가 캐싱되는 시간 수를 표시하는 데 사용되는 템플릿을 지정할 수 있습니다. 또한 eCatalog를 자동으로 게시할지 여부를 지정할 수 있습니다.
* InfoPanel 데이터 피드 패널을 사용하면 InfoPanel 롤오버 텍스트에 표시할 텍스트가 포함된 CSV 파일을 지정하고 정보 업데이트 시간을 예약할 수 있습니다.
* [메타데이터 가져오기] 대화 상자([맵 페이지] 보기에서 액세스함)에서는 롤오버 텍스트 정보가 포함된 탭으로 구분된 TXT 파일을 가져올 수 있습니다. 이 TXT 선택 사항이나 [데이터 피드] 패널 및 CSV 파일 선택 사항을 롤오버 텍스트에 사용할 수 있습니다.
* [맵 페이지] 보기에서는 특정 이미지 맵에 대해 표시되는 xml을 미리 보는 선택 사항을 제공합니다.

## eCatalog에 대한 응답 템플릿 설정 {#set-up-a-response-template-for-ecatalogs}

정보 패널에 텍스트를 표시하기 위해 세 가지 사전 설정 응답 템플릿 중 하나를 선택할 수 있습니다. 이러한 사전 설정 응답 템플릿은 열과 행 수, 서체 크기, 글꼴 등 정보 패널에 정보를 표시하는 방법을 결정합니다. 사전 설정 응답 템플릿을 선택하거나 고유한 템플릿 중 하나를 만들 수 있습니다.

>[!NOTE]
>
>[뷰어 사전 설정]에서 응답 템플릿을 설정할 수도 있습니다. 뷰어 사전 설정에서 응답 템플릿을 대신 사용하려면 뷰어 사전 설정에서 정보 서버 URL의 끝에 `fmt=1`를 추가합니다.
>
>[eCatalog 뷰어 사전 설정](setting-ecatalog-viewer-presets.md#setting_up_ecatalog_viewer_presets)을 참조하십시오.

1. eCatalog 를 두 번 클릭하여 세부 사항 보기에서 열립니다.
1. **[!UICONTROL InfoPanel 설정]** 패널을 선택합니다.
1. 응답 템플릿을 선택합니다.

   * [응답 템플릿] 메뉴에서 사전 설정을 선택합니다. 템플릿 디자인의 XML이 [사용자 템플릿] 상자에 표시됩니다.
   * 자체 응답 템플릿을 만들려면 **[!UICONTROL 사용자 지정]**&#x200B;을 선택합니다. [사용자 템플릿] 상자에 템플릿 XML 정의를 입력합니다. 사전 설정 템플릿을 고유한 템플릿의 기초로 사용할 수 있습니다.

1. (선택 사항) 기본 응답 상자에 Adobe Dynamic Media Classic에서 이미지 맵에 대한 정보를 검색하는 동안 오류가 발생하면 표시할 텍스트를 입력합니다. 예를 들어 시스템에 회사 이름과 eCatalog 이름이 수신되었지만 롤오버 식별자가 수신되지 않은 경우 이 메시지가 사용자에게 표시됩니다.
1. [응답 TTL] 상자에 데이터 캐싱 전에 대기할 시간 수를 입력합니다.

   * 하루 종일 데이터가 자주 업데이트되는 경우 더 작은 숫자를 설정합니다.
   * 데이터가 비교적 안정적이며 하루 종일 자주 업데이트할 필요가 없는 경우 더 큰 숫자를 설정합니다. 기본값은 10시간입니다.

1. **[!UICONTROL 게시]**&#x200B;를 선택합니다.

## 전자 카탈로그의 정보 패널에 대한 소스 컨텐츠 가져오기 {#import-source-content-for-the-info-panel-in-ecatalogs}

eCatalog의 정보 패널 소스 텍스트에 쉼표로 구분된 값 파일(CSV)이나 탭으로 구분된 파일(TXT)을 사용할 수 있습니다. 탭으로 구분된 파일은 UTF16(유니코드) 인코딩을 사용해야 합니다. 각 파일 유형을 서로 다른 방법으로 가져옵니다.

소스 컨텐츠 형식을 지정할 때는 다음 지침에 주의하십시오.

* 탭으로 구분된 데이터와 쉼표로 구분된 데이터가 롤오버 템플릿에 필요한 개수만큼 열을 포함하고 있는지 확인합니다.
* 데이터의 첫 번째 항목이나 열이 이미지 맵 URL의 rollover_key 값과 연결된 롤오버 식별자인지 확인합니다.
* 식별자 뒤에 있는 각 탭 또는 쉼표로 구분된 항목이 응답 템플릿에 대체하려는 항목인지 확인합니다. 따라서 첫 번째 열은 $1$로 대체되고 두 번째 열은 $2$ 로 대체됩니다.

### 외부에서 호스팅된 위치에서 eCatalog 로 CSV 컨텐츠를 가져옵니다. {#import-csv-content-into-ecatalogs-from-an-externally-hosted-location}

1. eCatalog 를 두 번 클릭하여 세부 사항 보기에서 열립니다.
1. **[!UICONTROL InfoPanel 데이터 피드]** 패널을 선택합니다.
1. [외부 호스팅된 CSV 파일 위치] 상자에 CSV 파일의 URL을 입력합니다. 이 필드에 URL을 붙여 넣거나 직접 입력할 수 있습니다.
1. (선택 사항) 일정 업데이트 메뉴를 사용하여 컨텐츠를 업데이트할 시간을 지정하고 **[!UICONTROL 추가]**&#x200B;를 선택합니다. 업데이트 시간을 여러 개 선택할 수 있습니다. 각 업데이트 시간이 [시간 업데이트] 상자에 표시됩니다. 시간을 제거하려면 시간을 선택하고 **[!UICONTROL 삭제]**&#x200B;를 선택합니다.
1. (선택 사항) **[!UICONTROL 지금 업데이트 실행]**&#x200B;을 선택하여 컨텐츠를 즉시 업데이트합니다.

### 탭으로 구분된 파일 또는 CSV 파일 가져오기 {#import-a-tab-delimited-or-csv-file}

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>SR changed this section 10/23/2012</p>

 -->

1. eCatalog 를 두 번 클릭하여 세부 사항 보기에서 엽니다.
1. **[!UICONTROL InfoPanel 설정]** 패널을 선택합니다.
1. **[!UICONTROL S7Info 컨텐츠 업로드]**&#x200B;를 선택합니다.
1. **[!UICONTROL 찾아보기]**&#x200B;를 선택하고, 사용할 탭으로 구분된 TXT 파일, CSV 또는 SSV 파일을 선택하고 **[!UICONTROL 열기]**&#x200B;를 선택합니다.
1. **[!UICONTROL 업로드]**&#x200B;를 선택합니다.

Dynamic Media Classic Adobe에서 업로드가 성공했는지 여부를 알려주는 이메일 메시지를 보냅니다.

## 이미지 맵의 롤오버 키 텍스트 미리 보기 {#preview-rollover-key-text-for-an-image-map}

[맵 페이지] 화면을 사용하여 eCatalog의 특정 페이지에 있는 이미지 맵의 정보 패널 텍스트를 쉽고 빠르게 볼 수 있습니다.

1. 카탈로그의 롤오버 **[!UICONTROL 편집]** 단추를 선택합니다.
1. **[!UICONTROL 페이지 매핑]**&#x200B;을 선택합니다.
1. 화면 오른쪽의 표 상단의 표시 메뉴에서 **[!UICONTROL 정보 패널]**&#x200B;을 선택합니다.

   정보 패널 텍스트가 있는 각 이미지 맵 평에 롤오버-키 텍스트가 표시됩니다.
