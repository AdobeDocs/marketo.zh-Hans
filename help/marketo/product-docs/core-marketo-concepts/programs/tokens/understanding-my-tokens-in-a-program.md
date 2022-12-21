---
unique-page-id: 1147114
description: 了解项目中的令牌 — Marketo文档 — 产品文档
title: 了解项目中的令牌
exl-id: 01b42272-c419-4cd5-ad30-87413ceb2032
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 1%

---

# 了解项目中的令牌 {#understanding-my-tokens-in-a-program}

令牌是一个变量，您可以在电子邮件、登陆页面和智能营销活动中使用，从而让您的生活更轻松。

除了我的令牌之外，您还可以在程序中使用任何内置令牌。 查看 [令牌概述](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md).

## 我的令牌  {#my-tokens}

我的令牌是任何人都可以创建的自定义变量。 是 [已创建](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md) 在campaign文件夹或项目群中。

我的令牌显示如下： `{{my.Name Of Token}}`

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
   <td>使用此令牌可 <a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">添加日历事件文件(.i</a><a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">cs)</a> 到您的电子邮件和登陆页面。</td> 
  </tr> 
  <tr> 
   <td><p>日期 <img alt="--" src="assets/image2014-9-25-16-3a44-3a47.png" data-linked-resource-id="3083231" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></p></td> 
   <td>此令牌包含日期值。 日期显示为年月日(例如，2016-05-23)。</td> 
  </tr> 
  <tr> 
   <td>电子邮件脚本 <img alt="--" src="assets/image2014-9-25-16-3a45-3a4.png" data-linked-resource-id="3083232" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>使用此令牌在电子邮件中执行Velocity脚本。 了解更多 <a href="https://developers.marketo.com/documentation/email-scripting/" title="关注链接" rel="nofollow">此处</a>. </td> 
  </tr> 
  <tr> 
   <td>数字<span> <img alt="--" src="assets/image2014-9-25-16-3a45-3a25.png" data-linked-resource-id="3083233" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></span></td> 
   <td>任意整数。 甚至可能是负面的。</td> 
  </tr> 
  <tr> 
   <td>富文本 <img alt="--" src="assets/image2014-9-25-16-3a46-3a22.png" data-linked-resource-id="3083234" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>这是HTML。 在电子邮件和登陆页面中使用。</td> 
  </tr> 
  <tr> 
   <td>得分 <img alt="--" src="assets/image2014-9-25-16-3a46-3a39.png" data-linked-resource-id="3083235" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>在 <a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md">更改分数流步骤</a>. </td> 
  </tr> 
  <tr> 
   <td colspan="1">SFDC营销活动 <img alt="--" src="assets/sfdc-campaign-icon.jpg" data-linked-resource-id="11379761" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114" title="--"></td> 
   <td colspan="1">使用此令牌可允许成为Marketo计划一部分的潜在客户也添加到要添加的任何SFDC促销活动中。</td> 
  </tr> 
  <tr> 
   <td>文本 <img alt="--" src="assets/image2014-9-25-16-3a46-3a54.png" data-linked-resource-id="3083236" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>只是一些短信。 当HTML超量终止时使用。 文本令牌的大小限制为524,288个字符(UTF-8)或2 MB。</td> 
  </tr> 
 </tbody> 
</table>

>[!CAUTION]
>
>在Microsoft Dynamics或Salesforce上从Sales Insight发送电子邮件时，我的令牌将无法解析；只会填充标准令牌（潜在客户、公司等）。 令牌的默认值 _will_ 但是，工作。

## 嵌套令牌 {#nesting-tokens}

创建新令牌后，树中的其他对象可以引用该令牌。 有一个用于创建令牌以便于管理的命名结构。

* **本地令牌：** 令牌是在该程序或文件夹中直接创建的。
* **继承令牌：** 令牌是在树中较高级别的程序或文件夹中的某个位置创建的。
* **已覆盖的令牌：** 令牌已继承，然后有人在此程序或文件夹中发生异常。

您可以创建全局变量，然后在树中的较低级别覆盖它们。

移动程序和文件夹也会影响令牌。 请始终检查以确保在移动过程中引用不会损坏。

>[!NOTE]
>
>如果您从参与计划发送的电子邮件是默认计划的子电子邮件（不是您的参与计划的本地电子邮件），则电子邮件中使用的任何“我的令牌”都将从子电子邮件所在的默认计划中解析。

>[!MORELIKETHIS]
>
>* [令牌概述](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md)
>* [管理我的令牌](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)

