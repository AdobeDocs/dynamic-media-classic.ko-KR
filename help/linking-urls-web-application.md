---
title: 웹 애플리케이션에 URL 연결
description: Adobe Dynamic Media Classic에서 웹 애플리케이션에 URL을 연결하는 방법을 알아봅니다.
uuid: 1179bdd3-9b39-47f9-945d-1c1ca186bf96
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 71299640-676d-49b7-841d-6118f31044e8
feature: Dynamic Media Classic
role: User
exl-id: ca629427-da33-4bab-9d08-6d9368042f7e
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 37%

---

# 웹 애플리케이션에 URL 연결{#linking-urls-to-your-web-application}

웹 사이트 및 애플리케이션이 URL 문자열을 통해 Dynamic Media Image Server 컨텐츠에 액세스합니다. 이미지를 게시하면 Adobe Dynamic Media Classic에서 Dynamic Media 이미지 서버에서 이미지 사전 설정을 참조하는 URL 문자열을 활성화합니다. 테스트를 위해 이 URL을 웹 브라우저에 붙여 넣을 수 있습니다.

웹 페이지 및 애플리케이션에 이러한 URL 문자열을 배치하려면 Adobe Dynamic Media Classic에서 복사합니다. 이미지 사전 설정으로 생성된 URL 문자열을 가져오려면 미리 보기 화면 또는 찾아보기 패널( 세부 사항 보기 )으로 이동합니다.

## 이미지 사전 설정 URL 가져오기 {#obtaining-an-image-preset-url}

[미리 보기] 또는 [세부 사항 보기]에서 이미지 사전 설정에 의해 생성된 URL 문자열을 얻을 수 있습니다. URL을 복사하면 필요한 경우 붙여 넣을 수 있도록 클립보드에 저장됩니다.

>[!NOTE]
>
>자산을 게시하기 전에는 URL이 활성화되지 않습니다.

### 미리 보기에서 이미지 사전 설정 URL 가져오기 {#obtaining-an-image-preset-url-from-preview}

1. 왼쪽의 자산 라이브러리 패널에서 미리 보려는 이미지 자산이 들어 있는 자산 폴더를 탐색합니다.
1. 다음 중 하나를 수행합니다.

   * 자산 창 위의 도구 모음 오른쪽에 있는 를 선택합니다 **[!UICONTROL 그리드 보기]**. 자산 창에서 단일 이미지 자산을 선택한 다음 축소판 이미지 아래에서 **[!UICONTROL 미리 보기]** > **[!UICONTROL 이미지 사전 설정 목록]**.
   * 자산 창 위의 도구 모음 오른쪽에 있는 를 선택합니다 **[!UICONTROL 목록 보기]**. 자산 창에서 단일 이미지 자산을 선택한 다음 축소판 이미지의 오른쪽으로 이동합니다. **[!UICONTROL 미리 보기]** > **[!UICONTROL 이미지 사전 설정 목록]**.
   * 자산 창 위의 도구 모음 오른쪽에 있는 를 선택합니다 **[!UICONTROL 세부 사항 보기]**. 동일한 도구 모음에서 **[!UICONTROL 미리 보기]** > **[!UICONTROL 이미지 사전 설정 목록]**.

1. (선택 사항) 이미지 사전 설정 목록의 복사 URL 생성을 위한 URL 인코딩 드롭다운 목록에서 이미지 자산을 복사할 때 이미지 자산의 URL에 적용할 URL 인코딩을 선택합니다.
1. 이미지 사전 설정 목록 창의 미리 보기 창의 오른쪽 위에서 을 선택합니다 **[!UICONTROL URL 복사]** 선택한 사전 설정 유형에 대해 설명합니다.
1. 이미지 사전 설정 목록 창의 오른쪽 아래 모서리에서 을(를) 선택합니다 **[!UICONTROL 닫기]** 자산 화면으로 돌아갑니다.

### 찾아보기 패널에서 이미지 사전 설정 URL 가져오기 {#obtaining-an-image-preset-url-from-the-browse-panel}

1. 왼쪽의 자산 라이브러리 패널에서 미리 보려는 이미지 자산이 들어 있는 자산 폴더를 탐색합니다.
1. 자산 창 위의 도구 모음 오른쪽에 있는 를 선택합니다 **[!UICONTROL 그리드 보기]**. [자산] 창에서 단일 이미지 자산을 선택합니다.
1. 자산 창 위의 도구 모음 오른쪽에 있는 를 선택합니다 **[!UICONTROL 세부 사항 보기]**.
1. 선택 **[!UICONTROL URL]** 을 클릭합니다.
1. 선택 **[!UICONTROL URL 복사]** 를 클립보드에 복사할 URL이 있는 이미지 사전 설정 이름 옆에 연결합니다.

## 이미지 사전 설정 URL 문자열 정보 {#about-image-preset-url-strings}

Dynamic Media 이미지 서버에 대한 이미지 크기 조정을 위한 URL 호출에는 다음과 같은 기본 구문이 있습니다.

*path*/*name of Image Server*/*account name*/*image name*?*modifier1*&amp;*modifier2*&amp;...

Dynamic Media 이미지 서버 URL에서 이미지 표시를 위한 서버 지침은 물음표(?) 뒤에 표시됩니다. 예를 들어 다음 URL 호출은 &quot;backpack&quot;이라는 이미지를 250픽셀 너비로 제공합니다.

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

URL에서 이미지 사전 설정 이름은 달러 기호($)로 묶여 있습니다. Dynamic Media 이미지 서버가 URL의 이미지 사전 설정 부분( `Large` 이 경우), &quot;큰&quot; 이미지 사전 설정에 정의된 크기 및 형식 지정 지침을 사용합니다.

## 웹 페이지에 동적 이미지 추가 {#adding-dynamic-images-to-your-web-page}

웹 페이지에 다이내믹 이미지를 추가하려면 `<IMG>` HTML 웹 페이지 코드의 태그는 일반적으로 Dynamic Media 이미지 서버에 요청을 수행하기 위해 Adobe Dynamic Media Classic URL 문자열을 사용하여 수정됩니다. 이 문자열은 이미지 사전 설정에 의해 정의된 크기 및 형식 지정 사양에 따라 이미지를 생성합니다.

예를 들어 다음과 같은 일반적인 정적 이미지 열기 호출이 있습니다.

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

이제 를 사용합니다 `<IMG>`태그로 정적 이미지에 대한 참조를 Adobe Dynamic Media Classic 플랫폼에 대한 이미지 사전 설정 호출로 바꿉니다. 샘플 호출은 다음과 같이 표시됩니다.

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$”
```

이 예에서는 Dynamic Media 이미지 서버가 `$thumbnail$` 및 는 `thumbnail`이미지 사전 설정. URL 문자열에서 제품 이미지 파일 이름(이 경우 `backpack_trns`)을 제외한 모든 항목은 대체로 페이지 템플릿에 내장됩니다. 상거래 서버에서 페이지 템플릿에 자동으로 삽입되는 요소는 이미지의 IPS ID 또는 이름뿐입니다.
