---
description: 最新发行说明 - Marketo 文档 - 产品文档
title: 最新发行说明
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 2d69e52883d141e3976c6d4fc1de6038675af602
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 2%

---

# 发行说明：2024年10月 {#release-notes-oct-24}

在下方，您会找到2024年10月版本中包含的所有功能。 检查您的Adobe Marketo Engage版本以了解功能可用性。

可以在此处](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}找到专门用于Adobe Dynamic Chat[的发行说明。

>[!AVAILABILITY]
>
>以星号（![星号](assets/yellow-star.png)）表示的功能是付费加载项。 请联系您的Marketo Engage代表以了解更多信息。

## 标准发行周期功能 {#standard-release-cycle-features}

以下功能属于标准发行周期，将于&#x200B;**2024年10月4日开始发行**，并在接下来的几周内分阶段推出剩余功能。 发行功能和日期可能会发生更改。 请检查每个功能旁边的状态信息。

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">功能</th> 
   <th style="width:10%">状态</th>
   <th style="width:25%">文档</th>
  </tr>
    <tr> 
   <td><strong>增强了交互式网络研讨会参与信息板中的注册数据</strong>：您现在可以在参与信息板中提供的报表中，查看哪些公司的出席人数最多，并了解公司、职称和行业的最新情况。</td> 
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
    <tr> 
   <td><strong>交互式网络研讨会的令牌化</strong>：您现在可以使用令牌在电子邮件和登陆页面中推广交互式网络研讨会，而无需手动添加网络研讨会详细信息。</td> 
   <td><i>即将推出</i></td>
   <td><i>即将推出</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
   <tr> 
   <td><strong>智能列表“设置为影响”计数</strong>：查看编辑Smart Campaign的资格规则时受影响的人员数量。</td> 
   <td>已发货</td>
   <td>不适用</td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
   <tr> 
   <td>导航边栏中的<strong>我的帐户按钮</strong>：对于已迁移到AdobeIdentity Management System的用户，左侧导航边栏中新增的“我的帐户”按钮允许您配置时区并访问订阅详细信息。</td> 
   <td>已发货</td>
   <td>不适用</td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
   <tr> 
   <td><strong>电子邮件性能报表增强功能</strong>：对电子邮件报表量度和活动跟踪进行了多项改进，提供了更多见解并提高了准确性。
   <ul>
   <li>从电子邮件性能量度中过滤删除和合并的人员</li>
   <li>电子邮件在等待响应活动三天后现在被分类为<i>已中止</i></li>
   <li>在营销活动级别打开的帐户电子邮件</li>
   <li>通过细化跟踪像素位置改进了电子邮件活动跟踪</li>
   </td> 
   <td>已发货</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md" target="_blank">电子邮件性能报表</a></td>
  </tr>
 </tbody> 
</table>
<br/>

## 公告 {#announcements}

* **QR代码弃用**： 2024年10月4日，将弃用推送通知和应用程序内消息传送资产中使用的该QR代码功能。 这包括为新的测试设备使用二维码，以及创建具有二维码的新资产。 弃用使用率较低的功能使我们能够将其资源重新分配到Marketo Engage的整体维护中。

* **Munchkin更改**

   * **新版本**：从2024年9月17日开始，[Munchkin](/help/marketo/product-docs/administration/setup-administration/munchkin.md){target="_blank"} v.164将开始推广到&#x200B;**管理员** > **Treasure Chest**&#x200B;中启用了“Munchkin Beta”设置的Marketo Engage实例。 该应用程序计划于10月29日开始推广到所有其他实例。 此版本会更新Munchkin Cookie的创建。 功能没有变化。

   * **已移除URL中的字符**：Munchkin JS创建的“访问网页”和“点击链接”活动现在将从所有URL字段中移除非URL编码的控制字符。 此更改旨在防止与这些类型的字符传播到不支持这些字符且在Marketo Engage中没有有效使用的系统相关的错误。
