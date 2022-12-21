---
unique-page-id: 2359644
description: 显示已知人员的自定义HTML表单 — Marketo文档 — 产品文档
title: 显示已知人员的自定义HTML表单
exl-id: 668216ea-7c2b-4204-81a5-56547c3baf1d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---

# 显示已知人员的自定义HTML表单 {#show-custom-html-form-for-known-people}

如果访客带有Cookie（过去提供电子邮件地址的已知人员），那么为什么还要费心使用表单？ 给他们下载按钮。 这是方法。

1. 转到 **营销活动**.

   ![](assets/login-marketing-activities-5.png)

1. 在 **营销活动**，选择您的表单并单击 **编辑表单**.

   ![](assets/image2014-9-15-12-3a24-3a6.png)

1. 在 **表单设置**，单击 **设置**.

   ![](assets/image2014-9-15-12-3a24-3a36.png)

1. 如果 **已知访客，节目**:to **自定义HTML**.

   ![](assets/image2014-9-15-12-3a24-3a59.png)

1. 单击 ![—](assets/image2014-9-25-14-3a1-3a26.png) 编辑 **自定义HTML** 将向已知人展示。

   ![](assets/image2014-9-15-12-3a25-3a38.png)

1. 有一些默认内容，但可以随意更改。

   ![](assets/image2014-9-15-12-3a25-3a49.png)

   可用令牌：

   | 令牌 | 描述 |
   |---|---|
   | `{{lead.FirstName}}` | 这将显示人员的名字。 |
   | `{{lead.LastName}}` | 这将显示人员的姓氏。 |
   | `{{form.Button:default=Download}}` | 此时将显示表单按钮。 替换 `=` 来更改按钮文本。 |
   | `{{form.NotYou:default=Not you?}}` | 如果人员是其他人，将显示一个链接。 替换 `=` 来更改链接文本。 |

   >[!CAUTION]
   >
   >只能使用上述四个令牌。 任何其他令牌在此处不起作用。

1. 单击 **完成**.

   ![](assets/image2014-9-15-12-3a27-3a25.png)

1. 单击 **批准并关闭**.

   >[!NOTE]
   >
   >表单必须获得批准才能在登陆页面上使用。

   ![](assets/image2014-9-15-12-3a27-3a53.png)

   >[!NOTE]
   >
   >记住 [批准登陆页面草稿](/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/approve-unapprove-or-delete-a-landing-page.md) 创建的URL。

   一块蛋糕！ 查看如果某个人返回同一表单，他们会看到什么：

   ![](assets/image2014-9-15-12-3a28-3a12.png)

   >[!TIP]
   >
   >您可以通过将表单跟踪页面设置为文件的URL，将按钮的单击定向到资产。
