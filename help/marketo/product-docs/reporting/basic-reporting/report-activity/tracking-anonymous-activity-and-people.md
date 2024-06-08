---
unique-page-id: 2360181
description: 跟踪匿名活动和人员 — Marketo文档 — 产品文档
title: 跟踪匿名活动和人员
exl-id: 95a39e57-4636-4bae-8ca8-00cb43cb566c
feature: Reporting
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# 跟踪匿名活动和人员 {#tracking-anonymous-activity-and-people}

首次访问Marketo时 [登陆页面](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) (或您的网站上具有 [Munchkin跟踪代码](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md))，Marketo将创建 _匿名活动_ 并使用浏览器Cookie对其进行跟踪。 在识别访客后，访客会变成用户，并且与浏览器Cookie关联的历史记录将合并到中。

1. 当有人出现以下情况时，将创建匿名活动：

   * 访问您的Marketo [登陆页面](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) 第一次。
   * 访问网站上具有 [Munchkin跟踪](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
   * 单击 [以网页形式查看](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) Marketo电子邮件中的链接。

   >[!NOTE]
   >
   >与Marketo电子邮件中的其他链接不同，以网页形式查看不会以电子邮件点击形式进行跟踪。

   当某人出现以下情况时，匿名活动会合并到新人员或现有人员中：

   * 单击 [Marketo电子邮件中的链接](/help/marketo/product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md).
   * 填写Marketo [表单](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md).
   * 使用Marketo的 [REST API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/leads) 或 [蒙奇金](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/lead-tracking) 用于将匿名活动与已知记录关联的API（适用于开发人员）。

   数据库中的某个名称可能与许多Cookie相关联，因为人们通常使用不同的设备和浏览器访问您的网站。

   >[!NOTE]
   >
   >将匿名记录合并到新的或现有的人员记录时，自定义字段值将 **非** 转接。

   >[!MORELIKETHIS]
   >
   >[在Web报表中显示人员或匿名访客](/help/marketo/product-docs/reporting/basic-reporting/report-activity/display-people-or-anonymous-visitors-in-web-reports.md)
