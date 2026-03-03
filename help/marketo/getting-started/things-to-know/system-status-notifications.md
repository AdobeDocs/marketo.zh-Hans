---
description: 订阅系统状态通知 — Marketo Engage文档 — 产品文档
title: 订阅系统状态通知
feature: Getting Started
exl-id: f4404a26-3b86-4dc7-8ecb-52a24fdb09b4
source-git-commit: b056173fbae44ec710ae17172b4a3fc162935dda
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 1%

---

# 订阅系统状态通知 {#subscribe-to-system-status-notifications}

了解如何订阅不同的状态通知以随时了解当前问题。

>[!PREREQUISITES]
>
>在创建订阅之前，您必须首先确定订阅所在的数据中心和面板/服务器。

## 识别您的数据中心 {#identify}

1. 在Marketo Engage的&#x200B;**管理员**&#x200B;部分中，单击&#x200B;**我的帐户**。

   ![](assets/subscribe-to-system-status-notifications-1.png)

1. 向下滚动至&#x200B;_支持信息_。

   ![](assets/subscribe-to-system-status-notifications-2.png)

在&#x200B;_数据中心_&#x200B;字段中，字母是数据中心，数字是面板。 在上面的示例中，用户位于位于舱49上的Ashburn数据中心。

在[步骤7（共](#create-a-subscription)部分）中，用户将选择区域位置&#x200B;**Marketo Ashburn**&#x200B;和面板&#x200B;**ab49**。

**数据中心缩写**

* ab：Ashburn
* sj：圣何塞
* sn：悉尼
* lon：伦敦
* nld：阿姆斯特丹

>[!TIP]
>
>此方法还可用于识别您的订阅使用的实时Personalization (RTP)面板/服务器。

## 创建订阅 {#create-a-subscription}

在[识别您的数据中心和pod/server](#identify)后，请按照以下步骤创建订阅。

1. 在[status.adobe.com](https://status.adobe.com)上，单击&#x200B;**管理订阅**。

   ![](assets/subscribe-to-system-status-notifications-3.png)

1. 使用您的Adobe凭据登录（如果尚未登录），或者单击&#x200B;**创建帐户**（如果没有）。

   ![](assets/subscribe-to-system-status-notifications-4.png)

1. 停留在&#x200B;_产品描述_&#x200B;选项卡中，然后单击&#x200B;**创建订阅**。

   ![](assets/subscribe-to-system-status-notifications-5.png)

1. 单击![Experience Cloud](assets/icon-plus-sign.png)旁边的&#x200B;_加号图标_&#x200B;图标展开菜单。 对&#x200B;_Adobe Marketo Engage_&#x200B;执行相同操作。

   ![](assets/subscribe-to-system-status-notifications-6.png){width="800"}

1. 选择要接收有关通知的产品产品/服务，然后单击&#x200B;**继续**。

   >[!TIP]
   >
   >选中&#x200B;_Adobe Marketo Engage_&#x200B;以选择全部。

   ![](assets/subscribe-to-system-status-notifications-7.png){width="800"}

1. 选择所需的事件类型。

   ![](assets/subscribe-to-system-status-notifications-8.png)

   <table style="width:500px;">
   <tr>
   <td style="width:35%;"><b>重大服务问题</b></td>
   <td>生产系统上多个用户的服务不可用或性能严重下降。</td>
   </tr>
   <tr>
   <td style="width:35%;"><b>轻微服务问题</b></td>
   <td>生产系统上的多个用户出现部分服务不可用或性能适度下降。</td>
   </tr>
   <tr>
   <td style="width:35%;"><b>服务维护</b></td>
   <td>计划窗口，用于执行可能影响产品可用性或性能的产品维护。</td>
   </tr>
   <tr>
   <td style="width:35%;"><b>公告</b></td>
   <td>具有广泛影响的全球、产品系列或产品相关消息。</td>
   </tr>
   </table>

1. 选择区域位置和环境。 单击&#x200B;**继续**。

   ![](assets/subscribe-to-system-status-notifications-9.png){width="900"}

   >[!NOTE]
   >
   >如果您错过了在何处查找此内容，请参阅[识别您的数据中心](#identify)。

1. 选择您的订阅首选项&#x200B;**电子邮件**&#x200B;或&#x200B;**Slack**，然后单击&#x200B;**继续**。

   ![](assets/subscribe-to-system-status-notifications-10.png)

1. 查看您的选择，然后单击&#x200B;**确认首选项**。

   ![](assets/subscribe-to-system-status-notifications-11.png)
