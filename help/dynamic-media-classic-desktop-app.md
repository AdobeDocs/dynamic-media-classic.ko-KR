---
title: Adobe Dynamic Media Classic 데스크탑 앱 - 이제 사용 가능
description: Adobe Dynamic Media Classic 데스크탑 애플리케이션에 대해 자세히 알아보십시오.
contentOwner: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
source-git-commit: 43e0c03b535d30ffed13e1e389935e34563baa9e
workflow-type: tm+mt
source-wordcount: '2036'
ht-degree: 1%

---

# 현재 사용 가능: Adobe Dynamic Media Classic 데스크탑 앱 {#dynamic-media-classic-desktop-app}

이제 Adobe Dynamic Media Classic 사용자는 브라우저에서 Adobe Flash 기술에 의존하지 않는 새로운 데스크탑 앱 환경에 액세스할 수 있습니다.

이 새 앱은 이제 Windows® 및 macOS에서 사용할 수 있습니다.

>[!IMPORTANT]
>
>Adobe은 2020년 10월 1일까지 새 Adobe Dynamic Media Classic 데스크탑 앱을 설치하도록 권장합니다. 이렇게 하면 2020년 12월 31일에 Adobe Flash Player이 더 이상 사용되지 않기 전에 원활하게 전환할 수 있습니다. 해당 날짜 이후, 제품에서 Adobe Dynamic Media Classic으로 레이블이 지정된 Adobe Dynamic Media Classic 사용자 인터페이스의 브라우저 버전에 로그인할 수 없습니다.

에 대한 FAQ 참조 [이제 새로운 Adobe Dynamic Media Classic 로그인 환경을 사용할 수 있습니다.](/help/new-ui-2020.md)

## Adobe Dynamic Media Classic 데스크탑 앱에 대한 시스템 요구 사항 {#system-requirements-dmc-app}

Adobe Dynamic Media Classic 데스크탑 앱은 다음 운영 체제와 호환됩니다.

* macOS 10.10 이상
* Windows® 7 이상

에서 전체 시스템 요구 사항 보기 [Adobe Dynamic Media Classic 데스크탑 앱에 대한 시스템 요구 사항](/help/system-requirements.md).

Adobe Dynamic Media Classic 데스크탑 애플리케이션 내의 업그레이드 알림이 다음에 대해 생성되지 않음 *부수적* 릴리스. 마이너 릴리스의 수정 사항으로 혜택을 받는 고객은 업그레이드할 수 있습니다.

## 최신 릴리스(20.22.2) macOS에서만 수정됨 {#release-feb2022}

* macOS Monterey - 후속 업로드 시 파일 업로드 페이지가 정지됩니다. <!-- https://jira.corp.adobe.com/browse/ASSETS-7948 -->

## 최신 릴리스의 수정 사항(20.22.1) {#release-jan2022}

* 이미지 편집 **[!UICONTROL 저장]** 단추가 작동하지 않습니다.
* 세트 편집기에서 **[!UICONTROL 닫기]**, **[!UICONTROL 저장]**, 및 **[!UICONTROL 다른 이름으로 저장]** 에서 에셋을 스크롤하면 버튼이 비활성화됨 **[!UICONTROL 에셋 추가]** 패널.
* **[!UICONTROL 재생]** 비디오 세부 사항 보기의 단추가 작동하지 않았습니다.
* 입력할 수 없음 `d` 및 `e` 위치: **[!UICONTROL 사용자 이름]** 및 **[!UICONTROL 암호]** macOS Monterey를 실행할 때 필드.
* 나머지 Analytics API를 버전 2.0으로 이동했습니다.

## 릴리스 20.21.3의 수정 사항 {#release-sept2021}

* 데스크탑 앱에서 일정 기간 동안 활동이 없으면 표시되는 자산의 깨진 축소판입니다.
* 일반적으로 설정 작업 후 데스크탑 앱이 응답하지 않습니다.
* 아래에서 난독화 및 잠금 모드 자동 활성화됨 요청 **[!UICONTROL 이미지 제공 테스트]**.

   다음을 참조하십시오 [보안 테스트 서비스 테스트](/help/testing-assets-making-them-public.md#testing-the-secure-testing-service).

* Adobe Analytics으로 인증 메커니즘을 업데이트했습니다. 새로운 통합 또는 일부 Analytics 변수를 Dynamic Media Classic 데스크탑 앱 내에서 업데이트해야 하는 경우와 관련이 있습니다.

   다음을 참조하십시오 [Adobe Analytics에 로그인](/help/log-analytics.md) 업데이트된 단계.

## 릴리스 20.21.2의 수정 사항 {#minor-release}

* 20.21.1의 알려진 제한 사항: **[!UICONTROL 서버]** 로그인 화면의 드롭다운 목록이 비어 있습니다.
* 위치 **[!UICONTROL 업로드 작업 옵션]**, 레이어 이름 지정 기본값 **[!UICONTROL Photoshop 옵션]**, 현재 **[!UICONTROL Photoshop 및 레이어 이름]**. PSD 파일의 레이어가 별도의 이미지로 업로드됩니다.
   * 의 초기 기본값 **[!UICONTROL 레이어 이름]**&#x200B;를 클릭하고 PSD 파일에서 레이어 이름이나 레이어 번호의 이름을 따라 이미지에 이름을 지정합니다. PSD 파일의 레이어 이름이 기본 Photoshop 레이어 이름인 경우 레이어 번호가 사용되었습니다.
   * 의 새로운 기본값 **[!UICONTROL Photoshop 및 레이어 이름]**&#x200B;는 PSD 파일 뒤에 레이어 이름 또는 레이어 번호를 붙여서 이미지 이름을 지정합니다. 레이어 번호는 PSD 파일의 레이어 이름이 Photoshop 기본 레이어 이름인 경우 사용됩니다.
   * 이제 Adobe Dynamic Media Classic의 레이어 이미지에 고유한 이름이 있으므로 기존 PSD 또는 템플릿(원본 PSD 파일에서 공유된 레이어 이름)에 대한 업데이트가 발생하지 않습니다.
* 자산의 축소판이 깨졌습니다.

## 릴리스 20.21.1의 수정 사항 {#latest-fixes-desktop-app}

* 시간 초과로 인해 로그인 문제가 발생하여 다음 메시지가 표시됩니다. *이 사용자는 권한 없이 그룹 또는 그룹에 할당될 수 있습니다. 관리자에게 문의하십시오.*
* 뷰어 사전 설정은 각각의 잘못된 암호 시도와 중복됩니다.
* 루트 폴더의 많은 자산으로 인해 데스크탑 애플리케이션이 응답하지 않습니다. (Windows®에서 수정되었으며 macOS에서 원하는 대로 작동합니다.)

## 릴리스 20.20.2의 수정 사항 {#previous-version-fixes-desktop-app}

* macOS 및 Windows® 모두에 대해 데스크탑 앱 사용자 인터페이스를 통해 업로드할 수 있는 파일 수에 대한 제한은 없습니다.
* 회사 간에 전환하려면 데스크톱 앱에서 로그아웃할 필요가 없습니다.
* 이제 붙여넣기 작업을 위한 Ctrl+V가 Windows®에서 작동합니다.
* 앞으로 데스크탑 앱의 새 버전이 출시되면 사용자는 데스크탑 앱 자체 내에서 알림을 받게 됩니다.

## macOS 또는 Windows®에서 최신 Adobe Dynamic Media Classic 데스크탑 앱을 다운로드하여 설치합니다. {#installation-dmc-app}

참조:

* [Mac에서 최신 Adobe Dynamic Media Classic 데스크탑 앱을 다운로드하여 자동 설치](#install-silent-mac-dmc-app)
* [Windows®에서 최신 Adobe Dynamic Media Classic 데스크탑 앱을 다운로드하여 자동으로 설치합니다.](#install-silent-windows-dmc-app)

1. 시스템에서 이전 Adobe Dynamic Media Classic 데스크탑 앱 버전을 모두 제거합니다.

1. Adobe Dynamic Media Classic 데스크탑 앱용 최신 설치 관리자를 다운로드합니다.

   * 최신 버전은 다음에서 사용할 수 있습니다.

      * [macOS (.DMG) - 다운로드](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)
      * [Windows (.EXE) - 다운로드](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)
   * 이전 버전은 다음에서 사용할 수 있습니다.

      * [macOS (.DMG) - 다운로드](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.dmg)
      * [Windows® (.EXE) - 다운로드](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.exe)


<!--         * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.dmg) -->

<!--    * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
        * [Windows® (.EXE) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe) -->

<!--    * [macOS (.DMG) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. 다운로드한 설치 관리자를 기준으로 다음 중 하나를 수행합니다.

   * **macOS** -에서 **[!UICONTROL 드래그하여 놓아 설치]** 대화 상자, 드래그 **[!UICONTROL Adobe Dynamic Media Classic]** 여기에 놓으세요 **[!UICONTROL 애플리케이션]**.

      ![macOS에서 설치 끌어서 놓기](/help/assets/dragondrop-install1.png)

   * 다음에서 **[!UICONTROL 애플리케이션]** 폴더에서 Adobe Dynamic Media Classic 아이콘을 탭합니다.
   * 대화 상자에서 을 누릅니다. **[!UICONTROL 열기]** Adobe Dynamic Media Classic 데스크탑 앱을 엽니다.

      ![다운로드한 앱 열기](/help/assets/open-dmclassicapp1.png)

   * **Windows** - 설치 관리자 바이너리를 실행하고 화면의 지침에 따라 데스크탑 앱을 설치합니다.

1. 애플리케이션을 열면 새 Adobe Dynamic Media Classic 로그인 페이지가 표시됩니다.

   ![Adobe Dynamic Media Classic 로그인](/help/assets/dmclassic-login1.png)

1. Adobe Dynamic Media Classic 데스크탑 앱에 로그인하려면 브라우저에서 Adobe Dynamic Media Classic에 로그온하는 데 사용한 자격 증명을 사용합니다.

   의 경우 **[!UICONTROL 서버]** 를 사용하려면 프로덕션 환경에 대한 다음 매핑을 참조하십시오.

   | 서버 | 브라우저 URL |
   | --- | --- |
   | NA 프로덕션(북미) | https://s7sps1.scene7.com/ |
   | EMEA 생산(유럽, 중동 및 아프리카) | https://s7sps3.scene7.com/ |
   | APAC 프로덕션(아시아 태평양) | https://s7sps5.scene7.com/ |

1. 로그인 후 친숙한 브라우저 사용자 인터페이스 경험을 확인합니다. 데스크탑 앱에서 평소대로 일상적인 Adobe Dynamic Media Classic 활동을 계속할 수 있습니다.

## 다운로드 및 *자동* macOS에 최신 Adobe Dynamic Media Classic 데스크탑 앱 설치 {#install-silent-mac-dmc-app}

참조:

* [Mac 또는 Windows®에서 최신 Adobe Dynamic Media Classic 데스크탑 앱을 다운로드하여 설치합니다.](#installation-dmc-app)
* [Windows®에서 최신 Adobe Dynamic Media Classic 데스크탑 앱을 다운로드하여 자동으로 설치합니다.](#install-silent-windows-dmc-app)

다운로드 및 *자동* macOS에 최신 버전의 Adobe Dynamic Media Classic 데스크탑 앱을 설치합니다.

1. 시스템에서 이전 Adobe Dynamic Media Classic 데스크탑 앱 버전을 모두 제거합니다.

1. macOS용 Adobe Dynamic Media Classic 데스크탑 앱용 최신 설치 관리자를 다운로드합니다.

   * [macOS (.DMG) - 다운로드](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)

1. 다음 명령을 사용하여 다운로드한 디스크 이미지(.DMG)를 마운트 지점에 마운트합니다.

   `hdiutil attach adobe-dynamic-media-classic-20.22.2.dmg -mountpoint <mount_point_path>`

1. .APP 파일을 복사할 위치: **[!UICONTROL 애플리케이션]** 다음 명령 사용:

   ```
   rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
   Unmount DMG - hdiutil detach <mount_point_path>
   ```

1. 애플리케이션을 열면 새 Adobe Dynamic Media Classic 로그인 페이지가 표시됩니다.

   ![Adobe Dynamic Media Classic 로그인](/help/assets/dmclassic-login1.png)

1. Adobe Dynamic Media Classic 데스크탑 앱에 로그인하려면 브라우저에서 Adobe Dynamic Media Classic에 로그온하는 데 사용한 자격 증명을 사용합니다.

   의 경우 **[!UICONTROL 서버]** 를 사용하려면 프로덕션 환경에 대한 다음 매핑을 참조하십시오.

   | 서버 | 브라우저 URL |
   | --- | --- |
   | NA 프로덕션(북미) | https://s7sps1.scene7.com/ |
   | EMEA 생산(유럽, 중동 및 아프리카) | https://s7sps3.scene7.com/ |
   | APAC 프로덕션(아시아 태평양) | https://s7sps5.scene7.com/ |

## 다운로드 및 *자동* windows®에 최신 Adobe Dynamic Media Classic 데스크탑 앱을 설치합니다. {#install-silent-windows-dmc-app}

사용하는 명령은 기본 MSI 자동 설치에 사용됩니다. 그러나 Adobe Dynamic Media Classic 데스크톱 앱 설치 관리자는 InstallShield를 사용하여 만든 InstallScript MSI 설치 프로그램입니다. 레코드 모드에서 설치 관리자를 실행하면 사용자 상호 작용이 응답 파일에 기록됩니다. 이 응답 파일은에 설명된 대로 자동 설치에 사용됩니다. [자동 모드로 설치 실행](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/SilentInstall.htm).

참조:

* [Mac 또는 Windows®에서 최신 Adobe Dynamic Media Classic 데스크탑 앱을 다운로드하여 설치합니다.](#installation-dmc-app)

* [macOS에서 최신 Adobe Dynamic Media Classic 데스크탑 앱을 다운로드하여 자동 설치](#install-silent-mac-dmc-app)

다운로드 및 *자동* windows®에 최신 버전의 Adobe Dynamic Media Classic 데스크탑 앱을 설치합니다.

1. 시스템에서 이전 Adobe Dynamic Media Classic 데스크탑 앱 버전을 모두 제거합니다.

1. Adobe Dynamic Media Classic 데스크탑 앱용 최신 설치 관리자를 다운로드합니다.

   * [Windows® (.EXE) - 다운로드](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

1. 다음 명령을 사용하여 레코드 모드에서 설치 관리자를 실행합니다.

   `adobe-dynamic-media-classic-20.22.1.exe /r /f1"C:\Setup.iss"`

1. GUI 설치 프로그램 창에서 설치 위치와 같은 상호 작용/입력이 기록되도록 설치하는 단계를 따르십시오. `Setup.iss` 파일.

1. 생성된 항목 복사 `Setup.iss` 파일 및 `adobe-dynamic-media-classic-20.22.1.exe` 다른 컴퓨터로 가져갑니다.

1. 자동 설치를 위해 다음 명령을 실행합니다.

   `adobe-dynamic-media-classic-20.22.1.exe /s /f1"C:\Setup.iss"`

   명령줄 매개 변수에 대한 자세한 내용은 다음 위치에서 확인할 수 있습니다. [Setup.exe 및 Update.exe 명령줄 매개 변수](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/IHelpSetup_EXECmdLine.htm?Highlight=Setup.exe%20and%20Update.exe%20Command-Line%20Parameters).

1. 애플리케이션을 열면 새 Adobe Dynamic Media Classic 로그인 페이지가 표시됩니다.

   ![Adobe Dynamic Media Classic 로그인](/help/assets/dmclassic-login1.png)

1. Adobe Dynamic Media Classic 데스크탑 앱에 로그인하려면 브라우저에서 Adobe Dynamic Media Classic에 로그온하는 데 사용한 자격 증명을 사용합니다.

   의 경우 **[!UICONTROL 서버]** 를 사용하려면 프로덕션 환경에 대한 다음 매핑을 참조하십시오.

   | 서버 | 브라우저 URL |
   | --- | --- |
   | NA 프로덕션(북미) | https://s7sps1.scene7.com/ |
   | EMEA 생산(유럽, 중동 및 아프리카) | https://s7sps3.scene7.com/ |
   | APAC 프로덕션(아시아 태평양) | https://s7sps5.scene7.com/ |

## Adobe Dynamic Media Classic 데스크탑 앱 사용에 대한 비디오 설명 {#dmc-app-video-walk-through}

시청 [Adobe Dynamic Media Classic 데스크탑 앱 사용에 대한 비디오 둘러보기](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application.html#dynamic-media) (길이: 2분 36초).

## 데스크탑 앱을 사용하여 컴퓨터의 이미지 캐시 및 자산 캐시를 지우는 중 {#clear-cache}

1. Adobe Dynamic Media Classic 데스크탑 앱에서 오른쪽 상단 모서리 근처에 있는 을 누릅니다 **[!UICONTROL 설정]** > **[!UICONTROL 개인 설정]**.
1. 다음에서 **[!UICONTROL 개인 설정]** 페이지, **[!UICONTROL 데스크탑]** 제목, 다음 중 하나를 수행합니다.
   * 컴퓨터에서 모든 Dynamic Media 캐시 이미지 Adobe 파일을 제거하려면 다음을 누릅니다. **[!UICONTROL 이미지 캐시 지우기]**, 다음 탭 **[!UICONTROL 확인]**.
   * 컴퓨터에서 Dynamic Media에 캐시된 모든 Adobe 에셋 파일을 제거하려면 을 누릅니다 **[!UICONTROL 자산 캐시 지우기]**, 다음 탭 **[!UICONTROL 확인]**.
1. 페이지의 오른쪽 아래 모서리에서 을 누릅니다 **[!UICONTROL 닫기]**.

### 이미지 캐시 및 자산 캐시를 수동으로 지우는 중

데스크탑 앱을 사용하여 이미지 및 자산 캐시를 지우는 것 외에도 파일 시스템에서 직접 캐시를 지울 수 있습니다.

1. 운영 체제를 기준으로 다음 위치로 이동합니다.

   * macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Adobe Dynamic Media Classic 20.21.1의 알려진 제한 사항

* 다음 **[!UICONTROL 서버]** Adobe Dynamic Media Classic 데스크탑 앱 20.21.1로 업데이트하면 드롭다운 목록이 비어 있습니다. 시나리오: Adobe Dynamic Media Classic 20.20.1 또는 20.20.2를 설치하고 로그인한 다음 애플리케이션을 닫습니다. 그런 다음 Adobe Dynamic Media Classic 20.21.1로 업데이트합니다. 로그인하려고 하면 **[!UICONTROL 서버]** 드롭다운 목록 **[!UICONTROL 계정에 로그인]** 대화 상자가 비어 있습니다. 이 문제를 해결하려면 다음을 수행하십시오 [수동으로 캐시 지우기](#clear-cache) (위의 단계 참조).

## Adobe Dynamic Media Classic 20.20.1의 알려진 제한 사항(20.20.2에서 해결됨)

**_Windows®에만 적용 - 데스크탑 앱 UI를 통해 업로드할 수 있는 파일 수에 제한이 있습니까?_**<br>예. 데스크탑 앱 UI를 통해 한 번에 최대 150개의 파일을 업로드할 수 있습니다.

**_Windows® 및 macOS에 적용 - 회사 간 전환은 어떻게 합니까?_**<br>회사 간에 전환하려면 다음 작업을 수행하십시오.

* Adobe Dynamic Media Classic 앱의 회사 드롭다운 목록에서 새 회사를 선택합니다.
* 팝업 창이 나타나면 을 누릅니다 **[!UICONTROL 확인]** 로그아웃한 후 앱을 닫습니다.

   ![새 회사를 사용하려면 앱을 다시 시작하십시오.](/help/assets/dmclassic-new-company1.png)

* Adobe Dynamic Media Classic을 다시 시작한 다음 평소대로 로그인하여 새 회사에서 작업하십시오.

## 팁과 트릭

**_Adobe Dynamic Media Classic 랜딩 페이지에 미디어 카트 패널을 볼 수 없습니다._**<br>Adobe Dynamic Media Classic에서 다음을 누릅니다**[!UICONTROL 설정 > 개인 설정&#x200B;]**. 브라우저 섹션에서 다음을 확인합니다**[!UICONTROL MediaPortal 기능 표시&#x200B;]**이(가) 선택(선택)되었습니다. 누르기**[!UICONTROL 저장 > 닫기&#x200B;]**.

**_에셋의 게시 상태(녹색 표시기)가 올바르게 반영되지 않았습니다._**<br>브라우저 사용자 인터페이스에서 자산의 올바른 게시 상태를 보려면 UI에 다시 로그인해야 합니다. 데스크탑 앱에서 Adobe은**[!UICONTROL 새로 고침&#x200B;]**아이콘(도구 모음 오른쪽)**[!UICONTROL 선택 안 함&#x200B;]**단추를 클릭합니다. 탭**[!UICONTROL 새로 고침&#x200B;]**아이콘: 지정된 페이지에 있는 모든 자산의 최신 상태를 볼 수 있습니다. 브라우저 UI에서와 같이 재로그인이 필요하지 않습니다.

![새로 고침 아이콘](/help/assets/refresh-icon1.png)
*새로 고침 아이콘*

**_데스크탑 앱에서 일괄처리 집합 사전 설정이 작동하지 않습니다._**<br>누르기**[!UICONTROL 업로드 > 작업 옵션 > 일괄처리 집합 사전 설정&#x200B;]**. 관련 항목 확인**[!UICONTROL 일괄처리 집합 사전 설정&#x200B;]**이(가) 활성화되었습니다. 클릭**[!UICONTROL 업로드 저장 및 제출&#x200B;]**.
