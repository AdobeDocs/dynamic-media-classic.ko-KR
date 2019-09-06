---
title: URL을 웹 애플리케이션에 연결
seo-title: URL을 웹 애플리케이션에 연결
description: 널
seo-description: URL를 웹 애플리케이션에 연결하는 방법을 알아봅니다.
uuid: 1179 BDD 3-9 B 39-47 F 9-945 D -1 C 1 CA 186 BF 96
contentOwner: 관리
content-type: 참조
products: sg_ Experiencemanager/dynamic-media-scene -7
geptopics: sg_ scenesevenondemand_ pk/categories/image_ sizing
discoiquuid: 71299640-676 D -49 B 7-841 D -6118 F 31044 E 8
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# URL을 웹 애플리케이션에 연결{#linking-urls-to-your-web-application}

웹 사이트와 애플리케이션은 URL 문자열을 통해 다이내믹 미디어 이미지 서버 컨텐츠에 액세스합니다. 이미지를 게시하면 Dynamic Media Classic에서 다이내믹 미디어 이미지 서버의 이미지 사전 설정을 참조하는 URL 문자열을 활성화합니다. 테스트를 위해 이 URL을 웹 브라우저에 붙여 넣을 수 있습니다.

웹 페이지와 애플리케이션에 이 URL 문자열을 배치하려면 Scene7 Publishing System에서 복사합니다. 이미지 사전 설정을 사용하여 생성된 URL 문자열을 얻으려면 [미리 보기] 화면이나 찾아보기 패널([세부 사항 보기])로 이동합니다.

## 이미지 사전 설정 URL 얻기 {#obtaining-an-image-preset-url}

[미리 보기] 또는 [세부 사항 보기]에서 이미지 사전 설정에 의해 생성된 URL 문자열을 얻을 수 있습니다. URL을 복사하면 필요한 경우 붙여 넣을 수 있도록 클립보드에 저장됩니다.

*****참고: 자산을 게시할 때까지 URL 이 활성화되지 않습니다.*

### 미리 보기에서 이미지 사전 설정 URL 얻기 {#obtaining-an-image-preset-url-from-preview}

1. 왼쪽의 자산 라이브러리 패널에서 미리 보려는 이미지 자산이 들어 있는 자산 폴더를 탐색합니다.
1. 다음 중 하나를 수행합니다.

   * [자산] 창 위의 도구 모음 오른쪽에서 [그리드 보기]를 클릭합니다. [자산] 창에서 단일 이미지 자산을 선택하고 썸네일 이미지 아래에서 [미리 보기] &gt; [이미지 사전 설정 목록]을 클릭합니다.
   * [자산] 창 위의 도구 모음 오른쪽에서 [목록 보기]를 클릭합니다. [자산] 창에서 단일 이미지 자산을 선택하고 썸네일 이미지 오른쪽에서 [미리 보기] &gt; [이미지 사전 설정 목록]을 클릭합니다.
   * [자산] 창 위의 도구 모음 오른쪽에서 [세부 사항 보기]를 클릭합니다. 동일한 도구 모음에서 [미리 보기] &gt; [이미지 사전 설정 목록]을 클릭합니다.

1. (선택 사항) [이미지 사전 설정 목록] 창 하단에 있는 [URL 복사 생성용 URL 인코딩] 드롭다운 목록에서 복사할 때 이미지 자산 URL에 적용할 URL 인코딩을 선택합니다.
1. [이미지 사전 설정 목록] 창의 미리 보기 창 오른쪽 위 영역에서 선택한 사전 설정 유형에 대해 [URL 복사]를 클릭합니다.
1. [이미지 사전 설정 목록] 창의 오른쪽 아래 모서리에서 [닫기]를 클릭하여 [자산] 화면으로 돌아갑니다.

### 찾아보기 패널에서 이미지 사전 설정 URL 얻기 {#obtaining-an-image-preset-url-from-the-browse-panel}

1. 왼쪽의 자산 라이브러리 패널에서 미리 보려는 이미지 자산이 들어 있는 자산 폴더를 탐색합니다.
1. [자산] 창 위의 도구 모음 오른쪽에서 [그리드 보기]를 클릭합니다. [자산] 창에서 단일 이미지 자산을 선택합니다.
1. [자산] 창 위의 도구 모음 오른쪽에서 [세부 사항 보기]를 클릭합니다.
1. 화면 오른쪽 패널에서 [URL]을 클릭하여 이미지 사전 설정 목록을 펼칩니다.
1. 클립보드로 복사하려는 URL이 포함된 이미지 사전 설정 이름 옆에 있는 [URL 복사] 링크를 클릭합니다.

## 이미지 사전 설정 URL 문자열 정보 {#about-image-preset-url-strings}

Dynamic Media 이미지 서버에 대한 이미지 크기 조정을 위한 URL 호출에는 다음과 같은 기본 구문이 있습니다.

*path*/*name of Image Server*/*account name*/*image name*?*modifier1*&amp;*modifier2*&amp;...

다이내믹 미디어 이미지 서버 URL에서 이미지를 표시하기 위한 서버에 대한 지침은 물음표 (?) 다음에 표시됩니다. 예를 들어 다음 URL 호출은 "backpack"이라는 이미지를 250픽셀 너비로 제공합니다.

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250
```

이미지 사전 설정 URL에는 적절한 크기 및 형식 지정 사양에 따라 이미지를 제공하기 위한 모든 수정자 지침이 포함됩니다. 이미지 사전 설정이 없을 경우 다음 URL 문자열에서 물음표(?) 뒤에 있는 모든 수정자 지침을 확인합니다.

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250&fmt=jpeg&qlt=80,0&resMode=sharp&op_usm=1.1,0.5,1,0
```

그러나 이미지 사전 설정을 사용하여 생성된 URL 문자열에는 이미지 사전 설정에 의해 정의된 지침 대신 이미지 사전 설정 이름이 표시됩니다. 예를 들어 위의 긴 URL을 참조하는 URL 문자열은 다음과 같습니다.

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?$Large$
```

URL에서 이미지 사전 설정 이름은 달러 기호($)로 묶여 있습니다. When a Dynamic Media Image Server encounters the Image Preset portion of the URL (the `Large` in this case), using the size and formatting instructions defined by the “Large” Image Preset.

## 웹 페이지에 동적 이미지 추가 {#adding-dynamic-images-to-your-web-page}

To add dynamic images to your web page, the `<IMG>` tag in your HTML web page code typically is modified using the Dynamic Media Classic URL string to make a request to Dynamic Media Image Servers. 이 문자열은 이미지 사전 설정에 의해 정의된 크기 및 형식 지정 사양에 따라 이미지를 생성합니다.

예를 들어 다음과 같은 일반적인 정적 이미지 열기 호출이 있습니다.

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

`<IMG>`이제 태그를 사용하여 정적 이미지에 대한 참조를 정적 Media Classic 플랫폼에 대한 이미지 사전 설정 호출로 바꿉니다. 샘플 호출은 다음과 같이 표시됩니다.

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$”
```

In this example, a Dynamic Media Image Server “looks up” the definition of `$thumbnail$` and dynamically generates the appropriate image with the sizing and formatting specifications defined by the `thumbnail`Image Preset. URL 문자열에서 제품 이미지 파일 이름(이 경우 `backpack_trns`)을 제외한 모든 항목은 대체로 페이지 템플릿에 내장됩니다. 상거래 서버에서 페이지 템플릿에 자동으로 삽입되는 요소는 이미지의 IPS ID 또는 이름뿐입니다.
