---
title: 글꼴
description: Adobe Dynamic Media Classic에서 글꼴을 사용하는 방법을 알아봅니다.
uuid: bddec9c2-8530-4bbd-8db7-1562a347e482
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 97cecd6a-30aa-44fe-a611-fd71b02fd5ae
feature: Dynamic Media Classic
role: User
exl-id: 186f4c7f-16f6-42f5-bc0e-55362c55e794
topic: Content Management
level: Intermediate
source-git-commit: 51c05c62448b39a75facb2e90cc9da5d0f26ab45
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 23%

---

# 글꼴{#fonts}

경우에 따라 Adobe Dynamic Media Classic에서 특정 글꼴로 텍스트를 입력하거나 렌더링하기 위해 글꼴 파일을 업로드해야 합니다. 예를 들어 템플릿 레이어의 텍스트에 특정 글꼴을 사용하려면 글꼴 파일을 업로드합니다. eCatalog 뷰어 페이지 번호를 특정 글꼴로 표시하려면 글꼴 파일을 업로드합니다.

Adobe Dynamic Media Classic은 다음 글꼴 유형을 지원합니다.

* 모든 TrueType 글꼴
* PostScript® 글꼴
* OpenType/TrueType 글꼴
* OpenType/PostScript 글꼴
* PhotoFonts

글꼴 파일을 업로드한 후 정보 편집 화면에서 해당 Adobe Dynamic Media Classic ID, 글꼴 이름 및 유형 정보를 변경할 수 있습니다.

>[!NOTE]
>
>Adobe Dynamic Media Classic 템플릿 레이어에서 글꼴을 사용하려면 모든 글꼴 스타일(굵게, 기울임체, 굵게/기울임체 및 보통)을 업로드하는 것이 좋습니다. Adobe Dynamic Media Classic은 요청을 처리하기 위해 이러한 글꼴 스타일이 필요합니다. 모두 업로드 중 `PostScript/Adobe Type1` 이러한 글꼴 중 일부에는 자세한 커닝 정보가 포함되어 있으므로 글꼴과 연관된 파일도 권장됩니다.

## 글꼴 파일 업로드 {#uploading-font-files}

다른 파일을 업로드할 때와 동일한 기술을 사용하여 글꼴 파일을 업로드합니다. 모든 Adobe Dynamic Media Classic 폴더에 글꼴 파일을 저장할 수 있습니다. [파일 업로드](uploading-files.md#uploading_your_files)를 참조하십시오.

## 글꼴 파일 정보 편집 {#editing-font-file-information}

글꼴의 ID 이름과 유형 정보를 변경할 수 있습니다. 글꼴 파일을 편집하면 검색 시 도움이 되며 글꼴을 더 쉽게 식별할 수 있습니다.

[찾아보기] 패널에서 [세부 사항 보기]에서 편집할 글꼴 파일을 선택하고 [파일] > [정보 편집]을 선택합니다. [정보 편집] 화면이 열립니다. 다음 옵션을 선택한 다음 을 선택합니다 **[!UICONTROL 제출]**.

* **[!UICONTROL 글꼴 이름]** - 이 이름은 게시할 때 글꼴을 식별합니다.

* **[!UICONTROL PostScript 이름]** - 이 이름은 글꼴의 전체 PostScript 이름입니다. 일반적으로 두께나 스타일을 나타냅니다.

* **[!UICONTROL RTF 이름]** - 이 이름은 템플릿 텍스트 레이어가 생성되는 RTF 편집기의 팝업 메뉴에 나타납니다.

* **[!UICONTROL 글꼴 패밀리 이름]** - 이 이름에는 스타일, 두께 또는 글꼴 유형 표시기 없이 글꼴 이름이 나열됩니다.

* **[!UICONTROL 글꼴 스타일]** - 옵션은 Plain, Bold, Italic 및 Bold-Italic 입니다.

* **[!UICONTROL 글꼴 유형]** - 옵션은 TrueType 및 Adobe Type 1입니다. 이러한 글꼴을 다른 이름으로 호출하는 경우 해당 이름을 입력할 수 있습니다.

* **[!UICONTROL 글꼴 유형 약어]** - 옵션은 다음과 같습니다.

   * **[!UICONTROL TTF]** - PDF/포스트스크립트 렌더링 및 이미지 제공에 사용되는 TrueType 글꼴 파일입니다.

   * **[!UICONTROL AFM]** - Adobe 글꼴 지표 정보가 포함되어 있으며 이미지 제공에 사용되는 Adobe PostScript 글꼴 파일입니다.

   * **[!UICONTROL PFM]** - 이진 글꼴 지표 정보가 포함된 Adobe PostScript 글꼴 파일입니다.

   * **[!UICONTROL PFB]** - 바이너리 글꼴 개요 정보가 포함된 Adobe PostScript 글꼴 파일로, PDF/PostScript 렌더링 및 이미지 제공에 사용됩니다.
