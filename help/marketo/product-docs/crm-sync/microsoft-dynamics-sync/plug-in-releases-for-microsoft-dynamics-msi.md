---
unique-page-id: 10099102
description: Microsoft Dynamics MSI的插件版本 — Marketo文档 — 产品文档
title: Microsoft Dynamics MSI的插件版本
exl-id: 830f7dc3-07fd-429b-b0fd-290ffdda88e6
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 6%

---

# Microsoft Dynamics MSI的插件版本 {#plug-in-releases-for-microsoft-dynamics-msi}

首次同步到Microsoft Dynamics时，您需要下载并安装Marketo Sales Insight (MSI)的最新版本插件。 Marketo会定期更新这些插件，以便您能够返回到相同位置下载新版本。

如果您使用Marketo的本机CRM同步解决方案到Dynamics，请 [下载最新的插件](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md){target="_blank"} corresponding to your Dynamics release. For those who have a custom sync and have purchased Marketo Sales Insight, the [package is here](https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip){target="_blank"}.

>[!NOTE]
>
>这些版本适用于Dynamics的内部部署和在线版本。

## 升级MSI解决方案 {#upgrading-your-msi-solution}

1. 导入最新版本的解决方案 _在现有的版本上_ 的CRM的CRM，方法是按 **导入** 按钮。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-1.png)

>[!NOTE]
>
>示例：如果您的Dynamics CRM版本为2.0.0.20，而最新版本为2.0.0.21，则您将导入 _超过_ 版本2.0.0.20。

1. 单击 **下一个**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-2.png)

1. 选择 **暂存升级** 和 **维护自定义项**，然后单击 **导入**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-3.png)

1. 单击 **下一个**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-4.png)

1. 成功导入后，您将看到两个MSI解决方案：MarketoSalesInsight和MarketoSalesInsight_Upgrade。 选择旧解决方案，然后单击Apply Solution Upgrade。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-5.png)

就是这样！ 升级后，您将只看到一个MSI解决方案。

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
   <td colspan="1">Insights的帐户布局：有趣的时刻、得分更改、Web活动、电子邮件活动</td> 
  </tr>
  <tr> 
   <td colspan="1">01/05/22</td> 
   <td colspan="1">2.0.0.26</td> 
   <td colspan="1">发送电子邮件的项目采用分数</td> 
  </tr>
  <tr> 
   <td colspan="1">10/28/21</td> 
   <td colspan="1">2.0.0.25</td> 
   <td colspan="1">产品采用率得分指标，新的全球功能板（Web活动、电子邮件、最佳匹配）</td> 
  </tr>
  <tr> 
   <td colspan="1">02/10/21</td> 
   <td colspan="1">2.0.0.22</td> 
   <td colspan="1">删除对MSI解决方案启用的自动审核和文档更改</td> 
  </tr>
  <tr> 
   <td colspan="1">10/01/20</td> 
   <td colspan="1">2.0.0.21</td> 
   <td colspan="1">错误修复：为具有销售分析角色的用户分配对MSI API配置字段的访问权限</td> 
  </tr> 
  <tr> 
   <td colspan="1">07/20/20</td> 
   <td colspan="1">2.0.0.20</td> 
   <td colspan="1">错误修复：为非同步记录添加验证消息</td> 
  </tr> 
  <tr> 
   <td colspan="1">06/12/20</td> 
   <td colspan="1">2.0.0.19</td> 
   <td colspan="1">错误修复：在MSD API配置上隐藏MSI密码密码</td> 
  </tr> 
  <tr> 
   <td colspan="1">05/26/20</td> 
   <td colspan="1">2.0.0.18</td> 
   <td colspan="1">错误修复：更改用于显示MSI按钮的MSI角色ID验证</td> 
  </tr> 
  <tr> 
   <td colspan="1">05/21/20</td> 
   <td colspan="1">2.0.0.17</td> 
   <td colspan="1">错误修复：取消隐藏所有者字段，并将字段设为非必填字段</td> 
  </tr> 
  <tr> 
   <td colspan="1">04/28/20</td> 
   <td colspan="1">2.0.0.16</td> 
   <td colspan="1">错误修复：正在删除MSD CRM Sitemap设置链接依赖关系</td> 
  </tr> 
 </tbody> 
</table>
