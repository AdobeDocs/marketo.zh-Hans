---
unique-page-id: 11387674
description: Marketo术语更新 — Marketo Docs — 产品文档
title: Marketo术语更新
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 0%

---


# Marketo术语{#updates-to-marketo-terminology}的更新

我们正在对我们的平台进行一些更改，这会影响某些东西的名称。 如果您在2016年3月有新的Marketo实例，或者您的公司在2016年7月之后续订，您现在可能会看到新术语。

尽管您可能在Marketo文档中看到不同的术语，但请放心，每篇文章都将很快更新以反映这些更改。 所有指令都是相同的。

那么，有什么变化？

## 潜在客户现在为人{#lead-is-now-person}

最大的变化是将潜在客户/潜在客户重命名为人/人。

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>旧</strong></td> 
   <td><strong>新增</strong></td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <img width="295" src="assets/leads.png" data-linked-resource-id="11387678" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
   <td> 
    <div> 
     <img width="295" src="assets/people.png" data-linked-resource-id="11387679" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

在某些情况下，“Lead”一词被简单地删除。

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>旧</strong></td> 
   <td><strong>新增</strong></td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <img src="assets/lead-database.png" data-linked-resource-id="11387676" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
   <td> 
    <div> 
     <p><img src="assets/database.png" data-linked-resource-id="11387677" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"></p> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

潜在客户和人员&#x200B;**是相同的东西**。

## 令牌{#tokens}

带有词“lead”的令牌&#x200B;**未更改**。 我们为任何混乱表示歉意；但是，更改所有令牌以匹配新术语将会破坏当前使用的大量令牌。 因此，您仍将看到“`{{lead.First Name}}`”等令牌。 没有特定于个人的令牌。

>[!NOTE]
>
>*是*&#x200B;一个名为“人物备注”的令牌，但该令牌始终存在。 它通常用于CRM中的描述字段（如果有）。

## 字段管理{#field-management}

包含“潜在客户”一词的字段已替换为“人员”，或“潜在客户”一词已被删除。 但是，“潜在客户所有者”字段是一个明显的例外。 现在，它被称为“销售所有者”。

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>旧</strong></td> 
   <td><strong>新增</strong></td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <img src="assets/lead-owner.png" data-linked-resource-id="11387757" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
   <td> 
    <div> 
     <img src="assets/sales-owner.png" data-linked-resource-id="11387758" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>有关受影响字段名称的完整列表，请访问此[支持文章](https://nation.marketo.com/docs/DOC-4218#jive_content_id_Field_Names_and_Tokens)。

## 实时个性化(RTP)现已成为Web个性化{#real-time-personalization-rtp-is-now-web-personalization}

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>旧</strong></td> 
   <td><strong>新增</strong></td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <img src="assets/rtp.png" data-linked-resource-id="11387692" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
   <td> 
    <div> 
     <img src="assets/web.png" data-linked-resource-id="11387693" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

除了名称更改外，它现在还包含四个单独的应用程序：

| ** [Web个性化](https://docs.marketo.com/display/DOCS/Web+Personalization+-+RTP)** | 在主屏幕上有自己的拼贴 |
|---|---|
| ** [基于帐户的Web营销](https://docs.marketo.com/display/DOCS/Account-Based+Web+Marketing)** | 可通过Web个性化拼贴访问 |
| ** [个性化重定位](https://docs.marketo.com/display/DOCS/Website+Retargeting)** | 可通过Web个性化拼贴访问 |
| ** [预测内容](https://docs.marketo.com/display/DOCS/Predictive+Content)** | 在主屏幕上有自己的拼贴 |

>[!NOTE]
>
>主屏幕上显示的拼贴将反映所购买的模块。

感谢您在此更新期间的耐心等待。
