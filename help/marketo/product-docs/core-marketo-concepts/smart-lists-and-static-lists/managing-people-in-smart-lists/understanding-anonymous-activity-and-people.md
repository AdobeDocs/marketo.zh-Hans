---
unique-page-id: 1147322
description: 了解匿名活动和人员——营销文档——产品文档
title: 了解匿名活动和人员
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---


# 了解匿名活动和人员 {#understanding-anonymous-activity-and-people}

第一次有人访问Marketo [l( `anding page`](http://docs.marketo.com/display/DOCS/Personalizing+Landing+Pages) 或您网站上包含Munchkin跟踪代码的页面 [)时，Marketo会创建一个*匿名的*](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)** 活动，并使用浏览器Cookie跟踪它。 一旦识别出来，它就变成人，与其浏览器cookie关联的历史记录将被合并。

**当某人** :

* 首次访问您的营销登陆页。

* 访问您网站上具有Munchkin跟踪 [的页面](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)。

* 单击Marketo [电子邮件中的](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) “网页视图”链接。

>[!NOTE]
>
>与Marketo电子邮件中的其他链接不 [同，视图作为网页](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) ，不会作为电子邮件单击进行跟踪。

当某人：

* 单击Marketo [电子邮件中的链接](../../../../product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md)。
* 填写营销 [表](../../../../product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md)。
* 使用Marketo的 [SOAP](http://docs.marketo.com/pages/viewpage.action?pageid=7509846)[或Munchkin](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) API（对于开发人员）将匿名人员与已知记录相关联。

数据库中的一个名称可能与许多cookies关联，因为人们经常使用不同的设备和浏览器访问您的站点。

>[!NOTE]
>
>当匿名记录合并到新记录或现有人员记录中时，自定义字段值将 **不会** 转移。

