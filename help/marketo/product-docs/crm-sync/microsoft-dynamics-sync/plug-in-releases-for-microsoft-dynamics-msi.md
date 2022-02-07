---
unique-page-id: 10099102
description: Microsoft Dynamics MSI的插件版本 — Marketo文档 — 产品文档
title: 适用于Microsoft Dynamics MSI的插件版本
exl-id: 830f7dc3-07fd-429b-b0fd-290ffdda88e6
source-git-commit: 7b22aec56d15826c1fecd2cf026c561c4df8531c
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 6%

---

# 适用于Microsoft Dynamics MSI的插件版本 {#plug-in-releases-for-microsoft-dynamics-msi}

首次同步到Microsoft Dynamics时，您需要下载并安装最新版本的Marketo Sales Insight(MSI)插件。 Marketo会定期更新这些插件，以便您可以返回到同一位置下载新版本。

请 [下载最新插件](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) 对应于您的Dynamics版本。

>[!NOTE]
>
>这些版本适用于Dynamics的内部版本和在线版本。

## 升级MSI解决方案 {#upgrading-your-msi-solution}

1. 导入解决方案的最新版本 _与现有版本相比_ ，方法是按 **导入** 按钮。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-1.png)

>[!NOTE]
>
>示例：如果您的Dynamics CRM具有版本2.0.0.20，且最新版本为2.0.0.21，则需要导入 _over_ 版本2.0.0.20。

1. 单击 **下一个**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-2.png)

1. 选择 **升级阶段** 和 **维护自定义**，然后单击 **导入**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-3.png)

1. 单击 **下一个**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-4.png)

1. 成功导入后，您将看到两个MSI解决方案：MarketoSalesInsight和MarketoSalesInsight_Upgrade。 选择旧版解决方案，然后单击“应用解决方案升级”。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-5.png)

就这样！ 升级后，您将只看到一个MSI解决方案。

## 版本更新 {#version-updates}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th colspan="1">发行日期</th> 
   <th colspan="1">版本</th> 
   <th colspan="1">注释</th> 
  </tr> 
  <tr> 
   <td colspan="1">02/03/22</td> 
   <td colspan="1">2.0.0.27</td> 
   <td colspan="1">用于分析的帐户布局：有趣的时刻、分数变化、Web活动、电子邮件活动</td> 
  </tr>
  <tr> 
   <td colspan="1">01/05/22</td> 
   <td colspan="1">2.0.0.26</td> 
   <td colspan="1">发送电子邮件的计划采用分数</td> 
  </tr>
  <tr> 
   <td colspan="1">10/28/21</td> 
   <td colspan="1">2.0.0.25</td> 
   <td colspan="1">产品采用分数量度，新的全局功能板（Web活动、电子邮件、最佳押注）</td> 
  </tr>
  <tr> 
   <td colspan="1">02/10/21</td> 
   <td colspan="1">2.0.0.22</td> 
   <td colspan="1">删除启用自动审核功能并对MSI解决方案进行文档更改</td> 
  </tr>
  <tr> 
   <td colspan="1">10/01/20</td> 
   <td colspan="1">2.0.0.21</td> 
   <td colspan="1">错误修复：为具有Sales Insight角色的用户分配对MSI API配置字段的访问权限</td> 
  </tr> 
  <tr> 
   <td colspan="1">07/20/20</td> 
   <td colspan="1">2.0.0.20</td> 
   <td colspan="1">错误修复：为非同步记录添加验证消息</td> 
  </tr> 
  <tr> 
   <td colspan="1">06/12/20</td> 
   <td colspan="1">2.0.0.19</td> 
   <td colspan="1">错误修复：在MSD API配置中隐藏MSI密码</td> 
  </tr> 
  <tr> 
   <td colspan="1">05/26/20</td> 
   <td colspan="1">2.0.0.18</td> 
   <td colspan="1">错误修复：更改MSI角色ID验证以显示MSI按钮</td> 
  </tr> 
  <tr> 
   <td colspan="1">05/21/20</td> 
   <td colspan="1">2.0.0.17</td> 
   <td colspan="1">错误修复：取消隐藏所有者字段，并使字段非必填项</td> 
  </tr> 
  <tr> 
   <td colspan="1">04/28/20</td> 
   <td colspan="1">2.0.0.16</td> 
   <td colspan="1">错误修复：删除MSD CRM站点地图设置链接依赖项</td> 
  </tr> 
 </tbody> 
</table>
