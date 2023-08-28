---
description: 操作评分行为 — Marketo文档 — 产品文档
title: 操作评分行为
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: 0f71600b18315feb3ef32e95dfb108b09c4cb79f
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 11%

---

# 操作评分行为 {#op-scoring-behavior}

此示例是使用Marketo Engage默认程序的行为评分的高级（标记化）操作程序。 在项目的“我的令牌”选项卡下查看和编辑评分值。 需要名为“行为得分”的自定义得分字段。

如需进一步的战略帮助或自定义计划，请联系Adobe客户团队或访问 [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"} 页面。

## 渠道摘要 {#channel-summary}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>渠道</th> 
   <th>成员资格状态</th>
   <th>Analytics行为</th>
   <th>项目类型</th>
  </tr> 
  <tr> 
   <td>可操作</td> 
   <td>01个成员</td>
   <td>可操作</td>
   <td>默认</td>
  </tr>
 </tbody> 
</table>

## 先决条件字段 {#prerequisite-fields}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>类型</th> 
   <th>友好名称</th>
   <th>API名称</th>
  </tr>
  <tr> 
   <td>得分</td> 
   <td>行为得分</td>
   <td>行为得分</td>
  </tr>
 </tbody> 
</table>

## 程序包含以下资产 {#program-contains-the-following-assets}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>类型</th> 
   <th>模板名称</th>
   <th>资源名称</th>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>电子邮件 — 单击电子邮件中的链接</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>表单 — 填写联系人表单</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>表单 — 填写内容表单</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>表单 — 填写默认表单</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>表单 — 填写事件表单</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>Web — 下载任何PDF</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>Web - PPC评分</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>Web — 访问关键网页</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>Web — 在1天内访问多个网页</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>现场活动 — 已参加</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>贸易展 — 受影响</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>贸易展 — 参观展位</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>网络研讨会 — 已参加</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>降低得分 — 无活动</td>
  </tr>
  <tr> 
   <td>Smart Campaign</td> 
   <td> </td>
   <td>降低得分 — 访问不受欢迎的网页</td>
  </tr>
  <tr> 
   <td>文件夹</td> 
   <td> </td>
   <td>交互</td>
  </tr>
  <tr> 
   <td>文件夹</td> 
   <td> </td>
   <td>项目状态更改</td>
  </tr>
  <tr> 
   <td>文件夹</td> 
   <td> </td>
   <td>得分衰减</td>
  </tr>
 </tbody> 
</table>

程序屏幕截图

## 我的令牌已包含 {#my-tokens-included}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>令牌类型</th> 
   <th>令牌名称</th>
   <th>值</th>
  </tr>
  <tr> 
   <td>得分</td> 
   <td><code>{{my.Decrease Score - No Activity}}</code></td>
   <td>-10</td>
  </tr>
  <tr> 
   <td>得分</td> 
   <td><code>{{my.Decrease Score - Visits Undesirable Web Pages}}</code></td>
   <td>-5</td>
  </tr>
  <tr> 
   <td>得分</td> 
   <td><code>{{my.Email - Clicks Link}}</code></td>
   <td>+2</td>
  </tr>
   <tr> 
   <td>得分</td> 
   <td><code>{{my.Form - Fills Out Contact Form}}</code></td>
   <td>+30</td>
  </tr>
  <tr> 
   <td>得分</td> 
   <td><code>{{my.Form - Fills Out Content Form}}</code></td>
   <td>+15</td>
  </tr>
  <tr> 
   <td>得分</td> 
   <td><code>{{my.Form - Fills Out Default Form}}</code></td>
   <td>+10</td>
  </tr>
   <tr> 
   <td>得分</td> 
   <td><code>{{my.Form - Fills-out Event Form}}</code></td>
   <td>+15</td>
  </tr>
  <tr> 
   <td>得分</td> 
   <td><code>{{my.Live Event - Attended}}</code></td>
   <td>+30</td>
  </tr>
   <tr> 
   <td>得分</td> 
   <td><code>{{my.Tradeshow - Influenced}}</code></td>
   <td>+20</td>
  </tr>
  <tr> 
   <td>得分</td> 
   <td><code>{{my.Tradeshow - Visited Booth}}</code></td>
   <td>+5</td>
  </tr>
  <tr> 
   <td>得分</td> 
   <td><code>{{my.Web - Downloaded Any PDF}}</code></td>
   <td>+5</td>
  </tr>
  <tr> 
   <td>得分</td> 
   <td><code>{{my.Web - PPC Scoring}}</code></td>
   <td>+15</td>
  </tr>
   <tr> 
   <td>得分</td> 
   <td><code>{{my.Web - Visits Key Web Pages}}</code></td>
   <td>+5</td>
  </tr>
  <tr> 
   <td>得分</td> 
   <td><code>{{my.Web - Visits Multiple Web Pages in 1 Day}}</code></td>
   <td>+5</td>
  </tr>
  <tr> 
   <td>得分</td> 
   <td><code>{{my.Webinar - Attended}}</code></td>
   <td>+20</td>
  </tr>
 </tbody> 
</table>

## 冲突规则 {#conflict-rules}

* **项目标记**
   * 在此订阅中创建标记 —  _推荐_
   * 忽略

* **同名登陆页面模板**
   * 复制原始模板 —  _推荐_
   * 使用目标模板

* **具有相同名称的图像**
   * 保留两个文件 —  _推荐_
   * 替换此订阅中的项目

* **同名电子邮件模板**
   * 保留两个模板 —  _推荐_
   * 替换现有模板

冲突规则屏幕截图

## 最佳实践 {#best-practices}

* 构建的每个营销活动都是以最佳实践构建为例，而不是特定于您的用例。 请记住更新智能营销活动以解决您的特定棘手问题和数据挑战。

* 请考虑更新此程序示例的命名约定，以符合您的命名约定。
