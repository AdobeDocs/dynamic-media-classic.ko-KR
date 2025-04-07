---
title: 관리 설정
description: Adobe Dynamic Media Classic의 관리 영역을 설정하는 방법을 알아봅니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin
exl-id: 14e3d8be-f265-4cec-aa8e-19ef71526b68
topic: Administration
level: Intermediate
source-git-commit: fc2138cc9fd08cb4ce7466724af03f0901edebf3
workflow-type: tm+mt
source-wordcount: '1995'
ht-degree: 29%

---

<!-- UPDATE TOPIC AFTER DECEMBER 31, 2020!!!! -->

# 관리 설정{#administration-setup}

관리 설정 화면은 Adobe Dynamic Media Classic 사용자를 관리하기 위한 것입니다. 이 화면을 사용하여 사용자가 Adobe Dynamic Media Classic에서 작업하고 다른 사용자와 이메일로 통신할 수 있습니다.

1. 관리 설정 옵션에 액세스하려면 **설정** > **개인 설정** > **관리 설정**&#x200B;으로 이동하십시오.

## 사용자 관리 {#user-administration}

모든 Adobe Dynamic Media Classic 사용자에게는 Adobe Dynamic Media Classic의 기능에 대한 권한 및 액세스 권한을 결정하는 역할이 할당됩니다. 관리자는 사용자가 지정된 회사에 대해 각기 다른 역할과 책임을 결정합니다.

일반적으로 Adobe Dynamic Media Classic은 첫 번째 회사 세트를 구성하고 회사 관리자를 할당합니다. 그런 다음 회사 관리자는 Adobe Dynamic Media Classic 사용자를 설정하고 관리합니다.

Adobe Dynamic Media Classic은 여러 사용자 역할을 지원합니다. 이러한 역할은 Adobe Dynamic Media Classic에 대해 설정된 회사에 액세스할 수 있습니다.

<!-- **Adobe Dynamic Media Classic Administrator** Can view and administer all features in Adobe Dynamic Media Classic, as well as set up companies and add administrators and users. -->

**Adobe Dynamic Media Classic 사용자**&#x200B;는 할당된 회사에 액세스할 수 있으며 관리 업무를 수행할 수 없습니다.

**Adobe Dynamic Media Classic 회사 관리자**&#x200B;는 자신의 회사만 보고 관리할 수 있습니다. 회사 관리자는 관리자 및 사용자 추가를 비롯한 모든 관리 기능을 수행할 수도 있습니다. 회사 관리자는 DMC 회사 관리 계정에 사용자를 추가할 수 있습니다. 이 역할이 기본 사용자 역할입니다.

사용자를 추가하면 Adobe Dynamic Media Classic에서 사용자에게 환영 이메일 메시지를 보냅니다. 메시지에는 암호와 Adobe Dynamic Media Classic URL이 포함되어 있습니다.

### 사용자 또는 관리자 추가 {#adding-a-user-or-administrator}

1. **[!UICONTROL 설정]** > **[!UICONTROL 응용 프로그램 설정]** > **[!UICONTROL 관리 설정]** > **[!UICONTROL 사용자 관리]**(으)로 이동합니다.
1. **[!UICONTROL 추가]**&#x200B;를 선택합니다.
1. 추가할 사용자나 관리자의 이름과 전자 메일 주소를 입력한 다음 **[!UICONTROL 다음]**&#x200B;을 선택합니다.

   >[!NOTE]
   >
   >전자 메일 주소에는 아포스트로피 문자(`'`)를 사용할 수 없습니다.

1. 사용자에게 역할을 할당하려면 역할 옵션을 선택합니다.

   [Adobe Dynamic Media Classic 사용자 역할 및 권한](administration-setup.md#user_administration)을 참조하세요.

1. 회사에 사용자를 추가하려면 회사 이름을 선택합니다.
1. 사용자를 그룹에 추가하려면( Media Portal 사용자 또는 기여자만 추가하는 경우) **[!UICONTROL 다음]**&#x200B;을(를) 선택하고 사용자를 추가하십시오.
1. 사용자 설정을 완료하려면 **[!UICONTROL 저장]**&#x200B;을 선택하세요.

   저장하면 사용자를 다른 회사에 추가할 것인지 묻는 메시지가 나타납니다. 회사에 사용자를 추가하려면 **[!UICONTROL 추가]**&#x200B;를 선택하세요.

   모든 신규 사용자에게는 임의로 생성된 암호가 주어집니다. 사용자는 Adobe Dynamic Media Classic 데스크탑 애플리케이션에 처음 로그인할 때 암호를 변경해야 합니다.

   새 사용자를 추가하면 환영 이메일이 전송됩니다. 이메일은 임시 암호를 제공하며 Adobe Dynamic Media Classic에 로그인하는 방법을 설명합니다.

   환영 이메일을 받지 못한 사용자는 Adobe Dynamic Media Classic 로그인 페이지(https://s7sps1.scene7.com)로 이동한 다음 **[!UICONTROL 내 암호 찾기]**&#x200B;를 선택합니다. 암호가 재설정되고 새 이메일이 전송됩니다. 사용자가 이메일을 받지 못하고 스팸 폴더에도 없는 경우 기술 지원에 문의하십시오.

   새 Media Portal 사용자를 추가할 때 **[!UICONTROL 설정]** > **[!UICONTROL 응용 프로그램 설정]** > **[!UICONTROL 사용자 관리]**(으)로 이동한 다음 **[!UICONTROL 사용자 목록 업로드]**&#x200B;를 선택하고 500명 이하의 사용자가 포함된 .csv 파일을 선택할 수도 있습니다.

### 사용자 삭제 {#delet-a-user}

사용자를 유효하지 않은 상태로 만들어 Adobe Dynamic Media Classic에서 삭제할 수 있습니다. 무효 사용자는 시스템과 모든 계정에서 제거됩니다.

1. **[!UICONTROL 설정]** > **[!UICONTROL 응용 프로그램 설정]** > **[!UICONTROL 관리 설정]** > **[!UICONTROL 사용자 관리]**(으)로 이동합니다.
1. 목록에서 사용자를 선택한 다음 **[!UICONTROL 편집]**&#x200B;을 선택합니다.
1. [유효]를 선택 취소합니다.
1. **[!UICONTROL 저장]**&#x200B;을 선택합니다.

### 사용자 활성화 또는 비활성화 {#activating-or-deactivating-users}

비활성화된 사용자는 [액세스할 계정 선택] 메뉴 상단에 나열된 계정을 시작할 수 있는 권한이 더 이상 없습니다.

1. **[!UICONTROL 설정]** > **[!UICONTROL 응용 프로그램 설정]** > **[!UICONTROL 관리 설정]** > **[!UICONTROL 사용자 관리]**(으)로 이동합니다.
1. 사용자 목록에서 사용자 이름 옆에 있는 **[!UICONTROL 활성]** 옵션을 선택하거나 선택 취소합니다.

### 사용자 정보 편집 {#editing-user-information}

편집할 수 있는 사용자 정보는 관리자로서의 역할 및 정보를 편집하려는 사용자에게 지정된 역할에 따라 다릅니다. 희미한 선택 사항(사용할 수 없음)은 편집할 수 없습니다.

1. **[!UICONTROL 설정]** > **[!UICONTROL 응용 프로그램 설정]** > **[!UICONTROL 관리 설정]** > **[!UICONTROL 사용자 관리]**(으)로 이동합니다.
1. 목록에서 사용자를 선택한 다음 **[!UICONTROL 편집]**&#x200B;을 선택합니다.
1. 테이블에서 권한 또는 액세스를 수정하려는 회사를 표시하는 항목을 선택한 다음 **[!UICONTROL 회사 관리]**&#x200B;를 선택합니다.
1. 사용자 역할을 선택합니다.
1. 사용자의 그룹 구성원을 변경하려면( Media Portal 사용자 또는 기여자를 편집하거나 추가하는 경우) **[!UICONTROL 다음]**&#x200B;을 선택하고 그룹 구성원을 편집합니다.
1. **[!UICONTROL 저장]**&#x200B;을 선택합니다.

### 사용자 목록 필터링 및 정렬 {#filtering-and-sorting-the-user-list}

사용자 목록을 필터링 및 정렬하여 사용자를 찾을 수 있습니다. [액세스할 계정 선택] 메뉴에서 선택한 계정에 관계없이 관리하는 모든 계정의 모든 사용자가 [사용자 목록]에 표시됩니다.

다음과 같은 사용자 목록 필터링 기법을 사용할 수 있습니다.

* **그룹별로 필터링**: **[!UICONTROL 그룹별]** 메뉴를 선택하고 그룹의 사용자로 목록을 좁히는 옵션을 선택하십시오.

* **사용자 역할별로 필터링**: **[!UICONTROL 사용자 역할별]** 메뉴를 선택하고 다른 유형의 사용자 또는 관리자로 목록을 좁히는 옵션을 선택하십시오.

* **필드 이름별로 필터링**: **[!UICONTROL 필드별로 필터링 사용]**&#x200B;을 선택합니다. **[!UICONTROL 필드 이름별]** 메뉴를 선택하고 목록을 필터링할 열을 선택한 다음 문자 필터 메뉴를 선택하고 문자를 선택합니다. 선택한 문자로 열 중 하나에서 목록이 필터링됩니다. 전체 목록을 보려면 **[!UICONTROL 필드별 필터링 활성화]** 옵션을 선택 취소하십시오.

* **잘못된 사용자 필터링**: **[!UICONTROL 잘못된 사용자 포함]**&#x200B;을 선택 취소합니다. 시스템에 있는 사용자만 검색 결과에 표시됩니다. 시스템 및 관리하는 계정에서 잘못된 사용자가 삭제되었습니다.

* **열 머리글별로 정렬**: 이름, 성 또는 전자 메일을 알파벳순으로 사용하여 모든 사용자를 상태별로 정렬할 머리글을 선택합니다. 또는 사용자 역할별로 정렬하거나 유효/무효 상태별로 정렬합니다.

많은 사용자가 있는 경우 [최대 목록 크기] 메뉴를 선택한 다음 숫자를 선택하여 목록의 크기를 제한할 수 있습니다.

<!-- CQDOC-16690 TOPIC REMOVED AS PER JIRA TICKET INSTRUCTIONS ### Linking an IMS user identity to an Adobe Dynamic Media Classic IPS user account {#linking-an-ims-user-identity-to-a-scene-ips-user-account}

You can link an Adobe IMS user identity to an Adobe Dynamic Media Classic IPS user account so you can use SSO (Single Sign On) to log on and launch Scene7 Publishing System from within Adobe Marketing Cloud.

1. Adobe should already have setup your account with an Adobe Marketing Cloud organization and linked it to your Scene7 Publishing System product context. If this setup is not yet done or you are unsure if it has been done, contact Adobe Customer Care.

   When the setup is complete, you can can log on to Adobe Marketing Cloud and link your Adobe Marketing Cloud identity to your Adobe Dynamic Media Classic user account by doing the following.

1. In Adobe Marketing Cloud, navigate to your account settings.
1. Select **Manage Organizations**.
1. Select **Link Account** or **Get Access**.
1. Select **Experience Manager**, and then type your credentials.

   Your credentials include your IPS company region, email address, and password.

1. Select **Link**.
1. When the link is set, you can launch Scene7 Publishing System from within Adobe Marketing Cloud, or you can launch it directly.

   Do one of the following:

    * To launch Adobe Dynamic Media Classic from within Adobe Marketing Cloud, in the left rail of Adobe Marketing Cloud, select **Solutions** > **Experience Manager**. Under the Adobe Dynamic Media Classic card, select **Launch**.
    * To log on to Scene7 Publishing System directly using your IMS credentials, use the following website:

      https://s7spsN.scene7.com/IpsWeb?ims=1

      Replace "N" in the above path with the number for your IPS company region. That is, N = 1 for North America; 3 for EMEA; or 5 for JAPAC.
 -->

## 대역폭 및 스토리지 {#bandwidth-storage}

Adobe Dynamic Media Classic 관리자는 관리하는 회사의 대역폭, 스토리지 및 기타 유형의 보고서를 생성할 수 있습니다. 이러한 보고서는 대역폭 및 저장소 페이지에서 사용할 수 있습니다.

이 페이지를 열려면 **[!UICONTROL 설정]** > **[!UICONTROL 개인 설정]**(으)로 이동하세요. **[!UICONTROL 관리 설정]**&#x200B;을 확장한 다음 **[!UICONTROL 대역폭 및 저장소]**&#x200B;를 선택합니다.

### 보고서 유형 {#types-of-reports}

다음 표에서는 [대역폭 및 저장소] 페이지에서 생성할 수 있는 보고서에 대해 설명합니다.

| 보고서 | 정보 | 사용 |
| --- | --- | --- |
| 대역폭 | | <!-- CQDOC-22504 --> **중요**: 대역폭 탭은 더 이상 지원되지 않습니다. 여전히 UI에 표시되지만 대역폭 데이터를 사용할 수 없으며 모든 값이 `0`(으)로 표시됩니다. |
| 저장소 | 저장소 사용 | 회사가 업로드한 데이터의 양을 추적합니다. |
| 이미지 내용 | 요청 유형 및 하위 유형별로 분류된 총 히트 수 및 이미지 게재 볼륨을 표시합니다. | 비비디오 자산의 지표를 포함하여 다양한 이미지 유형에 대한 요청 및 볼륨 수를 추적합니다. <!-- CQDOC-22504 --> |
| 도메인 | 도메인별 URL 요청 수 | 특정 회사에 대한 이미지 요청의 도메인을 기준으로 이미지 사용을 추적합니다. (Adobe Dynamic Media Classic은 계정당 두 개 이상의 도메인을 제공할 수 있습니다. 자세한 내용은 기술 지원팀에 문의하십시오. |
| 비디오 스트리밍 | 스트리밍 비디오의 대역폭 사용 | 특정 기간 동안 회사별 스트리밍 비디오 사용을 추적하여 트래픽 패턴을 확인합니다. |
| 비디오 컨텐츠 | 각기 다른 비디오의 재생 시간 | 가장 많이 본 비디오와 가장 적게 본 비디오를 확인합니다. |

[이미지 내용] 보고서에서는 다음 이미지 유형에 대한 요청 정보를 제공합니다.

* **이미지 요청**: 이미지를 요청합니다.

* **썸네일 요청**: 뷰어에서 견본 또는 대체 이미지를 요청합니다.

* **마스크 요청**: 회색 음영 마스크를 반환하는 이미지에 대한 요청입니다.

* **뷰어 타일 요청**: 뷰어가 로드한 이미지 요청입니다.

* **VNT 개체 요청**: 이미지 렌더링 요청에서 요청된 비네팅에 지정된 개체가 있는 이미지를 반환합니다.

* **VNT 정보 요청**: 요청된 비네팅에 대한 정보를 반환하는 이미지 렌더링 요청.

>[!NOTE]
>
>[비디오 스트리밍] 보고서는 스트리밍 비디오에만 적용됩니다. 점진적 비디오 보기를 추적하지 않습니다.

### 보고서 생성 {#generating-a-report}

대역폭, 저장소, 이미지 내용, 도메인, 비디오 스트리밍 또는 비디오 컨텐츠 보고서를 생성하려면 다음 단계를 수행합니다.

1. **[!UICONTROL 설정]** > **[!UICONTROL 개인 설정]**(으)로 이동합니다.
1. 관리 설정을 확장한 다음 **[!UICONTROL 대역폭 및 저장소]**&#x200B;를 선택합니다.
1. 탭을 선택하십시오. **[!UICONTROL 대역폭]**, **[!UICONTROL 저장소]**, **[!UICONTROL 이미지 콘텐츠]**, **[!UICONTROL 도메인]**, **[!UICONTROL 비디오 스트리밍]** 또는 **[!UICONTROL 비디오 콘텐츠]**.

   [보고서 유형](administration-setup.md#types_of_reports)을 참조하십시오.

### 다양한 방법으로 데이터 보기 {#viewing-data-in-different-ways}

[대역폭 및 저장소] 페이지에서 보고서를 생성한 후 정보 보기 선택 사항을 선택할 수 있습니다. 정보를 제공하는 방법(차트 또는 데이터 그리드에서 정보 보기)을 선택하고 정보 캡처 기간을 지정할 수 있습니다. [데이터 보기]에서 정보를 정렬하고 열을 다시 정렬할 수도 있습니다.

* **차트 또는 데이터 그리드에서 데이터 보기**: 차트에서 데이터를 보려면 **[!UICONTROL 차트 보기]**&#x200B;를 선택하고 데이터 그리드에서 데이터를 보려면 **[!UICONTROL 데이터 보기]**&#x200B;를 선택하십시오.

* **보고서 프레젠테이션 형식을 선택하십시오**: 보고서 형식 메뉴에서 **[!UICONTROL 요약]**, **[!UICONTROL 일별]** 또는 **[!UICONTROL 월별]**&#x200B;을 선택하여 요약 형식, 일별 또는 월별로 데이터를 구성하십시오. 모든 보고서에서 이 선택 사항을 제공하는 것은 아닙니다.

* **기간 지정**: 보고서 기간을 정의할 옵션을 선택한 다음 기간을 정의한 후 **[!UICONTROL 업데이트]**&#x200B;를 선택합니다.

* **미리 정의된 기간**: 미리 정의된 보고서 메뉴에서 옵션을 선택합니다. 예를 들어 전달의 데이터를 캡처하려면 [지난 달]을 선택합니다.

* **사용자 지정 기간**: 미리 정의된 보고서 메뉴에서 **[!UICONTROL 사용자 지정]**&#x200B;을 선택합니다. 그런 다음 **[!UICONTROL 월 시작]**(또는 **[!UICONTROL 시작 날짜]**) 메뉴에서 날짜를 선택하고 # of months(또는 # or Days) 메뉴에서 날짜를 선택합니다. 도메인 및 비디오 컨텐츠 보고서의 경우 보고서 정보를 캡처할 특정 시작 날짜와 종료 날짜를 선택할 수 있습니다.

* **데이터 정렬(데이터 보기 전용)**: 열에 있는 정보를 정렬합니다. 열의 제목을 선택합니다. 내림차순으로 정렬하려면 다시 선택하십시오.

* **열 다시 정렬(데이터 보기 전용)**: 열을 데이터 그리드의 다른 위치로 이동하려면 해당 제목을 끕니다.

### 보고서 내보내기 및 인쇄 {#exporting-and-printing-reports}

보고서를 생성한 후 스프레드시트 및 기타 애플리케이션에서 사용하기 위해 해당 데이터를 내보낼 수 있습니다. 보고서를 인쇄할 수도 있습니다.

* **보고서 데이터 내보내기**: 데이터 보기에서 데이터를 필요에 따라 정렬하고 정렬합니다. 그런 다음 **[!UICONTROL 내보내기]** 메뉴를 열고 형식을 선택합니다. **[!UICONTROL 탭으로 구분]**, **[!UICONTROL 쉼표로 구분]** 또는 **[!UICONTROL HTML 형식]**. 선택한 형식으로 데이터가 클립보드에 복사됩니다. 이제 스프레드시트나 기타 애플리케이션에 데이터를 붙여 넣을 수 있습니다.

* **보고서 인쇄**: **[!UICONTROL 인쇄]**&#x200B;를 선택하고 [인쇄] 대화 상자에서 원하는 옵션을 선택한 다음 **[!UICONTROL 확인]**&#x200B;을 선택합니다.

## 이미지 오류 {#image-errors}

Adobe Dynamic Media Classic 관리자는 이미지 오류 보고서를 생성할 수 있습니다. 이미지 오류 보고서는 지난 24시간 동안 현재 로그인한 회사에서 가장 많이 발생한 이미지 오류 20개 목록을 제공합니다. 이미지 오류 보고서를 생성하려면 다음을 수행합니다.

1. **[!UICONTROL 설정]** > **[!UICONTROL 개인 설정]**(으)로 이동합니다.
1. 관리 설정을 확장한 다음 **[!UICONTROL 이미지 오류]**&#x200B;를 선택합니다.
1. 다음 중 하나를 수행합니다(선택 사항).

   * 제목 정보별로 오류를 정렬하려면 제목을 선택합니다. 기본적으로 오류는 발생 횟수를 기준으로 가장 많이 발생한 오류에서 가장 적게 발생한 오류 순으로 정렬되어 있습니다.
   * 오류에 대한 [응답] 필드 위로 커서를 이동하여 특정 오류 메시지를 표시합니다.
   * 이미지 또는 레퍼러 웹 페이지에 대한 링크를 보려면 커서를 URL 필드 또는 레퍼러 필드 위로 이동합니다.
   * 링크를 실제 이미지로 복사하려면 **[!UICONTROL URL 복사]**&#x200B;를 선택하십시오. 브라우저 창에 이 링크를 붙여 넣어 이미지로 이동하고 오류를 조사할 수 있습니다.
   * 레퍼러 웹 페이지에 링크를 복사하려면 **[!UICONTROL 레퍼러 복사 URL]**&#x200B;을(를) 선택합니다.

현재 로그인한 회사에 대해 오류가 표시됩니다. 각 오류에는 다음 정보가 포함됩니다.

* **이미지 ID**: 문제가 되는 이미지의 ID입니다.

* **Time**: 오류가 처음 보고된 시간부터 마지막 오류가 보고된 시간까지의 시간 범위입니다. 지난 24시간 이내에 해당됩니다.

* **Count**: 이미지에 보고된 오류 수입니다.

* **응답**: 특정 오류 메시지. 오류는 4xx 또는 5xx입니다.

* **URL**: Adobe Dynamic Media Classic의 이미지에 대한 URL을 나열합니다.

* **레퍼러**: 초기 요청이 발생한 웹 사이트의 URL을 지정합니다. 레퍼러는 이미지에 대한 링크가 있는 모든 웹 사이트일 수 있습니다.

테스트를 간소화하기 위해 [URL] 및 [레퍼러] 열에는 [URL 복사]가 연결되어 있습니다.
