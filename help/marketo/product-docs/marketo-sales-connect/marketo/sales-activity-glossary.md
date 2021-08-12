---
description: 销售活动术语表 — Marketo文档 — 产品文档
title: 销售活动术语表
hide: true
hidefromtoc: true
source-git-commit: 70f17106efe52ee742c8e31013e533fc36ce9835
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 3%

---

# 销售活动术语表 {#sales-activity-glossary}

在Sales Connect中，当卖家：向销售频率添加潜在客户、向他们发送电子邮件或致电活动，则该潜在客户将记录在Marketo活动历史记录下。 此外，当潜在客户参与电子邮件、打开次数、点击次数和回复时，也会被记录。

以下活动将从Sales Connect登录Marketo。

>[!NOTE]
>
>这些活动和属性可在我们的REST和批量API中使用。

## 活动 {#activities}

<table>
 <tr>
  <th>销售活动</th>
  <th>属性</th>
 </tr>
 <tr>
  <th rowspan="3">发送销售电子邮件</th>
  <td>发送者</td>
 </tr>
 <tr>
  <td>源</td>
 </tr>
 <tr>
  <td>模板ID</td>
 </tr>
 <tr>
  <th rowspan="3">打开销售电子邮件</th>
  <td>发送者</td>
 </tr>
 <tr>
  <td>源</td>
 </tr>
 <tr>
  <td>模板ID</td>
 </tr>
 <tr>
  <th rowspan="4">点击了销售电子邮件</th>
  <td>链接</td>
 </tr>
 <tr>
  <td>发送者</td>
 </tr>
 <tr>
  <td>源</td>
 </tr>
 <tr>
  <td>模板ID</td>
 </tr>
 <tr>
  <th rowspan="2">已收到销售电子邮件</th>
  <td>接收者</td>
 </tr>
 <tr>
  <td>源</td>
 </tr>
 <tr>
  <th rowspan="4">销售电子邮件退回</th>
  <td>详细信息</td>
 </tr>
 <tr>
  <td>模板ID</td>
 </tr>
 <tr>
  <td>电子邮件</td>
 </tr>
 <tr>
  <td>发送者</td>
 </tr>
 <tr>
  <th rowspan="7">已接到销售电话</th>
  <td>销售电话由</td>
 </tr>
 <tr>
  <td>销售电话状态</td>
 </tr>
 <tr>
  <td>销售呼叫主体</td>
 </tr>
 <tr>
  <td>销售活动名称</td>
 </tr>
 <tr>
  <td>销售活动URL</td>
 </tr>
 <tr>
  <td>已拨打销售电话号码</td>
 </tr>
 <tr>
  <td>源</td>
 </tr>
 <tr>
  <th rowspan="6">添加到Sales Campaign</th>
  <td>销售活动名称</td>
 </tr>
 <tr>
  <td>销售电话状态</td>
 </tr>
 <tr>
  <td>销售活动URL</td>
 </tr>
 <tr>
  <td>发送者</td>
 </tr>
 <tr>
  <td>源</td>
 </tr>
 <tr>
  <td>销售活动ID</td>
 </tr>
 <tr>
  <th rowspan="6">从Sales Campaign中删除</th>
  <td>销售活动名称</td>
 </tr>
 <tr>
  <td>销售电话状态</td>
 </tr>
 <tr>
  <td>销售活动URL</td>
 </tr>
 <tr>
  <td>发送者</td>
 </tr>
 <tr>
  <td>源</td>
 </tr>
 <tr>
  <td>销售活动ID</td>
 </tr>
</table>

## 描述 {#descriptions}

<table> 
 <tr>
  <th>属性</th>
  <th>描述</th>
 </tr>
 <tbody> 
  <tr> 
   <td><strong>发送者</strong></td>
   <td>发送电子邮件的人的电子邮件地址。</td> 
  </tr> 
  <tr> 
   <td><strong>源</strong></td> 
   <td>活动的来源。 将设置为“Tout”（输出），用于Sales Connect活动。</td> 
  </tr> 
  <tr> 
   <td><strong>模板ID</strong></td> 
   <td>当源为Tout时，模板ID将为Marketo Sales Connect模板ID。 使用此选项可定位特定模板，而不是主题行，该主题行可能存在于多个模板中。
</td> 
  </tr> 
  <tr> 
   <td><strong>接收者</strong></td> 
   <td>发送电子邮件的人的电子邮件地址。</td> 
  </tr> 
  <tr> 
   <td><strong>详细信息</strong></td> 
   <td>退回错误消息详细信息。</td> 
  </tr> 
  <tr> 
   <td><strong>电子邮件</strong></td> 
   <td>退回的电子邮件地址。</td> 
  </tr> 
 </tbody> 
</table>