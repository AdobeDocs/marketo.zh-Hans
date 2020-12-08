---
unique-page-id: 1146999
description: 有趣时刻的令牌——营销文档——产品文档
title: 有趣时刻的令牌
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 0%

---


# 有趣时刻的令牌 {#tokens-for-interesting-moments}

>[!NOTE]
>
>**先决条件**
>
>* 学习如何使用 [有趣的时刻流步骤](../../../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md)。
>* 进一步了 [解令牌](http://docs.marketo.com/display/docs/tokens)。

>



## 可用令牌 {#available-tokens}

查看 [令牌概述](../../../../../../product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) ，查看您可以放入一个有趣时刻的所有令牌。

## 触发令牌 {#trigger-tokens}

根据在智能活动中使用的触发器，还提供其他触发令牌。

* `{{trigger.Trigger Name}}` 这总是实际的触发。 例如：单击电子邮件中的链接。
* `{{trigger.Name}}` 是触发活动的资产的名称。 例如：网页上的“点击链接”是URL本身、Salesforce触发器的主题等。
* 其他触发器基于约束可用，如下所示：

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th><br></th> 
   <th><code>{{trigger.Trigger Name}}</code></th> 
   <th><code>{{trigger.Name}}</code></th> 
   <th><code>{{trigger.Link}}</code></th> 
   <th><code>{{trigger.Subject}}</code></th> 
   <th><code>{{trigger.Category}}</code></th> 
   <th><code>{{trigger.Details}}</code></th> 
   <th><code>{{trigger.Web Page}}</code></th> 
   <th><code>{{trigger.Client IP Address}}</code></th> 
   <th><code>{{trigger.Sent By}}</code></th> 
   <th><code>{{trigger.Received By}}</code></th> 
  </tr> 
  <tr> 
   <td>单击电子邮件中的链接</td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>电子邮件弹出很硬</td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>电子邮件弹回软</td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>电子邮件已发送</td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>打开电子邮件</td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>取消订阅电子邮件</td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><br></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>单击销售电子邮件中的链接</td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>已发送销售电子邮件</td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>打开销售电子邮件</td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>收到销售电子邮件</td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
  </tr> 
  <tr> 
   <td colspan="1">销售电子邮件退回</td> 
   <td colspan="1"><img src="assets/check.svg" alt="（勾号）"></td> 
   <td colspan="1"><img src="assets/check.svg" alt="（勾号）"></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
  </tr> 
  <tr> 
   <td>填写表单</td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><img src="assets/check.svg" alt="（勾号）"></td> 
   <td><br></td> 
   <td><p><br></p></td> 
  </tr> 
  <tr> 
   <td colspan="1">访问网页*</td> 
   <td colspan="1"><img src="assets/check.svg" alt="（勾号）"></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><img src="assets/check.svg" alt="（勾号）"></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>如果它没有勾号（勾号） ![](assets/check.svg) ，它会在有趣的时刻返回一个空字符串（无）。

*触发访 **问网页中** ，还有几个令牌：

* `{{trigger.Referrer}}`
* `{{trigger.Search Engine}}`
* `{{trigger.Search Query}}`

>[!TIP]
>
>总是测试有趣的时刻，确保它们以您期望的方式呈现。
>
>另外，请确保销售人员对它感兴趣，而不仅仅是您。 ![（眨眼）](assets/wink.svg)>

