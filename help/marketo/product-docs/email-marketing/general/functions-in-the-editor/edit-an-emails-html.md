---
unique-page-id: 1900554
description: 编辑电子邮件的HTML- Marketo文档 — 产品文档
title: 编辑电子邮件的HTML
exl-id: 9dc8e44d-d9da-4bc2-950f-3ffbb976f5d5
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# 编辑电子邮件的HTML {#edit-an-emails-html}

有时，您可能需要修改电子邮件的基础HTML。 有时，您可能会使用外部系统来设计和构建电子邮件的代码。 无论哪种方式，您都可以在电子邮件编辑器中轻松导入和/或编辑代码。

## 编辑HTML {#edit-html}

1. 选择您的电子邮件并单击 **编辑草稿**.

   ![](assets/teamspidey.jpg)

1. 单击 **编辑代码**.

   ![](assets/two-4.png)

1. 进行任何更改。 单击 **保存** 完成时。

   ![](assets/three-3.png)

   >[!NOTE]
   >
   >随你改变。 您可以替换整个HTML或进行细微调整。

1. 单击 **代码操作** 下拉列表，将代码下载为.html文件（在CSS中内嵌）或验证HTML。

   ![](assets/four-2.png)

   >[!NOTE]
   >
   >电子邮件的最佳实践是使所有样式都内联。 在 `<head>` 中。

## 从模板中断电子邮件 {#breaking-an-email-from-its-template}

这些代码更改 **将不会** 从模板中断开电子邮件：

* 编辑任何模块的内容（包括在模块内添加新元素）
* 向容器添加新模块
* 从容器中删除模块

* 更改模块外任何元素的mkto特定属性（例如，“mktoName”或“mktoImgUrl”）
* 编辑任何元素（富文本、图像、视频等）的内容 模块外部

您可以在代码编辑器中执行这些操作 **will** 从模板中断电子邮件：

* 在元素或模块之外更改代码中的任何内容
* 添加或更改模块外任何元素的非mkto属性（例如，“id”或“style”）
* 删除模块外的元素

## 搜索代码 {#search-code}

使用搜索代码功能，可高效查找和替换电子邮件HTML代码中的内容。

1. 在电子邮件的代码中，单击 **搜索代码**.

   ![](assets/five-2.png)

1. 输入要查找的内容并单击 **查找下一个** 向前搜索或 **查找上一个** 向后搜索。 您还可以选择 **替换** 和 **全部替换**.

   ![](assets/six-1.png)

1. 单击 **关闭** 完成时。

   ![](assets/seven.png)

   >[!NOTE]
   >
   >搜索代码在 [电子邮件模板编辑器](/help/marketo/product-docs/email-marketing/general/email-editor-2/create-an-email-template.md).

我们建议您继续使用Marketo的内置功能编辑电子邮件，但如果需要，此代码编辑器可提供灵活性。
