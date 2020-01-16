---
title: 이미지 품질 최적화 우수 사례
seo-title: 이미지 품질 최적화 우수 사례
description: 널
seo-description: 이미지 품질을 최적화하기 위한 모범 사례를 살펴보십시오.
uuid: 102e83fe-ee2a-443b-ba92-6ad5cc3daef0
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 8164466e-2520-482a-88ec-6191fdc77ea3
translation-type: tm+mt
source-git-commit: 6b0833287291f6475ab15106e8f33ed0dda0b2d4

---


# 이미지 품질 최적화 우수 사례{#best-practices-for-optimizing-the-quality-of-your-images}

허용되는 결과를 렌더링하는 데는 많은 요소가 기여하므로 이미지 품질 최적화 프로세스는 시간이 많이 소요될 수 있습니다. 또한 이미지 품질은 개인마다 다르게 생각하므로 결과는 어느 정도 주관적입니다. 따라서 구조화된 실험이 중요합니다.

Dynamic Media Classic에는 이미지를 조정 및 최적화하고 결과를 렌더링하기 위한 100개 이상의 이미지 제공 명령이 포함되어 있습니다. 다음 지침은 프로세스를 간소화하고 일부 필수 명령 및 우수 사례를 사용하여 좋은 결과를 빨리 얻는 데 도움이 될 수 있습니다.

스마트 [이미징을](https://helpx.adobe.com/experience-manager/6-3/assets/using/imaging-faq.html)참조하십시오.

## Best practices for image format (&amp;fmt=) {#best-practices-for-image-format-fmt}

* JPG 또는 PNG는 양질의 이미지를 관리할 수 있는 크기 및 용량으로 제공하는 데 적합합니다.
* URL에 형식 명령을 제공하지 않으면 기본적으로 JPG로 전달됩니다.
* JPG는 10:1 비율로 압축하며 일반적으로 작은 크기의 이미지 파일을 만듭니다. PNG는 이미지에 흰색 배경이 들어 있을 때와 같이 일부 경우를 제외하면 약 2:1 비율로 압축합니다. 일반적으로 PNG 파일 크기는 JPG 파일보다 큽니다.
* JPG는 손실 압축을 사용하며, 이것은 압축 중에 그림 요소(픽셀)가 제거됨을 의미합니다. 반면에 PNG는 비손실 압축을 사용합니다.
* JPG는 종종 가장자리와 대비가 선명한 합성 이미지보다 원본에 더 충실한 사진 이미지를 압축하는 데 사용합니다.
* 이미지에 투명도가 포함되어 있는 경우, JPG는 투명도를 지원하지 않으므로 PNG를 사용합니다.

As a best practice for image format, start with the most common setting `&fmt=JPG`.

## 이미지 크기 우수 사례 {#best-practices-for-image-size}

동적으로 이미지 크기를 줄이는 것은 다이내믹 미디어 이미지 제공에서 수행하는 가장 일반적인 작업 중 하나입니다. 이 작업에는 크기 지정이 포함되며, 원할 경우 이미지의 크기를 줄이는 데 사용되는 다운샘플링 모드 지정도 포함됩니다.

* For image sizing, the best and most straightforward approach is to use `&wid=<value>` and `&hei=<value>` or just `&hei=<value>`. 이 매개 변수들은 종횡비에 따라 이미지 너비를 자동으로 설정합니다.
* `&resMode=<value>` 다운샘플링에 사용되는 알고리즘을 제어합니다. 다음으로 `&resMode=sharp2`시작하십시오. 이 값은 최상의 이미지 품질을 제공합니다. While using the downsampling value `=bilin` is faster, it often results in the aliasing of artifacts.

이미지 크기 조정, 사용 `&wid=<value>&hei=<value>&resMode=sharp2` 또는 `&hei=<value>&resMode=sharp2`

## 이미지 선명하게 하기 우수 사례 {#best-practices-for-image-sharpening}

이미지 선명하게 하기는 웹 사이트에서 이미지를 제어하는 가장 복잡한 작업으로, 많은 실수가 발생합니다. 다음 유용한 리소스를 참조하여 Dynamic Media Classic에서 선명하게 하기 및 언샵 마스크가 작동하는 방식에 대해 자세히 알아보십시오.

Best practices white paper [Sharpening images in Adobe Scene7 Publishing System and on Image Server](/help/assets/s7_sharpening_images.pdf).

또한 [언샵 마스크로](https://helpx.adobe.com/photoshop/atv/cs6-tutorials/sharpening-an-image-with-unsharp-mask.html)이미지 선명하게 하기를 참조하십시오.

Dynamic Media Classic을 사용하면 통합, 전달 시 또는 두 가지 모두에서 이미지를 선명하게 만들 수 있습니다. 하지만 대부분의 경우, 두 가지 방식을 모두 사용하지는 않고 어느 한 가지 방법만 사용하여 이미지를 선명하게 해야 합니다. URL에서 제공 시 이미지를 선명하게 하면 일반적으로 가장 좋은 결과를 얻게 됩니다.

사용할 수 있는 이미지 선명하게 하기 방법에는 다음 두 가지가 있습니다.

* Simple sharpening ( `&op_sharpen`) - Similar to the sharpen filter used in Photoshop, simple sharpening applies basic sharpening to the final view of the image following dynamic resizing. 하지만 이 방법은 사용자가 구성할 수 없습니다. The best practice is to not use `&op_sharpen` unless required.
* Unsharp masking ( `&op_USM`) - Unsharp masking is an industry standard sharpening filter. 아래의 지침에 따라 언샵 마스킹으로 이미지를 선명하게 하는 것이 좋습니다. 언샵 마스킹을 사용하면 다음 3가지 매개 변수를 제어할 수 있습니다.

   * `&op_sharpen=amount,radius,threshold`

      * `amount` (0-5, 효과의 강도)
      * `radius` (0-250, 선명해진 개체 둘레에 그려진 &quot;선명하게 하는 선&quot;의 너비에 대한 픽셀 단위 측정값)

         매개 변수 `radius`와 `amount`는 서로 반대로 작용합니다. Reducing `radius` can be compensated by increasing `amount`. `Radius`를 사용하면 높은 값은 넓은 범위의 픽셀을 선명하게 하는 반면, 낮은 값은 가장자리 픽셀만 선명하게 하는 방식으로 미세하게 조정할 수 있습니다.

      * `threshold` (0-255, 효과의 민감도)

         이 매개 변수는, 가장자리 픽셀로 간주되고 필터가 선명하게 하기 전에, 선명하게 되는 픽셀과 주변 영역 간의 필수 차이를 결정합니다. 임계값은 피부 톤과 같이 유사한 색상 영역을 지나치게 선명하게 하는 것을 방지하는 데 유용합니다. 예를 들어 임계값 12는 &quot;노이즈&quot;를 추가하지 않도록 피부 톤 밝기에서 약간의 변형을 무시하는 반면, 속눈썹이 피부와 접촉하는 지점과 같은 고대비 영역에는 여전히 가장자리 대비를 추가합니다.
      필터와 함께 사용하는 우수 사례 등 이러한 세 가지 매개 변수를 설정하는 방법에 대한 자세한 내용은 다음 리소스를 참조하십시오.

      Dynamic Media Classic 도움말 항목에서는 이미지 [선명하게](https://help.adobe.com/en_US/scene7/using/WS389B162D-2981-41e5-9253-15D22D2ECBC8.html)만들기에 대해 설명합니다.

      Best practices white paper [Sharpening images in Adobe Scene7 Publishing System and on Image Server](/help/assets/s7_sharpening_images.pdf).

   * Dynamic Media Classic에서는 네 번째 매개 변수를 제어할 수도 있습니다.단색( `0,1`). 이 매개 변수는 언샵 마스킹이 값 `0`을 따로따로 사용하여 각 색상 구성 요소에 적용될지, 아니면 값 `1`을 사용하여 이미지 밝기/강도에 적용될지를 결정합니다.


언샵 마스크 반경 매개 변수로 시작하는 것이 좋습니다. 시작할 수 있는 반경 설정은 다음과 같습니다.

* 웹 사이트: 0.2-0.3픽셀
* 사진 인쇄(250-300ppi): 0.3-0.5픽셀
* 오프셋 인쇄(266-300ppi): 0.7-1.0픽셀
* 캔버스 인쇄(150ppi): 1.5-2.0픽셀

양을 1.75에서 4까지 점진적으로 늘립니다. 선명하게 하기가 여전히 원하는 대로 되지 않을 경우, 소수점만큼 반경을 늘리고 다시 양을 1.75에서 4까지 실행합니다. 필요에 따라 반복합니다.

모노크롬 매개 변수 설정을 0으로 둡니다.

## JPEG 압축(&amp;qlt=) 우수 사례 {#best-practices-for-jpeg-compression-qlt}

* 이 매개 변수는 JPG 인코딩 품질을 제어합니다. 값이 클수록 이미지 품질은 높지만 파일 크기도 큼을 의미하고, 값이 작을수록 이미지 품질은 낮지만 파일 크기도 작음을 의미합니다. 이 매개 변수의 범위는 0-100입니다.
* 품질에 대해 최적화하기 위해, 매개 변수 값을 100으로 설정하지 마십시오. 설정 90 또는 95와 100 간의 차이는 거의 감지할 수 없지만, 100은 이미지 파일의 크기를 불필요하게 늘립니다. Therefore, to optimize for quality but avoid image files becoming too large, set the `qlt=` value to 90 or 95.
* To optimize for a small image file size but keep image quality at an acceptable level, set the `qlt=` value to 80. 70에서 75 아래의 값은 상당한 이미지 품질 저하를 초래합니다.
* As a best practice, to stay in the middle, set the `qlt=` value to 85 to stay in the middle.
* `qlt=`=에 색도 플래그 사용

   * The `qlt=` parameter has a second setting that lets you turn on RGB chromaticity downsampling using the normal value `,0` (default), or turn it off using the value `,1`.
   * To keep it simple, start with RGB chromaticity downsampling turned off ( `,1`). 이렇게 설정하면 특히 선명한 가장자리와 대비가 많은 합성 이미지의 경우 일반적으로 나은 이미지 품질을 얻을 수 있습니다.

As a best practice for JPG compression use `&qlt=85,0`.

## Best practices for JPEG sizing (&amp;jpegSize=) {#best-practices-for-jpeg-sizing-jpegsize}

`jpegSize`는 메모리가 제한된 장치에 전달할 이미지가 특정 크기를 초과하지 않도록 사용하려는 경우에 유용한 매개 변수입니다.

* This parameter is set in kilobytes ( `jpegSize=<size_in_kilobytes>`). 이미지 제공에 허용되는 최대 크기를 정의합니다.
* `&jpegSize=` jpg 압축 매개 변수와 상호 작용합니다 `&qlt=`. If the JPG response with the specified JPG compression parameter ( `&qlt=`) does not exceed the `jpegSize` value, the image is returned with `&qlt=` as defined. Otherwise, `&qlt=` is gradually decreased until the image fits in the maximum allowed size, or until the system determines it cannot fit and returns an error.

As a best practice, set `&jpegSize=` and add the parameter `&qlt=` if you are delivering JPG images to devices with limited memory.

## 우수 사례 요약 {#best-practices-summary}

이미지 품질은 높이면서 파일 크기는 줄이려면 다음 매개 변수 조합으로 시작하는 것이 좋습니다.

`fmt=jpg&qlt=85,0&resMode=sharp2&op_usm=1.75,0.3,2,0`

대부분의 상황에서 이 설정 조합을 이용하면 우수한 결과를 얻을 수 있습니다.

이미지에 추가적인 최적화가 필요한 경우, 반경을 0.2 또는 0.3으로 설정한 상태로 시작하여 선명하게 하기(언샵 마스킹) 매개 변수를 점진적으로 미세 조정한 다음, 양을 1.75에서 최대값 4(Photoshop에서 400%와 같음)까지 점진적으로 늘립니다. 원하는 결과가 나왔는지 확인하십시오.

선명하기 하기 결과가 여전히 만족스럽지 않으면, 반경을 소수점 크기로 증가시킵니다. 모든 소수점 증분의 경우, 양을 1.75에서 다시 시작하여 4까지 점진적으로 증가시킵니다. 원하는 결과를 얻을 때까지 이 프로세스를 반복하십시오. 위의 값은 크리에이티브 스튜디오에서 확인한 접근 방법이며, 다른 값으로 시작하고 다른 전략을 수행할 수 있습니다. 결과가 만족스러운지 여부는 주관적인 문제이므로, 구조화된 실험이 핵심입니다.

실험을 하게 되면, 워크플로우를 최적화하는 데 유용한 다음의 일반적 제안 사항을 확인할 수도 있습니다.

* Dynamic Media Classic URL에서 직접 또는 조정 작업을 위한 실시간 미리 보기를 제공하는 Scene7 Publishing System의 이미지 조정 기능을 사용하여 실시간으로 다양한 매개 변수를 테스트해 보십시오.
* Dynamic Media 이미지 제공 명령을 이미지 사전 설정으로 그룹화할 수 있는 것이 좋습니다. An image preset is basically URL command macros with custom preset names such as `$thumb_low$` and `&product_high$`. URL 경로의 사용자 지정 사전 설정 이름은 이 사전 설정을 호출합니다. 이와 같은 기능은 웹 사이트의 다양한 이미지 사용 패턴에 대한 명령 및 품질 설정을 관리하는 데 도움이 되며 URL의 전체 길이를 단축합니다.
* 또한 Dynamic Media Classic은 통합 시 선명하게 하기 이미지를 적용하는 등 이미지 품질을 조정할 수 있는 고급 방법을 제공합니다. 렌더링 결과를 추가적으로 조정하고 최적화하기 위해 이 옵션을 선택할 수 있는 고급 사용 사례에서 Adobe Professional Services는 사용자 지정된 인사이트 및 우수 사례로 도움을 줄 수 있습니다.

