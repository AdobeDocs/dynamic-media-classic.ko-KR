---
title: 피어와 자산 변경 내용을 실시간으로 공유
description: Adobe Dynamic Media Classic에서 피어와 자산 변경 사항을 실시간으로 공유하는 방법을 알아봅니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management,Collaboration
role: Admin,User
exl-id: d74b4966-fe43-4349-bbe1-3a379c49bf1f
topic: Administration, Collaboration
level: Intermediate
source-git-commit: 163eb32112ec6fbefd1dacf48212353ff3053d54
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 26%

---

# 피어와 자산 변경 내용을 실시간으로 공유{#sharing-asset-changes-with-peers-in-real-time}

동일한 회사의 컴퓨터에서 실행 중인 Adobe Dynamic Media Classic의 복사본이 여러 개 있다고 가정해 봅시다. 이러한 시나리오에서는 모든 Dynamic Media Classic 클라이언트의 다음 작업이 모든 피어 클라이언트로 실시간으로 업데이트됩니다.

* 에셋 편집(빌더, 이미지 편집기 등)
* 자산 이름 바꾸기
* 자산 삭제
* 자산 이동
* 하나 이상의 자산 업로드(데스크톱 및 FTP)
* 폴더 만들기, 삭제 또는 이름 바꾸기

원래 클라이언트가 변경된 후 동일한 회사에 로그인한 모든 피어 클라이언트가 변경 내용으로 업데이트됩니다. 피어가 이미지 편집기나 빌더에서 변경되는 자산을 편집 중인 경우가 아니면 알림 없이 피어에 변경 사항이 적용됩니다.

로그인할 때 피어 업데이트를 허용하거나 거부하라는 메시지가 표시됩니다. 이 메시지가 한 번만 표시되도록 선택을 &quot;저장&quot;할 수 있습니다. 선택을 지우려면 [글로벌 설정]의 [피어 지원 네트워킹] 패널에서 해당 사이트를 삭제합니다.

피어에 의해 변경된 에셋을 편집하는 경우 변경 사항을 빌더 또는 편집기로 수집하라는 메시지가 표시됩니다. **[!UICONTROL 예]**&#x200B;를 선택하면 빌더 또는 편집기가 에셋에 대한 모든 변경 내용을 취소하고 업데이트된 에셋을 가져옵니다. **[!UICONTROL 아니요]**&#x200B;를 선택한 경우 자산은 빌더 또는 편집기에서 변경되지 않으며 변경한 내용은 해당 세션에서 유지됩니다.

에셋을 저장하면 최신 버전이 존재한다는 알림과 함께 변경 내용으로 에셋을 덮어쓸 것인지 묻는 메시지가 표시됩니다.
