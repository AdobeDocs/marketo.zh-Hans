---
unique-page-id: 2360181
description: 跟踪匿名活动和人员 — Marketo文档 — 产品文档
title: 跟踪匿名活动和人员
exl-id: 95a39e57-4636-4bae-8ca8-00cb43cb566c
feature: Reporting
source-git-commit: e3f61755dccd9bea1378a429fc428b440fc3ecb4
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# 跟踪匿名活动和人员 {#tracking-anonymous-activity-and-people}

首次访问Marketo [登陆页面](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md)(或网站上具有[Munchkin跟踪代码](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)的页面)时，Marketo会创建一个&#x200B;_匿名活动_&#x200B;并使用浏览器Cookie对其进行跟踪。 在识别访客后，访客会变成用户，并且与浏览器Cookie关联的历史记录将合并到中。

1. 当有人出现以下情况时，将创建匿名活动：

   * 首次访问您的Marketo [登陆页面](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md)。
   * 访问网站上具有[Munchkin跟踪](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)的页面。
   * 单击Marketo电子邮件中的[以网页形式查看](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)链接。

   >[!NOTE]
   >
   >与Marketo电子邮件中的其他链接不同，以网页形式查看不会以电子邮件点击形式进行跟踪。

   当某人出现以下情况时，匿名活动会合并到新人员或现有人员中：

   * 单击Marketo电子邮件](/help/marketo/product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md)中的[链接。
   * 填写Marketo [表单](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md)。
   * 使用Marketo的[REST API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/leads)或[Munchkin](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/leadtracking/lead-tracking) API（适用于开发人员）将匿名活动与已知记录相关联。

   数据库中的某个名称可能与许多Cookie相关联，因为人们通常使用不同的设备和浏览器访问您的网站。

   >[!NOTE]
   >
   >将匿名记录合并到新的或现有的人员记录中时，自定义字段值将&#x200B;**不会**&#x200B;转移。

   >[!MORELIKETHIS]
   >
   >[在Web报告中显示联系人或匿名访客](/help/marketo/product-docs/reporting/basic-reporting/report-activity/display-people-or-anonymous-visitors-in-web-reports.md)
