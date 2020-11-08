---
title: 게시 설정
seo-title: 게시 설정
description: 널
seo-description: '[게시 설정] 화면 설정에 따라 자산이 Dynamic Media Classic 서버에서 웹 사이트 또는 애플리케이션으로 기본적으로 제공되는 방법이 결정됩니다.'
uuid: 196f25c8-abf5-4c5d-8f6f-bc70007a0301
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: cba59093-28b6-4490-b838-d942b72ad1ec
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '2421'
ht-degree: 64%

---


# 게시 설정 {#publish-setup}

[게시 설정] 화면 설정에 따라 자산이 Dynamic Media Classic 서버에서 웹 사이트 또는 애플리케이션으로 기본적으로 제공되는 방법이 결정됩니다. 설정이 지정되지 않은 경우 Dynamic Media Classic 서버는 [게시 설정] 화면의 기본 설정에 따라 자산을 제공합니다. 예를 들어 해상도 특성을 포함하지 않는 이미지를 제공하는 요청은 [이미지 서버] 화면의 [기본 개체 해상도] 설정을 사용하여 이미지를 만듭니다.

관리자는 [이미지 서버], [이미지 렌더러] 및 [비네팅] 화면의 기본 설정을 변경하여 서버의 자산 제공에 대한 기본 설정을 지정할 수 있습니다.

[게시 설정] 화면을 열려면 [설정] > [애플리케이션 설정] > [게시 설정]을 클릭합니다.

>[!NOTE]
>
>[게시 설정] 화면은 숙련된 웹 사이트 개발자와 프로그래머를 위한 것입니다. Dynamic Media Classic에서는 이러한 화면에서 설정을 변경하는 사용자가 Dynamic Media Classic, HTTP 프로토콜 표준 및 규칙 및 기본 이미징 기술에 익숙하다고 가정합니다.

## 이미지 서버 {#image-server}

1 [이미지 서버] 화면에서는 이미지 서버의 이미지 제공에 대한 기본 설정을 지정합니다. 다음 5가지 범주로 설정을 사용할 수 있습니다. 설정에 대한 자세한 내용은 [이미지 서버] 화면 자체를 참조하십시오.

Dynamic Media Classic 지원 담당자의 지원을 통해서만 이러한 설정을 변경합니다.

**카탈로그 관리** 이러한 설정에 따라 Dynamic Media Classic 및 카탈로그가 상호 작용하는 방법이 결정됩니다. 대부분의 웹 서버와 달리 다이내믹 미디어 이미지 서버 URL 호출은 이미지 파일이 적합한 파일이 아닌 매니페스트 또는 카탈로그 파일로 이동합니다. 카탈로그 파일(eCatalog 아님)에는 각 이미지의 경로와 함께 이미지 서버에 게시되는 모든 컨텐츠 목록이 들어 있습니다. Digimarc ID가 있는 경우 [Digimarc 사용자 정보] 섹션에서 사용자 정보를 입력합니다.

**요청 속성** 이러한 설정은 서버에서 전달할 수 있는 이미지에 제한을 적용합니다. 예를 들어, *최대* 응답 이미지 크기 제한은 **** 너비 **[!UICONTROL 5000]** 및 높이 **[!UICONTROL 5]** 00입니다.

**기본 요청 속성** 이 설정은 이미지의 기본 모양과 관련이 있습니다.

**공통 축소판 속성** 이러한 설정은 축소판 이미지의 기본 모양 및 정렬과 관련이 있습니다.

**카탈로그 필드 기본값** 이 설정은 이미지의 해상도 및 기본 축소판 유형과 관련이 있습니다.

**색상 관리 속성** 이 설정에 따라 사용되는 ICC 색상 프로필이 결정됩니다.

**호환성 속성** 이 설정을 사용하면 텍스트 레이어의 맨 앞 및 뒤에 있는 단락이 이전 버전과의 호환성을 위해 버전 3.6에서와 같이 처리됩니다.

**현지화 지원** 이 설정을 사용하면 여러 로케일 특성을 관리할 수 있습니다. 또한 로케일 맵 문자열을 지정할 수 있으므로 뷰어에서 여러 도구 설명을 지원하려는 언어를 정의할 수 있습니다.

예를 들어 여러 국가에서 팔리는 다국적 브랜드인 경우 각 국가에서 자체 로케일별 뷰어를 사용하도록 할 수 있습니다. 이 기능을 수행하려면 로케일 맵 문자열을 지정합니다. 그런 다음 원하는 언어로 번역된 텍스트 문자열을 추가하여 뷰어의 사전 설정에서 도구 설명 텍스트를 편집합니다.

>[!NOTE]
> 로컬라이제이션 지원 옵션을 설정하려면 Admin Console을 [사용하여 지원 사례를 만듭니다.](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) 지원 케이스에 설치 도움말을 요청합니다.

**현지화 지원** 설정에 대한 자세한 내용은 [자산 현지화를 설정할 때 고려 사항](publish-setup.md#considerations_when_setting_up_localization_of_assets)을 참조하십시오.

### 자산 현지화를 설정할 때 고려 사항 {#considerations-when-setting-up-localization-of-assets}

>[!NOTE]
>
>로케일 맵 필드와 같이 Dynamic Media Classic에서 현지화 지원 옵션을 설정하려면 Admin Console을 [사용하여 지원 사례를 만듭니다.](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) 지원 케이스에 설치 도움말을 요청합니다.

Dynamic Media Classic을 사용하는 일반적인 방법은 전자 상거래 웹 사이트에서 제품 이미지를 관리하는 것입니다. 국제 산업은 유사한 제품에 대한 자산이 나라마다 다르게 보이는 문제에 직면하고 있습니다. 보통 차이는 전체 미디어에서 매우 작은 부분에 대한 것입니다. 이러한 차이를 각 국가의 모든 자산을 복사하고 차이만 다시 써서 해결하는 것은 엄청난 노력을 요하는 일이며 하나의 마스터 자산이라는 표현과 모순됩니다. 이와 같은 자산의 차이점은 서로 다른 오디오 트랙을 사용하는 국가별 비디오에서부터 제품과 함께 사용되는 전원 코드의 미묘하지만 중요한 차이에 이르기까지 다양할 수 있습니다. Dynamic Media Classic에서는 기본 조회 메커니즘을 사용합니다. 사용자는 필요한 로케일에서 시작하여 이미지 서버가 검색하는 자산 접미어 순서를 정의합니다.

**자산을 현지화하는 방법**

IS(이미지 제공) 요청에 대한 로케일은 다음의 IS/IR(이미지 렌더링) 명령으로 식별됩니다.

`locale=`

이 명령은 대소문자를 구분하지 않는 로케일 ID(locId) 문자열을 허용합니다. 로케일 ID는 보통 문자 및 &quot;_&quot;으로 구성된 2-6자의 문자열입니다.

IS supports arbitrary printable ASCII strings.The `locale=` command has a global scope, meaning that it is applied to the entire request, including all nested IS and IR requests, referenced templates, and image layers. 각 레이어의 다른 로케일과 같이, 요청에 대해 여러 로케일은 지원되지 않습니다. 하지만, 중첩된 요청에서 명시적 무시의 허용은 가능할 수 있습니다.

If `locale=` is not specified, `attribute::DefaultLocale` is passed to the translation engines. Limited input validation is applied to the `locale=` value. Empty `locale=` values are permitted. Because `locale=` has a global scope, `attribute::DefaultLocale` is provided by the main catalog for the entire request.

Some of the benefits of using `locale=` and `attribute::DefaultLocale` include the following:

* 여러 로케일에 대한 컨텐츠 공유.
* 일반 ID를 사용하여 로케일별 컨텐츠 액세스.
* 로케일 접두어와 접미어 또는 별도의 카탈로그에 있는 로케일별 컨텐츠와 같이, 로케일별 컨텐츠의 이름 지정 규칙 및 관리와 관련한 유연성 허용.
* 로케일별 버전에 대한 직접 액세스 지원.
* 이미지 집합과 같은 집계 개체에는 잠재적인 로케일별 컨텐츠에 대한 일반적인 참조가 들어 있을 수 있습니다.
* 이미지, 이미지 집합, 비네팅, 재질 및 뷰어 구성 레코드를 포함하여 현지화가 필요할 수 있는 카탈로그로 관리되는 모든 컨텐츠를 지원합니다.
* IPS 데이터베이스 및 IS 매니페스트 메커니즘에 대한 변경 사항을 최소화.
* RFC IS-63을 구현하면 비디오 및 스킨과 같은 정적 컨텐츠에 대한 지원이 추가됩니다.
* 기본 로케일을 구성할 수 있습니다.

**응용 시나리오**

| 애플리케이션 | 시나리오 |
|--- |--- |
| 뷰어 현지화 | 정적 컨텐츠 카탈로그가 구현되면 현지화는 IS에 수행되는 모든 요청에 추가되는 locale= 매개 변수로 제어됩니다. 구성 레코드, 스킨, 시작 화면 등에는 로케일별 차이가 있을 수도 있고 없을 수도 있습니다. 현지화되는 컨텐츠와 ID를 아는 데 필요한 뷰어 없이도 IS에 의해 올바른 컨텐츠가 제공됩니다. |
| 이미지 및 비디오 | 다국어 회사에는 종종 일반적인 컨텐츠와 로케일별 컨텐츠가 혼합되어 있습니다. 이러한 메커니즘에서, 이미지나 비디오 참조는 일반적일 수 있으며, IS는 사용 가능할 경우 로케일별 컨텐츠를 제공합니다. |
| 이미지 집합 및 미디어 집합 | eCatalog가 완전히 다른 경우처럼 전체 이미지 세트가 일반에서 로케일별 이미지 세트로 변환하는 경우 등 일부 로케일에 대해 다를 수 있습니다. 일반적으로 일반 세트의 개별 ID는 지역화된 내용을 참조할 수 있습니다. 예를 들어, 대부분의 가전 제품 사진은 제어판 사진을 제외하면 모든 언어에서 동일할 수 있습니다. IS는 자동으로 ID를 전환하므로, 로케일별 이미지 집합을 생성할 필요가 없습니다. |

**자산 현지화 구현**

Dynamic Media Classic 및 이미지 서비스에는 이미지와 정적 컨텐츠의 지역화를 허용하는 인터페이스가 있습니다.

현지화를 하지 않는 이미지 서버 URL은 다음과 같은 모습입니다.

`https://server/is/image/company/image`

With localization, an Image Server URL adds the `locale=` parameter to the path, as in the following:

`https://server/is/image/company/image?locale=de_DE`

On receipt of the http call by the Image Server, the `locale=` parameter is parsed through the localeMap field found in **Setup** > **Application Setup** > **Publish Setup** > **Image Server** > **Localization Support** group.

로케일 맵 필드에는 파이프 기호(|)를 사용하여 구별되는 항목 목록이 들어 있습니다.

각 항목은 쉼표로 구분된 값 목록으로 구성됩니다. The first value is the search value that is passed by the `locale=` parameter. 나머지 값은 기존 이미지가 나올 때까지 연속적으로 시도되는 접미어/대체 값입니다.

접미어 값 또는 대체 값의 적용 여부는 **설정** > **애플리케이션 설정** > **게시 설정** > **이미지 서버** > **현지화 지원** 그룹에 있는 [전역 로케일] 설정에 따라 결정됩니다.

>[!NOTE]
>
>글로벌 로케일 설정은 현재 Dynamic Media Classic 인터페이스가 아닌 API를 통해 설정하는 경우에만 가능합니다.

**접미어 예제**

| URL | localeMap ID | 결과 |
|--- |--- |--- |
| `https://server/is/image/company/image?locale=de_DE` | `de_DE,_DE,|fr_FR,_FR,` | 정의된 전역 로케일이 없습니다. 로케일 매개 변수 de_DE가 로케일 맵의 첫 번째 항목에 대응됩니다. 첫 번째 해당 값 _DE는 자산 image_DE에 접미어로 추가되고 이미지 서버에서 이 자산을 찾으려는 시도가 수행됩니다. 서버에 있는 경우, 반환됩니다. 없으면, 두 번째 값 “”이 접미어로 사용되어 이미지 자체가 반환됩니다. |

**대체 예제**

| URL | 전역 로케일 및 로케일 맵 ID | 결과 |
|--- |--- |--- |
| `https://server/is/image/company/image-main-01?locale=de_DE` | `GlobalLocale=mainlocaleMap -` <br><br/> `de_DE,de,main|fr_FR,fr,main` | 위의 대체 예에서, GlobalLocale은 main으로 설정됩니다. 로케일 매개 변수 de_DE가 로케일 맵의 첫 번째 항목에 대응됩니다. GlobalLocale 하위 문자열이 검색되어 localeMap에서 첫 번째 해당 값 de로 대체되어 image-de-01이 됩니다. 이미지 서버에 있는 경우, 반환됩니다. 없는 경우에는, 두 번째 값이 대체되어, image-main-01이 됩니다. |

URL에 정의된 로케일이 없으면, 이미지 서버는 DefaultLocale이 정의되어 있는 경우 DefaultLocale을 가져오고, URL에 적용합니다.

If an unknown or empty locale parameter is supplied with `locale=`, then the localeMap is scanned for the empty value “starting with,”. 기본 로케일을 알 수 없는 로케일에 적용하기 위해서는 이것을 구성해야 합니다.

**defaultImage 정보**

이미지 서버는 요청된 로케일에 대한 선택 사항을 번갈아 시도합니다. 일치 항목이 없는 경우, 로케일 선택 사항은 defaultImage에 적용되며, 일치 버전이 반환됩니다. 따라서 각 로케일에 현지화 없이 이미지에 대한 옵션이 포함되거나, 현지화된 기본 이미지 버전은 Dynamic Media Classic에서 사용할 수 있어야 합니다.

**localeMap을 찾는 시나리오**

다음 로케일을 지원하려고 한다고 가정합니다.

`en, en_us, en_uk, de, de_at, de_de, fr`

You map these locales to the suffixes `_E`, `_G`, and `_F`, for English, German, and French, respectively. 모든 예의 경우, 일반 입력 이미지 ID는 `myImg`입니다.

*localeMap을 찾기 위한 표준 동작*

로케일 ID는 해당 접미어에 매핑됩니다. 카탈로그에 로케일별 ID가 없을 경우, 일반 ID가 사용됩니다. 일반 ID에 매핑하는 빈 locSuffix 값을 주목하십시오.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,`

| 로케일= | 검색할 출력 ID |
|--- |--- |
| en,en_us, en_uk | myImg_E,myImg |
| de,de_de,de_at | myImg_D,myImg |
| fr | myImg_F,myImg |
| 기타 모든 항목 | - |

*로케일을 모를 때 localeMap 찾기*

특정 ID 또는 일반 ID에 알 수 없는 로케일을 매핑할 수 있습니다. 이 예제의 경우, 알 수 없는 로케일을 영어 ID에 매핑하거나, 영어 ID가 없을 경우 일반 ID에 매핑할 수 있습니다.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,_E,`

| 로케일= | 검색할 출력 ID |
|--- |--- |
| de,de_de,de_at | myImg_D,myImg |
| fr | myImg_F,myImg |
| 기타 모든 항목 | myImg_E,myImg |

You could also have a dedicated locSuffix, such as U, just for unknown locales, and force to the default image if no `_U` exists, as in the following:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,U`

또는, 다음과 같이 일반 ID에 바로 매핑 할 수 있습니다.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,`

*여러 계층 조회를 사용하여 localeMap 찾기*

종종 스킨 노출과 같이, 유럽, 중동 및 북아메리카 영역과 같이 로케일을 지역 표준을 나타내도록 그룹화하는 것이 유용할 수 있습니다. 다중 계층 조회를 사용하여 이러한 작업을 수행할 수 있습니다.

이 예제의 경우, 서구 및 중동에 사용할 컬렉션을 지원하려 한다고 가정합니다. 두 컬렉션은 모두 일반 이미지 컬렉션을 기반으로 하며, 모두 여러 이미지를 추가하거나 수정합니다. Both collections are then further refined for specific locales, such as `m1, m2` for two middle-eastern variants, and `w1, w2,` and `w3` for three Western locales, except that images are shared for `w1` and `w3`. 알 수 없는 로케일은 일반 컬렉션에만 매핑되고, 로케일별 이미지에는 액세스하지 못했습니다. 다음은 맵이 표시되는 모습입니다.

`attribute::LocaleMap=w1,-W,|w2,-W2,-W,|w3,-W,|m1,-M1,-M,|m2,-M2,-M,|,`

| 로케일= | 검색할 출력 ID |
|--- |--- |
| w1, w3 | myImg-W, myImg |
| w2 | myImg-W2, myImg-W, myImg |
| m1 | myImg-M1, myImg-M, myImg |
| m2 | myImg-M2, myImg-M, myImg |
| 기타 모든 항목 | mylmg |

*특정 ID를 검색하여 localeMap 찾기*

일부 이미지 이름 지정 규칙은 일반 이미지 ID를 지원하지 않습니다. 요청의 일반 ID는 카탈로그에서 특정 ID에 매핑해야 합니다. 그러나, 특정 ID를 정확히 모르는 경우가 있을 수 있습니다.

Using the first example as a basis, images for all languages may have the suffixes `_1`, `_2`, or `_3`. Images that are specific to French locales may have the suffixes `_22` or `_23` suffix. And images that are specific to German locales may have the suffixes `_470` or `_480`.

`attribute::LocaleMap=,_1,_2,_3|fr,_22,_23,_1,_2,_3|de,_470,_480,_1,_2,_3|de_at,_470,_480,_1,_2,_3|de_de,_470,_480,_1,_2,_3`

| 로케일= | 검색할 출력 ID |
|--- |--- |
| fr | myImg_22, myImg_23, myImg_1, myImg_2, myImg_3 |
| de, de_at, de_de | myImg_470, myImg_480, myImg_1, myImg_2,myImg_3 |
| 기타 모든 항목 | myImg_1, myImg_2, myImg_3 |

**현지화 지원을 구현할 때 중요한 고려 사항**

* 현지화는 ID 기반 자산 호출에 제한되며, 경로 기반 자산 호출에서는 사용할 수 없습니다. 따라서, 로케일로 비디오를 호출할 경우, 회사/자산 ID로 호출해야 하며, 비디오의 전체 경로는 없습니다. 이것은 해당 메서드가 경로 기반 비디오에만 사용하기 위한 것이므로 현지화에는 rtmp를 사용할 수 없음을 의미합니다.
* localeMap이 활성화된 경우 단일 비디오가 들어 있는 혼합 미디어 집합은 사용할 수 없으며, 다른 경우 이 집합의 컨텐츠 호출은 실패합니다. 이 문제를 해결하려면 단일 비디오를 적응형 비디오 집합에 추가하면 됩니다. 그런 다음, 혼합 미디어 집합에 적응형 비디오 집합을 추가합니다.
* 적응형 비디오 집합의 컨텐츠에 대한 요청과 같은 특정 요청은 현지화되지 않습니다. 따라서 현지화에 적응형 비디오 집합을 사용할 생각이라면, 적응형 비디오 집합을 혼합 미디어 집합 내에 배치해야 합니다. Then, call the set into a Mixed Media viewer with the `locale=` parameter.

## 이미지 렌더러 {#image-renderer}

[이미지 렌더러] 화면에서는 이미지 렌더링 서버의 이미지 집합 제공에 대한 기본 설정을 지정합니다. 다음 5가지 범주로 설정을 사용할 수 있습니다. 설정에 대한 자세한 내용은 [이미지 서버] 화면 자체를 참조하십시오.

**카탈로그 관리** 이러한 설정에 따라 Dynamic Media Classic 및 카탈로그 파일의 상호 작용 방식이 결정됩니다. Dynamic Media Classic Render 서버 URL 호출은 카탈로그에 대해 수행되므로 서버에서 이미지를 전달하는 호출이 수행됩니다. Dynamic Media Classic 지원 담당자의 지원을 통해서만 이러한 설정을 변경합니다.

**세션 속성** 이 설정은 오류 매개 변수, 상대 이미지 URL에 대한 URL 및 개체 겹침 허용 여부를 설정합니다.

**기본 재료 속성** 이 설정은 이미지의 기본 해상도 및 선명하게 하기 설정을 설정합니다.

**응답 이미지 속성** 이 설정은 이미지의 기본 모양과 관련이 있습니다.

**색상 관리 속성** 이 설정은 이미지의 기본 색상 설정과 관련이 있습니다.

## 비네팅 {#vignette}

[비네팅] 화면에서는 비네팅의 기본 모양에 대한 설정을 제공합니다. 자세한 오류 설명은 화면 자체를 참조하십시오.
