---
title: 공개하기 전에 자산 테스트
description: 공개하기 전에 Adobe Dynamic Media Classic에서 자산을 테스트하는 방법을 알아봅니다.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: fd78d535-391e-43eb-a8aa-25fa6c2885cb
topic: Content Management
level: Intermediate
source-git-commit: 29752cf9eca0fc9bb760c721e1c3dc8e4ef912c3
workflow-type: tm+mt
source-wordcount: '1061'
ht-degree: 19%

---

# 공개하기 전에 자산 테스트 {#testing-assets-before-making-them-public}

보안 테스트는 구성 가능한 IP 주소 및 범위 세트를 기반으로 보안 테스트 환경을 정의하고 강력한 B2B 솔루션을 구축할 수 있도록 해줍니다. 이 기능을 사용하면 Adobe Dynamic Media Classic 배포와 콘텐츠 관리 및 비즈니스 시스템의 아키텍처를 일치시킬 수 있습니다.

보안 테스트를 사용하면 게시되지 않은 컨텐츠가 포함된 웹 사이트의 스테이징 버전을 미리 볼 수 있습니다.

원하는 경우 다음과 같은 이유로 에셋을 공개적으로 사용할 수 있도록 하지 않고 스테이징 환경을 만듭니다.

* 공식 출시 전에 웹 사이트를 미리 봅니다(스테이징 웹 사이트).
* B2B 웹 애플리케이션에서 가격을 표시하는 eCatalogs와 같이 제한된 액세스가 필요한 자산을 제공합니다.
* 제품 정보 관리 시스템, 고객 서비스 애플리케이션, 교육 사이트 등의 일부로 방화벽 뒤에 있는 자산을 사용합니다.

>[!NOTE]
>
>보안 테스트는 Adobe Dynamic Media Classic 액세스에 영향을 주지 않습니다. Adobe Dynamic Media Classic 보안은 일관되게 유지되며 Adobe Dynamic Media Classic 및 관련 웹 서비스에 액세스하기 위해 일반적인 자격 증명이 필요합니다.

## 보안 테스트가 작동하는 방법 {#how-secure-testing-works}

대부분의 회사는 방화벽 뒤에서 인터넷을 실행합니다. 인터넷에 대한 액세스는 특정 경로 및 일반적으로 제한된 범위의 공개 IP 주소를 통해 가능합니다.

회사 네트워크에서 [https://www.whatismyip.com](https://www.whatismyip.com/)과(와) 같은 웹 사이트를 사용하여 공용 IP 주소를 확인하거나 회사 IT 조직에 이 정보를 요청할 수 있습니다.

Adobe Dynamic Media Classic은 보안 테스트를 통해 스테이징 환경 또는 내부 애플리케이션을 위한 전용 이미지 서버를 구축합니다. 이 서버에 대한 모든 요청은 원본 IP 주소를 확인합니다. 수신 요청이 승인된 IP 주소 목록 내에 없는 경우 실패 응답이 반환됩니다. Adobe Dynamic Media Classic 회사 관리자는 회사의 보안 테스트 환경에 대해 승인된 IP 주소 목록을 구성합니다.

원본 요청의 위치를 확인해야 하므로 보안 테스트 서비스의 트래픽은 공용 Dynamic Media 이미지 서버 트래픽과 같은 컨텐츠 배포 네트워크를 통해 라우팅되지 않습니다. 보안 테스트 서비스에 대한 요청은 공개 Dynamic Media 이미지 서버에 비해 대기 시간이 약간 더 깁니다.

게시되지 않은 자산은 게시하지 않아도 보안 테스트 서비스에서 즉시 사용할 수 있습니다. 이 방법으로 에셋이 공개 이미지 서버에 게시되기 전에 미리 보기를 실행할 수 있습니다.

>[!NOTE]
>
>보안 테스트 서비스는 내부 게시 컨텍스트로 구성된 카탈로그 서버를 사용합니다. 따라서 회사가 보안 테스트에 게시하도록 구성된 경우 Adobe Dynamic Media Classic에 업로드된 모든 자산은 즉시 보안 테스트 서비스에서 사용할 수 있습니다. 이 기능은 업로드 시 자산이 게시로 표시되는지 여부에 관계없이 적용됩니다.

보안 테스트 서비스는 현재 다음과 같은 에셋 유형 및 기능을 지원합니다.

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved "Render Server requests" from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* 이미지.
* 비네팅(렌더링 서버 요청).
* 렌더링 서버 요청(지원되지만 고객이 명시적으로 요청해야 함)
* 집합(이미지 집합, eCatalog, 렌더 집합 및 미디어 집합 등)
* 표준 Adobe Dynamic Media Classic 리치 미디어 뷰어.
* Adobe Dynamic Media Classic OnDemand JSP 페이지
* PDF 파일 및 점진적으로 제공되는 비디오와 같은 정적 컨텐츠.
* HTTP 비디오 스트리밍.
* 점진적 비디오 스트리밍.

다음 자산 유형 및 기능은 현재 지원되지 않습니다.

* Adobe Dynamic Media Classic 정보 또는 eCatalog 검색
* RTMP 비디오 스트리밍
* W2P(Web to Print)
* UGC(사용자 생성 컨텐츠) 서비스

>[!IMPORTANT]
>
>Adobe Dynamic Media Classic의 신규 또는 기존 UGC 벡터 이미지 자산에 대한 지원은 2021년 9월 30일에 종료되었습니다.

## 보안 테스트 서비스 테스트 {#testing-the-secure-testing-service}

보안 테스트 서비스를 테스트하여 예상대로 작동하는지 확인하십시오.

<!-- >[!NOTE]
>
>*If you do not mention any IPs under **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]** > **[!UICONTROL Test Image Service]***: If you add an IP only, that IP is able to call the assets and no other IP are allowed to make the calls. As long there is no IP mentioned under that section, all IPs are allowed to make the calls for the assets, and they show up. -->

### 계정 준비

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under "Prepare your account" 9/10/2012</p>

 -->

1. Adobe 고객 지원 센터에 문의하여 계정에서 보안 테스트를 사용하도록 요청하십시오.
1. Adobe Dynamic Media Classic의 전역 탐색 모음에서 **[!UICONTROL 설정]** > **[!UICONTROL Publish 설정]** > **[!UICONTROL 이미지 서버]**(으)로 이동합니다.
1. 이미지 서버 Publish 페이지의 **[!UICONTROL `Publish Context`]** 드롭다운 목록에서 **[!UICONTROL 이미지 제공 테스트]**&#x200B;를 선택합니다.
1. 클라이언트 주소 필터에 대해 **[!UICONTROL 추가]**&#x200B;를 선택합니다.
1. 주소를 활성화(설정)하도록 확인란을 선택한 다음 각 텍스트 필드에 IP 주소와 네트워크 마스크를 입력합니다.

   >[!NOTE]
   >
   >단일 IP 주소와 네트워크 마스크를 추가하면 해당 주소가 에셋을 호출할 수 있습니다. 그러나 추가하는 다른 IP 주소 및 네트 마스크는 에셋 호출을 수행할 수 없습니다. 따라서 위의 단계에서 확인란을 비활성화(끄기)하여 IP 주소 및 넷 마스크를 지정하는 기능을 끄는 것이 좋습니다. 이렇게 하면 *모든* IP 주소가 에셋 호출을 할 수 있으며 모두 표시됩니다.

1. 다음 중 하나를 수행하십시오.
   * IP 주소를 더 추가해야 하는 경우 앞의 두 단계를 반복합니다.
   * 다음 단계로 진행합니다.
1. 이미지 서버 Publish 페이지의 왼쪽 아래에서 **[!UICONTROL 저장]**&#x200B;을 선택합니다.
1. 원하는 이미지를 Adobe Dynamic Media Classic 계정에 업로드합니다.

   [파일 업로드](uploading-files.md#uploading_files)를 참조하십시오.

1. 일부 이미지는 게시용으로 표시되어 있고 다른 이미지는 표시 해제되어 있는지 확인한 다음 게시 작업을 제출하십시오.

   [Publish 파일](publishing-files.md#publishing_files)을 참조하세요.

1. **[!UICONTROL 설정]** > **[!UICONTROL 응용 프로그램 설정]** > **[!UICONTROL 일반 설정]**(으)로 이동하여 보안 테스트 서비스의 이름을 결정합니다.
1. [애플리케이션 일반 설정] 페이지의 [서버] 그룹에서 **[!UICONTROL [게시 컨텍스트 서버 이름 테스트]]**&#x200B;의 오른쪽에 있는 이름을 찾습니다.

서버 이름이 없거나 서버에 대한 URL이 작동하지 않는 경우 Adobe 지원 센터에 문의하십시오.

### 웹 사이트 변형 준비

게시되거나 게시되지 않은 자산에 연결된 두 가지 변형의 웹 사이트가 필요합니다.

* 공개 버전: 기존 Adobe Dynamic Media Classic URL 구문을 사용하여 자산을 연결합니다.
* 스테이징 버전: 동일한 구문을 사용하지만 보안 테스트 사이트 이름을 사용하여 자산을 연결합니다.

### 테스트 실행

다음 테스트를 수행합니다.

1. 자산이 회사 네트워크에서 보이는지 확인합니다.

   이전에 정의한 IP 주소 범위로 식별된 회사 네트워크 내에서 웹 사이트의 스테이징 버전은 게시로 표시되는지 여부에 관계없이 모든 이미지를 표시합니다. 따라서 미리 보기 승인이나 제품 출시 전에 실수로 이미지를 사용할 수 있게 하지 않고 테스트할 수 있습니다.

   사이트의 공개 버전에 Adobe Dynamic Media Classic에서 이전에 경험한 대로 게시된 자산이 표시되는지 확인합니다.

1. 회사 네트워크 외부에서 게시되지 않은 자산(즉, 게시용으로 표시되지 않은 자산)이 서드파티 액세스로부터 보호되는지 확인합니다.

   외부(예: 홈 컴퓨터 또는 3G 연결을 통해)에서 네트워크에 액세스한 다음 사이트의 공개 버전에 게시된 자산이 모두 표시되지만 게시되지 않은 컨텐츠는 표시되지 않는지 확인하십시오.

   승인되지 않은 IP 주소에서 보안 테스트 서비스에 액세스 중이기 때문에 스테이징 버전이 모든 자산을 표시하지 않는지 확인합니다.
