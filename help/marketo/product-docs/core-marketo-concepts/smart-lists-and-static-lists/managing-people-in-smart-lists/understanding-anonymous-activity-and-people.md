---
unique-page-id: 1147322
description: 了解匿名活动和人员 — Marketo文档 — 产品文档
title: 了解匿名活动和人员
exl-id: 1676e8f3-9138-42ed-8bb4-40e195391fc4
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# 了解匿名活动和人员 {#understanding-anonymous-activity-and-people}

首次访问Marketo登陆页面(或网站上具有 [Munchkin跟踪代码](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)， Marketo创建 _匿名活动_ 并使用浏览器Cookie对其进行跟踪。 标识后，它就会成为人员，并且与其浏览器Cookie关联的历史记录将合并到中。

>[!IMPORTANT]
>
>启用Beta版功能 **已知的Munchkin V2匿名重放活动** 确保在匿名商机成功合并到已知记录后，始终重播由匿名商机促销触发的营销活动。 因此，任何重播营销活动中由更改数据值步骤更改的自定义字段将保留在已知记录中。

**匿名** 当有人执行以下操作时创建活动：

* 首次访问Marketo登陆页面。
* 访问网站上具有 [Munchkin跟踪](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
* 单击 [以网页形式查看](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) Marketo电子邮件中的链接。

>[!NOTE]
>
>与Marketo电子邮件中的其他链接不同， [以网页形式查看](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) 不会被跟踪为电子邮件点击。

当某人出现以下情况时，匿名活动会合并到新人员或现有人员中：

* 单击 [Marketo电子邮件中的链接](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).
* 填写Marketo [表单](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md).
* 使用Marketo的 [SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md) 或 [蒙奇金](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) 用于将匿名人员与已知记录关联的API（适用于开发人员）。

数据库中的某个名称可能与许多Cookie相关联，因为人们通常使用不同的设备和浏览器访问您的网站。

>[!NOTE]
>
>将匿名记录合并到新的或现有的人员记录时，自定义字段值将 **非** 转接。
