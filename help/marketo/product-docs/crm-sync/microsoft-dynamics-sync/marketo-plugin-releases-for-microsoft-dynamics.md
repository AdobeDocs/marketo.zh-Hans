---
unique-page-id: 10099389
description: Microsoft Dynamics的Marketo插件发行版 — Marketo Docs — 产品文档
title: Microsoft Dynamics的Marketo插件版本
translation-type: tm+mt
source-git-commit: d1d74e24c07578b1b0c2696c08fe5a5be543cce8
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 6%

---


# Microsoft Dynamics {#marketo-plugin-releases-for-microsoft-dynamics}的Marketo插件版本

首次同步到Microsoft Dynamics时，请下载适用于Marketo的插件的最新版本。 Marketo会定期更新这些插件，因此您可以返回同一位置下载新版本。

[下载与您的](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) Dynamics版本对应的最新插件。

![](assets/lead-management-solution.png)

## 更新Dynamics解决方案{#updating-your-dynamics-solution}

1. 在现有版本的Dynamics CRM上导入解决方案的最新版本(例如：如果您的Dynamics CRM有版本1.4，且最新版本为1.5，则可导入&#x200B;_over_&#x200B;版本1.4)。

1. 您将看到以下弹出窗口。 选择&#x200B;**更新**&#x200B;和&#x200B;**维护自定义**，然后单击&#x200B;**导入**。

![](assets/marketo-plugin-releases-for-microsoft-dynamics-2.png)

## 最新版本{#latest-versions}

>[!NOTE]
>
>这些版本适用于Dynamics的内部和在线版本。

<table> 
 <tbody> 
  <tr> 
   <th colspan="1">版本</th> 
   <th colspan="1">发行日期</th> 
   <th>附注</th> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.0</td> 
   <td colspan="1">10/16/20</td> 
   <td colspan="1">增加了对与MS Dynamics活动同步的支持。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.24</td> 
   <td colspan="1">8/22/18</td> 
   <td colspan="1">增加了对开箱即用支持，可使Microsoft Dynamics 9.x版的联系流程成为可能。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.23</td> 
   <td colspan="1">6/27/18</td> 
   <td colspan="1">错误修复：尝试安装Marketo Solutions for Dynamics 2013时出现业务流程错误。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.22</td> 
   <td colspan="1">9/29/17</td> 
   <td colspan="1">错误修复：内部修订。</td> 
  </tr> 
  <tr> 
   <td colspan="1"><p>4.0.0.21</p></td> 
   <td colspan="1">11/9/16</td> 
   <td colspan="1">错误修复：该插件未订阅捕获自定义对象的状态更改的事件。 此修复特定于Dynamics CRM On Premise 2011。 </td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.20</td> 
   <td colspan="1">7/22/16</td> 
   <td colspan="1">错误修复：未完全捕获机会联系角色的更新。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.19</td> 
   <td colspan="1">6/28/16</td> 
   <td colspan="1"><p>错误修复：在创建该机会时，会注意到在marketo日志中对customeropentityrole的不必要的更新事务。 </p><p>错误修复：删除customeroperityrole实体时记录了额外的删除事务。</p></td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.18</td> 
   <td colspan="1">5/31/16</td> 
   <td colspan="1">错误修复： 使自定义对象的更新和删除异步进行。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.17</td> 
   <td colspan="1">4/8/16</td> 
   <td colspan="1">错误修复：当潜在客户的同步过滤器设置为NO，而业务机会和联系人没有同步过滤器时，当潜在客户合格时，不会为联系人和业务机会生成创建日志。</td> 
  </tr> 
  <tr> 
   <td colspan="1">2.0.0.16</td> 
   <td colspan="1">3/29/16</td> 
   <td>错误修复：关闭同步过滤器时，将记录“分配”事件。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.15</td> 
   <td colspan="1">3/3/16</td> 
   <td colspan="1">错误修复：客户无法在CRM中创建潜在客户，因为登录用户没有Marketo Config权限。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.14</td> 
   <td colspan="1">1/18/16</td> 
   <td colspan="1">错误修复：为普通Dynamics用户创建了访问限制，以解决安全问题。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.13</td> 
   <td colspan="1">12/30/15</td> 
   <td>错误修复：Dynamics中的更新未同步到Marketo以获取步骤和图像。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.12</td> 
   <td colspan="1">11/12/15</td> 
   <td colspan="1">错误修复：当同步过滤器设置为false时，潜在客户记录正在同步到Marketo。</td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[下载Marketo Lead Management解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)
