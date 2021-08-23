---
title: Media Portal 사용자 추가 및 관리
description: Dynamic Media Classic에서 Media Portal 사용자를 추가하고 관리하는 방법을 알아봅니다.
uuid: 96d4103c-6428-4ce1-b9e4-231599304f27
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 5e933045-ce1a-41b9-ba8b-2151c396b7a2
feature: Dynamic Media Classic,공동 작업,자산 관리
role: Admin,User
exl-id: 9590c53c-fd38-4bf2-b723-cd7369702364
source-git-commit: 1d30c98b76ebe78ff60bae87bd112de7a577182d
workflow-type: tm+mt
source-wordcount: '1018'
ht-degree: 58%

---

# Media Portal 사용자 추가 및 관리{#adding-and-managing-media-portal-users}

관리자는 사용자를 추가 및 관리하고, 사용자가 암호를 변경할 수 있는지 여부를 결정하고, 사용자 정보를 편집하고, 사용자 목록을 업로드할 수 있습니다. 이러한 작업은 [사용자 관리] 화면에서 수행합니다. 이 화면에 액세스하려면 **[!UICONTROL 설정]** > **[!UICONTROL 응용 프로그램 설정]** > **[!UICONTROL 관리 설정]** > **[!UICONTROL 사용자 관리]**&#x200B;로 이동합니다.

>[!NOTE]
>
>사용자를 추가하기 전에 사용자를 관리하기 위한 그룹을 설정합니다. Media Portal에서는 사용자를 하나 이상의 그룹에 지정하지 않을 경우 사용자를 추가할 수 없습니다. 자세한 내용은 [Media Portal 그룹 만들기 및 관리](creating-media-portal-groups.md#creating_and_managing_media_portal_groups)를 참조하십시오.

## Media Portal 암호 관리 {#handling-media-portal-passwords}

관리자가 등록하면 Media Portal 사용자, 기여자 및 기여자-사용자에게 암호가 포함된 환영 이메일 메시지가 전송됩니다. 관리자는 Media Portal 사용자가 이 암호를 변경할 수 있는지 여부를 결정할 수 있습니다.

1. **[!UICONTROL 설정]** > **[!UICONTROL Media Portal 설정]** > **[!UICONTROL 일반 설정]**&#x200B;으로 이동합니다.
1. [일반 설정] 페이지에서 **[!UICONTROL [Media Portal 사용자가 암호를 변경하도록 허용]]**&#x200B;을 선택하거나 선택 취소합니다.
1. **[!UICONTROL 저장]**&#x200B;을 선택합니다.

>[!NOTE]
>
>암호를 변경할 수 있는 Media Portal 사용자는 **[!UICONTROL 설정]** > **[!UICONTROL 개인 설정]**&#x200B;을 선택하고 개인 설정 화면에서 암호를 변경하면 됩니다.

## Media Portal 사용자 추가 {#adding-a-media-portal-user}

1. **[!UICONTROL 설정]** > **[!UICONTROL 응용 프로그램 설정]** > **[!UICONTROL 관리 설정]** > **[!UICONTROL 사용자 관리]**&#x200B;로 이동합니다.
1. 사용자 관리 페이지에서 **추가**&#x200B;를 선택합니다.
1. 사용자 추가 대화 상자의 사용자 정보 패널에서 사용자의 이름, 성 및 전자 메일 주소를 입력한 다음 **[!UICONTROL 다음]**&#x200B;을 선택합니다.
1. [회사/역할] 패널의 [회사] 드롭다운 목록에서 사용자의 회사를 선택합니다.
1. 역할 목록에서 미디어 포털 역할을 선택한 다음 **[!UICONTROL 다음]**&#x200B;을 선택합니다.

   [Media Portal 사용자 역할](media-portal-user-roles.md#media_portal_user_roles)을 참조하십시오.

1. [액세스 그룹] 패널에서 하나 이상의 그룹을 선택합니다.

   [Media Portal 그룹 만들기 및 관리](creating-media-portal-groups.md#creating_and_managing_media_portal_groups)를 참조하십시오.

1. (선택 사항) **[!UICONTROL 전자 메일 설정]**&#x200B;을 선택하여 기본 설정과 다른 전자 메일 설정을 선택합니다.

   [Media Portal 사용자에 대한 환영 이메일 메시지 설정](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users)을 참조하십시오.

1. **[!UICONTROL 사용자 추가]**&#x200B;를 선택합니다.

사용자를 추가하면 Media Portal에서 사용자에게 환영 이메일 메시지를 보냅니다. 이 메시지에는 임시 암호와 Media Portal URL이 들어 있습니다.

## Media Portal 사용자 목록 업로드 {#uploading-a-media-portal-user-list}

추가할 사용자가 여러 명인 경우 사용자 목록을 업로드할 수 있습니다. 사용자가 현재 선택한 계정에 자동으로 추가됩니다.

사용자 정보가 포함된 CSV(쉼표로 구분된 값) 파일로 사용자 목록을 만듭니다. 목록을 업로드하면 목록에 있는 사용자가 지정된 그룹 지정과 함께 계정에 자동으로 추가됩니다. Media Portal 링크와 임시 암호가 포함된 환영 이메일이 새 사용자에게 각각 전송됩니다.

### CSV 파일 만들기 {#creating-the-csv-file}

다음 형식과 필드를 준수하는 CSV 파일(filename.csv)을 만듭니다. 파일의 첫 번째 행에는 다음 표에 나열된 열 머리글이 포함되어야 합니다. 열 순서는 원하는 대로 변경할 수 있습니다. 모든 열이 필수입니다.

| 열 이름 | 설명 |
|--- |--- |
| 이름 | 이름입니다. |
| 성 | 성입니다. |
| 이메일 | 유효한 이메일 주소입니다. |
| 암호 | 대/소문자를 구분하는 암호 문자열입니다. |
| 사용자 역할 | MediaPortalAdminMediaPortalUserMediaPortalContributorMediaPortalContributorUser |
| 그룹 | 쉼표로 구분된 각 사용자에 대한 하나 이상의 계정 그룹 지정 목록입니다. 계정 이름에 접두어를 추가하고 슬래시(/)로 구분하여 그룹을 지정합니다. 예를 들어 PortalCo/IT와 같이 지정할 수 있으며 여기서 PortalCo는 계정이고 IT는 PortalCo 계정 내의 그룹입니다. |

다음 샘플 스프레드시트는 CSV 파일의 레이아웃을 지정하는 방법을 보여 줍니다.

| 이름 | 성 | 이메일 | 암호 | 사용자 역할 | 그룹 |
|--- |--- |--- |--- |--- |--- |
| 프레리 | Kat | `prairiek@company.com` | 시작 | Media Portal 관리자 | PortalCo/IT,PortalCo/Admin |
| 릭 | 브로크 | `rickb@myco.com` | 시작 | Media Portal 사용자 | PortalCo/MktgGroup, PortalCo/test |

### CSV 파일 업로드 {#uploading-the-csv-file}

1. [사용자 관리 설정] 화면을 엽니다.
1. **[!UICONTROL 사용자 목록 업로드]**&#x200B;를 선택합니다.
1. 업로드할 파일 선택 대화 상자에서 CSV 파일을 선택한 다음 **[!UICONTROL 열기]**&#x200B;를 선택합니다.

목록에 있는 각 사용자가 지정한 그룹에 자동으로 추가됩니다. 환영 이메일 메시지가 각 사용자에게 전송됩니다.

>[!NOTE]
>
>CSV 파일의 형식이 잘못된 경우 다음 오류 메시지가 표시됩니다. &quot;업로드된 CSV 파일을 처리하는 중 오류가 발생했습니다. 파일 컨텐츠에 유효한 데이터가 포함되어 있는지 확인하십시오.&quot; 또한 CSV에 기존 IP 또는 IPS 사용자가 포함되어 있는 경우 해당 사용자는 [사용자 목록]에 추가되지 않습니다.

## 선택 가능한 Media Portal 사용자 목록 생성 {#generating-a-selectable-list-of-media-portal-users}

Media Portal 사용자의 이름과 이메일 주소를 팝업 창에 표시할 수 있습니다. 이 목록은 Media Portal 외부에서 사용하기 위해 사용자 이름과 주소를 잘라내어 붙여 넣으려는 경우에 유용합니다.

1. **[!UICONTROL 설정]** > **[!UICONTROL 응용 프로그램 설정]** > **[!UICONTROL 관리 설정]** > **[!UICONTROL 사용자 관리]**&#x200B;로 이동합니다.
1. **[!UICONTROL 사용자 역할별]** 드롭다운 목록에서 Media Portal 사용자 역할의 이름을 선택하고 **[!UICONTROL 새로 고침]**&#x200B;을 선택하여 Media Portal 사용자의 한 클래스 이름을 표시합니다.
1. **[!UICONTROL 팝업 목록]**&#x200B;을 선택합니다. 이 목록을 복사하여 붙여넣습니다.

## Media Portal 사용자에 대한 환영 이메일 메시지 설정 {#setting-up-the-welcome-e-mail-message-for-media-portal-users}

새 Media Portal 사용자, 기여자 및 기여자-사용자를 추가할 때 환영 이메일을 보낼 수 있습니다. 이 이메일 메시지를 구성하거나 Dynamic Media Classic에서 보내지 않도록 지정할 수 있습니다.

1. **[!UICONTROL 설정]** > **[!UICONTROL 응용 프로그램 설정]** > **[!UICONTROL 관리 설정]** > **[!UICONTROL 사용자 관리]**&#x200B;로 이동합니다.
1. 사용자 관리 설정 화면에서 **[!UICONTROL 전자 메일 설정]**&#x200B;을 선택합니다.
1. [이메일 설정] 대화 상자에서 다음 중 원하는 설정을 지정합니다.

   * **[!UICONTROL 이메일 보내기]**  - 새 사용자에게 등록한 전자 메일을 통해 알리지 않으려면 이 옵션을 선택 취소합니다.

   * **[!UICONTROL 기본 암호]**  - 새 사용자의 임시 암호를 입력하거나, Dynamic Media Classic에서 임의 암호를 생성하도록 필드를 비워 둡니다. 사용자는 처음 로그인할 때 암호를 변경하라는 메시지가 표시됩니다.

   * **[!UICONTROL 대체 URL]**  - 사용자가 다른 URL을 통해 Dynamic Media Classic에 액세스하는 경우 기본값과 다른 URL을 입력합니다.

## 다른 사용자 관리 작업 {#other-user-management-tasks}

[사용자 관리 설정] 화면에서 시작하여 다음 작업을 수행할 수도 있습니다.

* **[!UICONTROL 사용자 목록 필터링 및 정렬]**  - Media Portal 사용자 목록을 필터링하여 사용자를 찾습니다.

* **[!UICONTROL 사용자 삭제]**  - 목록에서 사용자를 제거합니다.

* **[!UICONTROL 사용자 활성화 및 비활성화]**  - 사용자가 폴더에 액세스하지 못하도록 일시 중단합니다.

* **[!UICONTROL 사용자 정보 편집]**  - 사용자에 대한 최신 정보를 입력합니다.

* **[!UICONTROL 사용자 정의 필드 만들기]**  - Dynamic Media Classic에서 자산을 구성하는 데 도움이 되도록 사용자 정의 사용자 정의 메타데이터 필드를 만듭니다. 또한 이 필드는 필요에 따라 활성화되거나 비활성화될 수 있습니다.

[사용자 지정 필드](application-setup.md#user_defined_fields)를 참조하십시오.
