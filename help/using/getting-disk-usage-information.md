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
autotag-review: '2026-05-13T19:50:49.049Z'
TQID: 'https://experienceleague.adobe.com/g-mRoL2yYGRH-uFr2ACD2qOxBAGUlMMtKKuKtsv2pQk'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 92
ht-degree: 42%

---

# 디스크 사용 정보 가져오기 {#get-disk-usage-information}

다음 예제와 같이 `disk_info` 매개 변수를 사용하여 회사의 디스크 공간 사용에 대한 정보를 검색할 수 있습니다.

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=d03b7e0b-c9dc-4c6c-af0b-419beeea1c63
```

샘플 응답은 다음과 같습니다.

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content: Images</serviceName> 
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
