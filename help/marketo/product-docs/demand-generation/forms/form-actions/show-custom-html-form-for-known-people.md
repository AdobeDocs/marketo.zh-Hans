---
unique-page-id: 2359644
description: 显示已知人员的自定义HTML表单 — Marketo文档 — 产品文档
title: 显示已知人员的自定义HTML表单
exl-id: 668216ea-7c2b-4204-81a5-56547c3baf1d
feature: Forms
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---

# 显示已知人员的自定义HTML表单 {#show-custom-html-form-for-known-people}

如果访客（以前提供过电子邮件地址的已知人员）已被确认，那么为什么要麻烦填写表单？ 只要给他们下载按钮就行。 下面是具体操作方法。

1. 转到 **营销活动**.

   ![](assets/login-marketing-activities-5.png)

1. 下 **营销活动**，选择您的表单并单击 **编辑表单**.

   ![](assets/image2014-9-15-12-3a24-3a6.png)

1. 下 **表单设置**，单击 **设置**.

   ![](assets/image2014-9-15-12-3a24-3a36.png)

1. 设置If **已知访客，节目**：至 **自定义HTML**.

   ![](assets/image2014-9-15-12-3a24-3a59.png)

1. 单击 ![—](assets/image2014-9-25-14-3a1-3a26.png) 编辑 **自定义HTML** 向已知人员显示。

   ![](assets/image2014-9-15-12-3a25-3a38.png)

1. 虽然有一些默认内容，但您可以随意对其进行更改。

   ![](assets/image2014-9-15-12-3a25-3a49.png)

   可用令牌：

   | 令牌 | 描述 |
   |---|---|
   | `{{lead.FirstName}}` | 这将显示人员的名字。 |
   | `{{lead.LastName}}` | 这将显示人员的姓氏。 |
   | `{{form.Button:default=Download}}` | 这将显示表单按钮。 将区域替换在 `=` 以更改按钮文本。 |
   | `{{form.NotYou:default=Not you?}}` | 该链接会显示该人员是其他人时的链接。 将区域替换在 `=` 以更改链接文本。 |

   >[!CAUTION]
   >
   >只能使用以上四个令牌。 此处无法使用任何其他令牌。

1. 单击 **完成**.

   ![](assets/image2014-9-15-12-3a27-3a25.png)

1. 单击 **批准并关闭**.

   >[!NOTE]
   >
   >该表单必须获得批准才能在登陆页面上使用。

   ![](assets/image2014-9-15-12-3a27-3a53.png)

   >[!NOTE]
   >
   >请记住 [批准登陆页面草稿](/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/approve-unapprove-or-delete-a-landing-page.md) 由表单更改创建。

   一块蛋糕！ 查看人员返回同一表单时会看到什么：

   ![](assets/image2014-9-15-12-3a28-3a12.png)

   >[!TIP]
   >
   >通过将表单跟进页面设置为文件的URL，您可以将单击按钮引导至资源。
