---
unique-page-id: 1147322
description: 了解匿名活动和人员 — Marketo文档 — 产品文档
title: 了解匿名活动和人员
exl-id: 1676e8f3-9138-42ed-8bb4-40e195391fc4
feature: Smart Lists
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---

# 了解匿名活动和人员 {#understanding-anonymous-activity-and-people}

首次访问Marketo登陆页面(或网站上具有[Munchkin跟踪代码](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}的页面)时，Marketo会创建一个&#x200B;*匿名活动*&#x200B;并使用浏览器Cookie对其进行跟踪。 标识后，它就会成为人员，并且与其浏览器Cookie关联的历史记录将合并到中。

>[!IMPORTANT]
>
>在已知&#x200B;**[!DNL Munchkin]上启用Beta功能** V2匿名重播活动可确保在匿名潜在客户成功合并到已知记录后，始终重播由匿名潜在客户促销触发的营销活动。 因此，任何重播营销活动中由更改数据值步骤更改的自定义字段将保留在已知记录中。

**在有人出现以下情况时创建匿名**&#x200B;活动：

* 首次访问Marketo登陆页面。
* 访问网站上具有[Munchkin跟踪](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}的页面。
* 单击Marketo电子邮件中的[以网页形式查看](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"}链接。

>[!NOTE]
>
>与Marketo电子邮件中的其他链接不同，[以网页形式查看](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"}不会以电子邮件点击形式进行跟踪。

当某人出现以下情况时，匿名活动会合并到新人员或现有人员中：

* 单击Marketo电子邮件[中的](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"}链接。
* 填写Marketo [表单](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md){target="_blank"}。
* 使用Marketo的[SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md){target="_blank"}或[Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"} API（适用于开发人员）将匿名人员与已知记录相关联。

数据库中的某个名称可能与许多Cookie相关联，因为人们通常使用不同的设备和浏览器访问您的网站。

>[!NOTE]
>
>将匿名记录合并到新的或现有的人员记录中时，自定义字段值将&#x200B;*不会*&#x200B;转移。
