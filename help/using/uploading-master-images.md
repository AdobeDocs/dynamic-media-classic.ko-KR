---
title: 1차 이미지 업로드
description: Adobe Dynamic Media Classic에 기본 이미지를 업로드하는 방법을 알아봅니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 410ba80c-7f01-4cd0-9ab3-db9658757ba7
topic: Content Management
level: Intermediate
source-git-commit: 914fde11270dc731a261da3305b29dd573584d93
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 2%

---

# 1차 이미지 업로드{#uploading-master-images}

Adobe Dynamic Media Classic에 이미지를 업로드하기 전에 이미지가 가장 고품질의 크기와 포맷인지 확인하십시오. Adobe Dynamic Media Classic에서는 충분한 픽셀 수(긴 크기가 1500~2000픽셀)로 고품질 이미지를 업로드하는 것이 좋습니다. 이 크기를 조정하면 필요한 모든 Dynamic Imaging을 사용할 수 있습니다.

이미지 업로드에 대한 자세한 내용은 을 참조하십시오. [파일 업로드](uploading-files.md#uploading_files).

**업로드할 1차 이미지 준비:**

Adobe Dynamic Media Classic에 업로드하기 전에 1차 이미지 파일을 준비합니다.

* **이미지 크기** - 사용할 것으로 예상되는 가장 큰 크기의 이미지를 만듭니다. 일반적인 이미지 크기는 1500픽셀에서 2500픽셀까지 가장 긴 크기입니다. Adobe Dynamic Media Classic [확대/축소] 기능을 사용하려는 경우 최적의 확대/축소 세부 정보를 위해 가장 긴 크기의 이미지가 2000픽셀 이상인 이미지를 사용하는 것이 좋습니다. Adobe Dynamic Media Classic은 이미지를 각각 최대 2500만 픽셀까지 렌더링할 수 있습니다. 예를 들어 5000 × 5000 MP 이미지나 다른 크기의 조합을 최대 25MP까지 사용할 수 있습니다.

* **파일 형식** - Adobe Dynamic Media Classic은 TIFF, BMP, JPEG, PSD, GIF 및 EPS을 포함한 모든 표준 이미지 파일 형식을 지원합니다. 손실 없는 이미지 형식(TIFF 및 PNG)이 권장됩니다. JPEG 이미지를 사용하는 경우 최고 품질 설정을 사용하십시오.

* **색상 공간** - RGB은 웹 이미지 프레젠테이션의 색상 공간입니다. 인쇄에 일반적으로 사용되는 CMYK 이미지는 업로드할 때 자동으로 RGB으로 변환됩니다. RGB으로 전환하기 위해 임베드된 ICC(International Color Consortium) 색상 프로파일이 있는 CMYK 이미지를 업로드하는 것이 좋습니다. 참조: [ICC(International Color Consortium) 프로파일](/help/using/icc-profiles.md).
