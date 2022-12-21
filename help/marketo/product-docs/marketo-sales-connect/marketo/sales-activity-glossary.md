---
description: 销售活动术语表 — Marketo文档 — 产品文档
title: 销售活动术语表
exl-id: c7805642-07b6-4697-9efe-5c673ae9ca53
source-git-commit: d261da2a2784ab322ef78fe22ef3d6b4321fc806
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 2%

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
  <th rowspan="9">发送销售电子邮件</th>
  <td>发送者</td>
 </tr>
 <tr>
  <td>源</td>
 </tr>
 <tr>
  <td>模板ID</td>
 </tr>
 <tr>
  <td>销售模板URL</td>
 </tr>
 <tr>
  <td>销售活动URL</td>
 </tr>
 <tr>
  <td>销售模板名称</td>
 </tr>
 <tr>
  <td>电子邮件主题</td>
 </tr>
 <tr>
  <td>销售活动名称</td>
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
  <td>模板ID</td>
 </tr>
 <tr>
  <td>销售模板URL</td>
 </tr>
 <tr>
  <td>销售活动URL</td>
 </tr>
 <tr>
  <td>销售模板名称</td>
 </tr>
 <tr>
  <td>电子邮件主题</td>
 </tr>
 <tr>
  <td>销售活动名称</td>
 </tr>
 <tr>
  <td>Marketo销售人员ID</td>
 </tr>
 <tr>
  <th rowspan="10">点击了销售电子邮件</th>
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
  <td>销售模板URL</td>
 </tr>
 <tr>
  <td>销售活动URL</td>
 </tr>
 <tr>
  <td>销售模板名称</td>
 </tr>
 <tr>
  <td>电子邮件主题</td>
 </tr>
 <tr>
  <td>销售活动名称</td>
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
  <th rowspan="11">已接到销售电话</th>
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
  <td>销售呼叫持续时间</td>
 </tr>
 <tr>
  <td>销售电话记录URL</td>
 </tr>
  <tr>
  <td>销售电话应答者</td>
 </tr>
 <tr>
  <td>Marketo销售人员ID</td>
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
   <td><strong>详细信息</strong></td> 
   <td>退回错误消息详细信息。</td> 
  </tr> 
  <tr> 
   <td><strong>电子邮件</strong></td> 
   <td>退回的电子邮件地址。</td> 
  </tr> 
  <tr> 
   <td><strong>链接</strong></td> 
   <td>已点击的URL。</td> 
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
   <td>应答呼叫的人员的姓名。</td> 
  </tr>
  <tr> 
   <td><strong>销售呼叫持续时间</strong></td> 
   <td>调用长度（以秒为单位）。</td> 
  </tr>
  <tr> 
   <td><strong>销售电话由</strong></td> 
   <td>拨打电话的销售人员的电子邮件地址。</td> 
  </tr>
  <tr> 
   <td><strong>销售电话记录URL</strong></td> 
   <td>呼叫录制的URL。</td> 
  </tr>
  <tr> 
   <td><strong>销售电话状态</strong></td> 
   <td>将保存调用的最终调用状态，其中包括：已完成，无应答，已取消，失败。</td> 
  </tr>
  <tr> 
   <td><strong>销售呼叫主体</strong></td> 
   <td>拨号器中销售用户选择的呼叫结果。</td> 
  </tr>
  <tr> 
   <td><strong>销售活动ID</strong></td> 
   <td>Sales Connect中Sales Campaign资产的唯一ID。</td> 
  </tr>
  <tr> 
   <td><strong>销售活动名称</strong></td> 
   <td>销售活动的名称。</td> 
  </tr>
  <tr> 
   <td><strong>销售活动URL</strong></td> 
   <td>Sales Campaign的Sales Connect URL。</td> 
  </tr>
  <tr> 
   <td><strong>销售电子邮件主题</strong></td> 
   <td>电子邮件的主题行后跟一个唯一ID(例如：我的主题行(MSC-12345678)</td> 
  </tr>
  <tr> 
   <td><strong>已拨打销售电话号码</strong></td> 
   <td>由销售部呼叫的电话号码。</td> 
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
   <td>活动的来源。 在2021年10月版之前，Sales Connect活动将设置为“Tout”。 在’21年10月版发布后，将成为Sales Connect活动的“销售应用程序”。</td>
  </tr> 
  <tr> 
   <td><strong>模板ID</strong></td> 
   <td>当源为Tout时，模板ID将为Marketo Sales Connect模板ID。 使用此选项可定位特定模板，而不是主题行，该主题行可能存在于多个模板中。
</td> 
  </tr> 
 </tbody> 
</table>
