---
unique-page-id: 10099102
description: Microsoft Dynamics MSI的插件版本 — Marketo文档 — 产品文档
title: Microsoft Dynamics MSI的插件版本
exl-id: 830f7dc3-07fd-429b-b0fd-290ffdda88e6
feature: Microsoft Dynamics
source-git-commit: 6dcda9b86555c17b3492a02f3985db7d2acd8a32
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# Microsoft Dynamics MSI的插件版本 {#plug-in-releases-for-microsoft-dynamics-msi}

首次同步到Microsoft Dynamics时，您需要下载并安装Marketo Sales Insight (MSI)的最新版本插件。 Marketo Engage会定期更新这些插件，以便您可以返回到相同位置下载新版本。

如果您使用Marketo本机CRM同步解决方案到Dynamics，请[下载与您的Dynamics版本对应的最新插件](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md){target="_blank"}。 对于拥有自定义同步功能并已购买Marketo Sales Insight的用户，[包位于此处](https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip){target="_blank"}。

>[!NOTE]
>
>这些版本适用于Dynamics的内部部署和在线版本。

## 升级MSI解决方案 {#upgrading-your-msi-solution}

1. 按Dynamics中的&#x200B;**[!UICONTROL 导入]**&#x200B;按钮，在Dynamics CRM的现有版本&#x200B;_上导入最新版本的解决方案_。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-1.png)

>[!NOTE]
>
>示例：如果您的Dynamics CRM版本为2.0.0.20，而最新版本为2.0.0.21，则您将导入&#x200B;_超过_&#x200B;版本2.0.0.20。

1. 单击&#x200B;**[!UICONTROL 下一步]**。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-2.png)

1. 选择&#x200B;**[!UICONTROL 升级阶段]**&#x200B;和&#x200B;**[!UICONTROL 维护自定义项]**，然后单击&#x200B;**[!UICONTROL 导入]**。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-3.png)

1. 单击&#x200B;**[!UICONTROL 下一步]**。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-4.png)

1. 成功导入后，您将看到两个MSI解决方案：MarketoSalesInsight和MarketoSalesInsight_Upgrade。 选择旧解决方案，然后单击Apply Solution Upgrade。

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-5.png)

就是这样！ 升级后，您将只看到一个MSI解决方案。

## 版本更新 {#version-updates}

<table> 
 <tbody> 
  <tr> 
   <th>发行日期</th> 
   <th>版本</th> 
   <th>备注</th> 
  </tr>
  <tr> 
   <td>02/14/24</td> 
   <td>2.00.31</td> 
   <td>更改了匿名Web活动上的分页。
   <p>
   从用户视图中加密密钥信息。 导入新包后需要更改密码才能进行加密。</td> 
  </tr>
  <tr> 
   <td>10/18/23</td> 
   <td>2.00.30</td> 
   <td>合并MSI错误日志，并删除Marketo错误实体上显示的信息通知。</td> 
  </tr>
  <tr> 
   <td>05/19/23</td> 
   <td>2.00.29</td> 
   <td>修复了全局功能板上的Web活动和兴趣时刻分页问题。</td> 
  </tr>
  <tr> 
   <td>03/23/23</td> 
   <td>2.00.28</td> 
   <td>已为CRM的非本机连接创建MSI的<a href="https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip">新包</a>。</td> 
  </tr>
  <tr> 
   <td>02/03/22</td> 
   <td>2.0.0.27</td> 
   <td>Insights的帐户布局：有趣的时刻、得分更改、Web活动、电子邮件活动。</td> 
  </tr>
  <tr> 
   <td>01/05/22</td> 
   <td>2.0.0.26</td> 
   <td>发送电子邮件的项目采用分数。</td> 
  </tr>
  <tr> 
   <td>10/28/21</td> 
   <td>2.0.0.25</td> 
   <td>产品采用率得分指标、新的全局功能板（Web活动、电子邮件、最佳匹配）。</td> 
  </tr>
  <tr> 
   <td>02/10/21</td> 
   <td>2.0.0.22</td> 
   <td>删除对MSI解决方案启用的自动审核和文档更改。</td> 
  </tr>
  <tr> 
   <td>10/01/20</td> 
   <td>2.0.0.21</td> 
   <td>错误修复：为具有Sales Insight角色的用户分配对MSI API配置字段的访问权限。</td> 
  </tr> 
  <tr> 
   <td>07/20/20</td> 
   <td>2.0.0.20</td> 
   <td>错误修复：为非同步记录添加验证消息。</td> 
  </tr> 
  <tr> 
   <td>06/12/20</td> 
   <td>2.0.0.19</td> 
   <td>错误修复：在MSD API配置上隐藏MSI密码密码。</td> 
  </tr> 
  <tr> 
   <td>05/26/20</td> 
   <td>2.0.0.18</td> 
   <td>错误修复：更改用于显示MSI按钮的MSI角色ID验证。</td> 
  </tr> 
  <tr> 
   <td>05/21/20</td> 
   <td>2.0.0.17</td> 
   <td>错误修复：取消隐藏所有者字段，并将字段设为非必填字段。</td> 
  </tr> 
  <tr> 
   <td>04/28/20</td> 
   <td>2.0.0.16</td> 
   <td>错误修复：正在删除MSD CRM Sitemap设置链接依赖关系。</td> 
  </tr> 
 </tbody> 
</table>
