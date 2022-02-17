---
unique-page-id: 10099389
description: Marketo Dynamics插件版本 — Marketo文档 — 产品文档
title: Marketo Dynamics的Microsoft插件版本
exl-id: c9c25e11-bcf7-49bf-920a-4182af27d278
source-git-commit: 1379fcbdc0a8673b1d6cb17a9d573d3625d5a1b8
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 7%

---

# Marketo Dynamics的Microsoft插件版本 {#marketo-plugin-releases-for-microsoft-dynamics}

首次同步到Microsoft Dynamics时，需下载最新版本的Marketo插件。 Marketo会定期更新这些插件，以便您可以返回到同一位置下载新版本。

[下载最新插件](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) 对应于您的Dynamics版本。

![](assets/marketo-plugin-releases-for-microsoft-dynamics-1.png)

## 更新Dynamics解决方案 {#updating-your-dynamics-solution}

1. 与现有版本的Dynamics CRM相比，导入解决方案的最新版本(例如：如果您的Dynamics CRM的版本为1.4，而最新版本为1.5，则需要导入 _over_ 版本1.4)。

1. 您将看到以下弹出窗口。 选择 **更新** 和 **维护自定义**，然后单击 **导入**.

![](assets/marketo-plugin-releases-for-microsoft-dynamics-2.png)

## 最新版本 {#latest-versions}

>[!NOTE]
>
>这些版本适用于Dynamics的内部版本和在线版本。

<table> 
 <tbody> 
  <tr> 
   <th colspan="1">版本</th> 
   <th colspan="1">发行日期</th> 
   <th>注释</th> 
  </tr> 
  <tr> 
   <td colspan="1">5.0.1.1</td> 
   <td colspan="1">02/04/21</td> 
   <td colspan="1">支持多选选项集字段同步（此功能仅适用于V9.X及更高版本）。.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.2.0.0</td> 
   <td colspan="1">10/16/20</td> 
   <td colspan="1">添加了对与MS Dynamics同步Campaign的支持。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.24</td> 
   <td colspan="1">8/22/18</td> 
   <td colspan="1">为Microsoft Dynamics 9.x版添加了对符合条件的现成潜在客户的联系流程支持。</td> 
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
   <td colspan="1">错误修复：插件未订阅捕获自定义对象状态更改的事件。 此修复专用于Dynamics CRM On Premise 2011。 </td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.20</td> 
   <td colspan="1">7/22/16</td> 
   <td colspan="1">错误修复：未完全捕获机会联系角色的更新。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.19</td> 
   <td colspan="1">6/28/16</td> 
   <td colspan="1"><p>错误修复：在创建该机会时，注意到了有关marketo日志中customeroptityrole的不必要更新事务。 </p><p>错误修复：删除customerportityrole实体时，记录了额外的删除事务。</p></td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.18</td> 
   <td colspan="1">5/31/16</td> 
   <td colspan="1">错误修复：将自定义对象的更新和删除设为异步。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.17</td> 
   <td colspan="1">4/8/16</td> 
   <td colspan="1">错误修复：当潜在客户将同步筛选器设置为NO，并且商机和联系人没有同步筛选器时，在潜在客户获得资格时，未为联系人和商机生成创建日志。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.16</td> 
   <td colspan="1">3/29/16</td> 
   <td>错误修复：同步过滤器关闭后，“分配事件”即被记录。</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.15</td> 
   <td colspan="1">3/3/16</td> 
   <td colspan="1">错误修复：由于登录用户没有Marketo配置权限，客户无法在CRM中创建潜在客户。</td> 
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
   <td colspan="1">错误修复：在同步筛选器设置为false时，潜在客户记录正在同步到Marketo。</td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[下载Marketo潜在客户管理解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)
