---
unique-page-id: 10099389
description: 适用于Microsoft Dynamics的Marketo插件版本 — Marketo文档 — 产品文档
title: 适用于Microsoft Dynamics的Marketo插件版本
exl-id: c9c25e11-bcf7-49bf-920a-4182af27d278
feature: Microsoft Dynamics
source-git-commit: 44bbd12ec5c5c213a977b9d99f455eefb99bf275
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# 适用于Microsoft Dynamics的Marketo插件版本 {#marketo-plugin-releases-for-microsoft-dynamics}

首次同步到Microsoft Dynamics时，您将下载Marketo的最新版本插件。 Marketo会定期更新这些插件，以便您能够返回到相同位置下载新版本。

[下载最新的插件](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"} 与您的Dynamics版本相对应。

![](assets/marketo-plugin-releases-for-microsoft-dynamics-1.png)

## 正在更新您的Dynamics解决方案 {#updating-your-dynamics-solution}

1. 在现有Dynamics CRM版本的基础上导入最新版本的解决方案(例如：如果Dynamics CRM的版本为1.4，而最新版本为1.5，则导入 _超过_ 版本1.4)。

1. 您将看到以下弹出窗口。 选择 **更新** 和 **维护自定义项**，然后单击 **导入**.

![](assets/marketo-plugin-releases-for-microsoft-dynamics-2.png)

## 最新版本 {#latest-versions}

>[!NOTE]
>
>这些版本适用于Dynamics的内部部署和在线版本。

<table> 
 <tbody> 
  <tr> 
   <th style="width:15%">版本</th> 
   <th style="width:20%">发行日期</th> 
   <th style="width:65%">备注</th> 
  </tr>
  <tr> 
   <td>5.0.2.1</td> 
   <td>10/13/23</td> 
   <td>错误修复：修复了与自定义实体同步相关的错误。</td> 
  </tr> 
  <tr> 
   <td>5.0.2.0</td> 
   <td>03/24/23</td> 
   <td>错误修复：修复了阻止在MS Dynamics上合并联系人的错误。</td> 
  </tr> 
  <tr> 
   <td>5.0.1.8</td> 
   <td>03/27/23</td> 
   <td>错误修复：阻止插件覆盖MS Dynamics中UI元素上的其他自定义项。</td> 
  </tr> 
  <tr> 
   <td>5.0.1.1</td> 
   <td>02/04/21</td> 
   <td>支持多选选项集字段同步（此功能仅适用于V9.X及更高版本）。</td> 
  </tr> 
  <tr> 
   <td>4.2.0.0</td> 
   <td>10/16/20</td> 
   <td>添加了对Campaign与MS Dynamics同步的支持。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.24</td> 
   <td>8/22/18</td> 
   <td>为开箱即用型添加支持，使潜在客户能够联系Microsoft Dynamics版本9.x的流程。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.23</td> 
   <td>6/27/18</td> 
   <td>错误修复：尝试安装适用于Dynamics 2013的Marketo解决方案时出现业务流程错误。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.22</td> 
   <td>9/29/17</td> 
   <td>错误修复：内部修订。</td> 
  </tr> 
  <tr> 
   <td><p>4.0.0.21</p></td> 
   <td>11/9/16</td> 
   <td>错误修复：插件未订阅捕获自定义对象状态更改的事件。 此修复特定于Dynamics CRM On Premise 2011。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.20</td> 
   <td>7/22/16</td> 
   <td>错误修复：未完全捕获机会联系人角色的更新。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.19</td> 
   <td>6/28/16</td> 
   <td>错误修复：创建机会时，在marketo日志中记录了customeropportunityrole上不必要的更新事务。<p>错误修复：删除customeropportunityrole实体时记录了额外的删除事务。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.18</td> 
   <td>5/31/16</td> 
   <td>错误修复：使自定义对象的更新和删除成为异步操作。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.17</td> 
   <td>4/8/16</td> 
   <td>错误修复：当商机将同步筛选器设置为NO，并且商机和联系人没有同步筛选器时，当商机符合条件时，不会为联系人和商机生成“创建日志”。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.16</td> 
   <td>3/29/16</td> 
   <td>错误修复：关闭同步筛选器时，记录了一个分配事件。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.15</td> 
   <td>3/3/16</td> 
   <td>错误修复：客户无法在CRM中创建潜在客户，因为登录用户没有Marketo配置权限。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.14</td> 
   <td>1/18/16</td> 
   <td>错误修复：为普通Dynamics用户创建了访问限制以解决安全问题。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.13</td> 
   <td>12/30/15</td> 
   <td>错误修复： Dynamics中的更新未同步到Marketo以获取步骤和图像。</td> 
  </tr> 
  <tr> 
   <td>4.0.0.12</td> 
   <td>11/12/15</td> 
   <td>错误修复：将同步筛选器设置为false时，潜在客户记录正在同步到Marketo。</td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[下载Marketo商机管理解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}
