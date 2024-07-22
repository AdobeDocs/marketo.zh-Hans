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

有时，您可能需要修改电子邮件的基础HTML。 有时，您可以使用外部系统来设计和构建电子邮件的代码。 无论采用哪种方式，您都可以在电子邮件编辑器中轻松导入和/或编辑代码。

## 编辑HTML {#edit-html}

1. 选择您的电子邮件并单击&#x200B;**编辑草稿**。

   ![](assets/teamspidey.jpg)

1. 单击&#x200B;**编辑代码**。

   ![](assets/two-4.png)

1. 进行任何更改。 完成后单击&#x200B;**保存**。

   ![](assets/three-3.png)

   >[!NOTE]
   >
   >随心所欲地改变。 您可以替换整个HTML或进行细微调整。

1. 单击&#x200B;**代码操作**&#x200B;下拉菜单以将代码下载为.html文件、内联CSS或验证HTML。

   ![](assets/four-2.png)

   >[!NOTE]
   >
   >处理电子邮件的最佳做法是内联所有样式。 多个电子邮件客户端不支持`<head>`部分中的CSS。

## 从模板中中断电子邮件 {#breaking-an-email-from-its-template}

这些代码更改&#x200B;**将不会**&#x200B;中断来自其模板的电子邮件：

* 编辑任何模块的内容（包括在模块内添加新元素）
* 将新模块添加到容器
* 从容器中删除模块

* 更改模块外任何元素的mkto特定属性（例如，“mktoName”或“mktoImgUrl”）
* 编辑任何元素的内容（富文本、图像、视频等） 模块外部

在代码编辑器&#x200B;**中可以执行的这些操作将**&#x200B;中断来自其模板的电子邮件：

* 在元素或模块之外更改代码中的任何内容
* 添加或更改模块外任何元素的非mkto属性（例如，“id”或“style”）
* 删除模块外部的元素

## 搜索代码 {#search-code}

使用搜索代码功能高效地查找和替换电子邮件HTML代码中的内容。

1. 在您的电子邮件代码中，单击&#x200B;**搜索代码**。

   ![](assets/five-2.png)

1. 输入要查找的内容，然后单击&#x200B;**查找下一个**&#x200B;进行正向搜索，或单击&#x200B;**查找上一个**&#x200B;进行反向搜索。 您还可以选择&#x200B;**替换**&#x200B;和&#x200B;**全部替换**。

   ![](assets/six-1.png)

1. 完成后单击&#x200B;**关闭**。

   ![](assets/seven.png)

   >[!NOTE]
   >
   >[电子邮件模板编辑器](/help/marketo/product-docs/email-marketing/general/email-editor-2/create-an-email-template.md)中也提供了搜索代码。

我们建议您使用Marketo的内置功能继续编辑电子邮件，但如果需要，此代码编辑器会提供灵活性。
