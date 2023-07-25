---
unique-page-id: 2360181
description: 跟踪匿名活动和人员 — Marketo文档 — 产品文档
title: 跟踪匿名活动和人员
exl-id: 95a39e57-4636-4bae-8ca8-00cb43cb566c
feature: Reporting
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 0%

---

# 跟踪匿名活动和人员 {#tracking-anonymous-activity-and-people}

首次访问Marketo时 [登陆页面](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) (或您的网站上具有 [Munchkin跟踪代码](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md))，Marketo会创建 _匿名活动_ 并使用浏览器Cookie对其进行跟踪。 在识别访客后，访客即会变成用户，并且与浏览器Cookie关联的历史记录会合并到中。

1. 当有以下人员时，将创建匿名活动：

   * 访问您的Marketo [登陆页面](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) 第一次。
   * 访问网站上具有 [Munchkin跟踪](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
   * 单击 [以网页查看](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) Marketo电子邮件的链接。

   >[!NOTE]
   >
   >与Marketo电子邮件中的其他链接不同，作为网页查看不会被跟踪为电子邮件点击。

   当某人出现以下情况时，匿名活动会合并到新人员或现有人员中：

   * 单击 [Marketo电子邮件中的链接](/help/marketo/product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md).
   * 填写Marketo [表单](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md).
   * 使用Marketo的 [REST API](https://developers.marketo.com/rest-api/lead-database/leads/) 或 [Munchkin](https://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/) 用于将匿名活动与已知记录关联的API（适用于开发人员）。

   数据库中的某个名称可能与许多Cookie相关联，因为人们通常使用不同的设备和浏览器访问您的网站。

   >[!NOTE]
   >
   >将匿名记录合并到新的或现有的人员记录中时，自定义字段值将 **非** 转接。

   >[!MORELIKETHIS]
   >
   >[在Web报表中显示人员或匿名访客](/help/marketo/product-docs/reporting/basic-reporting/report-activity/display-people-or-anonymous-visitors-in-web-reports.md)
