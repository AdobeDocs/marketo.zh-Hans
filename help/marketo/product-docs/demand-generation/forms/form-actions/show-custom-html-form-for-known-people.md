---
unique-page-id: 2359644
description: 显示已知人员的自定义HTML表单- Marketo Docs —— 产品文档
title: 显示已知用户的自定义HTML表单
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---


# 显示已知用户的自定义HTML表单 {#show-custom-html-form-for-known-people}

如果访客使用cookie（过去提供电子邮件地址的已知人员），那么为什么要费心使用表单？ 只需给他们下载按钮。 这是方法。

>[!NOTE]
>
>**FYI**
>
>Marketo现在正在所有订阅实现语言标准化，因此您可能会在订阅和docs.marketo.com中看到潜在客户／潜在客户。 这些术语的含义是相同的；它不影响文章说明。 还有一些其他变化。 [了解更多](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

1. 转到营 **销****活动**。

   ![](assets/login-marketing-activities-5.png)

1. 在“营 **销******&#x200B;活动 **”** 下，选择表单，然后单 **击“编**&#x200B;辑表单”。

   ![](assets/image2014-9-15-12-3a24-3a6.png)

1. 在“ **表单****设置**”下，单 **击设置**。

   ![](assets/image2014-9-15-12-3a24-3a36.png)

1. 如果已知 **访客** , **则设置“显示**:到 **自定****义HTML**。

   ![](assets/image2014-9-15-12-3a24-3a59.png)

1. 单击 ![-](assets/image2014-9-25-14-3a1-3a26.png) 以编辑将显 **示** 给已知人 **** 员的自定义HTML。

   ![](assets/image2014-9-15-12-3a25-3a38.png)

1. 有一些默认内容，但可以随意更改。

   ![](assets/image2014-9-15-12-3a25-3a49.png)

   可用令牌：

   | 令牌 | 说明 |
   |---|---|
   | `{{lead.FirstName}}` | 将显示该人的名字。 |
   | `{{lead.LastName}}` | 将显示该人的姓。 |
   | `{{form.Button:default=Download}}` | 此时将显示表单按钮。 替换按钮文 `=` 本后的区域。 |
   | `{{form.NotYou:default=Not you?}}` | 这将显示一个链接，以防此人是其他人。 替换链接文本 `=` 后的区域。 |

   >[!CAUTION]
   >
   >只能使用上述四个令牌。 此处不能使用任何其他令牌。

1. 单击 **完成**。

   ![](assets/image2014-9-15-12-3a27-3a25.png)

1. 单击 **批准并关闭**。

   >[!NOTE]
   >
   >必须批准表单才能用于登陆页。

   ![](assets/image2014-9-15-12-3a27-3a53.png)

   >[!NOTE]
   >
   >**提醒**
   >
   >
   >请记住 [批准由表单更改](../../../../product-docs/demand-generation/landing-pages/understanding-landing-pages/approve-unapprove-or-delete-a-landing-page.md) 创建的登陆页草稿。

   ![](assets/image2014-9-15-12-3a28-3a12.png)

   >[!TIP]
   >
   >您可以通过将表单跟进页面设置到文件的URL，将按钮的单击指向资产。

蛋糕！ 查看如果某个人返回同一表单会看到什么：