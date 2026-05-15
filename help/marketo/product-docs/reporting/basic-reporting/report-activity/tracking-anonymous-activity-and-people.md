---
unique-page-id: 2360181
description: 了解如何在Marketo Engage中跟踪匿名活动和人员，包括跟踪匿名活动和。 使用本指南完成您的下一步。
title: 跟踪匿名活动和人员
exl-id: 95a39e57-4636-4bae-8ca8-00cb43cb566c
feature: Reporting
TQID: https://experienceleague.adobe.com/BZakQFVtQystRyrlzo81s-p8N65LXHUJ2ZoSAzeTG6Q
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 255
ht-degree: 8%

---

# 跟踪匿名活动和人员 {#tracking-anonymous-activity-and-people}

首次访问Marketo [登陆页面](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md)（或网站上具有[Munchkin跟踪代码](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)的页面）时，Marketo会创建一个&#x200B;_匿名活动_&#x200B;并使用浏览器Cookie对其进行跟踪。 在识别访客后，访客会变成用户，并且与浏览器Cookie关联的历史记录将合并到中。

1. 当有人出现以下情况时，将创建匿名活动：

   * 首次访问您的Marketo [登陆页面](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md)。
   * 访问网站上具有[Munchkin跟踪](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)的页面。
   * 单击Marketo电子邮件中的[以网页形式查看](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)链接。

   >[!NOTE]
   >
   >与Marketo电子邮件中的其他链接不同，以网页形式查看不会以电子邮件点击形式进行跟踪。

   当某人出现以下情况时，匿名活动会合并到新人员或现有人员中：

   * 单击Marketo电子邮件[&#128279;](/help/marketo/product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md)中的链接。
   * 填写Marketo [表单](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md)。
   * 使用Marketo的[REST API](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/rest/lead-database/leads)或[Munchkin](https://experienceleague.adobe.com/zh-hans/docs/marketo-developer/marketo/javascriptapi/leadtracking/lead-tracking) API（适用于开发人员）将匿名活动与已知记录相关联。

   数据库中的某个名称可能与许多Cookie相关联，因为人们通常使用不同的设备和浏览器访问您的网站。

   >[!NOTE]
   >
   >将匿名记录合并到新的或现有的人员记录中时，自定义字段值将&#x200B;**不会**&#x200B;转移。

   >[!MORELIKETHIS]
   >
   >[在Web报告中显示联系人或匿名访客](/help/marketo/product-docs/reporting/basic-reporting/report-activity/display-people-or-anonymous-visitors-in-web-reports.md)
