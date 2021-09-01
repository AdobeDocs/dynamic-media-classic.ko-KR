---
title: 템플릿 파일 업로드
description: Adobe Dynamic Media Classic에서 템플릿 파일을 업로드하는 방법을 알아봅니다.
uuid: e19979b5-3f41-49c5-99aa-107ede3be98c
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 75658717-5c39-473e-9d32-718d00706310
feature: Dynamic Media Classic
role: User
exl-id: a105c18a-7e06-43cb-938c-a3bcdc3e9d22
source-git-commit: 8bc49ae3704f0551c70d68a0ddd63725bdcc645c
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 38%

---

# 템플릿 파일 업로드{#uploading-template-files}

템플릿 작성을 시작하기 전에 템플릿에 필요한 파일을 Adobe Dynamic Media Classic에 업로드합니다. Adobe® Photoshop® PSD 또는 이미지 파일에서 템플릿을 작성할 수 있습니다. 투명도를 허용하기 때문에 TIFF 및 PNG 이미지가 권장됩니다.

>[!NOTE]
>
>Adobe Dynamic Media Classic에서는 템플릿에 있는 투명한 TIFF 또는 PSD 이미지를 웹 사이트에 표시할 정확한 크기로 사용하는 것이 좋습니다. 템플릿을 게시할 때 동일한 크기인 이미지 사전 설정을 사용하여 이미지를 호출합니다. 크기에 주의하여 템플릿 크기가 원래 디자인된 크기보다 작거나 크게 조정(재샘플링)되지 않도록 합니다.

Adobe Photoshop PSD 파일이나 이미지 파일에서 템플릿을 만들 수 있습니다.

파일 업로드에 대한 자세한 지침은 [파일 업로드](uploading-files.md#uploading_files)를 참조하십시오. 템플릿 파일을 업로드하는 경우 다음 사항에 주의합니다.

* PSD 파일을 업로드하는 경우 해당 파일에서 템플릿을 만들 수 있습니다. Adobe Dynamic Media Classic에서는 PSD의 각 레이어에 대해 별도의 이미지를 만듭니다. 업로드 작업 옵션 대화 상자에서 **[!UICONTROL Photoshop 옵션]**&#x200B;을 선택하고 **[!UICONTROL 레이어 유지]** 및 **[!UICONTROL 템플릿 만들기]**&#x200B;를 선택합니다. 그런 다음 **[!UICONTROL 레이어 이름 지정]** 드롭다운 목록에서 옵션을 선택하여 PSD의 레이어에서 Dynamic Media Classic이 만드는 이미지의 이름을 지정합니다.
[PSD 업로드 선택 사항](psd-files.md#psd_upload_options)을 참조하십시오.

<!-- THERE IS NO LONGER AN IMAGE EDITING OPTIONS MENU * If you are uploading images, you can create a mask from its clipping path. This option applies to images created with image-editing applications in which a clipping path was created. In the Upload Job Options dialog box, select Image Editing Options and select the Create Mask From Clipping Path option. 
See [Image editing options at upload](image-editing-options-upload.md#image-editing-options-at-upload). -->

>[!MORELIKETHIS]
>
>* [파일 업로드](uploading-files.md#uploading_your_files)
>* [PSD 파일 작업](psd-files.md#working_with_psd_files)

