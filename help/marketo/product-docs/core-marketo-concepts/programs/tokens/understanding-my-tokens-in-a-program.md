---
unique-page-id: 1147114
description: 了解项目中的我的令牌 — Marketo文档 — 产品文档
title: 了解程序中的我的令牌
exl-id: 01b42272-c419-4cd5-ad30-87413ceb2032
feature: Tokens
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 1%

---

# 了解程序中的我的令牌 {#understanding-my-tokens-in-a-program}

令牌是一个变量，您可以在电子邮件、登陆页面和智能营销活动中使用它来简化您的工作。

除了“我的令牌”之外，您还可以使用程序中的任何内置令牌。 查看 [令牌概述](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md).

## 我的令牌  {#my-tokens}

我的令牌是任何人都可以创建的自定义变量。 它们是 [已创建](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md) 在campaign文件夹或程序中。

我的令牌的显示方式如下： `{{my.Name Of Token}}`

示例:

* `{{my.Event Date}}`
* `{{my.Webinar Speaker}}`

<table> 
 <thead> 
  <tr> 
   <th>令牌类型</th> 
   <th>描述</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>日历文件 <img alt="—" src="assets/image2014-9-25-16-3a44-3a19.png" data-linked-resource-id="3083230" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>使用此令牌可以 <a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">添加日历事件文件(.i</a><a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">cs)</a> 到您的电子邮件和登陆页面。</td> 
  </tr> 
  <tr> 
   <td><p>日期 <img alt="--" src="assets/image2014-9-25-16-3a44-3a47.png" data-linked-resource-id="3083231" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></p></td> 
   <td>此令牌包含日期值。 日期显示为年 — 月 — 日（例如，2016-05-23）。</td> 
  </tr> 
  <tr> 
   <td>电子邮件脚本 <img alt="--" src="assets/image2014-9-25-16-3a45-3a4.png" data-linked-resource-id="3083232" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>使用此令牌可在您的电子邮件中执行Velocity脚本。 了解详情 <a href="https://developers.marketo.com/documentation/email-scripting/" title="关注链接" rel="nofollow">此处</a>. </td> 
  </tr> 
  <tr> 
   <td>数字<span> <img alt="--" src="assets/image2014-9-25-16-3a45-3a25.png" data-linked-resource-id="3083233" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></span></td> 
   <td>任意整数。 甚至可能是负数。</td> 
  </tr> 
  <tr> 
   <td>富文本 <img alt="--" src="assets/image2014-9-25-16-3a46-3a22.png" data-linked-resource-id="3083234" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>这是HTML。 在电子邮件和登陆页面中使用它。</td> 
  </tr> 
  <tr> 
   <td>得分 <img alt="--" src="assets/image2014-9-25-16-3a46-3a39.png" data-linked-resource-id="3083235" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>在中使用此令牌 <a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md">更改得分流程步骤</a>. </td> 
  </tr> 
  <tr> 
   <td colspan="1">SFDC营销活动 <img alt="--" src="assets/sfdc-campaign-icon.jpg" data-linked-resource-id="11379761" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114" title="--"></td> 
   <td colspan="1">使用此令牌可允许将成为Marketo项目一部分的潜在客户也添加到添加的任何其他SFDC Campaign中。</td> 
  </tr> 
  <tr> 
   <td>文本 <img alt="--" src="assets/image2014-9-25-16-3a46-3a54.png" data-linked-resource-id="3083236" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>只是一些文字。 在HTML过度使用时使用它。 文本令牌的大小限制为524,288个字符(UTF-8)或2 MB。</td> 
  </tr> 
 </tbody> 
</table>

>[!CAUTION]
>
>在Microsoft Dynamics或Salesforce上从Sales Insight发送电子邮件时，无法解析我的令牌；仅填充标准令牌（潜在客户、公司等）。 令牌的默认值 _将_ 但工作。

## 嵌套令牌 {#nesting-tokens}

创建新令牌时，树中的其他对象可以引用该令牌。 有一个创建令牌的命名结构，以便轻松管理。

* **本地令牌：** 令牌直接在该程序或文件夹中创建。
* **继承的令牌：** 令牌是在树上更高级别的程序或文件夹中的某个位置创建的。
* **被覆盖的令牌：** 令牌已被继承，然后有人在此程序或文件夹中生成异常。

您可以生成全局变量，然后在树中的较低级别覆盖它们。

移动程序和文件夹也会影响令牌。 请务必检查以确保在移动过程中参照不会断开。

>[!NOTE]
>
>如果您从参与计划发送的电子邮件是默认计划的子电子邮件（不是参与计划的本地项目），则电子邮件中使用的任何“我的令牌”都是从子电子邮件所在的默认计划解析的。

>[!MORELIKETHIS]
>
>* [令牌概述](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md)
>* [管理我的令牌](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)
