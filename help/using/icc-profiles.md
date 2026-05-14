---
title: ICC(International Color Consortium) 프로파일
description: Adobe Dynamic Media Classic의 ICC 프로필에 대해 알아봅니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
feature: Dynamic Media Classic
role: User
exl-id: 989f2761-f5d0-4ece-b2a6-f7b4577aa8a2
topic: Administration, Content Management
level: Intermediate
autotag-review: '2026-05-13T19:59:42.608Z'
TQID: 'https://experienceleague.adobe.com/eGKamqA47mITzfyTuHoFYLfWEXOP0jAl5XWDpihGjZA'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 528
ht-degree: 31%

---

# ICC 프로필{#icc-profiles}

ICC(International Color Consortium) 프로파일은 이미지 파일을 한 색상 공간에서 다른 색상 공간으로 올바르게 변환하는 방법을 설명하는 파일입니다. ICC 프로필은 이미지의 올바른 색상을 가져오는 데 도움이 됩니다. 예를 들어 컴퓨터 모니터에 인쇄용으로 설계된 이미지를 올바르게 표시하려면 ICC 프로파일을 선택할 수 있습니다. 이 프로필은 이미지를 다른 색상 공간으로 전환하고 색상이 온라인에서 올바르게 표시되게 합니다.

Adobe Dynamic Media Classic에서 이미지를 업로드할 때 ICC 프로파일을 선택하여 이미지를 다른 색상 공간으로 변환할 수 있습니다. 모든 표준 Photoshop ICC 프로파일은 Adobe Dynamic Media Classic에서 기본적으로 사용할 수 있습니다. [업로드] 화면에서 색상 프로필 이름을 보려면 [색상 프로필] 메뉴를 선택합니다. [사용자 지정 전환]을 선택한 다음 [전환 출처] 및 [전환 타겟] 메뉴에서 ICC 프로필 이름을 선택합니다.

업로드 시 [이미지 편집 옵션](image-editing-options-upload.md#image-editing-options-at-upload)을 참조하세요.

기본 ICC 프로파일을 사용하는 것 외에도 다른 ICC 프로파일을 Adobe Dynamic Media Classic에 업로드하여 색상 공간 변환에 사용할 수 있도록 할 수 있습니다. 찾아보기 패널에서 세부 사항 보기로 전환하여 ICC 프로파일의 프로파일 클래스, 색상 공간 유형 및 PCS 유형을 조사합니다.

요약하면 ICC 프로파일의 주요 사항은 다음과 같습니다.

* ICC 프로파일을 사용하면 이미지 파일에 대해 서로 다른 색상 공간 간에 올바른 색상 변환이 가능합니다.
* Adobe Dynamic Media Classic은 강력한 이미지 변환을 위해 모든 표준 Photoshop ICC 프로파일을 통합합니다.
* 사용자 정의 ICC 프로파일은 고급 색상 공간 변환 요구 사항을 위한 유연성을 추가합니다.
* 세부 정보 보기에서 프로필 클래스 및 PCS 유형과 같은 세부 정보를 보면 ICC 설정을 관리하는 데 도움이 됩니다.
* ICC 프로파일을 업로드하는 것은 간단하며 Dynamic Media Classic의 폴더 간에 쉽게 액세스할 수 있습니다.


## ICC 프로파일 업로드 {#uploading-icc-profiles}

파일을 업로드할 때와 동일한 기술을 사용하여 ICC 프로필을 업로드합니다. 모든 Adobe Dynamic Media Classic 폴더에 ICC 프로파일을 저장할 수 있습니다.

[파일 업로드](uploading-files.md#uploading_your_files)를 참조하세요.

## ICC 프로파일 검사 {#examining-an-icc-profile}

ICC 프로파일을 검사하려면 [찾아보기] 패널에서 프로파일을 선택하고 [세부 사항 보기]에 표시합니다. 세부 사항 보기는 ICC 프로파일에 대한 다음 정보를 제공합니다.

* **[!UICONTROL 프로필 클래스]**: ICC는 응용 프로그램 유형을 포함하도록 각 클래스를 정의합니다. 예를 들어 입력 프로필은 디지털 카메라 및 스캐너와 같은 장치에 적용됩니다. 출력 프로필은 프린터에 적용됩니다.

* **[!UICONTROL 색상 공간 유형]**: 이 숫자는 ICC에서 정의한 프로필의 &quot;입력&quot; 색상 공간입니다. 색상 공간 유형은 색상 공간의 구성 요소 수와 이러한 구성 요소의 해석을 정의합니다. 예를 들어 RGB는 빨간색, 녹색 및 파란색의 세 가지 구성 요소로 이루어진 색상 공간입니다. 이 색상 공간 유형은 공간의 특정 색상 특성(예: 기본 색도)을 정의하지 않습니다.

* **[!UICONTROL PCS 유형]**: 이 PCS 유형은 프로필의 &quot;출력&quot; 색상 공간(프로필 연결 공간)입니다. 예를 들어 색상 프로필에서 RGB를 PCS로 전환한 다음 CMYK로 전환할 수 있습니다.

색상 또는 이미지에 태그를 지정하는 데 유용한 입력, 표시 또는 출력 프로필의 경우 PCS 유형은 XYZ 또는 Lab입니다. 이 프로필을 ICC 사양에 정의된 특정 색상 공간으로 해석합니다.
