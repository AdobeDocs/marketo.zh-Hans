---
unique-page-id: 1147322
description: 了解匿名活动和人员——营销文档——产品文档
title: 了解匿名活动和人员
translation-type: tm+mt
source-git-commit: 07f713ece9832b7696451001f61c6a3b45b4a94a
workflow-type: tm+mt
source-wordcount: '208'
ht-degree: 0%

---


# 了解匿名活动和人员{#understanding-anonymous-activity-and-people}

第一次有人访问Marketo登陆页（或您网站上具有[Munchkin跟踪代码](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)的页面）时，Marketo会创建&#x200B;_匿名活动_&#x200B;并使用浏览器cookie跟踪它。 一旦识别出来，它就变成人，与其浏览器cookie关联的历史记录将被合并。

**当某** 人发生以下情况时，将创建匿名活动：

* 首次访问您的营销登陆页。
* 访问您网站上具有[Munchkin跟踪](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)的页面。
* 单击Marketo电子邮件中的[视图作为Web页](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)链接。

>[!NOTE]
>
>与Marketo电子邮件中的其他链接不同，[作为网页的视图](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)不会作为电子邮件单击进行跟踪。

当某人：

* 单击Marketo电子邮件](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md)中的[链接。
* 填写[Form](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md)的标记。
* 使用Marketo的[SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md)或[ Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) API（对于开发人员）将匿名人员与已知记录相关联。

数据库中的一个名称可能与许多cookies关联，因为人们经常使用不同的设备和浏览器访问您的站点。

>[!NOTE]
>
>当匿名记录合并到新记录或现有人员记录中时，自定义字段值将&#x200B;**不**&#x200B;转移。
