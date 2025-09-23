---
unique-page-id: 2359644
description: 显示已知人员的自定义HTML表单 — Marketo文档 — 产品文档
title: 为已知用户显示自定义 HTML 表单
exl-id: 668216ea-7c2b-4204-81a5-56547c3baf1d
feature: Forms
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 7%

---

# 为已知用户显示自定义 HTML 表单 {#show-custom-html-form-for-known-people}

如果访客以前提供过其全名和电子邮件地址，并且您不希望他们获得整个表单，请了解如何向他们显示一些自定义HTML（例如，只需下载按钮）。

1. 转到&#x200B;**[!UICONTROL Marketing Activities]**。

   ![](assets/login-marketing-activities-5.png)

1. 在&#x200B;**[!UICONTROL Marketing Activities]**&#x200B;下，选择您的表单并单击&#x200B;**[!UICONTROL Edit Form]**。

   ![](assets/image2014-9-15-12-3a24-3a6.png)

1. 在&#x200B;**[!UICONTROL Form Settings]**&#x200B;下，单击&#x200B;**[!UICONTROL Settings]**。

   ![](assets/image2014-9-15-12-3a24-3a36.png)

1. 设置If **[!UICONTROL Known Visitor, Show]**：为&#x200B;**[!UICONTROL Custom HTML]**。

   ![](assets/image2014-9-15-12-3a24-3a59.png)

1. 单击![—](assets/image2014-9-25-14-3a1-3a26.png)以编辑将向已知人员显示的&#x200B;**[!UICONTROL Custom HTML]**。

   ![](assets/image2014-9-15-12-3a25-3a38.png)

1. 虽然有一些默认内容，但您可以随意对其进行更改。

   ![](assets/image2014-9-15-12-3a25-3a49.png)

   可用令牌：

   | 令牌 | 描述 |
   |---|---|
   | `{{lead.FirstName}}` | 这将显示人员的名字。 |
   | `{{lead.LastName}}` | 这将显示人员的姓氏。 |
   | `{{form.Button:default=Download}}` | 这将显示表单按钮。 替换`=`之后的区域以更改按钮文本。 |
   | `{{form.NotYou:default=Not you?}}` | 该链接会显示该人员是其他人时的链接。 替换`=`之后的区域以更改链接文本。 |

   >[!CAUTION]
   >
   >只能使用以上四个令牌。 此处无法使用任何其他令牌。

1. 单击 **[!UICONTROL Finish]**。

   ![](assets/image2014-9-15-12-3a27-3a25.png)

1. 单击 **[!UICONTROL Approve and Close]**。

   >[!NOTE]
   >
   >该表单必须获得批准才能在登陆页面上使用。

   ![](assets/image2014-9-15-12-3a27-3a53.png)

   >[!NOTE]
   >
   >请记住[批准由表单更改创建的登陆页面草稿](/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/approve-unapprove-or-delete-a-landing-page.md)。

   一块蛋糕！ 查看人员返回同一表单时会看到的内容：

   ![](assets/image2014-9-15-12-3a28-3a12.png)

   >[!TIP]
   >
   >通过将表单跟进页面设置为文件的URL，您可以将单击按钮引导至资源。
