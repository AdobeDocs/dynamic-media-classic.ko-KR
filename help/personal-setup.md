---
title: 개인 설정
description: 모든 사용자는 Adobe Dynamic Media Classic의 개인 설정 화면에서 설정을 변경할 수 있습니다.
uuid: 29cb825a-f158-4a1e-9d5f-7636ee411b6e
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 6314e7b7-5bde-4fe2-8674-e4fc525d4d1c
feature: Dynamic Media Classic
role: Admin,User
exl-id: a019f973-7647-466f-8af3-5312e9225e89
source-git-commit: cb55e09a997b9d36002c4ac429603576d52fb8bd
workflow-type: tm+mt
source-wordcount: '823'
ht-degree: 25%

---

# 개인 설정 {#personal-setup}

모든 사용자는 [개인 설정] 화면의 설정을 변경할 수 있습니다. 개인 설정 화면을 열려면 다음 위치로 이동합니다. **[!UICONTROL 설정]** > **[!UICONTROL 개인 설정]**.

>[!NOTE]
>
>개인 설정 화면에는 Adobe Dynamic Media Classic에서 보유하고 있는 회사 관리자, 관리자 또는 사용자 역할이 나열됩니다.

[개인 설정] 설정은 찾아보기 패널의 기본적인 행동, 이메일을 전달받는 방식, 암호 설정을 제어합니다. 다음을 선택하십시오. **[!UICONTROL 저장]** 이 설정을 변경한 후에.

## 내 계정 정보

계정 이름, 이름, 사용자 이름(이메일 주소) 및 지정된 사용자 역할을 식별합니다.

## 데스크톱

* **이미지 캐시 지우기** - 컴퓨터에서 모든 Adobe Dynamic Media 캐시 이미지 파일을 제거합니다.
* **자산 캐시 지우기** Adobe - 컴퓨터에서 Dynamic Media 캐시 에셋 파일을 모두 제거합니다.

데스크탑 앱을 사용하여 이미지 및 자산 캐시를 지우는 것 외에도 파일 시스템에서 직접 캐시를 지울 수 있습니다. 운영 체제를 기준으로 다음 위치로 이동합니다.

* macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
* Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Creative Suite Extension

**Adobe Dynamic Media Creative Suite 확장을 설치하려면:**

1. Adobe Dynamic Media Classic의 도구 모음에서 **[!UICONTROL 설정]** > **[!UICONTROL 개인 설정]**, Creative Suite 확장에서 을 선택합니다. **[!UICONTROL 지금 다운로드]** 을(를) 다운로드하려면 `s7csxs.zxp` 파일.
1. 다음 항목 선택 **[!UICONTROL 설치]** 및 **[!UICONTROL 시스템 요구 사항]** 확장에 대한 추가 정보 링크.

<!--    A readme file is included at the root of the unzipped file to provide you with additional information about the extension.

1. Depending on your installed operating system, do one of the following: -->

<!-- #### Windows

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, select CC-2014.</li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64.</li><li>Select libraries > flame, and then copy `aflame.dll` to Adobe Illustrator's executable folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`. </li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead. <br/><ul><li>Return to the same libraries folder, select flamingo, and then copy `aflamingo.dll` to the same Adobe Illustrator executable folder that you used in the previous step. </li><li>Return to the win32 or win64 folder that you selected in step 2, and then copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`. </li></ul> <br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, select CC. </li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64.</li><li> Copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, select 6.0. </li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64. </li><li>Copy AdobeS7FXGFileFormat.aip to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|

#### Mac

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, select CC-2014 > mac64.</li><li>Select libraries > flame, and then copy the `aflame.framework` folder to Adobe Illustrator package contents folder. For example, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. (To open Adobe Illustrator’s package contents folder, right-select on the Adobe illustrator CC 2014 icon and select Show Package Contents from context menu).</li><li>Return to the same libraries folder, select `flamingo`, and then copy the `aflamingo.framework` folder to the same Adobe Illustrator package contents folder that you used in the previous step.</li><li>Return to the mac64 folder that you selected in step 1, and then copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, select CC > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, select 6.0 > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul>|

The plug-in is now available for you to use in Adobe Illustrator. -->

## 브라우저

* **[!UICONTROL 썸네일 크기]** - [찾아보기] 패널의 [격자 보기]에서 축소판 이미지의 기본 크기를 결정합니다.
* **[!UICONTROL 기본 자산 라이브러리 보기]** - 빌드 세트에 대한 자산 라이브러리의 자산을 썸네일로 표시할지 또는 이름별로 표시할지 여부를 결정합니다. 자산 라이브러리에서 대량의 자산을 작업하는 경우 이름별로 자산을 볼 수 있습니다. 예를 들어 많은 PDF 파일이 포함된 큰 eCatalog를 작성하는 경우 이름별로 자산을 표시하여 목록을 더 짧게 만들 수 있습니다.
* **[!UICONTROL 기본 찾아보기 정렬 순서]** - 탐색 패널에 에셋이 기본적으로 표시되는 순서를 결정합니다. 메뉴에서 오름차순 또는 내림차순으로 정렬 기준을 선택합니다.
* **[!UICONTROL 기본 찾아보기 위치]** - 찾아보기 위치를 기본, 마지막으로 검색한 폴더 또는 탐색하고 식별한 특정 위치로 설정할 수 있습니다. 브라우징 위치를 설정하여 파일과 폴더를 오름차순이나 내림차순으로 정렬할 수도 있습니다.
* **[!UICONTROL 기본 찾아보기 보기]** - [찾아보기] 패널을 처음 열 때 표시되는 기본 보기가 [격자 보기]인지 [목록 보기]인지 결정합니다.
* **[!UICONTROL 시작 화면 표시]** - 시작 시작 시작 화면을 포함하여 시작 화면을 표시할지 여부를 결정합니다.
* **[!UICONTROL 툴팁 표시]** - 포인터를 단추, 메뉴 및 탐색 링크 위로 이동할 때 도구 설명을 표시할지 여부를 결정합니다. 도구 설명에 화면 사용자 인터페이스 항목이 설명되어 있습니다.
* **[!UICONTROL 바둑판 배경]** - 이미지 뒤에 바둑판 레이어를 표시하여 알파 채널이 있는 이미지의 투명한 영역을 쉽게 볼 수 있습니다.
* **[!UICONTROL 파일 크기 표시]** - 검색할 때 에셋의 파일 크기를 표시합니다.
* **[!UICONTROL 검색에 UDF 포함]** - 실행하는 대부분의 메타데이터 검색에 대한 시스템 성능을 향상시키기 위해 선택을 취소했습니다(기본값).

   대부분의 메타데이터 검색에서 사용자 지정 필드를 포함하는 이점을 이용하는 경우, 이 선택 사항을 선택하여 이 기능을 켤 수 있습니다. 또는, [고급 검색]을 사용하여 사용자 지정 필드를 포함하는 것보다 더 선택 사항이 많고 빠른 검색 환경을 제공할 수 있습니다.

   [고급 검색 수행](searching-assets.md#conducting_an_advanced_search)을 참조하십시오.

   [사용자 지정 필드](application-setup.md#user_defined_fields)도 참조하십시오.

* **[!UICONTROL 기본 검색 유형]** - 다음 두 옵션 중에서 선택할 수 있습니다. **[!UICONTROL 다음 포함]** 지정한 값에 대한 전체 문자열을 검색합니다. **[!UICONTROL 시작]** 는 문자열의 시작부터 검색하고 보다 빠르게 결과를 반환합니다. **[!UICONTROL 다음 포함]**. 두 옵션 모두 다음에 설정된 기본값을 무시합니다. **[!UICONTROL 설정]** > **[!UICONTROL 응용 프로그램 설정]** > **[!UICONTROL 응용 프로그램 일반 설정]** 관리자.
* **[!UICONTROL 명령 피드백 표시]** - 서버에 대한 명령 요청 표시를 켜려면 선택하고, 끄려면 선택을 취소합니다.
* **[!UICONTROL 내보내는 중 대화 상자 표시]** - 내보내는 동안 팝업 대화 상자를 표시하려면 선택합니다. 이 옵션을 선택 해제(해제)해도 내보내기 결과를 검색하기 위해 작업 페이지로 이동할 수 있습니다.

## 이메일

* **[!UICONTROL 이메일 옵션]** - 업로드 및 게시 작업이 완료되면 Adobe Dynamic Media Classic에서 이메일로 알릴 방법을 선택하십시오. 작업 완료 알림은 경고나 오류가 발생한 경우에만 받아볼 수 있습니다.
* **[!UICONTROL 이메일 범위]** - 회사에 대한 모든 작업 이메일을 받는지 또는 시작한 업로드 및 게시 작업에 대한 전자 메일만 받는지 여부를 결정합니다.
* **[!UICONTROL 이메일 유형]** - 업로드 작업 및 게시 작업이 완료될 때 알림을 받을지 여부를 결정합니다.

## 언어

* **[!UICONTROL 기본 언어]** - 인터페이스에 사용할 언어를 결정합니다.

## 암호

* **[!UICONTROL 현재 암호]** - 현재 암호로 암호를 입력합니다.
* **[!UICONTROL 새 암호]** - 유효한 새 암호를 입력합니다. 암호는 다음 요구 사항을 충족해야 합니다.
   * 길이는 8~25자 사이여야 합니다.
   * 소문자를 하나 이상 포함해야 합니다.
   * 대문자를 하나 이상 포함해야 합니다.
   * 숫자를 하나 이상 포함해야 합니다.
   * 다음 특수 문자 중 하나 이상을 포함해야 합니다. `# $ & - _ : { }`
* **[!UICONTROL 암호 다시 입력]** - 새 암호를 다시 입력하여 올바르게 입력했는지 확인합니다.
* **[!UICONTROL 암호 만료]** - 72일 이후에 암호가 만료되는지 여부를 보안 기준으로 결정합니다. [예]를 선택하면 72일 이후 암호를 생성하라는 메시지가 표시됩니다.
