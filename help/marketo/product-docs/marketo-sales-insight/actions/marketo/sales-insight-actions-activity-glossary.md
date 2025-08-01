---
description: 销售Insight操作活动术语表 — Marketo文档 — 产品文档
title: Sales Insight Actions活动术语表
exl-id: fd0f632c-6f0d-49f9-a805-0730595c81fd
feature: Sales Insight Actions
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 5%

---

# [!DNL Sales Insight Actions]活动术语表 {#sales-insight-actions-activity-glossary}

在[!DNL Sales Insight Actions]中，当销售商：将销售线索添加到促销活动、向他们发送销售电子邮件或发出出站销售呼叫时，该销售线索将记录在该销售线索的Marketo活动历史记录下。 此外，当商机收到电子邮件、打开、点击和回复时，也会记录该商机。

以下活动将从[!DNL Sales Insight Actions]记录到Marketo。

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
  <th rowspan="9">[!UICONTROL Send Sales Email]</th>
  <td>[!UICONTROL Sent By]</td>
 </tr>
 <tr>
  <td>来源</td>
 </tr>
 <tr>
  <td>[!UICONTROL Template ID]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Template URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Template Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Email Subject]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Person ID]</td>
 </tr>
 <tr>
  <th rowspan="9">[!UICONTROL Open Sales Email]</th>
  <td>[!UICONTROL Sent By]</td>
 </tr>
 <tr>
  <td>来源</td>
 </tr>
 <tr>
  <td>[!UICONTROL Template ID]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Template URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Template Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Email Subject]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Person ID]</td>
 </tr>
 <tr>
  <th rowspan="10">[!UICONTROL Clicked Sales Email]</th>
  <td>[!UICONTROL Link]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sent By]</td>
 </tr>
 <tr>
  <td>来源</td>
 </tr>
 <tr>
  <td>[!UICONTROL Template ID]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Template URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Template Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Email Subject]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Person ID]</td>
 </tr>
<tr>
  <th rowspan="3">[!UICONTROL Replied to Sales Email]</th>
  <td>[!UICONTROL Received By]</td>
 </tr>
 <tr>
  <td>来源</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Person ID]</td>
 </tr>
 <tr>
  <th rowspan="11">[!UICONTROL Received Sales Call]</th>
  <td>[!UICONTROL Sales Call Made By]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Call Status]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Call Subject]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Phone Number Called]</td>
 </tr>
 <tr>
  <td>来源</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Call Duration]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Call Recording URL]</td>
 </tr>
  <tr>
  <td>[!UICONTROL Sales Call Answered By]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Person ID]</td>
 </tr>
 <tr>
  <th rowspan="6">[!UICONTROL Add to Sales Campaign]</th>
  <td>[!UICONTROL Sales Campaign Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Call Status]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sent By]</td>
 </tr>
 <tr>
  <td>来源</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign ID]</td>
 </tr>
 <tr>
  <th rowspan="6">[!UICONTROL Remove from Sales Campaign]</th>
  <td>[!UICONTROL Sales Campaign Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Call Status]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sent By]</td>
 </tr>
 <tr>
  <td>来源</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign ID]</td>
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
  <td>模板 ID</td>
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
   <td><strong>[!UICONTROL Details]</strong></td>
   <td>退回错误消息详细信息。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Email]</strong></td>
   <td>退回的电子邮件地址。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Link]</strong></td>
   <td>已单击的URL。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Marketo Sales Person ID]</strong></td>
   <td>[!DNL Sales Insight Actions]中人员记录的唯一ID。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Received By]</strong></td>
   <td>发送电子邮件的人员的电子邮件地址。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Call Answered By]</strong></td>
   <td>接听电话的人员姓名。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Call Duration]</strong></td>
   <td>呼叫的长度（以秒为单位）。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Call Made By]</strong></td>
   <td>进行呼叫的销售人员的电子邮件地址。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Call Recording URL]</strong></td>
   <td>通话录制的URL。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Call Status]</strong></td>
   <td>将保存呼叫的最终呼叫状态，包括：已完成、无应答、已取消、失败。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Call Subject]</strong></td>
   <td>拨号器中的销售用户选择的呼叫结果。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Campaign ID]</strong></td>
   <td>[!DNL Sales Insight Actions]中促销活动资产的唯一ID。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Campaign Name]</strong></td>
   <td>促销活动的名称。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Campaign URL]</strong></td>
   <td>[!DNL Sales Insight Actions] 销售促销活动的URL。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Email Subject]</strong></td>
   <td>电子邮件主题行后跟一个唯一ID(例如：我的主题行(SIA-12345678)</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Phone Number Called]</strong></td>
   <td>销售人员呼叫的电话号码。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Template Name]</strong></td>
   <td>[!DNL Sales Insight Actions]中电子邮件模板的名称。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Template URL]</strong></td>
   <td>[!DNL Sales Insight Actions] 电子邮件模板的URL。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sent By]</strong></td>
   <td>发送电子邮件的人员的电子邮件地址。</td>
  </tr>
  <tr>
   <td><strong>来源</strong></td>
   <td>活动的Source。 在2021年10月版发布之前，将针对[!DNL Sales Insight Actions]活动设置为“Tout”。 在2021年10月版发布后，将成为[!DNL Sales Insight Actions]活动的“销售应用程序”。</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Template ID]</strong></td>
   <td>当源为Tout时，模板ID将为[!DNL Marketo Sales Insight Actions]模板ID。 使用此项来定位特定模板，而不是可能存在于多个模板中的主题行。
</td>
  </tr>
 </tbody>
</table>
