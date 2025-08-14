---
title: 업로드된 래스터 이미지 에셋 삭제
description: Adobe Dynamic Media Classic에서 업로드된 에셋을 삭제하는 방법을 알아봅니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: User
exl-id: d845bcb2-f914-4727-8df2-049dc172f266
topic: Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '136'
ht-degree: 34%

---

# 업로드된 자산 삭제{#deleting-an-uploaded-asset}

이 형식의 `delete` 매개 변수를 사용하여 자산을 삭제할 수 있습니다.

```as3
https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

다음은 이미지 자산을 삭제한 경우의 응답 예입니다.

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content: Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>delete</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>Delete request for1442564.tif</title> 
            <message>Your file was successfully deleted</message> 
        </response> 
    </user_generated_content> 
</scene7>
```

URL 쿼리 문자열에 다음 필드를 사용하여 자산을 삭제할 수 있습니다.

| URL 매개 변수 | 필수/선택 | 값 |
| --- | --- | --- |
| `op` | 필수 | 삭제 |
| `shared_secret` | 필수 | 회사의 공유 비밀인 키. |
| `image_name` | 필수 | 삭제할 자산 이름입니다. |

<!-- <li>For Vector:fxg_name</li> -->

>[!IMPORTANT]
>
>2023년 5월 1일부터 Dynamic Media의 UGC 에셋은 업로드일로부터 최대 60일 동안 사용할 수 있습니다. 60일 이후에는 에셋이 제거됩니다.

>[!NOTE]
>
>Adobe Dynamic Media Classic의 신규 또는 기존 UGC 벡터 이미지 자산에 대한 지원은 2021년 9월 30일에 종료되었습니다.

**샘플 이미지 URL:**

`https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

<!-- **Sample vector URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=delete&shared_secret=2160a8fa-cec6-45ba-8d59- ca595f6d2b47& &fxg_name=8875744.fxg` -->
