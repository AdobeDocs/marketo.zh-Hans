---
unique-page-id: 2360181
description: 跟踪匿名活动和人员 — Marketo文档 — 产品文档
title: 跟踪匿名活动和人员
exl-id: 95a39e57-4636-4bae-8ca8-00cb43cb566c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 0%

---

# 跟踪匿名活动和人员 {#tracking-anonymous-activity-and-people}

第一次有人访问Marketo [登陆页面](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) (或您网站上具有 [Munchkin跟踪代码](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)),Marketo将创建 _匿名活动_ 并使用浏览器Cookie进行跟踪。 识别访客后，该访客将成为人员，并且与浏览器Cookie关联的历史记录会合并到中。

1. 当某人：

   * 访问Marketo [登陆页面](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) 第一次。
   * 访问您网站上具有 [蒙奇金跟踪](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
   * 单击 [作为网页查看](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) 链接。

   >[!NOTE]
   >
   >与Marketo电子邮件中的其他链接不同，“查看为网页”不会作为电子邮件点击进行跟踪。

   当某人：

   * 单击 [Marketo电子邮件中的链接](/help/marketo/product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md).
   * 填写Marketo [表单](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md).
   * 使用Marketo [REST API](https://developers.marketo.com/rest-api/lead-database/leads/) 或 [蒙奇金](https://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/) 用于将匿名活动与已知记录关联的API（面向开发人员）。

   数据库中的一个名称可能与许多Cookie关联，因为用户通常使用不同的设备和浏览器访问您的网站。

   >[!NOTE]
   >
   >当匿名记录合并到新的或现有的人员记录中时，自定义字段值将 **not** 转移。

   >[!MORELIKETHIS]
   >
   >[在Web报表中显示人员或匿名访客](/help/marketo/product-docs/reporting/basic-reporting/report-activity/display-people-or-anonymous-visitors-in-web-reports.md)
