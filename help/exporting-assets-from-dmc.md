---
title: Adobe Dynamic Media Classic에서 자산 내보내기
description: Adobe Dynamic Media Classic에서 자산을 내보내는 방법을 알아봅니다.
uuid: d42b7a73-80c0-4a9a-a04e-7ef53e6fcf22
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eb850ec7-a669-41ea-b2b0-4c9178e34f95
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 5e3b0002-5ae2-4437-862f-caa098b04362
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 52%

---

# Adobe Dynamic Media Classic에서 자산 내보내기{#exporting-assets-from-dmc}

Adobe Dynamic Media Classic에서 편집한 자산을 로컬 네트워크 드라이브에 저장할 수 있습니다. 내보낸 자산은 이메일로 전송하거나 다운로드하기 위해 ZIP 파일로 번들됩니다.

내보내기 작업에 대해 ZIP 압축 파일의 최대 파일 크기는 1 GB입니다. 또한 내보내기 작업당 최대 500개의 자산을 사용할 수 있습니다.

Adobe Dynamic Media Classic은 작업 화면에 내보내기 작업 레코드를 유지합니다.

**Adobe Dynamic Media Classic에서 자산을 내보내려면 다음을 수행하십시오.**

1. 내보낼 자산을 선택한 다음 **[!UICONTROL 파일]** > **[!UICONTROL 내보내기]**&#x200B;로 이동합니다.
1. [선택한 자산 내보내기] 창에서 **[!UICONTROL [이미지 선택 사항]]**&#x200B;을 클릭하고 다음 중 원하는 선택 사항을 지정합니다. 사용자가 사용할 수 있는 선택 사항은 관리자가 결정합니다.

   * **[!UICONTROL 사전 설정]**  - 선택적으로, 자산을 내보낼 때 자산 형식을 지정하려면 이미지 사전 설정을 선택합니다. 이미지 사전 설정을 선택하면 자산이 이미지 사전 설정에서 정의된 형식을 사용하기 때문에 다른 형식 지정 선택 사항은 사용할 수 없습니다.

   * **[!UICONTROL 변환]**  - 자산 파일 또는 원본 이미지를 변환합니다.

   * **[!UICONTROL 크기]**  - 표준 크기를 선택할 수 있습니다. 또는 **[!UICONTROL 크기]** 드롭다운 목록에서 **[!UICONTROL 기타]**&#x200B;을 선택하고 원하는 측정 단위를 선택한 다음 너비와 높이를 지정할 수 있습니다.

      또한 [Media Portal 사용자가 사용할 수 있는 내보내기 옵션 지정](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users)을 참조하십시오.

   * **[!UICONTROL 형식]**  - 이미지 형식을 선택합니다.

   * **[!UICONTROL 색상]**  - RGB, CMYK 또는 회색을 선택합니다.

   * **[!UICONTROL 해상도]**  - 72ppi, 150ppi 또는 300ppi를 선택합니다.

   * **[!UICONTROL 작업 이름]**  - 내보내기에 작업 이름을 지정할 수 있습니다.

   * **[!UICONTROL 이메일 발송자]**  - 이메일을 통해 자산을 보내려면 이메일 주소를 입력합니다(선택적). 이메일 메시지에는 수신자가 자산을 다운로드하기 위해 이동할 수 있는 URL이 표시됩니다.

1. **[!UICONTROL 내보내기]**&#x200B;를 선택합니다.

다음 세 가지 기본 내보내기 작업이 지원됩니다.

* 원본 파일(자산의 원본 파일 내보내기)
* 사전 설정을 사용하여 전환(이미지 사전 설정을 사용하여 자산 형식 지정)
* 사전 설정 없이 전환(내보내기 대화 상자를 사용하여 이미지 수정자 지정)

다음 자산 유형은 내보낼 수 없습니다. 다른 모든 사용자는 내보내기를 생성합니다.

* 이미지 집합
* 렌더 집합
* 회전 집합
* 미디어 집합
* 다중 비트 전송률 집합
* eCatalog

또한 템플릿은 &quot;원본 파일&quot;로 내보낼 수 없습니다.

전환을 사용하여 다음 자산 유형을 내보낼 수 있습니다.

* 이미지
* 템플릿
* 조정된 이미지
* PDF(변환된 페이지 생성)
* PostScript®

다양한 자산 유형의 많은 자산을 내보내는 경우 다음 동작이 발생합니다.

* 내보낼 수 없는 모든 자산 유형이 작업 전송 전에 목록에서 제거됩니다.
* 전환이 요청된 경우 전환할 수 있는 모든 유형이 전환되고 기타 모든 유형은 원본으로 내보내집니다.
