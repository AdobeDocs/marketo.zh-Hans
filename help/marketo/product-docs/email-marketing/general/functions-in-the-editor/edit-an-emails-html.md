---
unique-page-id: 1900554
description: 编辑电子邮件的HTML- Marketo文档 — 产品文档
title: 编辑电子邮件的HTML
exl-id: 9dc8e44d-d9da-4bc2-950f-3ffbb976f5d5
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# 编辑电子邮件的HTML {#edit-an-emails-html}

有时您可能需要修改电子邮件的基础HTML。 有时，您可以使用外部系统来设计和构建电子邮件的代码。 无论哪种方式，您都可以在电子邮件编辑器中轻松导入和/或编辑代码。

## 编辑HTML {#edit-html}

1. 选择您的电子邮件并单击 **编辑草稿**.

   ![](assets/teamspidey.jpg)

1. 单击 **编辑代码**.

   ![](assets/two-4.png)

1. 进行任何更改。 单击 **保存** 完成时。

   ![](assets/three-3.png)

   >[!NOTE]
   >
   >随心所欲地改变。 您可以替换整个HTML或进行细微调整。

1. 单击 **代码操作** 下拉菜单以将代码下载为.html文件、内联CSS或验证HTML。

   ![](assets/four-2.png)

   >[!NOTE]
   >
   >电子邮件的最佳实践是使所有样式内联。 多个电子邮件客户端不支持中的CSS `<head>` 部分。

## 从电子邮件模板中断电子邮件 {#breaking-an-email-from-its-template}

这些代码更改 **不会** 从模板中断电子邮件：

* 编辑任何模块的内容（包括在模块内添加新元素）
* 将新模块添加到容器
* 从容器中删除模块

* 更改模块外任何元素的mkto特定属性（例如，“mktoName”或“mktoImgUrl”）
* 编辑任何元素的内容（富文本、图像、视频等） 模块外部

可在代码编辑器中执行的操作 **将** 从电子邮件模板中断电子邮件：

* 在元素或模块之外更改代码中的任何内容
* 添加或更改模块外任何元素的非mkto属性（例如，“id”或“style”）
* 删除模块外部的元素

## 搜索代码 {#search-code}

使用搜索代码功能高效地查找和替换电子邮件HTML代码中的内容。

1. 在电子邮件的代码中，单击 **搜索代码**.

   ![](assets/five-2.png)

1. 输入要查找的内容，然后单击 **查找下一个** 要向前搜索或 **查找上一个** 进行反向搜索。 您还可以选择执行以下操作 **Replace** 和 **全部替换**.

   ![](assets/six-1.png)

1. 单击 **关闭** 完成时。

   ![](assets/seven.png)

   >[!NOTE]
   >
   >搜索代码也可在以下位置找到： [电子邮件模板编辑器](/help/marketo/product-docs/email-marketing/general/email-editor-2/create-an-email-template.md).

我们建议您继续使用Marketo的内置功能编辑电子邮件，但如果需要，此代码编辑器会提供灵活性。
