---
title: 글꼴
seo-title: 글꼴
description: 널
seo-description: Dynamic Media Classic에서 글꼴을 사용하는 방법을 살펴봅니다.
uuid: bddec 9 c 2-8530-4 bbd -8 db 7-1562 a 347 e 482
contentOwner: 관리
content-type: 참조
products: sg_ Experiencemanager/dynamic-media-scene -7
geptopics: sg_ scenesevenondemand_ pk/categories/support_ files
discoiquuid: 97 CECD 6 A -30 AA -44 FE-A 611-FD 71 B 02 FD 5 AE
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# 글꼴{#fonts}

텍스트를 특정 글꼴로 입력하거나 렌더링하기 위해 Scene7 Publishing System에서 글꼴 파일을 업로드해야 하는 경우도 있습니다. 예를 들어 템플릿 레이어의 텍스트에 특정 글꼴을 사용하려면 글꼴 파일을 업로드합니다. eCatalog 뷰어 페이지 번호를 특정 글꼴로 표시하려면 글꼴 파일을 업로드합니다.

Dynamic Media Classic는 다음과 같은 글꼴 유형을 지원합니다.

* 모든 TrueType 글꼴
* PostScript® 글꼴
* OpenType/TrueType 글꼴
* OpenType/PostScript 글꼴
* PhotoFonts

글꼴 파일을 업로드한 후 [정보 편집] 화면에서 해당 SPS ID, 글꼴 이름 및 유형 정보를 변경할 수 있습니다.

>[!NOTE]
>
>템플릿 레이어에서 글꼴을 사용하려는 경우 Dynamic Media Classic 에서는 모든 글꼴 스타일 (굵게, 기울임체, 굵게/기울임꼴 및 일반) 를 업로드할 것을 권장합니다. 요청을 처리하려면 Dynamic Media Classic에서 이러한 글꼴 스타일을 필요로 합니다. 일부 글꼴에는 자세한 커닝 정보가 포함되어 있으므로 글꼴과 관련된 모든 PostScript/Adobe Type 1 파일을 업로드하는 것이 좋습니다.

## 글꼴 파일 업로드 {#uploading-font-files}

다른 파일을 업로드할 때와 동일한 기술을 사용하여 글꼴 파일을 업로드합니다. 글꼴 파일은 임의 SPS 폴더에 저장할 수 있습니다. [파일 업로드](uploading-files.md#uploading_your_files)를 참조하십시오.

## 글꼴 파일 정보 편집 {#editing-font-file-information}

글꼴의 ID 이름과 유형 정보를 변경할 수 있습니다. 글꼴 파일을 편집하면 검색 시 도움이 되며 글꼴을 더 쉽게 식별할 수 있습니다.

[세부 사항 보기]에서 편집하려는 글꼴 파일을 찾아보기 패널에서 선택한 다음 [파일] &gt; [정보 편집]을 선택합니다. [정보 편집] 화면이 열립니다. 다음 선택 사항을 선택한 다음 [전송] 단추를 선택합니다.

**글꼴 이름** 이 이름은 글꼴을 게시할 때 식별합니다.

**PostScript 이름** 이 이름은 글꼴의 전체 PostScript 이름입니다. 일반적으로 두께나 스타일을 나타냅니다.

**RTF 이름** 이 이름은 템플릿 텍스트 레이어가 만들어지는 RTF 편집기의 팝업 메뉴에 표시됩니다.

**글꼴 모음 이름** 이 이름에 스타일, 두께 또는 글꼴 유형 표시기 없이 글꼴 이름이 표시됩니다.

**글꼴 스타일** 옵션은 일반, 굵게, 기울임꼴 및 굵은 기울임체로 표시됩니다.

**글꼴 유형** Truetype 및 Adobe Type 1 입니다. 이러한 글꼴을 다른 이름으로 호출하는 경우 해당 이름을 입력할 수 있습니다.

**글꼴 유형 약어** 옵션은 다음과 같습니다.

**TTF** truetype 글꼴 파일을 PDF/PostScript 렌더링 및 이미지 제공에 사용합니다.

**Adobe 글꼴 지표 정보가 포함되어 있고 이미지 제공에 사용되는 AFM** Adobe PostScript 글꼴 파일입니다.

**이진 글꼴 지표 정보가 포함된 PFM** Adobe PostScript 글꼴 파일입니다.

**바이너리 글꼴 외곽선 정보가 포함되어 있고 PDF/PostScript 렌더링 및 이미지 제공에 사용되는 PFB** Adobe PostScript 글꼴 파일입니다.
