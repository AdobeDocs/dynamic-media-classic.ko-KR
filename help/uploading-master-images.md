---
title: 마스터 이미지 업로드
description: 마스터 이미지를 업로드하는 방법을 알아봅니다.
uuid: 50bcf2e2-852b-48f1-a7c7-5063a87ce9c1
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 8c94bafc-94cc-496f-a394-a945cd7b02cf
feature: Dynamic Media Classic,자산 관리
role: User
exl-id: 410ba80c-7f01-4cd0-9ab3-db9658757ba7
source-git-commit: 885fcd16559d31d3b9bad88705b4b6bec18515ee
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 15%

---

# 마스터 이미지 업로드{#uploading-master-images}

Dynamic Media Classic에 이미지를 업로드하기 전에 이미지가 가장 높은 품질의 크기와 포맷인지 확인하십시오. Dynamic Media Classic에서는 충분한 픽셀 수(긴 크기의 1500~2000픽셀)로 고품질 이미지를 업로드하는 것이 좋습니다. 이 크기 조정을 통해 필요한 모든 다이내믹 이미징을 사용할 수 있습니다.

이미지 업로드에 대한 자세한 내용은 [파일 업로드](uploading-files.md#uploading_files)를 참조하십시오.

**업로드할 마스터 이미지 준비:**

Dynamic Media Classic에 업로드하기 전에 마스터 이미지 파일을 준비합니다.

* **이미지 크기**  - 사용할 것으로 예상되는 가장 큰 크기 이미지를 만듭니다. 일반적인 이미지 크기는 가장 긴 크기의 1500픽셀에서 2500픽셀 사이입니다. 확대/축소 기능을 사용하려면 가장 긴 크기 2000픽셀 이상의 이미지를 사용하여 최적의 확대/축소 세부 사항을 확인하는 것이 좋습니다. Dynamic Media Classic은 이미지를 각각 최대 25메가픽셀까지 렌더링할 수 있습니다. 예를 들어, 5000 x 5000 MP 이미지 또는 최대 25MP의 다른 크기 조합을 사용할 수 있습니다.

* **파일 형식**  - Dynamic Media Classic은 TIFF, BMP, JPEG, PSD, GIF 및 EPS를 포함한 모든 표준 이미지 파일 형식을 지원합니다. 손실 없는 이미지 형식(TIFF 및 PNG)이 권장됩니다. JPEG 이미지를 사용하는 경우 최고 품질의 설정을 사용하십시오.

* **색상 공간**  - RGB는 웹 이미지 프레젠테이션을 위한 색상 공간입니다.인쇄에 일반적으로 사용되는 CMYK 이미지는 업로드할 때 자동으로 RGB로 변환됩니다. RGB로 전환하는 데 사용되는 임베드된 ICC 색상 프로필이 있는 CMYK 이미지를 업로드하는 것이 좋습니다. [ICC 프로필](/help/icc-profiles.md)을 참조하십시오.
