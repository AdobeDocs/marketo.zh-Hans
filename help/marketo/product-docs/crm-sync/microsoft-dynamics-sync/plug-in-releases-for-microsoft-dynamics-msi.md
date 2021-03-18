---
unique-page-id: 10099102
description: 适用于Microsoft Dynamics MSI的插件版本 — Marketo Docs — 产品文档
title: 适用于Microsoft Dynamics MSI的插件版本
translation-type: tm+mt
source-git-commit: d1d74e24c07578b1b0c2696c08fe5a5be543cce8
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 4%

---


# 适用于Microsoft Dynamics MSI {#plug-in-releases-for-microsoft-dynamics-msi}的插件版本

首次同步到Microsoft Dynamics时，请下载并安装适用于Marketo Sales Insight(MSI)的最新版插件。 Marketo会定期更新这些插件，因此您可以返回同一位置下载新版本。

请[下载与Dynamics版本对应的最新插件](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md)。

>[!NOTE]
>
>这些版本适用于Dynamics的内部和在线版本。

## 升级MSI解决方案{#upgrading-your-msi-solution}

1. 通过按Dynamics中的&#x200B;**导入**&#x200B;按钮，将解决方案&#x200B;_导入到Dynamics CRM的现有版本_&#x200B;上。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-1.png)

>[!NOTE]
>
>示例：如果您的Dynamics CRM具有版本2.0.0.20，且最新版本为2.0.0.21，则应导入&#x200B;_over_&#x200B;版本2.0.0.20。

1. 单击&#x200B;**下一步**。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-2.png)

1. 选择&#x200B;**升级的舞台**&#x200B;和&#x200B;**维护自定义**，然后单击&#x200B;**导入**。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-3.png)

1. 单击&#x200B;**下一步**。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-4.png)

1. 成功导入后，您将看到两个MSI解决方案：MarketoSalesInsight和MarketoSalesInsight_Upgrade。 选择旧版解决方案，然后单击“应用解决方案升级”。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-5.png)

就这样！ 升级后，您只能看到一个MSI解决方案。

## 版本更新{#version-updates}

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
   <th colspan="1">附注</th> 
  </tr> 
  <tr> 
   <td colspan="1">10/1/20</td> 
   <td colspan="1">2.0.0.21</td> 
   <td colspan="1">错误修复：为具有Sales Insight角色的用户分配对MSI API配置字段的访问权限</td> 
  </tr> 
  <tr> 
   <td colspan="1">07/20/20</td> 
   <td colspan="1">2.0.0.20</td> 
   <td colspan="1">错误修复：为未同步记录添加验证消息</td> 
  </tr> 
  <tr> 
   <td colspan="1">06/12/20</td> 
   <td colspan="1">2.0.0.19</td> 
   <td colspan="1">错误修复：要隐藏MSD API配置上的MSI密码</td> 
  </tr> 
  <tr> 
   <td colspan="1">05/26/20</td> 
   <td colspan="1">2.0.0.18</td> 
   <td colspan="1">错误修复：更改显示MSI按钮的MSI角色ID验证</td> 
  </tr> 
  <tr> 
   <td colspan="1">05/21/20</td> 
   <td colspan="1">2.0.0.17</td> 
   <td colspan="1">错误修复：取消隐藏所有者字段并使字段非必填</td> 
  </tr> 
  <tr> 
   <td colspan="1">04/28/20</td> 
   <td colspan="1">2.0.0.16</td> 
   <td colspan="1">错误修复：删除MSD CRM站点地图设置链接依赖关系</td> 
  </tr> 
 </tbody> 
</table>
