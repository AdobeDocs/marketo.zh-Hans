---
unique-page-id: 1147322
description: 了解匿名活动和人员 — Marketo文档 — 产品文档
title: 了解匿名活动和人员
exl-id: 1676e8f3-9138-42ed-8bb4-40e195391fc4
source-git-commit: cc66f4ff2e3e0e6ddfabab91215e3ad31f3b9226
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# 了解匿名活动和人员 {#understanding-anonymous-activity-and-people}

首次有人访问Marketo登陆页面(或您网站上具有 [Munchkin跟踪代码](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md), Marketo创建 _匿名活动_ 并使用浏览器Cookie进行跟踪。 识别后，该用户即成为人员，并且与其浏览器Cookie关联的历史记录会合并到中。

>[!IMPORTANT]
>
>启用测试版功能 **已知的Munchkin V2匿名重播活动** 确保在将匿名潜在客户成功合并到已知记录后，始终重播由匿名潜在客户促销活动触发的营销活动。 因此，任何重播营销活动中通过“更改数据值”步骤更改的自定义字段将保留在已知记录中。

**匿名** 活动时：

* 首次访问您的Marketo登陆页面。
* 访问您网站上具有 [蒙奇金跟踪](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
* 单击 [作为网页查看](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) 链接。

>[!NOTE]
>
>与Marketo电子邮件中的其他链接不同， [作为网页查看](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) 不会作为电子邮件点击进行跟踪。

当某人：

* 单击 [Marketo电子邮件中的链接](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).
* 填写Marketo [表单](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md).
* 使用Marketo [SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md) 或 [蒙奇金](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) 用于将匿名人员与已知记录关联的API（面向开发人员）。

数据库中的一个名称可能与许多Cookie关联，因为用户通常使用不同的设备和浏览器访问您的网站。

>[!NOTE]
>
>当匿名记录合并到新的或现有的人员记录中时，自定义字段值将 **not** 转移。
