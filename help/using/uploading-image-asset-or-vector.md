---
title: 래스터 이미지 자산 업로드
description: 래스터 이미지 에셋을 Adobe Dynamic Media Classic에 업로드하는 방법을 알아봅니다
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: User
exl-id: 2ef78fe6-1e7c-4f48-86da-137ddaa55bbf
topic: Content Management
level: Intermediate
source-git-commit: ae7d0c6d3047d68ed3da4187ef516dc51c95de30
workflow-type: tm+mt
source-wordcount: '1008'
ht-degree: 57%

---

# 래스터 이미지 자산 업로드 {#uploading-an-image-asset-or-a-vector-asset}

이미지 자산을 업로드하려면 먼저 공유 비밀 키를 요청합니다. 이 공유 보안 키를 사용하여 업로드 토큰을 검색합니다. 그런 다음 업로드 토큰을 사용하여 래스터 이미지 에셋을 업로드합니다.

>[!IMPORTANT]
>
>2023년 5월 1일부터 Dynamic Media의 UGC 에셋은 업로드일로부터 최대 60일까지 사용할 수 있습니다. 60일 이후에는 에셋이 제거됩니다.

>[!NOTE]
>
>Adobe Dynamic Media Classic의 신규 또는 기존 UGC 벡터 자산에 대한 지원은 2021년 9월 30일에 종료되었습니다.

## 공유 암호 키 요청 {#requesting-a-shared-secret-key}

요청 a *공유 암호 키* 작성자: [Admin Console을 사용하여 지원 사례를 만듭니다.](https://helpx.adobe.com/enterprise/using/support-for-experience-cloud.html) 지원 사례에서 공유 암호 키를 요청합니다.

이메일 메시지에 이미지 자산을 업로드하는 데 사용할 회사 이름을 제공합니다. Adobe Dynamic Media Classic에서 키를 받으면 나중에 사용할 수 있도록 로컬에 저장합니다.

## 업로드 토큰 검색 {#retrieving-the-upload-token}

*업로드 토큰*&#x200B;은 아무도 동일한 공유 보안 키를 사용하여 자산을 업로드할 수 없게 하며, 업로드가 합법적이고 신뢰할 수 있는 소스에서 제공된 것인지 확인합니다.

업로드 토큰은 특정 시간 동안만 사용할 수 있는 영숫자 문자열입니다. 업로드 토큰을 검색할 수 있도록 다음 URL을 사용하여 공유 암호 키를 대체하십시오.

* 래스터 이미지
  `https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602`이 예제에서 공유 암호 키는 `fece4b21-87ee-47fc-9b99-2e29b78b602`

<!-- * Vector
  `https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9`In this example, the shared-secret key is `2d19f60e-890a-4e79-a1a5-9ac2875429b9` -->

기본적으로 업로드 토큰은 검색한 지 5분(300초) 후에 만료됩니다. 더 많은 시간을 요청하려면 다음을 포함하십시오. `expires` 를 입력합니다. 예를 들어 다음 샘플 이미지 URL은 1800초 동안 유효한 업로드 토큰을 검색합니다.

```as3
https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=1800
```

이미지에 대한 성공적인 응답은 다음과 유사하게 표시됩니다.

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
| --- | --- | --- |
| op | 필수 | get_uploadtoken |
| 공유 암호 | 필수 | 업로드를 수행하는 회사의 공유 보안 키입니다. |
| 만료 | 선택적 | 업로드 토큰이 유효한 시간(초)입니다. 지정하지 않으면 기본값은 300초입니다. |

**샘플 래스터 이미지 URL:**

`https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=600`

<!-- **Sample vector URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9&expires=5000` -->

**허용된 HTTP 메서드:**
`GET` 및 `POST`

이제 이미지 자산을 업로드할 수 있습니다.

다음을 참조하십시오 [이미지 자산 업로드](uploading-image-asset-or-vector.md#uploading_an_image_asset).

## 래스터 이미지 자산 업로드 {#uploading-an-image-asset}

특정 시간 동안 유효한 업로드 토큰을 검색한 후 이미지 자산을 업로드할 수 있습니다. 다음 예와 같이 자산을 멀티파트/양식 게시로 업로드하고 나머지 값을 URL 쿼리 문자열로 보냅니다.

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company
```

다음 `upload_token` 및 `company_name` 필드는 필수입니다.

다음을 참조하십시오 [업로드 토큰 검색](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

다음을 참조하십시오 [공유 암호 키 검색](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

다음 예와 같이 다른 선택적 값을 URL 쿼리 문자열로 보낼 수도 있습니다.

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=jpg,gif
```

다음 `file_limit` 매개 변수는 파일 크기 제한(바이트)을 지정합니다. 다음 `file_exts` 매개 변수는 업로드에 허용되는 파일 이름 확장자를 지정합니다. 두 값은 모두 선택 사항입니다.

허용되는 파일 이름 확장자와 파일 크기 제한에 대해 애플리케이션에서 글로벌 제한이 설정됩니다. 요청에 보내는 내용이 글로벌 제한의 하위 집합이면 허용됩니다. 글로벌 제한은 다음과 같습니다.

| 글로벌 제한 | 값 |
| --- | --- |
| 모든 클라이언트의 파일 크기 | 20 MB |
| 업로드가 지원되는 이미지 파일 형식 | BMP, GIF, JPG, PNG, PSD, TIFF |

다음 HTML 양식을 사용하여 자산을 업로드할 수 있습니다. 이 양식에서 사용자는 다음 정보를 입력해야 합니다.

* 회사 이름.
* 업로드 토큰.
* 파일 크기 제한.
* 파일 이름 확장자 목록입니다.
* 자산과 연결된 색상 프로파일 및 파일 이름을 유지할지 여부입니다.
* 녹아웃 배경 사용 여부. [녹아웃 배경]을 활성화하면 [모퉁이], [허용치] 및 [채우기 방법]을 설정합니다.
에서 녹아웃 배경 보기 [업로드 시 이미지 세부 조정 옵션](image-editing-options-upload.md#image-editing-options-at-upload).
* 업로드할 파일의 이름입니다.

을(를) 선택하여 위 양식과 연결된 HTML 소스 코드를 볼 수 있습니다. [https://s7ugc1.scene7.com/ugc/upload.html](https://s7ugc1.scene7.com/ugc/upload.html)

Firefox에서 브라우저 창을 마우스 오른쪽 단추로 클릭하고 를 선택합니다. **[!UICONTROL 페이지 소스 보기]**. 이 코드는 사용자가 선택할 때 실행되는 해당 URL 쿼리 문자열 및 POST 메서드를 보여 줍니다 **[!UICONTROL 제출]**.

Internet Explorer에서 XML 응답을 보려면 **[!UICONTROL 보기]** > **[!UICONTROL 소스]**. Firefox에서 XML 응답을 보려면 **[!UICONTROL 도구]** > **[!UICONTROL 브라우저 도구]** > **[!UICONTROL 웹 개발자 도구]**. XML 응답을 보려는 경우 Firefox를 사용하는 것이 좋습니다.

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

자산은 다른 ImageServing 리소스와 같으며, 자산에 처리 쿼리를 적용할 수 있습니다. 예를 들어 다음 URL은 지정된 너비 및 높이까지 확장된 에셋을 요청합니다.

```as3
https://s7w2p1.scene7.com/is/image/S7WebUGC/ugc/9536356.tif?&wid=800&hei=100&fit=stretch
```

멀티파트/양식 게시로 업로드할 자산을 보내고 나머지 값을 URL 쿼리 문자열로 보냅니다. URL 쿼리 문자열에 다음 필드를 사용하여 자산을 업로드할 수 있습니다.

| URL 매개 변수 | 필수 또는 선택 사항 | 값 |
| --- | --- | --- |
| `op` | 필수 | 업로드 |
| `upload_token` | 필수 | 회사와 관련된 공유 보안 키의 업로드 토큰입니다. |
| `company_name` | 필수 | 업로드를 수행하는 회사 이름입니다. |
| `file_limit` | 선택적 | 자산의 파일 크기 제한(바이트)입니다. |
| `file_exts` | 선택적 | 이미지 자산 파일에 허용되는 확장자 목록입니다. |
| `preserve_colorprofile` | 선택적 | 임베드된 색상 프로필을 유지하고 업로드한 파일을 PTIFF 형식으로 전환합니다. 가능한 값은 true 또는 false입니다. 기본값은 false입니다. |
| `preserve_filename` | 선택적 | 업로드한 자산의 파일 이름을 유지합니다. 가능한 값은 true 또는 false입니다. 기본값은 false입니다. |

>[!NOTE]
>
>업로드할 자산을 멀티파트 POST 요청의 유일한 필드로 보내야 합니다.

**샘플 URL:**

`https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company`

**허용되는 HTTP 메서드:**

POST

### 이미지에 대한 자산 메타데이터 가져오기 {#getting-asset-metadata-for-images}

다음을 사용할 수 있습니다. `image_info` 업로드한 에셋에 대한 메타데이터를 검색하려면 다음 예를 참조하십시오.

```as3
https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

성공적인 응답의 예는 다음과 유사하게 표시됩니다.

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
| --- | --- | --- |
| `op` | 필수 | image_info |
| `shared_secret` | 필수 | 회사의 공유 보안 키입니다. |
| `image_name` | 필수 | 이미지 이름입니다. |

**샘플 URL:**

`https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**허용되는 HTTP 메서드:**

GET 및 POST

<!-- ## Upload a vector asset {#uploading-a-vector-asset}

>[!IMPORTANT]
>
>Support for new or existing UGC vector image assets in Adobe Dynamic Media Classic end on September 30, 2021.

After you retrieve an upload token that is valid for a specific amount of time, you can upload a vector asset. You upload the asset as a multipart/form post while sending the rest of the values as a URL query string, as shown in this example:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company
```

The `upload_token` and `company_name` fields are required.

See [Retrieve the upload token](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

See [Retrieve a shared-secret key](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

You can also send other optional values as URL query strings, as in this example:

```as3
https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=ai,pdf
```

The `file_limit` parameter specifies the file-size limit in bytes. The `file_exts` parameter specifies the filename extensions that are allowed for upload. Both of these values are optional.

A global limit is set in the application for the file size limit and the filename extensions allowed. If what you send in the request is a subset of the global limits, it is honored. The global limits are the following:

| Global limit | Value |
| --- | --- |
| File size for all clients | 20 MB |
| Supported vector file formats for upload | AI, EPS, PDF (only when the PDF is previously opened and saved in Adobe Illustrator CS6) |

The following HTML form lets a user upload an asset. The form asks the user to enter the following information:

* A company name.
* An upload token.
* A file size limit.
* A list of filename extensions.
* Whether to preserve the color profile and file name associated with the asset.
* Whether to use Knockout Background. If you enable Knockout Background, set the Corner, Tolerance, and Fill Method.
See Knockout Background in [Image fine-tuning options at upload](image-editing-options-upload.md#image-editing-options-at-upload).
* The name of the file to upload.

The following HTML code is displayed when you right-click in the browser window, and then select **[!UICONTROL View Source]** for the form shown in the example. The code shows the corresponding URL query string and the POST method that are run when the user selects **[!UICONTROL Submit]**.

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
<td><strong>Select Submit to upload your Vector: </strong></td> 
<td><input type="submit" value="Submit"></td> 
</tr> 
</table> 
</form> 
</body>
```

To view the XML response in Internet Explorer, go to **[!UICONTROL View]** > **[!UICONTROL Source]**. To view XML response in Firefox, go to **[!UICONTROL Tools]** > **[!UICONTROL Browser Tools]** > **[!UICONTROL Page Source]**. Firefox is recommended for viewing XML responses.

The following is a sample response from a successful upload:

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
>The uploaded asset (AI, EPS, PDF so on) is converted to the FXG format and the response sends a direct link to that FXG asset.

The asset is like any other Web-to-print resource; you apply processing queries to it. For example, the following URL converts an FXG resource into a 500x500 png image.

```as3
https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg?fmt=png&wid=500&hei=500
```

Send the asset to upload as a multipart/form post while sending the rest of the values as a URL query string. You can use the following fields in the URL query string to upload an asset:

| URL Parameter | Required or Optional | Value |
| --- | --- | --- |
| `op` | Required | upload |
| `upload_token` | Required | Upload token for the shared-secret key associated with the company. |
| `company_name` | Required | Name of the company performing the upload. |
| `file_limit` | Optional | File size limit, in bytes, for the asset. |
| `file_exts` | Optional | List of allowable extensions for the asset file. |

>[!NOTE]
>
>You are required to send the asset to be uploaded as the only field in a multipart POST request.

**Sample URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_to ken=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company`

**Allowed HTTP method:**

POST
 -->