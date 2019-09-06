---
title: Scene7 Publishing System에서 자산 내보내기
seo-title: Scene7 Publishing System에서 자산 내보내기
description: 널
seo-description: Scene 7 Publishing System에서 자산을 내보내는 방법을 알아봅니다.
uuid: d 42 b 7 a 73-80 c 0-4 a 9 a-a 04 e -7 ef 53 e 6 fcf 22
contentOwner: 관리
content-type: 참조
products: sg_ Experiencemanager/dynamic-media-scene -7
geptopics: sg_ scenesevenondemand_ pk/categories/managing_ assets
discoiquuid: EB 850 EC 7-A 669-41 EA-B 2 B 0-4 C 9178 E 34 F 95
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Scene7 Publishing System에서 자산 내보내기{#exporting-assets-from-scene-publishing-system}

Scene7 Publishing System에서 편집한 자산을 로컬 네트워크 드라이브에 저장할 수 있습니다. 내보낸 자산은 이메일로 전송하거나 다운로드하기 위해 ZIP 파일로 번들됩니다.

내보내기 작업에 대해 ZIP 압축 파일의 최대 파일 크기는 1 GB입니다. 또한 내보내기 작업 당 최대 500 개의 자산을 내보낼 수 있습니다.

Dynamic Media Classic는 작업 화면에 내보내기 작업 기록을 유지합니다.

**Scene7 Publishing System에서 자산을 내보내려면**

1. 내보내려는 자산을 선택한 다음 **[파일]** &gt; **[내보내기]**&#x200B;를 클릭합니다.
1. [선택한 자산 내보내기] 창에서 **[이미지 선택 사항]**&#x200B;을 클릭하고 다음 중 원하는 선택 사항을 지정합니다. 사용자가 사용할 수 있는 선택 사항은 관리자가 결정합니다.

   **사전 설정을** 선택적으로, 내보낼 때 형식을 지정할 이미지 사전 설정을 선택합니다. 이미지 사전 설정을 선택하면 자산이 이미지 사전 설정에서 정의된 형식을 사용하기 때문에 다른 형식 지정 선택 사항은 사용할 수 없습니다.

   **변환자산** 파일이나 원본 이미지를 변환합니다.

   **크기표준** 크기를 선택할 수 있습니다. 또한 [크기] 드롭다운 목록에서 [기타]를 클릭하고 원하는 측정 단위를 선택한 다음 너비와 높이를 지정할 수 있습니다.

   또한 [Media Portal 사용자가 사용할 수 있는 내보내기 선택 사항 지정](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users)을 참조하십시오.

   **형식** 이미지 형식을 선택합니다.

   **색상** RGB, CMYK 또는 회색을 선택합니다.

   **해상도** 72, 150 또는 300 ppi를 선택합니다.

   **작업 이름** 내보내기에 작업 이름을 할당할 수 있습니다.

   **이메일을 보내어** 전자 메일을 통해 자산을 보낼 전자 메일 주소를 입력합니다. 이메일 메시지에는 수신자가 자산을 다운로드하기 위해 이동할 수 있는 URL이 표시됩니다.

1. **내보내기**&#x200B;를 클릭합니다.

다음 세 가지 기본 내보내기 작업이 지원됩니다.

* 원본 파일(자산의 원본 파일 내보내기)
* 사전 설정을 사용하여 전환(이미지 사전 설정을 사용하여 자산 형식 지정)
* 사전 설정 없이 전환(내보내기 대화 상자를 사용하여 이미지 수정자 지정)

다음 자산 유형은 내보낼 수 없습니다. 다른 모든 자산은 내보내기를 생성해야 합니다.

* 이미지 집합
* 렌더 집합
* 회전 집합
* 미디어 집합
* 다중 비트 전송률 집합
* eCatalog

또한 템플릿은 "원본 파일"로 내보낼 수 없습니다.

전환을 사용하여 다음 자산 유형을 내보낼 수 있습니다.

* 이미지
* 템플릿
* 조정된 이미지
* PDF(전환된 페이지 생성)
* Postscript

다양한 자산 유형의 많은 자산을 내보내는 경우 다음 동작이 발생합니다.

* 내보낼 수 없는 모든 자산 유형이 작업 전송 전에 목록에서 제거됩니다.
* 전환이 요청된 경우 전환할 수 있는 모든 유형이 전환되고 기타 모든 유형은 원본으로 내보내집니다.

