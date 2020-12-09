---
unique-page-id: 5472348
description: 使现有的自由格式登陆页模板与移动设备兼容- Marketo Docs —— 产品文档
title: 使现有自由格式登陆页模板与移动设备兼容
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---


# 使现有自由格式登陆页模板与移动设备兼容 {#make-an-existing-free-form-landing-page-template-mobile-compatible}

>[!NOTE]
>
>登陆页模板在2015年1月版 [本之](../../../../release-notes/2015/release-notes-january-2015.md)前创建，需要升级为与移动设备兼容。

此操作可在两个位置完成，即模板编辑器和登陆页编辑器。

## 从模板编辑器升级 {#upgrade-from-the-template-editor}

1. 转到Design **Studio**。

   ![](assets/designstudio-1.png)

1. 选择 **模板**。

   ![](assets/image2015-1-22-20-3a20-3a2.png)

1. 选择Mobile Compatible为 **No的** 模 **板**。

   ![](assets/image2015-1-22-20-3a22-3a24.png)

1. 单击“ **编辑草稿**”。

   ![](assets/image2015-1-22-20-3a25-3a36.png)

1. 单击“ **使移动设备兼容**”。

   ![](assets/image2015-1-22-20-3a30-3a33.png)

1. 单击 **升级**。

   ![](assets/image2015-1-22-20-3a32-3a45.png)

   您的登陆页模板现在与移动兼容！

   >[!NOTE]
   >
   >升级应不会造成任何损害，但应确保检查页面是否有任何差异。 升级将创建使用该模板的任何登陆页的草稿。

   ![](assets/image2015-1-22-20-3a36-3a43.png)

## 什么使模板移动兼容？ {#what-makes-a-template-mobile-compatible}

问得好！ 模板必须具有以下标记：

`<pre data-theme="Confluence">Must have <!DOCTYPE HTML> Must have a <HEAD> element Must have a <TITLE> in the <HEAD> element Must have <META CHARSET="UTF-8"> within the <HEAD> element Must have a <BODY> element that contains one (and only one) <DIV class="mktoContent"></DIV></pre>`  如果一切顺利，您将看到这条消息。

![](assets/image2015-1-22-20-3a41-3a31.png)

如果出错，将显示错误消息，单击“修复”以修复问题，然后重复验证过程。

![](assets/image2015-1-22-20-3a43-3a20.png)

如果对模板进行了任何更改，请单击“模板操作”，然后选择“验证移动兼容性”。

## 从自由形式登陆页编辑器升级模板 {#upgrading-a-template-from-the-free-form-landing-page-editor}

当您编辑登陆页并单击移动选项卡时，有时会注意到该模板尚未升级。 不要害怕！ 您可以立即升级。

1. 单击“移 **动** ”选项卡。

   ![](assets/image2015-1-22-20-3a48-3a19.png)

1. 单击复选框，然后单击“ **激活**”。

   ![](assets/image2015-1-22-20-3a49-3a34.png)

   >[!NOTE]
   >
   >激活模板的移动版本将创建使用该模板的任何登陆页的草稿。

太棒了！ 您现在可 [以自定义所有使用](../../../../product-docs/demand-generation/landing-pages/free-form-landing-pages/customize-mobile-view-for-your-free-form-landing-page.md) 此模板的登陆页的移动视图。

>[!MORELIKETHIS]
>
>* [为自由形式视图自定义移动登陆页](../../../../product-docs/demand-generation/landing-pages/free-form-landing-pages/customize-mobile-view-for-your-free-form-landing-page.md)

>



