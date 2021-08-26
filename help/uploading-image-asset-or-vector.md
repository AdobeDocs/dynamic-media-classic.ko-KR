---
title: 이미지 자산 또는 벡터 자산 업로드
description: 이미지 자산 또는 벡터 자산을 업로드하는 방법을 알아봅니다.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: User
exl-id: 2ef78fe6-1e7c-4f48-86da-137ddaa55bbf
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '1495'
ht-degree: 78%

---

# 이미지 자산 또는 벡터 자산 업로드{#uploading-an-image-asset-or-a-vector-asset}

이미지 자산을 업로드하려면 먼저 공유 비밀 키를 요청합니다. 이 공유 보안 키를 사용하여 업로드 토큰을 검색합니다. 그런 다음 업로드 토큰을 사용하여 이미지 자산 또는 벡터 자산을 업로드합니다.

## 공유 보안 키 요청 {#requesting-a-shared-secret-key}

Admin Console을 사용하여 *공유-암호 키*&#x200B;를 요청 하여 지원 사례를 만듭니다.[](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) 지원 사례에서 공유 암호 키를 요청합니다.

이메일 메시지에 이미지 자산을 업로드하는 데 사용할 회사 이름을 제공합니다. Dynamic Media Classic Adobe에서 키를 받은 후 나중에 사용할 수 있도록 로컬에 저장합니다.

## 업로드 토큰 검색 {#retrieving-the-upload-token}

*업로드 토큰*&#x200B;은 아무도 동일한 공유 보안 키를 사용하여 자산을 업로드할 수 없게 하며, 업로드가 합법적이고 신뢰할 수 있는 소스에서 제공된 것인지 확인합니다.

업로드 토큰은 특정 시간 동안만 사용할 수 있는 영숫자 문자열입니다. 업로드 토큰을 검색할 수 있도록 공유 암호 키를 대체하려면 다음 URL을 사용하십시오.

* 이미지
   `https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602`이 예제에서 공유 암호 키는 다음과 같습니다  `fece4b21-87ee-47fc-9b99-2e29b78b602`

* 벡터
   `https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9`이 예제에서 공유 암호 키는 다음과 같습니다  `2d19f60e-890a-4e79-a1a5-9ac2875429b9`

기본적으로 업로드 토큰은 검색한 지 5분(300초) 후에 만료됩니다. 추가 시간을 요청하려면 URL에 `expires`와 요청하는 시간(초)을 포함합니다. 예를 들어 다음 샘플 이미지 URL은 1800초 동안 유효한 업로드 토큰을 검색합니다.

```as3
https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=1800
```

이미지에 대한 성공적인 응답은 다음과 비슷합니다.

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
        <serviceName>User Generated Content - Images</serviceName> 
        <version>1.0.0</version> 
        <operationName>get_uploadtoken</operationName> 
        <serviceStatus>SUCCESS</serviceStatus> 
        <title>Upload Token for fece4b21-87ee-47fc-9b99-2e29b78b602</title> 
        <message> 
            <uploadtoken>aa2a378a-cd25-4c80-994d-312094e0ef20_1800</uploadtoken> 
            <expiration_in_seconds>1800</expiration_in_seconds> 
        </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

이후 요청에 사용하기 위해 업로드 토큰을 로컬에 저장합니다.

URL 쿼리 문자열에 다음 필드를 사용하여 업로드 토큰을 검색할 수 있습니다.

| URL 매개 변수 | 필수 또는 선택 사항 | 값 |
|--- |--- |--- |
| op | 필수 | get_uploadtoken |
| shared_secret | 필수 | 업로드를 수행하는 회사의 공유 보안 키입니다. |
| expires | 선택 사항입니다 | 업로드 토큰이 유효한 시간(초)입니다. 지정하지 않으면 기본값은 300초입니다. |

**샘플 이미지 URL:**

`https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=600`

**샘플 벡터 URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9&expires=5000`

**허용되는 HTTP 메서드:**
`GET`  및  `POST`

이제 이미지 자산을 업로드할 수 있습니다.

[이미지 자산 업로드](uploading-image-asset-or-vector.md#uploading_an_image_asset)를 참조하십시오.

## 이미지 자산 업로드 {#uploading-an-image-asset}

특정 시간 동안 유효한 업로드 토큰을 검색한 후 이미지 자산을 업로드할 수 있습니다. 다음 예와 같이 자산을 멀티파트/양식 게시로 업로드하고 나머지 값을 URL 쿼리 문자열로 보냅니다.

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company
```

`upload_token` 및 `company_name` 필드가 필요합니다.

[업로드 토큰 검색](uploading-image-asset-or-vector.md#retrieving_the_upload_token)을 참조하십시오.

[공유 보안 키 검색](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key)을 참조하십시오.

다음 예와 같이 다른 선택적 값을 URL 쿼리 문자열로 보낼 수도 있습니다.

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=jpg,gif
```

`file_limit` 매개 변수는 파일 크기 제한을 바이트 단위로 지정합니다. `file_exts` 매개 변수는 업로드할 수 있는 파일 이름 확장자를 지정합니다. 두 값은 모두 선택 사항입니다.

허용되는 파일 이름 확장자와 파일 크기 제한에 대해 애플리케이션에서 글로벌 제한이 설정됩니다. 요청에 보내는 내용이 글로벌 제한의 하위 집합이면 허용됩니다. 글로벌 제한은 다음과 같습니다.

| 글로벌 제한 | 값 |
|--- |--- |
| 모든 클라이언트의 파일 크기 | 20 MB |
| 업로드가 지원되는 이미지 파일 형식 | BMP, GIF, JPG, PNG, PSD |

다음 HTML 양식을 사용하여 자산을 업로드할 수 있습니다. 이 양식에서 사용자는 다음 정보를 입력해야 합니다.

* 회사 이름.
* 업로드 토큰.
* 파일 크기 제한.
* 파일 이름 확장자 목록.
* 자산과 연관된 색상 프로필 및 파일 이름을 보존할지 여부.
* 녹아웃 배경 사용 여부. 배경 녹아웃(Cnoting Background)을 활성화할 경우 코너(Corner), 공차(Tolerance) 및 채우기 방법(Fill Method)을 설정합니다.
업로드](image-editing-options-upload.md#image-editing-options-at-upload)의 [이미지 편집 옵션에서 배경 녹아웃 을 참조하십시오.
* 업로드할 파일 이름.

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Art Spec: If not leaving art spec, delete only the first of the 2 &lt;draft-comment> elements under &lt;adobefig>.</p>

 -->

[https://s7ugc1.scene7.com/ugc/upload.html](https://s7ugc1.scene7.com/ugc/upload.html)을 클릭하여 위의 양식과 연결된 HTML 소스 코드를 볼 수 있습니다

Firefox에서 브라우저 창에서 마우스 오른쪽 단추를 클릭하고 **[!UICONTROL 페이지 소스 보기]**&#x200B;를 클릭합니다. 이 코드는 사용자가 **[!UICONTROL [전송]]**&#x200B;을 클릭할 때 실행되는 POST 메서드와 해당 URL 쿼리 문자열을 보여 줍니다

Internet Explorer에서 XML 응답을 보려면 **[!UICONTROL [보기]]** > **[!UICONTROL [소스]]**&#x200B;를 클릭합니다. Firefox에서 XML 응답을 보려면 **[!UICONTROL 도구]** > **[!UICONTROL 브라우저 도구]** > **[!UICONTROL 웹 개발자 도구]**&#x200B;를 클릭합니다. XML 응답을 보려는 경우 Firefox를 사용하는 것이 좋습니다.

다음은 성공적인 업로드에 대한 샘플 응답입니다.

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>upload</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>Your file has been uploaded Successfully.</title> 
            <message> 
            <url>https://s7w2p1.scene7.com/is/image/ </url> 
            <path>000Company/ugc/1442564.tif</path> 
            <fullurl>https://s7w2p1.scene7.com/is/image/000Company/ugc/1442564.tif </fullurl> 
            </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

>[!NOTE]
>
>업로드한 자산(JPG, GIF 등)이 PTIFF 형식으로 전환되고 응답에서 해당 PTIFF 자산에 대한 직접 링크를 보냅니다.

자산은 다른 ImageServing 리소스와 같으며, 자산에 처리 쿼리를 적용할 수 있습니다. 예를 들어 다음 URL은 지정한 너비와 높이로 늘린 자산을 요청합니다.

```as3
https://s7w2p1.scene7.com/is/image/S7WebUGC/ugc/9536356.tif?&wid=800&hei=100&fit=stretch
```

멀티파트/양식 게시로 업로드할 자산을 보내고 나머지 값을 URL 쿼리 문자열로 보냅니다. URL 쿼리 문자열에 다음 필드를 사용하여 자산을 업로드할 수 있습니다.

| URL 매개 변수 | 필수 또는 선택 사항 | 값 |
|--- |--- |--- |
| `op` | 필수 | 업로드 |
| `upload_token` | 필수 | 회사와 관련된 공유 보안 키의 업로드 토큰입니다. |
| `company_name` | 필수 | 업로드를 수행하는 회사 이름입니다. |
| `file_limit` | 선택 사항입니다 | 자산의 파일 크기 제한(바이트)입니다. |
| `file_exts` | 선택 사항입니다 | 이미지 자산 파일에 허용되는 확장자 목록입니다. |
| `preserve_colorprofile` | 선택 사항입니다 | 임베드된 색상 프로필을 유지하고 업로드한 파일을 PTIFF 형식으로 전환합니다. 가능한 값은 true 또는 false입니다. 기본값은 false입니다. |
| `preserve_filename` | 선택 사항입니다 | 업로드한 자산의 파일 이름을 유지합니다. 가능한 값은 true 또는 false입니다. 기본값은 false입니다. |

>[!NOTE]
>
>업로드할 자산을 멀티파트 POST 요청의 유일한 필드로 보내야 합니다.

**샘플 URL:**

`https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company`

**허용되는 HTTP 메서드:**

POST

### 이미지의 자산 메타데이터 가져오기 {#getting-asset-metadata-for-images}

다음 예와 같이 `image_info`를 사용하여 업로드한 자산의 메타데이터를 검색할 수 있습니다.

```as3
https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

성공적인 응답의 예는 다음과 유사하게 나타납니다.

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>image_info</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>More information on 1442564.tif</title> 
            <message> 
            File created on Tue Sep 08 19:02:04 CDT 2009, File Size = 243494 bytes 
            <imageFormat>Tiff</imageFormat> 
            <colorSpace>Rgb</colorSpace> 
            <width>686</width> 
            <height>457</height> 
            </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

URL 쿼리 문자열에 다음 필드를 사용하여 자산에 대한 정보를 요청할 수 있습니다.

| URL 매개 변수 | 필수 또는 선택 사항 | 값 |
|--- |--- |--- |
| `op` | 필수 | image_info |
| `shared_secret` | 필수 | 회사의 공유 보안 키입니다. |
| `image_name` | 필수 | 이미지 이름입니다. |

**샘플 URL:**

`https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**허용되는 HTTP 메서드:**

GET 및 POST

## 벡터 자산 업로드 {#uploading-a-vector-asset}

특정 시간 동안 유효한 업로드 토큰을 검색한 후 벡터 자산을 업로드할 수 있습니다. 다음 예와 같이 자산을 멀티파트/양식 게시로 업로드하고 나머지 값을 URL 쿼리 문자열로 보냅니다.

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company
```

`upload_token` 및 `company_name` 필드가 필요합니다.

[업로드 토큰 검색](uploading-image-asset-or-vector.md#retrieving_the_upload_token)을 참조하십시오.

[공유 보안 키 검색](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key)을 참조하십시오.

다음 예와 같이 다른 선택적 값을 URL 쿼리 문자열로 보낼 수도 있습니다.

```as3
https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=ai,pdf
```

`file_limit` 매개 변수는 파일 크기 제한을 바이트 단위로 지정합니다. `file_exts` 매개 변수는 업로드할 수 있는 파일 이름 확장자를 지정합니다. 두 값은 모두 선택 사항입니다.

허용되는 파일 이름 확장자와 파일 크기 제한에 대해 애플리케이션에서 글로벌 제한이 설정됩니다. 요청에 보내는 내용이 글로벌 제한의 하위 집합이면 허용됩니다. 글로벌 제한은 다음과 같습니다.

| 글로벌 제한 | 값 |
|--- |--- |
| 모든 클라이언트의 파일 크기 | 20MB |
| 업로드가 지원되는 벡터 파일 형식 | AI, EPS, PDF(PDF가 이전에 열리고 Adobe Illustrator CS6에 저장된 경우에만) |

다음 HTML 양식을 사용하여 자산을 업로드할 수 있습니다. 이 양식에서 사용자는 다음 정보를 입력해야 합니다.

* 회사 이름.
* 업로드 토큰.
* 파일 크기 제한.
* 파일 이름 확장자 목록.
* 자산과 연관된 색상 프로필 및 파일 이름을 보존할지 여부.
* 녹아웃 배경 사용 여부. 배경 녹아웃(Cnoting Background)을 활성화할 경우 코너(Corner), 공차(Tolerance) 및 채우기 방법(Fill Method)을 설정합니다.
업로드](image-editing-options-upload.md#image-editing-options-at-upload)의 [이미지 편집 옵션에서 배경 녹아웃 을 참조하십시오.
* 업로드할 파일 이름.

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Art Spec: If not leaving art spec, delete only the first of the 2 &lt;draft-comment> elements under &lt;adobefig>.</p>

 -->

다음 HTML 코드는 브라우저 창에서 마우스 오른쪽 단추를 클릭하고 예제에 표시된 양식에 대해 **[!UICONTROL 소스 보기]**&#x200B;를 클릭하면 표시됩니다. 이 코드는 사용자가 **[!UICONTROL [전송]]**&#x200B;을 클릭할 때 실행되는 POST 메서드와 해당 URL 쿼리 문자열을 보여 줍니다

```as3
<body> 
<script language="javascript"> 
function uploadImage() 
{ 
document.image_upload.action="vector?op=upload&company_name="+document.image_upload.company_name.value+"&upload_token="+document.image_upload.upload_token.value+"&file_limit="+document.image_upload.file_limit.value+"&file_exts="+document.image_upload.file_exts.value; 
return true; 
} 
</script> 
<form method="POST" enctype="multipart/form-data" name="image_upload" id="image_upload" onSubmit="return uploadImage();"> 
<table> 
<tr><td colspan="2"><strong> UGC Vector Upload Test Page: </strong></td></tr> 
<tr><td colspan="2"></td></tr> 
<tr><td><strong> Company Name</strong></td><td><input type="text" size="40" name="company_name"></td></tr> 
<tr><td><strong> Upload Token </strong></td><td><input type="text" size="40" name="upload_token"></td></tr> 
<tr><td><strong> File Size Limit (in bytes) </strong></td><td><input type="text" size="40" name="file_limit"> bytes</td></tr> 
<tr><td><strong> File Extensions allowed </strong></td><td><input type="text" size="40" name="file_exts"></td></tr> 
<tr><td colspan="2"></td></tr> 
<tr> 
<td><strong>File to upload: : </strong></td> 
<td><input name="filename" type="file" id="filename" size="58" maxlength="1024" /></td> 
</tr> 
<tr><td colspan="2"></td></tr> 
<tr> 
<td><strong>Click Submit to upload your Vector: </strong></td> 
<td><input type="submit" value="Submit"></td> 
</tr> 
</table> 
</form> 
</body>
```

Internet Explorer에서 XML 응답을 보려면 **[!UICONTROL [보기]]** > **[!UICONTROL [소스]]**&#x200B;를 클릭합니다. Firefox에서 XML 응답을 보려면 **[!UICONTROL 도구]** > **[!UICONTROL 브라우저 도구]** > **[!UICONTROL 페이지 소스]**&#x200B;를 클릭합니다. XML 응답을 보려는 경우 Firefox를 사용하는 것이 좋습니다.

다음은 성공적인 업로드에 대한 샘플 응답입니다.

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
    <scene7> 
    <user_generated_content> 
    <response> 
    <serviceName>User Generated Content -Vector</serviceName> 
    <version>1.0.0</version> 
    <operationName>upload</operationName> 
    <serviceStatus>SUCCESS</serviceStatus> 
    <title>Your file has been uploaded Successfully.</title> 
    <message> 
    <url>https://s7w2p1.scene7.com/is/agm</url> 
    <path>W2PTest/ugc/8875744.fxg</path> 
    <fullurl> 
        https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg 
    </fullurl> 
</message> 
</response> 
</user_generated_content> 
</scene7>
```

>[!NOTE]
>
>업로드한 자산(AI, EPS, PDF 등)이 FXG 형식으로 전환되고 응답이 해당 FXG 자산에 대해 직접 링크를 보냅니다.

자산은 다른 Web-to-Print 리소스와 같습니다. 처리 쿼리를 적용합니다. 예를 들어 다음 URL은 FXG 리소스를 500x500png 이미지로 전환합니다.

```as3
https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg?fmt=png&wid=500&hei=500
```

멀티파트/양식 게시로 업로드할 자산을 보내고 나머지 값을 URL 쿼리 문자열로 보냅니다. URL 쿼리 문자열에 다음 필드를 사용하여 자산을 업로드할 수 있습니다.

| URL 매개 변수 | 필수 또는 선택 사항 | 값 |
|--- |--- |--- |
| `op` | 필수 | 업로드 |
| `upload_token` | 필수 | 회사와 관련된 공유 보안 키의 업로드 토큰입니다. |
| `company_name` | 필수 | 업로드를 수행하는 회사 이름입니다. |
| `file_limit` | 선택 사항입니다 | 자산의 파일 크기 제한(바이트)입니다. |
| `file_exts` | 선택 사항입니다 | 자산 파일에 허용되는 확장자 목록입니다. |

>[!NOTE]
>
>업로드할 자산을 멀티파트 POST 요청의 유일한 필드로 보내야 합니다.

**샘플 URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_to ken=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company`

**허용되는 HTTP 메서드:**

POST
