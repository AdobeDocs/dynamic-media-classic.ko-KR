---
title: 이미지 품질 최적화 우수 사례
description: 이미지 품질을 최적화하는 모범 사례에 대해 알아봅니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 3c50e706-b9ed-49db-8c08-f179de52b9cf
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T17:39:42.316Z'
TQID: 'https://experienceleague.adobe.com/kw-spdqv6ArVEWk8ID4mnQjYrS25RZntKOJ7-tESasY'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: bcc5edb5-84c3-4940-9f84-ed88b6c16274
  - id: cdd65e7e-8839-44a2-bc21-0e03623b5dd1
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: b29d7cc6962ca9e7724bb43987947b08af5cd4d7
workflow-type: tm+mt
source-wordcount: 1591
ht-degree: 27%

---

# 이미지 품질 최적화 우수 사례{#best-practices-for-optimizing-the-quality-of-your-images}

이미지 품질을 최적화하는 데는 시간이 오래 걸릴 수 있습니다. 많은 요소가 허용되는 결과를 렌더링하는 데 기여합니다. 또한 이미지 품질은 개인마다 다르게 생각하므로 결과는 어느 정도 주관적입니다. 구조화된 실험은 필수적입니다.

Adobe Dynamic Media Classic에는 이미지 및 렌더링 결과를 조정하고 최적화하는 100개 이상의 이미지 제공 명령이 포함되어 있습니다. 다음 지침은 프로세스를 간소화하고 일부 필수 명령 및 우수 사례를 사용하여 좋은 결과를 빨리 얻는 데 도움이 될 수 있습니다.

[스마트 이미징](https://experienceleague.adobe.com/ko/docs/experience-manager-65/content/assets/dynamic/imaging-faq)도 참조하세요.

>[!TIP]
>
>Dynamic Media [_스냅숏_](https://snapshot.scene7.com/)을(를) 사용하여 Dynamic Media 이미지 수정자 및 스마트 이미징의 이점을 알아보십시오.
>
> 스냅샷은 최적화된 동적 이미지 제공을 위한 Dynamic Media의 기능을 보여 주도록 설계된 시각적 데모 도구입니다. 테스트 이미지 또는 Dynamic Media URL로 실험하여 다음과 같은 다양한 Dynamic Media 이미지 수정자의 출력을 시각적으로 관찰할 수 있습니다.
>
>* 파일 크기(WebP 및 AVIF 게재 포함)
>* 네트워크 대역폭
>* DPR(장치 픽셀 비율)
>
>스냅숏을 사용하는 방법을 알아보려면 [스냅숏 교육 비디오](https://experienceleague.adobe.com/ko/docs/experience-manager-learn/assets/dynamic-media/images/dynamic-media-snapshot)&#x200B;(3분 17초)를 보세요.


## 이미지 형식(&amp;fmt=) 우수 사례 {#best-practices-for-image-format-fmt}

* JPG 또는 PNG는 양질의 이미지를 관리할 수 있는 크기 및 용량으로 제공하는 데 적합합니다.
* URL에 format 명령이 제공되지 않으면 기본적으로 Dynamic Media 이미지 제공은 게재를 위해 JPG으로 설정됩니다.
* JPG는 10:1 비율로 압축하며 일반적으로 작은 크기의 이미지 파일을 만듭니다. PNG는 이미지에 투명한 배경이 포함된 경우를 제외하고 약 2:1의 비율로 압축됩니다. 일반적으로 PNG 파일 크기는 JPG 파일보다 큽니다.
* JPG는 손실 압축을 사용하며, 이것은 압축 중에 그림 요소(픽셀)가 제거됨을 의미합니다. 반면에 PNG는 비손실 압축을 사용합니다.
* JPG는 종종 가장자리와 대비가 선명한 합성 이미지보다 원본에 더 충실한 사진 이미지를 압축하는 데 사용합니다.
* 이미지에 투명도가 포함되어 있는 경우, JPG는 투명도를 지원하지 않으므로 PNG를 사용합니다.

이미지 형식에 대한 우수 사례로는 가장 일반적인 설정 `&fmt=JPG`(으)로 시작하십시오.

## 이미지 크기 우수 사례 {#best-practices-for-image-size}

이미지 크기를 동적으로 줄이는 것은 Dynamic Media 이미지 제공이 수행하는 가장 일반적인 작업 중 하나입니다. 이 작업에는 크기 지정이 포함되며, 원할 경우 이미지의 크기를 줄이는 데 사용되는 다운샘플링 모드 지정도 포함됩니다.

* 이미지 크기를 조정하려면 `&wid=<value>` 및 `&hei=<value>`을(를) 사용하십시오. 이러한 매개 변수는 종횡비에 따라 이미지 폭을 자동으로 설정합니다.
* `&resMode=<value>` 다운샘플링에 사용되는 알고리즘을 제어합니다. `&resMode=sharp2`(으)로 시작합니다. 이 값은 최상의 이미지 품질을 제공합니다. 다운샘플링 값 `bilin`을(를) 사용하는 속도가 더 빠르지만 에일리어싱 아티팩트가 발생하는 경우가 많습니다.

이미지 크기 조정에 대한 우수 사례로 `&wid=<value>&hei=<value>&resMode=sharp2`을(를) 사용하십시오. `&hei=<value>&resMode=sharp2`

## 이미지 선명하게 하기 우수 사례 {#best-practices-for-image-sharpening}

이미지 선명하게 하기는 웹 사이트에서 이미지를 제어할 때 가장 복잡한 측면이며 오류가 많이 발생하는 곳입니다. Adobe Dynamic Media Classic에서 선명하게 하기 및 언샵 마스킹이 작동하는 방법에 대한 자세한 내용은 다음 유용한 리소스를 참조하십시오.

PDF의 모범 사례 백서로서 [Adobe Dynamic Media Classic 및 이미지 서버에서 이미지 선명하게 하기](/help/using/assets/s7_sharpening_images.pdf)를 호출했습니다.

<!-- Give a 404 See also [Sharpening an image with unsharp mask](https://helpx.adobe.com/photoshop/atv/cs6-tutorials/sharpening-an-image-with-unsharp-mask.html). -->

Adobe Dynamic Media Classic에서는 수집, 전달 또는 둘 다 동안 이미지를 선명하게 할 수 있습니다. 그러나 일반적으로 한 가지 방법을 사용하여 이미지를 선명하게 하지만 둘 다 선명하게 하지는 않습니다. URL을 통해 전달 시 이미지를 선명하게 하면 일반적으로 최상의 결과를 얻을 수 있습니다.

사용할 수 있는 이미지 선명하게 하기 방법에는 두 가지가 있습니다.

* 단순 선명하게 하기( `&op_sharpen`): Adobe Photoshop에서 사용되는 선명하게 하기 필터와 유사하게, 단순 선명하게 하기는 동적 크기 조정 후 이미지의 최종 보기에 기본 선명하게 하기를 적용합니다. 하지만 이 방법은 사용자가 구성할 수 없습니다. 필요한 경우가 아니면 `&op_sharpen`을(를) 사용하지 않는 것이 좋습니다.
* 언샵 마스킹(`&op_USM`): 언샵 마스킹은 선명하게 하기를 위한 업계 표준 필터입니다. 아래의 지침에 따라 언샵 마스킹으로 이미지를 선명하게 하는 것이 좋습니다. 언샵 마스킹을 사용하면 다음 3가지 매개 변수를 제어할 수 있습니다.

  * `&op_sharpen=amount,radius,threshold`

    * `amount`(0-5, 효과의 강도)
    * `radius`(0-250, 선명하게 표시된 개체 주위에 그려진 &quot;선명하게 하기 선&quot;의 너비(픽셀 단위)입니다.)

      매개 변수 `radius`과(와) `amount`은(는) 역관계를 갖습니다. `amount`을(를) 늘려 `radius`을(를) 줄이는 것을 보상할 수 있습니다. `Radius`은(는) 값이 낮을수록 가장자리 픽셀만 선명하게 하므로 더 세밀하게 제어할 수 있으며 값이 높을수록 더 넓은 범위의 픽셀이 선명해집니다.

    * `threshold`(0-255, 효과 민감도)

      이 매개 변수는, 가장자리 픽셀로 간주되고 필터가 선명하게 하기 전에, 선명하게 되는 픽셀과 주변 영역 간의 필수 차이를 결정합니다. 임계값은 피부 톤과 같이 유사한 색상 영역을 지나치게 선명하게 하는 것을 방지하는 데 유용합니다. 예를 들어, 임계값 12는 피부 색조 밝기의 미세한 변화를 무시하여 &quot;노이즈&quot;를 추가하는 것을 피하는 동시에 속눈썹이 피부와 만나는 지점과 같은 고대비 영역에 가장자리 대비를 추가합니다.

      필터에 사용할 모범 사례를 포함하여 이러한 세 매개 변수를 설정하는 방법에 대한 자세한 내용은 [Adobe Dynamic Media Classic 및 이미지 서버에서 이미지 선명하게 하기](/help/using/assets/s7_sharpening_images.pdf)를 참조하십시오.

    * Adobe Dynamic Media Classic을 사용하면 네 번째 매개 변수인 단색(`0,1`)도 제어할 수 있습니다. 이 매개 변수는 값 `0`을(를) 사용하여 각 색상 구성 요소에 언샵 마스킹을 별도로 적용할지 또는 값 `1`을(를) 사용하여 이미지 밝기/강도에 적용할지 여부를 결정합니다.

언샵 마스크 반경 매개 변수로 시작하는 것이 좋습니다. 시작할 수 있는 반경 설정은 다음과 같습니다.

* 웹 사이트: 0.2-0.3픽셀
* 사진 인쇄(250-300ppi): 0.3-0.5픽셀
* 오프셋 인쇄(266-300ppi): 0.7-1.0픽셀
* 캔버스 인쇄(150ppi): 1.5-2.0픽셀

양을 1.75에서 4까지 점진적으로 늘립니다. 선명하게 하기가 여전히 원하는 결과가 아닌 경우 반지름을 소수점 단위로 늘리고 크기를 1.75에서 4로 다시 설정합니다. 필요에 따라 반복합니다.

모노크롬 매개 변수 설정을 0으로 둡니다.

## JPEG 압축 모범 사례(`&qlt=`) {#best-practices-for-jpeg-compression-qlt}

* 이 매개 변수는 JPG 인코딩 품질을 제어합니다. 값이 클수록 이미지 품질은 높지만 파일 크기도 큼을 의미하고, 값이 작을수록 이미지 품질은 낮지만 파일 크기도 작음을 의미합니다. 이 매개 변수의 범위는 0-100입니다.
* 품질에 대해 최적화하기 위해, 매개 변수 값을 100으로 설정하지 마십시오. 90 또는 95와 100 사이의 차이는 거의 감지할 수 없다. 그러나 100은 불필요하게 이미지 파일의 크기를 늘립니다. 따라서 품질을 최적화하지만 이미지 파일이 너무 커지지 않도록 하려면 `qlt=` 값을 90 또는 95로 설정하십시오.
* 이미지 파일 크기는 작지만 이미지 품질을 허용 가능한 수준으로 유지하려면 `qlt=` 값을 80으로 설정합니다. 70 내지 75 미만의 값은 상당한 이미지 품질 저하를 초래한다.
* 중간에 머무르려면 `qlt=` 값을 85로 설정하는 것이 좋습니다.
* 크로마 플래그 `qlt=` 사용 중

  * `qlt=` 매개 변수에는 일반적인 값 `,0`(기본값)을 사용하여 RGB 색도 다운샘플링을 켜거나 `,1` 값을 사용하여 해제할 수 있는 두 번째 설정이 있습니다.
  * RGB 색도 다운샘플링이 꺼진 상태로 시작합니다(`,1`). 이렇게 설정하면 특히 선명한 가장자리와 대비가 많은 합성 이미지의 경우 일반적으로 나은 이미지 품질을 얻을 수 있습니다.

JPG 압축에 대한 우수 사례로 `&qlt=85,0`을(를) 사용하십시오.

## JPEG 크기 지정(&amp;jpegSize=) 우수 사례 {#best-practices-for-jpeg-sizing-jpegsize}

`jpegSize` 매개 변수는 이미지가 특정 크기를 초과하지 않도록 하려는 경우에 유용합니다. 이 매개 변수는 메모리가 제한된 장치에 전달하기 위한 것입니다.

* 이 매개 변수는 KB(`jpegSize=<size_in_kilobytes>`) 단위로 설정되어 있습니다. 이미지 제공에 허용되는 최대 크기를 정의합니다.
* `&jpegSize=`이(가) JPG 압축 매개 변수 `&qlt=`과(와) 상호 작용합니다. 지정된 JPG 압축 매개 변수(`&qlt=`)의 JPG 응답이 `jpegSize` 값을 초과하지 않으면 정의된 대로 이미지가 `&qlt=`(으)로 반환됩니다. 그렇지 않으면 이미지가 최대 허용 크기에 맞출 때까지 `&qlt=`이(가) 점차적으로 줄어듭니다. 또는 이미지에 맞지 않으면 오류가 반환됩니다.

메모리가 제한된 장치에 JPG 이미지를 전달할 때 `&jpegSize=`을(를) 설정하고 매개 변수 `&qlt=`을(를) 포함하는 것이 좋습니다.

## 우수 사례 요약 {#best-practices-summary}

높은 이미지 품질과 작은 파일 크기를 달성하려면 다음 매개 변수 조합으로 시작하는 것이 좋습니다.

`fmt=jpg&qlt=85,0&resMode=sharp2&op_usm=1.75,0.3,2,0`

이러한 설정의 조합은 대부분의 상황에서 탁월한 결과를 생성합니다.

이미지를 추가로 최적화해야 하는 경우 반지름이 0.2 또는 0.3으로 설정된 것부터 시작하여 선명하게 하기(언샵 마스킹) 매개 변수를 점진적으로 미세 조정합니다. 그런 다음 양을 1.75에서 최대 4까지 점진적으로 늘립니다([!DNL Adobe Photoshop]의 400%에 해당). 원하는 결과가 나왔는지 확인하십시오.

선명하기 하기 결과가 여전히 만족스럽지 않으면, 반경을 소수점 크기로 증가시킵니다. 소수점 증가마다 양을 1.75로 재설정하고 점차적으로 4로 늘립니다. 원하는 결과를 얻을 때까지 이 프로세스를 반복하십시오. 위의 값은 Creative Studio에서 확인한 접근 방식이지만 다른 값을 사용하고 다른 절차를 따를 수 있습니다. 그 결과가 만족스러운지 아닌지는 주관적인 문제이기 때문에 구조적인 실험이 필요하다.

실험할 때 워크플로를 최적화하는 데 도움이 되는 일반적인 제안은 다음과 같습니다.

* URL에서 직접 또는 [!DNL Adobe Dynamic Media Classic] 이미지 조정 도구를 사용하여 실시간으로 다양한 매개 변수를 테스트합니다. 후자는 조정 작업을 위한 실시간 미리보기를 제공합니다.
* 가장 좋은 방법은 명령을 제공하는 Dynamic Media 이미지를 이미지 사전 설정으로 그룹화할 수 있다는 것입니다. 이미지 사전 설정은 `$thumb_low$` 및 `$product_high$`과(와) 같은 사용자 지정 사전 설정 이름이 있는 URL 명령 매크로 집합입니다. URL 경로의 사용자 지정 사전 설정 이름은 이러한 사전 설정을 호출합니다. 이와 같은 기능은 웹 사이트의 다양한 이미지 사용 패턴에 대한 명령 및 품질 설정을 관리하는 데 도움이 되며 URL의 전체 길이를 단축합니다.
* Adobe Dynamic Media Classic은 또한 수집 시 이미지 선명하게 하기를 적용하는 등, 이미지 품질을 조정하는 고급 방법을 제공합니다. 렌더링된 결과를 추가로 조정하고 최적화하는 것이 선택 사항인 고급 사용 사례의 경우 Adobe Professional Services을 통해 사용자 지정된 insight 및 모범 사례를 확인할 수 있습니다.
