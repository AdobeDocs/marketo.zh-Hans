---
unique-page-id: 1147114
description: 了解项目中的令牌 — Marketo Docs — 产品文档
title: 了解我的令牌在项目
exl-id: 01b42272-c419-4cd5-ad30-87413ceb2032
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# 了解项目{#understanding-my-tokens-in-a-program}中的令牌

令牌是一个变量，您可以在电子邮件、登陆页和智能活动中使用它，使您的生活更轻松。

除了“我的令牌”之外，您还可以在项目中使用任何内置令牌。 请查看[令牌概述](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md)。

## 我的令牌{#my-tokens}

我的令牌是任何人都可以创建的自定义变量。 它们在活动文件夹或项目中创建[。](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)

我的令牌显示如下：`{{my.Name Of Token}}`

示例：

* `{{my.Event Date}}`
* `{{my.Webinar Speaker}}`

<table> 
 <thead> 
  <tr> 
   <th>令牌类型</th> 
   <th>说明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>日历文件 <img alt="—" src="assets/image2014-9-25-16-3a44-3a19.png" data-linked-resource-id="3083230" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>使用此令牌<a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">向您的电子邮件和登陆页中添加日历事件文件(.i</a><a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">cs)</a>。</td> 
  </tr> 
  <tr> 
   <td><p>日期 <img alt="—" src="assets/image2014-9-25-16-3a44-3a47.png" data-linked-resource-id="3083231" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></p></td> 
   <td>此令牌包含日期值。 日期显示为年月日(例如，2016-05-23)。</td> 
  </tr> 
  <tr> 
   <td>电子邮件脚本 <img alt="—" src="assets/image2014-9-25-16-3a45-3a4.png" data-linked-resource-id="3083232" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>使用此令牌在您的电子邮件中执行Velocity脚本。 了解更多<a href="https://developers.marketo.com/documentation/email-scripting/" title="跟踪链接" rel="nofollow">此处</a>。 </td> 
  </tr> 
  <tr> 
   <td>编号<span> <img alt="—" src="assets/image2014-9-25-16-3a45-3a25.png" data-linked-resource-id="3083233" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></span></td> 
   <td>任何整数。 甚至可能是负面的。</td> 
  </tr> 
  <tr> 
   <td>富文本 <img alt="—" src="assets/image2014-9-25-16-3a46-3a22.png" data-linked-resource-id="3083234" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>这是HTML。 在电子邮件和登陆页中使用。</td> 
  </tr> 
  <tr> 
   <td>得分 <img alt="—" src="assets/image2014-9-25-16-3a46-3a39.png" data-linked-resource-id="3083235" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>在<a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md">更改得分流步骤</a>中使用此令牌。 </td> 
  </tr> 
  <tr> 
   <td colspan="1">SFDC活动 <img alt="—" src="assets/sfdc-campaign-icon.jpg" data-linked-resource-id="11379761" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114" title="—"></td> 
   <td colspan="1">使用此令牌可允许将成为Marketo项目一部分的潜在客户也添加到添加的任何SFDC活动。</td> 
  </tr> 
  <tr> 
   <td>文本 <img alt="—" src="assets/image2014-9-25-16-3a46-3a54.png" data-linked-resource-id="3083236" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>只是一些短信。 在HTML过度激活时使用它。 文本令牌的大小限制为524,288个字符(UTF-8)或2 MB。</td> 
  </tr> 
 </tbody> 
</table>

>[!CAUTION]
>
>在Microsoft Dynamics或Salesforce上从Sales Insight发送电子邮件时，我的令牌将无法解析；只有标准令牌才会填充(潜在客户、公司等)。 但是，令牌&#x200B;_的默认值将_&#x200B;有效。

## 嵌套令牌{#nesting-tokens}

创建新标记时，树中的其他对象可以引用该标记。 有一种命名结构，用于创建令牌以便于管理。

* **本地令牌：** 该令牌是在该项目或文件夹中创建的。
* **继承的令** 牌：令牌是在树中某个较高级别项目或文件夹中创建的。
* **被覆盖的** 令牌：该令牌被继承，然后有人在此项目或文件夹中发生异常。

您可以生成全局变量，然后在树中的较低级别覆盖它们。

移动项目和文件夹也会影响令牌。 始终检查以确保在移动过程中不会损坏引用。

>[!NOTE]
>
>如果您从参与项目发送的电子邮件是默认项目的子电子邮件(不是您的参与项目的本地电子邮件)，则电子邮件中使用的任何“我的令牌”都将从子电子邮件所在的默认项目解析。

>[!MORELIKETHIS]
>
>* [令牌概述](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md)
>* [管理我的令牌](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)

