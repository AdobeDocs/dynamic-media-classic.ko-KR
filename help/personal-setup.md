---
title: 개인 설정
description: 모든 사용자는 Dynamic Media Classic의 [개인 설정] 화면에서 설정을 변경할 수 있습니다.
uuid: 29cb825a-f158-4a1e-9d5f-7636ee411b6e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 6314e7b7-5bde-4fe2-8674-e4fc525d4d1c
feature: Dynamic Media Classic
role: Administrator,Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '1197'
ht-degree: 78%

---


# 개인 설정 {#personal-setup}

모든 사용자는 [개인 설정] 화면의 설정을 변경할 수 있습니다. [개인 설정] 화면을 열려면 [설정] > [개인 설정]을 클릭합니다.

>[!NOTE]
>
>[개인 설정] 화면에는 Dynamic Media Classic에서 가지고 있는 사용자 역할이 나열됩니다.회사 관리자, 관리자 또는 사용자.

[개인 설정] 설정은 찾아보기 패널의 기본적인 행동, 이메일을 전달받는 방식, 암호 설정을 제어합니다. 이러한 설정을 변경한 후 [저장]을 클릭해야 합니다.

## 내 계정 정보

계정 이름, 이름, 사용자 이름(이메일 주소) 및 지정된 사용자 역할을 식별합니다.

### 데스크톱 버전

지금 설치를 클릭하여 로컬 하드 드라이브에 데스크탑 버전의 Dynamic Media Classic을 설치합니다. 또는 [지금 재설치]를 클릭하여 데스크톱 버전을 다시 설치합니다.

## 로컬 하드 드라이브에 플러그인 설치

1. Dynamic Media Classic의 [개인 설정] 페이지에서 Web-to-Print용 Illustrator 플러그인 아래의 **지금 다운로드**&#x200B;을 클릭하여 **Illustrator Plug-in for Web-to-Print.zip** 파일을 다운로드합니다.
1. ZIP 파일의 압축을 임시 폴더에 해제합니다.

   플러그인에 대한 추가 정보를 제공하기 위해 압축을 푼 파일의 루트에 readme 파일이 포함되어 있습니다.

1. 설치된 운영 체제에 따라 다음 중 하나를 수행합니다.

### Windows

| 실행 중인 버전 | 수행할 작업 |
|--- |--- |
| Adobe Creative Cloud 2014의 Adobe Illustrator 18 | <ul><li>압축을 푼 폴더의 루트에서 CC-2014를 클릭합니다.</li><li>사용하는 Adobe Illustrator의 비트 버전에 따라 win32 또는 win64를 클릭합니다.</li><li>라이브러리 > flame을 클릭한 다음 `aflame.dll`을 Adobe Illustrator의 실행 가능한 폴더에 복사합니다. (예: `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`) </li></ul><br/>**참고**:이 예제 경로는 64비트 위치에 대한 것입니다.32비트 위치는 프로그램 파일(x86)에 속할 수 있습니다.  <br/><ul><li>동일한 라이브러리 폴더로 돌아가 flamingo를 클릭한 다음 `aflamingo.dll`을 이전 단계에서 사용한 것과 동일한 Adobe Illustrator 실행 가능한 폴더에 복사합니다. </li><li>2단계에서 선택한 win32 또는 win64 폴더로 돌아간 다음 `AdobeS7FXGFileFormat.aip`를 Adobe Illustrator의 플러그인 폴더에 복사합니다. (예: `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`) </li></ul> <br/>**참고**:이 예제 경로는 64비트 위치에 대한 것입니다.32비트 위치는 프로그램 파일(x86)에 속할 수 있습니다. |
| Adobe Creative Cloud의 Adobe Illustrator 17 | <ul><li>압축을 푼 폴더의 루트에서 CC를 클릭합니다. </li><li>사용하는 Adobe Illustrator의 비트 버전에 따라 win32 또는 win64를 클릭합니다.</li><li> `AdobeS7FXGFileFormat.aip`을(를) Adobe Illustrator의 플러그인 폴더에 복사합니다. (예: `C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`)</li></ul><br/>**참고**:이 예제 경로는 64비트 위치에 대한 것입니다.32비트 위치는 프로그램 파일(x86)에 속할 수 있습니다. |
| Adobe Creative Suite 6의 Adobe Illustrator 16 | <ul><li>압축을 푼 폴더의 루트에서 6.0을 클릭합니다. </li><li>사용하는 Adobe Illustrator의 비트 버전에 따라 win32 또는 win64를 클릭합니다. </li><li>AdobeS7FXGFileFormat.aip를 Adobe Illustrator의 플러그인 폴더에 복사합니다. (예: `C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`)</li></ul><br/>**참고**:이 예제 경로는 64비트 위치에 대한 것입니다.32비트 위치는 프로그램 파일(x86)에 속할 수 있습니다. |

### Mac

| 실행 중인 버전 | 수행할 작업 |
|--- |--- |
| Adobe Creative Cloud 2014의 Adobe Illustrator 18 | <ul><li>압축을 푼 폴더의 루트에서 CC-2014 > mac64를 클릭합니다.</li><li>라이브러리 > flame을 클릭한 다음 `aflame.framework` 폴더를 Adobe Illustrator 패키지 컨텐츠 폴더에 복사합니다. (예: `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`) (Adobe Illustrator의 패키지 내용 폴더를 열려면 Adobe illustrator CC 2014 아이콘을 마우스 오른쪽 버튼으로 클릭하고 컨텍스트 메뉴에서 패키지 내용 표시를 클릭합니다.)</li><li>동일한 라이브러리 폴더로 돌아가 `flamingo`를 클릭한 다음 `aflamingo.framework` 폴더를 이전 단계에서 사용한 것과 동일한 Adobe Illustrator 패키지 컨텐츠 폴더에 복사합니다.</li><li>1단계에서 선택한 mac64 폴더로 돌아간 다음 `AdobeS7FXGFileFormat.aip`를 Adobe Illustrator의 플러그인 폴더에 복사합니다. (예: `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`)</li></ul><br/> |
| Adobe Creative Cloud의 Adobe Illustrator 17 | <ul><li>압축을 푼 폴더의 루트에서 CC > mac64를 클릭합니다</li><li>`AdobeS7FXGFileFormat.aip` 폴더를 Adobe Illustrator의 플러그인 폴더에 복사합니다. (예: `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`)</li></ul><br/> |
| Adobe Creative Suite 6의 Adobe Illustrator 16 | <ul><li>압축을 푼 폴더의 루트에서 6.0 > mac}64를 클릭합니다</li><li>`AdobeS7FXGFileFormat.aip` 폴더를 Adobe Illustrator의 플러그인 폴더에 복사합니다. (예: `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`)</li></ul> |

이제 Adobe Illustrator에서 이 플러그인을 사용할 수 있습니다.

### 브라우저

* **썸네일 크기**
   * 찾아보기 패널의 [그리드 보기]에서 썸네일 이미지의 기본 크기를 결정합니다.
* **기본 자산 라이브러리 보기**
   * 빌드 집합에 대한 자산 라이브러리의 자산을 썸네일로 표시할지, 아니면 이름별로 표시할지 결정합니다. 자산 라이브러리에서 대량의 자산을 작업하는 경우 이름별로 자산을 볼 수 있습니다. 예를 들어 많은 PDF 파일이 포함된 큰 eCatalog를 작성하는 경우 이름별로 자산을 표시하여 목록을 더 짧게 만들 수 있습니다.
* **기본 브라우징 정렬 순서**
   * 찾아보기 패널에서 기본으로 표시되는 자산의 정렬 순서를 결정합니다. 메뉴에서 오름차순 또는 내림차순으로 정렬 기준을 선택합니다.
* **기본 브라우징 위치**
   * 브라우징 위치를 기본값인 마지막으로 찾은 폴더나 탐색하고 식별할 특정 위치로 설정할 수 있습니다. 브라우징 위치를 설정하여 파일과 폴더를 오름차순이나 내림차순으로 정렬할 수도 있습니다.
* **기본 브라우징 보기**
   * 찾아보기 패널을 처음 열었을 때 기본 보기 설정을 [그리드 보기] 또는 [목록 보기]로 결정합니다.
* **시작 화면 표시**
   * 시작 화면을 포함하여 시작 화면을 표시할지 여부를 결정합니다.
* **도구 설명 표시**
   * 단추, 메뉴, 탐색 링크 위로 마우스 포인터를 이동할 때 도구 설명의 표시 여부를 결정합니다. 도구 설명은 화면의 항목을 설명합니다.
* **바둑판 배경**
   * 이미지 뒤에 바둑판 배경 레이어를 표시하여 알파 채널을 가진 이미지의 투명한 부분을 쉽게 확인할 수 있습니다.
* **파일 크기 표시**
   * 탐색 시 자산의 파일 크기를 표시합니다.
* **검색에 UDF 포함**
   * 실행하는 대부분의 메타데이터 검색에 대한 시스템 성능 향상을 위해 선택 취소됨(기본값).

대부분의 메타데이터 검색에서 사용자 지정 필드를 포함하는 이점을 이용하는 경우, 이 선택 사항을 선택하여 이 기능을 켤 수 있습니다. 또는, [고급 검색]을 사용하여 사용자 지정 필드를 포함하는 것보다 더 선택 사항이 많고 빠른 검색 환경을 제공할 수 있습니다.

[고급 검색 수행](searching-assets.md#conducting_an_advanced_search)을 참조하십시오.

[사용자 지정 필드](application-setup.md#user_defined_fields)도 참조하십시오.

* **기본 검색 유형**
   * 기본 검색 유형인 [포함] 또는 [시작 문자]를 선택합니다.
* **Media Portal 기능 표시**
   * 미디어 카트 등의 Media Portal 기능에 액세스하려면 이 선택 사항을 선택합니다.
* **명령 피드백 표시**
   * 서버에 대한 명령 요청을 표시합니다.
* **내보내는 중 대화 상자 표시**
   * 내보내기 시 대화 상자를 표시합니다. 이 선택 사항을 선택 취소한 경우에도 [작업] 페이지로 이동하여 내보내기 결과를 검색할 수 있습니다.

## 이메일

* **이메일 선택 사항**
   * 업로드 및 게시 작업이 완료되면 이메일로 Dynamic Media Classic에 알려 주는 방법을 선택합니다. 작업 완료 알림은 경고나 오류가 발생한 경우에만 받아볼 수 있습니다.
* **이메일 범위**
   * 회사에 대한 모든 작업 이메일을 받을지, 아니면 직접 시작한 업로드 및 게시 작업에 대한 이메일만 받을지 결정합니다.
* **이메일 유형**
   * 업로드 및 게시 작업이 완료될 때 알림을 받을지 여부를 결정합니다.
* **언어**
* **기본 언어**
   * 인터페이스 언어를 결정합니다.
* **암호**
* **새 암호**
   * 새 유효한 암호를 입력합니다. 암호는 다음 요구 사항을 충족해야 합니다.
      * 8-25자 사이여야 합니다.
      * 소문자를 하나 이상 포함
      * 하나 이상의 대문자 포함
      * 하나 이상의 숫자 포함
      * 다음 특수 문자 중 하나 이상을 포함합니다.#$&amp;-_:{}
* **암호 다시 입력**
   * 입력된 암호가 정확한지 확인하기 위해 새 암호를 재입력합니다.
* **암호 만료일**
   * 보안 수단으로 암호가 72일 후 만료되도록 설정합니다. [예]를 선택하면 72일 후에 새 암호를 만들라는 메시지가 표시됩니다.
