---
title: ICC 프로필
seo-title: ICC 프로필
description: 널
seo-description: ICC 프로파일에 대한 자세한 내용을 살펴보십시오.
uuid: 708 FF 2 AD -9 A 47-4 E 3 E-B 643-5 B 19648 F 726 B
contentOwner: 관리
content-type: 참조
products: sg_ Experiencemanager/dynamic-media-scene -7
geptopics: sg_ scenesevenondemand_ pk/categories/support_ files
discoiquuid: 44 F 1 B 4 C 4-6 D 7 F -4 E 0 F -84 CE -11 D 26745 E 0 F 0
translation-type: tm+mt
source-git-commit: 75f006fd81b0fe2dad5479cdd98e45eaada46b2a

---


# ICC 프로필{#icc-profiles}

ICC(International Color Consortium) 프로필은 이미지 파일을 한 색상 공간에서 다른 색상 공간으로 올바르게 전환하는 방법을 설명하는 파일입니다. ICC 프로필은 이미지의 올바른 색상을 가져오는 데 도움이 됩니다. 예를 들어 컴퓨터 모니터에 인쇄하기 위한 이미지를 올바르게 표시하기 위해 ICC 프로필을 선택할 수 있습니다. 이 프로필은 이미지를 다른 색상 공간으로 전환하고 색상이 온라인에서 올바르게 표시되게 합니다.

Scene7 Publishing System에서 이미지를 업로드할 때 ICC 프로필을 선택하여 이미지를 다른 색상 공간으로 전환할 수 있습니다. SPS에서는 기본적으로 모든 표준 Photoshop ICC 프로필을 사용할 수 있습니다. [업로드] 화면에서 색상 프로필 이름을 보려면 [색상 프로필] 메뉴를 선택합니다. [사용자 지정 전환]을 선택한 다음 [전환 출처] 및 [전환 타겟] 메뉴에서 ICC 프로필 이름을 선택합니다. [업로드 시 이미지 편집 선택 사항](image-editing-options-upload.md#image-editing-options-at-upload)을 참조하십시오.

기본 ICC 프로필을 사용하는 것은 물론 다른 ICC 프로필을 SPS로 업로드하고 색상 공간 전환에 사용할 수 있게 설정할 수 있습니다. 찾아보기 패널에서 [세부 사항 보기]로 전환하여 ICC 프로필의 프로필 클래스, 색상 공간 유형 및 PCS 유형을 조사합니다.

## ICC 프로필 업로드 {#uploading-icc-profiles}

파일을 업로드할 때와 동일한 기술을 사용하여 ICC 프로필을 업로드합니다. ICC 프로필은 임의 SPS 폴더에 저장할 수 있습니다. [파일 업로드](uploading-files.md#uploading_your_files)를 참조하십시오.

## ICC 프로필 검사 {#examining-an-icc-profile}

ICC 프로필을 검사하려면 찾아보기 패널에서 ICC 프로필을 선택하고 [세부 사항 보기]에 표시합니다. [세부 사항 보기]에서는 ICC 프로필에 대한 다음 정보를 제공합니다.

**프로필 클래스** ICC (International Color Consortium) 는 각 클래스를 정의하여 애플리케이션 유형을 다룹니다. 예를 들어 입력 프로필은 디지털 카메라, 스캐너 등의 장치에 적용되고 출력 프로필은 프린터에 적용됩니다.

**색상 공간 유형** 이 숫자는 ICC에서 정의한 대로 프로파일의 "입력" 색상 공간입니다. 색상 공간 유형은 색상 공간의 구성 요소 수와 이러한 구성 요소의 해석을 정의합니다. 예를 들어 RGB는 빨간색, 녹색 및 파란색의 세 가지 구성 요소로 이루어진 색상 공간입니다. 이 색상 공간 유형은 공간의 특정 색상 특성(예: 기본 색도)을 정의하지 않습니다.

**PCS 유형** 이 PCS 유형은 프로필의 "출력" 색상 공간 (프로필 연결 공간) 입니다. 예를 들어 색상 프로필에서 RGB를 PCS로 전환한 다음 CMYK로 전환할 수 있습니다.

색상이나 이미지를 태그 지정하는 데 유용한 입력, 표시 또는 출력 프로필의 경우 PCS 유형은 XYZ 또는 Lab입니다. 이 프로필을 ICC 사양에 정의된 특정 색상 공간으로 해석합니다.