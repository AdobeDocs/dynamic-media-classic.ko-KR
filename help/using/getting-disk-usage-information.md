---
title: 디스크 사용 정보 가져오기
description: Adobe Dynamic Media Classic에서 디스크 사용 정보를 가져오는 방법에 대해 알아봅니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 337a4681-ac9a-40d9-82e8-1999bbed980c
topic: Administration, Content Management
level: Intermediate
source-git-commit: f054057d383b26e9088582f418f62504c3f327d8
workflow-type: tm+mt
source-wordcount: '91'
ht-degree: 42%

---

# 디스크 사용 정보 가져오기 {#get-disk-usage-information}

다음을 사용할 수 있습니다. `disk_info` 매개 변수를 사용하여 다음 예와 같이 회사의 디스크 공간 사용에 대한 정보를 검색합니다.

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
| --- | --- | --- |
| op | 필수 | disk_info |
| 공유 암호 | 필수 | 회사의 공유 비밀인 키 |

다음 샘플 코드는 000Company에 대한 디스크 정보를 가져옵니다.

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b9602
```
