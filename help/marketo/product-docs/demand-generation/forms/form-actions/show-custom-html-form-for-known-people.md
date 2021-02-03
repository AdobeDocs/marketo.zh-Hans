---
unique-page-id: 2359644
description: 显示已知人员的自定义HTML表单- Marketo Docs —— 产品文档
title: 显示已知用户的自定义HTML表单
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---


# 显示已知用户的自定义HTML表单{#show-custom-html-form-for-known-people}

如果访客使用cookie（过去提供电子邮件地址的已知人员），那么为什么要费心使用表单？ 只需给他们下载按钮。 这是方法。

1. 转到&#x200B;**营销活动**。

   ![](assets/login-marketing-activities-5.png)

1. 在&#x200B;**营销活动**&#x200B;下，选择您的表单，然后单击&#x200B;**编辑表单**。

   ![](assets/image2014-9-15-12-3a24-3a6.png)

1. 在&#x200B;**表单设置**&#x200B;下，单击&#x200B;**设置**。

   ![](assets/image2014-9-15-12-3a24-3a36.png)

1. 如果&#x200B;**已知访客，则设置Show**:到&#x200B;**自定义HTML**。

   ![](assets/image2014-9-15-12-3a24-3a59.png)

1. 单击![—](assets/image2014-9-25-14-3a1-3a26.png)可编辑将向已知用户显示的&#x200B;**自定义HTML**。

   ![](assets/image2014-9-15-12-3a25-3a38.png)

1. 有一些默认内容，但可以随意更改。

   ![](assets/image2014-9-15-12-3a25-3a49.png)

   可用令牌：

   | 令牌 | 说明 |
   |---|---|
   | `{{lead.FirstName}}` | 将显示该人的名字。 |
   | `{{lead.LastName}}` | 将显示该人的姓。 |
   | `{{form.Button:default=Download}}` | 此时将显示表单按钮。 替换`=`后面的区域以更改按钮文本。 |
   | `{{form.NotYou:default=Not you?}}` | 这将显示一个链接，以防此人是其他人。 替换`=`后面的区域以更改链接文本。 |

   >[!CAUTION]
   >
   >只能使用上述四个令牌。 此处不能使用任何其他令牌。

1. 单击&#x200B;**完成**。

   ![](assets/image2014-9-15-12-3a27-3a25.png)

1. 单击&#x200B;**批准并关闭**。

   >[!NOTE]
   >
   >必须批准表单才能用于登陆页。

   ![](assets/image2014-9-15-12-3a27-3a53.png)

   >[!NOTE]
   >
   >请记住[批准由表单更改创建的登陆页草稿](/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/approve-unapprove-or-delete-a-landing-page.md)。

   蛋糕！ 查看如果某个人返回同一表单会看到什么：

   ![](assets/image2014-9-15-12-3a28-3a12.png)

   >[!TIP]
   >
   >您可以通过将表单跟进页面设置到文件的URL，将按钮的单击指向资产。
