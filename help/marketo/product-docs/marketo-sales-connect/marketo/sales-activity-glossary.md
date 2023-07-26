---
description: 销售活动术语表 — Marketo文档 — 产品文档
title: 销售活动术语表
exl-id: c7805642-07b6-4697-9efe-5c673ae9ca53
feature: Marketo Sales Connect
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 2%

---

# 销售活动术语表 {#sales-activity-glossary}

在Sales Connect中，当销售商：将销售线索添加到销售节奏、向他们发送电子邮件或使呼叫成为活动时，它将被记录在Marketo活动历史记录下。 此外，当潜在客户收到电子邮件、打开、点击和回复时，也会被记录。

以下活动将从Sales Connect记录到Marketo。

>[!NOTE]
>
>可以从我们的REST和批量API使用这些活动和属性。

## 活动 {#activities}

<table>
 <tr>
  <th>销售活动</th>
  <th>属性</th>
 </tr>
 <tr>
  <th rowspan="9">发送销售电子邮件</th>
  <td>发送者</td>
 </tr>
 <tr>
  <td>源</td>
 </tr>
 <tr>
  <td>模板Id</td>
 </tr>
 <tr>
  <td>销售模板URL</td>
 </tr>
 <tr>
  <td>促销活动URL</td>
 </tr>
 <tr>
  <td>销售模板名称</td>
 </tr>
 <tr>
  <td>电子邮件主题</td>
 </tr>
 <tr>
  <td>促销活动名称</td>
 </tr>
 <tr>
  <td>Marketo销售人员ID</td>
 </tr>
 <tr>
  <th rowspan="9">打开销售电子邮件</th>
  <td>发送者</td>
 </tr>
 <tr>
  <td>源</td>
 </tr>
 <tr>
  <td>模板Id</td>
 </tr>
 <tr>
  <td>销售模板URL</td>
 </tr>
 <tr>
  <td>促销活动URL</td>
 </tr>
 <tr>
  <td>销售模板名称</td>
 </tr>
 <tr>
  <td>电子邮件主题</td>
 </tr>
 <tr>
  <td>促销活动名称</td>
 </tr>
 <tr>
  <td>Marketo销售人员ID</td>
 </tr>
 <tr>
  <th rowspan="10">点击的销售电子邮件</th>
  <td>链接</td>
 </tr>
 <tr>
  <td>发送者</td>
 </tr>
 <tr>
  <td>源</td>
 </tr>
 <tr>
  <td>模板Id</td>
 </tr>
 <tr>
  <td>销售模板URL</td>
 </tr>
 <tr>
  <td>促销活动URL</td>
 </tr>
 <tr>
  <td>销售模板名称</td>
 </tr>
 <tr>
  <td>电子邮件主题</td>
 </tr>
 <tr>
  <td>促销活动名称</td>
 </tr>
 <tr>
  <td>Marketo销售人员ID</td>
 </tr>
<tr>
  <th rowspan="3">已回复销售电子邮件</th>
  <td>接收者</td>
 </tr>
 <tr>
  <td>源</td>
 </tr>
 <tr>
  <td>Marketo销售人员ID</td>
 </tr>
 <tr>
  <th rowspan="11">已收到的销售电话</th>
  <td>销售呼叫发起人</td>
 </tr>
 <tr>
  <td>销售呼叫状态</td>
 </tr>
 <tr>
  <td>销售拜访主题</td>
 </tr>
 <tr>
  <td>促销活动名称</td>
 </tr>
 <tr>
  <td>促销活动URL</td>
 </tr>
 <tr>
  <td>已呼叫的销售电话号码</td>
 </tr>
 <tr>
  <td>源</td>
 </tr>
 <tr>
  <td>销售呼叫持续时间</td>
 </tr>
 <tr>
  <td>销售电话录音URL</td>
 </tr>
  <tr>
  <td>销售电话应答者</td>
 </tr>
 <tr>
  <td>Marketo销售人员ID</td>
 </tr>
 <tr>
  <th rowspan="6">添加到销售活动</th>
  <td>促销活动名称</td>
 </tr>
 <tr>
  <td>销售呼叫状态</td>
 </tr>
 <tr>
  <td>促销活动URL</td>
 </tr>
 <tr>
  <td>发送者</td>
 </tr>
 <tr>
  <td>源</td>
 </tr>
 <tr>
  <td>促销活动ID</td>
 </tr>
 <tr>
  <th rowspan="6">从促销活动中删除</th>
  <td>促销活动名称</td>
 </tr>
 <tr>
  <td>销售呼叫状态</td>
 </tr>
 <tr>
  <td>促销活动URL</td>
 </tr>
 <tr>
  <td>发送者</td>
 </tr>
 <tr>
  <td>源</td>
 </tr>
 <tr>
  <td>促销活动ID</td>
 </tr>
 <tr>
  <th rowspan="5">销售电子邮件退回</th>
  <td>详细信息</td>
 </tr>
 <tr>
  <td>电子邮件</td>
 </tr>
 <tr>
  <td>发送者</td>
 </tr>
 <tr>
  <td>Marketo销售人员ID</td>
 </tr>
 <tr>
  <td>模板Id</td>
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
   <td><strong>详细信息</strong></td> 
   <td>退回错误消息详细信息。</td> 
  </tr> 
  <tr> 
   <td><strong>电子邮件</strong></td> 
   <td>退回的电子邮件地址。</td> 
  </tr> 
  <tr> 
   <td><strong>链接</strong></td> 
   <td>已单击的URL。</td> 
  </tr> 
  <tr> 
   <td><strong>Marketo销售人员ID</strong></td> 
   <td>Sales Connect中人员记录的唯一ID。</td> 
  </tr> 
  <tr> 
   <td><strong>接收者</strong></td> 
   <td>发送电子邮件的人员的电子邮件地址。</td> 
  </tr>
  <tr> 
   <td><strong>销售电话应答者</strong></td> 
   <td>接听电话的人员姓名。</td> 
  </tr>
  <tr> 
   <td><strong>销售呼叫持续时间</strong></td> 
   <td>呼叫的长度（以秒为单位）。</td> 
  </tr>
  <tr> 
   <td><strong>销售呼叫发起人</strong></td> 
   <td>进行呼叫的销售人员的电子邮件地址。</td> 
  </tr>
  <tr> 
   <td><strong>销售电话录音URL</strong></td> 
   <td>通话录制的URL。</td> 
  </tr>
  <tr> 
   <td><strong>销售呼叫状态</strong></td> 
   <td>将保存呼叫的最终呼叫状态，包括：已完成、无应答、已取消、失败。</td> 
  </tr>
  <tr> 
   <td><strong>销售拜访主题</strong></td> 
   <td>拨号器中的销售用户选择的呼叫结果。</td> 
  </tr>
  <tr> 
   <td><strong>促销活动ID</strong></td> 
   <td>Sales Connect中Sales Campaign资产的唯一ID。</td> 
  </tr>
  <tr> 
   <td><strong>促销活动名称</strong></td> 
   <td>促销活动的名称。</td> 
  </tr>
  <tr> 
   <td><strong>促销活动URL</strong></td> 
   <td>Sales Campaign的Sales Connect URL。</td> 
  </tr>
  <tr> 
   <td><strong>销售电子邮件主题</strong></td> 
   <td>电子邮件的主题行后跟一个唯一ID(例如：我的主题行(MSC-12345678)</td> 
  </tr>
  <tr> 
   <td><strong>已呼叫的销售电话号码</strong></td> 
   <td>销售人员呼叫的电话号码。</td> 
  </tr>
  <tr> 
   <td><strong>销售模板名称</strong></td> 
   <td>Sales Connect中电子邮件模板的名称。</td> 
  </tr>
  <tr> 
   <td><strong>销售模板URL</strong></td> 
   <td>电子邮件模板的Sales Connect URL。</td> 
  </tr>
  <tr> 
   <td><strong>发送者</strong></td>
   <td>发送电子邮件的人员的电子邮件地址。</td> 
  </tr> 
  <tr> 
   <td><strong>源</strong></td> 
   <td>活动的源。 对于2021年10月版发行之前的Sales Connect活动，将被设置为“Tout”。 在2021年10月发布之后，将成为Sales Connect活动的“Sales App”。</td>
  </tr> 
  <tr> 
   <td><strong>模板Id</strong></td> 
   <td>当源为Tout时，模板ID将为Marketo Sales Connect模板ID。 使用此项来定位特定模板，而不是可能存在于多个模板中的主题行。
</td> 
  </tr> 
 </tbody> 
</table>
