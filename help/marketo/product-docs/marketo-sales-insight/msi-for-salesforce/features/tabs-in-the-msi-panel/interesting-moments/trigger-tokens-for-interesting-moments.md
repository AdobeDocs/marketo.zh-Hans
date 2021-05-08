---
unique-page-id: 1146999
description: 为有趣的时刻触发令牌 — Marketo Docs — 产品文档
title: 触发有趣的瞬间的令牌
exl-id: 666a6eed-c432-4088-b4f1-54c996eca64c
translation-type: tm+mt
source-git-commit: f4c773ca76542827a498940f44b018ddb71816d6
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---

# 触发有趣时刻的令牌{#trigger-tokens-for-interesting-moments}

>[!PREREQUISITES]
>
>了解如何使用[有趣的力矩流步骤](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md)。

## 可用令牌{#available-tokens}

请访问[令牌概述](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md)，查看可放置到有趣时刻的所有令牌。

## 触发器令牌{#trigger-tokens}

根据在智能活动中使用的触发器，将提供其他触发器令牌。

* `{{trigger.Trigger Name}}` 这总是实际的触发。例如：单击电子邮件中的链接。
* `{{trigger.Name}}` 是触发活动的资产的名称。例如：网页上的点击链接是URL本身，是Salesforce触发器的主题，等等。
* 其他触发器基于约束可用，如下所列。

**电子邮件触发器**

<table style="table-layout:auto"> 
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
   <th><code>{{trigger.Referrer}}</code></th>
   <th><code>{{trigger.Search Engine}}</code></th>
   <th><code>{{trigger.Search Query}}</code></th>
   <th><code>{{trigger.Browser}}</code></th>
  </tr> 
  <tr> 
   <td>单击电子邮件中的链接</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>电子邮件已硬弹回</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>电子邮件弹回软</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>电子邮件已送达</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>打开电子邮件</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
    <tr> 
   <td>已转发给朋友的电子邮件</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
    <tr> 
   <td>已转发至朋友电子邮件</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="检查"></td>
  </tr> 
  <tr> 
   <td>取消订阅电子邮件</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
 </tbody> 
</table>

**Salesforce触发器**

<table style="table-layout:auto"> 
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
   <th><code>{{trigger.Referrer}}</code></th>
   <th><code>{{trigger.Search Engine}}</code></th>
   <th><code>{{trigger.Search Query}}</code></th>
   <th><code>{{trigger.Browser}}</code></th>
  </tr> 
  <tr> 
   <td>销售电子邮件中的点击链接</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>已发送销售电子邮件</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>打开销售电子邮件</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>销售电子邮件退回</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>收到销售电子邮件</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
    <tr> 
   <td>已更新业务机会</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
    <tr> 
   <td>所有者更改</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>人员已转换</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>从SFDC删除人员</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>人员已同步到SFDC</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>从Opportunity中删除</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>已从SFDC活动中删除</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>活动已记录</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>活动已更新</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>添加到Opportunity</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>添加到SFDC活动</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>状态在SFDC活动中更改</td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
 </tbody> 
</table>

**Sales Connect触发器**

<table style="table-layout:auto"> 
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
   <th><code>{{trigger.Referrer}}</code></th>
   <th><code>{{trigger.Search Engine}}</code></th>
   <th><code>{{trigger.Search Query}}</code></th>
   <th><code>{{trigger.Browser}}</code></th>
  </tr> 
  <tr> 
   <td>销售电子邮件中的点击链接</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>已发送销售电子邮件</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>打开销售电子邮件</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>销售电子邮件退回</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>收到销售电子邮件</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>添加到销售活动</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr>
   <td>所有者更改</td> 
   <td>已从销售活动中删除</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>已收到销售电话</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
 </tbody> 
</table>

**杂项**

<table style="table-layout:auto"> 
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
   <th><code>{{trigger.Referrer}}</code></th>
   <th><code>{{trigger.Search Engine}}</code></th>
   <th><code>{{trigger.Search Query}}</code></th>
   <th><code>{{trigger.Browser}}</code></th>
  </tr> 
  <tr> 
   <td>填写表单</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>访问网页</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>单击网页上的链接</td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="检查"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>如果它没有检查![(tick)](assets/check.png)，那么在有趣的时刻它将返回空字符串（无）。

*触发器&#x200B;**访问网页**&#x200B;还有一些额外的令牌：

* `{{trigger.Referrer}}`
* `{{trigger.Search Engine}}`
* `{{trigger.Search Query}}`

>[!TIP]
>
>总是测试您的有趣时刻，确保它们以您期望的方式呈现。
>
>另外，请确保销售人员感兴趣，而不仅仅是您！
