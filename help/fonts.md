---
title: 글꼴
description: Dynamic Media Classic에서 글꼴을 사용하는 방법을 알아봅니다.
uuid: bddec9c2-8530-4bbd-8db7-1562a347e482
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 97cecd6a-30aa-44fe-a611-fd71b02fd5ae
feature: Dynamic Media Classic
role: Business Practitioner
exl-id: 186f4c7f-16f6-42f5-bc0e-55362c55e794
source-git-commit: 27d9a9b9f158846b54e4318119aec9e4dc9c4c0d
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 36%

---

# 글꼴{#fonts}

경우에 따라 Dynamic Media Classic에서 특정 글꼴로 텍스트를 입력하거나 렌더링하려면 글꼴 파일을 업로드해야 합니다. 예를 들어 템플릿 레이어의 텍스트에 특정 글꼴을 사용하려면 글꼴 파일을 업로드합니다. eCatalog 뷰어 페이지 번호를 특정 글꼴로 표시하려면 글꼴 파일을 업로드합니다.

Dynamic Media Classic에서는 다음 글꼴 유형을 지원합니다.

* 모든 TrueType 글꼴
* PostScript® 글꼴
* OpenType/TrueType 글꼴
* OpenType/PostScript 글꼴
* PhotoFonts

글꼴 파일을 업로드한 후 Dynamic Media Classic ID와 글꼴 이름을 변경하고, 정보 편집 화면에서 정보를 입력할 수 있습니다.

>[!NOTE]
>
>템플릿 계층에서 글꼴을 사용하려면 모든 글꼴 스타일(굵게, 기울임체, 굵게/기울임체 및 일반)을 업로드하는 것이 좋습니다. Dynamic Media Classic에서는 요청을 처리하기 위해 이러한 글꼴 스타일이 필요합니다. 일부 글꼴에는 자세한 커닝 정보가 포함되어 있으므로 글꼴과 관련된 모든 PostScript/Adobe Type 1 파일을 업로드하는 것이 좋습니다.

## 글꼴 파일 업로드 {#uploading-font-files}

다른 파일을 업로드할 때와 동일한 기술을 사용하여 글꼴 파일을 업로드합니다. Dynamic Media Classic 폴더에 글꼴 파일을 저장할 수 있습니다. [파일 업로드](uploading-files.md#uploading_your_files)를 참조하십시오.

## 글꼴 파일 정보 편집 {#editing-font-file-information}

글꼴의 ID 이름과 해당 유형 정보를 변경할 수 있습니다. 글꼴 파일을 편집하면 검색 시 도움이 되며 글꼴을 더 쉽게 식별할 수 있습니다.

[세부 사항 보기]에서 편집하려는 글꼴 파일을 찾아보기 패널에서 선택한 다음 [파일] > [정보 편집]을 선택합니다. [정보 편집] 화면이 열립니다. 다음 선택 사항을 선택한 다음 [전송] 단추를 선택합니다.

* **글꼴 이름**  - 이 이름은 글꼴이 게시될 때 글꼴을 식별합니다.

* **PostScript 이름**  - 이 이름은 글꼴의 전체 PostScript 이름입니다. 일반적으로 두께나 스타일을 나타냅니다.

* **RTF 이름**  - 이 이름은 템플릿 텍스트 레이어가 생성되는 RTF 편집기의 팝업 메뉴에 나타납니다.

* **글꼴 패밀리 이름**  - 이 이름은 스타일, 가중치 또는 글꼴 유형 표시기 없이 글꼴 이름이 나열됩니다.

* **글꼴 스타일**  - 옵션은 일반, 굵게, 기울임체 및 굵은 기울임체입니다.

* **글꼴 유형**  - 옵션이 TrueType과 Adobe Type 1입니다. 이러한 글꼴을 다른 이름으로 호출하는 경우 해당 이름을 입력할 수 있습니다.

* **글꼴 유형 약어**  - 옵션은 다음과 같습니다.

   * **** PDF/PostScript 렌더링 및 이미지 제공에 사용되는 TTFTtrueType 글꼴 파일입니다.

   * **** Adobe 글꼴 지표 정보를 포함하고 이미지 제공 시 사용되는 AFMAadobe PostScript 글꼴 파일입니다.

   * **** 이진 글꼴 지표 정보가 포함된 PFMAadobe PostScript 글꼴 파일입니다.

   * **** PDF/PostScript 렌더링 및 이미지 제공용으로 사용되는 바이너리 글꼴 개요 정보를 포함하는 PFBAadobe PostScript 글꼴 파일입니다.
