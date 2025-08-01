---
unique-page-id: 11387674
description: Marketo术语更新 — Marketo文档 — 产品文档
hide: true
hidefromtoc: true
title: Marketo术语更新
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 1%

---

# Marketo术语更新 {#updates-to-marketo-terminology}

我们正在对我们的平台进行一些更改，这些更改将影响某些项目的名称。 如果您在2016年3月拥有新的Marketo实例，或者贵公司在2016年7月之后续订，则您现在可能看到新术语。

虽然您在Marketo文档中可能会看到不同的术语，但请放心，每篇文章都将很快更新以反映这些更改。 所有指令都相同。

那么，有什么变化呢？

## 潜在客户现在是人员 {#lead-is-now-person}

最大的变化是将潜在客户/潜在客户重命名为人员/人员。

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

在某些情况下，“Lead”一词会被简单地删除。

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

潜在客户和人员&#x200B;**是同一回事**。

## 令牌 {#tokens}

包含单词lead **的令牌未更改**。 很抱歉会造成任何混淆；但是，更改所有令牌以匹配新术语会破坏当前正在使用的令牌。 因此您仍会看到“`{{lead.First Name}}`”之类的令牌。 没有特定于人员的令牌。

>[!NOTE]
>
>*有*&#x200B;个名为“人员笔记”的令牌，但该令牌始终存在。 它通常用于CRM中的描述字段（如果有的话）。

## 字段管理 {#field-management}

包含术语Lead的字段已替换为Person，或者单词Lead已删除。 但是，“Lead Owner”字段是一个显着例外。 它现在被称为“销售负责人”。

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
>有关受影响的字段名称的完整列表，请访问此[支持文章](https://nation.marketo.com/docs/DOC-4218#jive_content_id_Field_Names_and_Tokens){target="_blank"}。

## 实时Personalization (RTP)现在更名为Web Personalization {#real-time-personalization-rtp-is-now-web-personalization}

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

除了名称更改之外，该应用程序现在还包括四个单独的应用程序：

| **[Web Personalization](https://docs.marketo.com/display/DOCS/Web+Personalization+-+RTP){target="_blank"}** | 在主屏幕上拥有自己的图块 |
|---|---|
| **[基于帐户的Web营销](https://docs.marketo.com/display/DOCS/Account-Based+Web+Marketing){target="_blank"}** | 可通过Web Personalization拼贴访问 |
| **[个性化重定位](https://docs.marketo.com/display/DOCS/Website+Retargeting){target="_blank"}** | 可通过Web Personalization拼贴访问 |
| **[预测内容](https://docs.marketo.com/display/DOCS/Predictive+Content){target="_blank"}** | 在主屏幕上拥有自己的图块 |

>[!NOTE]
>
>主屏幕上显示的图块将反映您购买的模块。

感谢您耐心等待本次更新。
