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
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 41%

---

# ICC 프로필{#icc-profiles}

ICC(International Color Consortium) 프로파일은 이미지 파일을 한 색상 공간에서 다른 색상 공간으로 올바르게 변환하는 방법을 설명하는 파일입니다. ICC 프로필은 이미지의 올바른 색상을 가져오는 데 도움이 됩니다. 예를 들어 컴퓨터 모니터에 인쇄용으로 설계된 이미지를 올바르게 표시하려면 ICC 프로파일을 선택할 수 있습니다. 이 프로필은 이미지를 다른 색상 공간으로 전환하고 색상이 온라인에서 올바르게 표시되게 합니다.

Adobe Dynamic Media Classic에서 이미지를 업로드할 때 ICC 프로파일을 선택하여 이미지를 다른 색상 공간으로 변환할 수 있습니다. 모든 표준 Photoshop ICC 프로파일은 Adobe Dynamic Media Classic에서 기본적으로 사용할 수 있습니다. [업로드] 화면에서 색상 프로필 이름을 보려면 [색상 프로필] 메뉴를 선택합니다. 그런 다음 [사용자 지정 원본] > [대상]을 선택하고 [변환 원본] 및 [변환 대상] 메뉴에서 ICC 프로파일 이름을 선택합니다.

업로드 시 [이미지 편집 옵션](image-editing-options-upload.md#image-editing-options-at-upload)을 참조하세요.

기본 ICC 프로파일을 사용하는 것 외에도 다른 ICC 프로파일을 Adobe Dynamic Media Classic에 업로드하여 색상 공간 변환에 사용할 수 있도록 할 수 있습니다. 찾아보기 패널에서 세부 사항 보기로 전환하여 ICC 프로파일의 프로파일 클래스, 색상 공간 유형 및 PCS 유형을 조사합니다.

## ICC 프로파일 업로드 {#uploading-icc-profiles}

파일을 업로드할 때와 동일한 기술을 사용하여 ICC 프로필을 업로드합니다. 모든 Adobe Dynamic Media Classic 폴더에 ICC 프로파일을 저장할 수 있습니다.

[파일 업로드](uploading-files.md#uploading_your_files)를 참조하세요.

## ICC 프로파일 검사 {#examining-an-icc-profile}

ICC 프로파일을 검사하려면 [찾아보기] 패널에서 프로파일을 선택하고 [세부 사항 보기]에 표시합니다. 세부 사항 보기는 ICC 프로파일에 대한 다음 정보를 제공합니다.

* **[!UICONTROL 프로필 클래스]**: ICC(International Color Consortium)는 응용 프로그램 유형을 포함하도록 각 클래스를 정의합니다. 예를 들어 입력 프로필은 디지털 카메라, 스캐너 등의 장치에 적용되고 출력 프로필은 프린터에 적용됩니다.

* **[!UICONTROL 색상 공간 유형]**: 이 숫자는 ICC에서 정의한 프로필의 &quot;입력&quot; 색상 공간입니다. 색상 공간 유형은 색상 공간의 구성 요소 수와 이러한 구성 요소의 해석을 정의합니다. 예를 들어 RGB는 빨간색, 녹색 및 파란색의 세 가지 구성 요소로 이루어진 색상 공간입니다. 이 색상 공간 유형은 공간의 특정 색상 특성(예: 기본 색도)을 정의하지 않습니다.

* **[!UICONTROL PCS 유형]**: 이 PCS 유형은 프로필의 &quot;출력&quot; 색상 공간(프로필 연결 공간)입니다. 예를 들어 색상 프로필에서 RGB를 PCS로 전환한 다음 CMYK로 전환할 수 있습니다.

색상이나 이미지를 태그 지정하는 데 유용한 입력, 표시 또는 출력 프로필의 경우 PCS 유형은 XYZ 또는 Lab입니다. 이 프로필을 ICC 사양에 정의된 특정 색상 공간으로 해석합니다.
