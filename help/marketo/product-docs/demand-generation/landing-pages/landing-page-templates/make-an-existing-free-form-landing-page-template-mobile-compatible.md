---
unique-page-id: 5472348
description: 使现有的自由表单登陆页面模板与移动设备兼容 — Marketo文档 — 产品文档
title: 使现有的自由表单登陆页面模板与移动设备兼容
exl-id: 942456a5-3f3e-4a71-aecc-4cc6bf6237b3
feature: Landing Pages
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 0%

---

# 使现有的自由表单登陆页面模板与移动设备兼容 {#make-an-existing-free-form-landing-page-template-mobile-compatible}

可以在模板编辑器和登陆页面编辑器这两个位置执行此操作。

## 从模板编辑器升级 {#upgrade-from-the-template-editor}

1. 转到 **Design Studio**.

   ![](assets/designstudio-1.png)

1. 选择 **模板**.

   ![](assets/image2015-1-22-20-3a20-3a2.png)

1. 选择模板，其中 **移动设备兼容** 是 **否**.

   ![](assets/image2015-1-22-20-3a22-3a24.png)

1. 单击 **编辑草稿**.

   ![](assets/image2015-1-22-20-3a25-3a36.png)

1. 单击 **使移动设备兼容**.

   ![](assets/image2015-1-22-20-3a30-3a33.png)

1. 单击 **升级**.

   ![](assets/image2015-1-22-20-3a32-3a45.png)

   您的登陆页面模板现在与移动设备兼容！

   >[!NOTE]
   >
   >升级应该无害，但请确保检查页面是否有任何差异。 升级将使用该模板创建任何登陆页面的草稿。

   ![](assets/image2015-1-22-20-3a36-3a43.png)

## 是什么使模板移动设备兼容？ {#what-makes-a-template-mobile-compatible}

好问题！ 您的模板必须具有以下标记：

`<pre data-theme="Confluence">Must have <!DOCTYPE HTML> Must have a <HEAD> element Must have a <TITLE> in the <HEAD> element Must have <META CHARSET="UTF-8"> within the <HEAD> element Must have a <BODY> element that contains one (and only one) <DIV class="mktoContent"></DIV></pre>`

如果一切正常，您将看到此消息。

![](assets/image2015-1-22-20-3a41-3a31.png)

如果出现错误，将显示一条错误消息，请单击“修复”以修复问题并重复验证过程。

![](assets/image2015-1-22-20-3a43-3a20.png)

如果对模板进行了任何更改，请单击模板操作，然后选择验证移动设备兼容性。

## 从自由格式登陆页面编辑器升级模板 {#upgrading-a-template-from-the-free-form-landing-page-editor}

在编辑登陆页并单击移动设备选项卡时，您有时会注意到模板尚未升级。 不要害怕！ 你可以在这里升级它。

1. 单击 **移动设备** 选项卡。

   ![](assets/image2015-1-22-20-3a48-3a19.png)

1. 单击该复选框，然后单击 **激活**.

   ![](assets/image2015-1-22-20-3a49-3a34.png)

   >[!NOTE]
   >
   >激活模板的移动版本将会创建使用该模板的任何登陆页面的草稿。

太棒了！ 您现在可以 [自定义移动设备视图](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/customize-mobile-view-for-your-free-form-landing-page.md) 您所有使用此模板的登陆页面的ID。
