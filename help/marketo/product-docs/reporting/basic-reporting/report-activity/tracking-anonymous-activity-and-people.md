---
unique-page-id: 2360181
description: 跟踪匿名活动和人员- Marketo Docs —— 产品文档
title: 跟踪匿名活动和人员
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---


# 跟踪匿名活动和人员{#tracking-anonymous-activity-and-people}

第一次有人访问Marketo [登陆页](../../../../product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md)（或您网站上具有[Munchkin跟踪代码](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)的页面）时，Marketo会创建&#x200B;*匿名* *活动*&#x200B;并使用浏览器cookie跟踪它。 一旦识别访客，它就变成人，与浏览器cookie关联的历史记录将被合并。

1. 当某人：

   * 首次访问您的登陆页[。](../../../../product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md)
   * 访问您网站上具有[Munchkin跟踪](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)的页面。
   * 单击Marketo电子邮件中的[视图作为Web页](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)链接。

   >[!NOTE]
   >
   >与Marketo电子邮件中的其他链接不同，视图作为网页不会作为电子邮件单击进行跟踪。

   当某人：

   * 单击Marketo电子邮件](../../../../product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md)中的[链接。
   * 填写[表单](http://docs.marketo.com/display/docs/forms)的标记。
   * 使用Marketo的[REST API](http://developers.marketo.com/rest-api/lead-database/leads/)或[Munchkin](http://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/) API（对于开发人员）将匿名活动与已知记录相关联。

   数据库中的一个名称可能与许多cookies关联，因为人们经常使用不同的设备和浏览器访问您的站点。

   >[!NOTE]
   >
   >当匿名记录合并到新记录或现有人员记录中时，自定义字段值将&#x200B;**不**&#x200B;转移。

   >[!NOTE]
   >
   >**相关文章**
   >
   >    
   >    
   >    * [在Web报告中显示人物或匿名访客](display-people-or-anonymous-visitors-in-web-reports.md)


   >[!NOTE]
   >
   >**深潜**
   >
   >
   >进一步了解[基本报告](http://docs.marketo.com/display/docs/basic+reporting)。

