---
title: 디스크 사용 정보 가져오기
seo-title: 디스크 사용 정보 가져오기
description: 널
seo-description: 디스크 사용 정보를 얻는 방법을 알아봅니다.
uuid: 01361693-53d0-4072-b7c3-f284631d28cf
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6763546d-83c4-42dc-879f-6bbfc8b56482
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '90'
ht-degree: 92%

---


# 디스크 사용 정보 가져오기 {#getting-disk-usage-information}

다음 예에 표시된 것처럼 `disk_info` 매개 변수를 사용하여 회사의 디스크 공간 사용 정보를 검색할 수 있습니다.

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=d03b7e0b-c9dc-4c6c-af0b-419beeea1c63
```

샘플 응답은 다음과 같습니다.

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>disk_info</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>Disk Information for d03b7e0b-c9dc-4c6c-af0b-419beeea1c63</title> 
            <message>Total Space available = 1395402342400 bytes. Total Space used = 0 bytes.</message> 
        </response> 
    </user_generated_content> 
</scene7>
```

URL 쿼리 문자열에 다음 필드를 사용하여 디스크 사용 정보를 가져올 수 있습니다.

| URL 매개 변수 | 필수/선택 | 값 |
|--- |--- |--- |
| op | 필수 | disk_info |
| shared_secret | 필수 | 회사의 공유 보안 키입니다. |

다음 샘플 코드는 000Company에 대한 디스크 정보를 가져옵니다.

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b9602
```

