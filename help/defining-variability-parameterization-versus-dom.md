---
title: '"가변성 정의: 매개 변수화 및 DOM 조작"'
seo-title: '"가변성 정의: 매개 변수화 및 DOM 조작"'
description: 널
seo-description: 매개 변수화와 DOM 조작을 통해 가변성을 정의하는 방법을 살펴봅니다.
uuid: dce424f2-07d8-4703-aa3a-40d2eee12f74
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template-publishing
discoiquuid: 5b844afe-ac55-4dd2-8fe8-125a9c9af948
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# 가변성 정의: 매개 변수화 및 DOM 조작{#defining-variability-parameterization-versus-dom-manipulation}

Dynamic Media Classic에서는 템플릿에서 변수 컨텐츠를 관리하는 두 가지 방법을 제공합니다. 두 가지 방법을 모두 사용하여 Illustrator에서 초기 템플릿을 디자인하고 템플릿을 Dynamic Media Classic FXG 파일 포맷으로 변환한 다음 SPS에 업로드합니다. 그러나 변수 요소에 대한 제어 수준과 사용하는 데 필요한 기술은 두 기술에서 서로 다릅니다.

* **Scene7 Publishing System**&#x200B;에서 매개 변수화이 기술은 SPS의 템플릿 게시 빌드 및 미리 보기 화면 또는 Web-to-Print용 Adobe Illustrator 플러그인에서 가변성을 정의합니다. 각각의 방법에서는 매개 변수를 만들고, 매개 변수 값을 지정하고, 결과를 테스트할 수 있는 도구를 제공합니다.

* **DOM 조작**&#x200B;이 기술을 사용하면 XML 수준에서 디자인과 템플릿을 제어할 수 있습니다. Dynamic Media Classic FXG 파일은 XML입니다. 이 방법을 사용할 경우 XML DOM(표시 개체 모델) 방법을 통해 디자인 템플릿을 편집할 수 있습니다. Illustrator에서 변수 요소에 s7:elementID를 표시하여 나중에 URL 명령으로 조작할 수 있게 합니다.

>[!MORELIKETHIS]
>
>* [Dynamic Media Classic에서 템플릿 매개 변수화](parameterizing-template-scene7.md#parameterizing_a_template_in_scene7)
>* [DOM 조작](dom-manipulation.md#dom_manipulation)

