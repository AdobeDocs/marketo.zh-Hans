---
unique-page-id: 4720257
description: 将Facebook自定义受众添加为LaunchPoint服务 — Marketo文档 — 产品文档
title: 将Facebook自定义受众添加为LaunchPoint服务
exl-id: 5c5b5c80-fd0f-482a-8163-6eef3dbcb236
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 0%

---

# 将Facebook自定义受众添加为LaunchPoint服务 {#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**需要管理员权限**

通过此集成，您可以将受众数据从Marketo静态和智能列表发送到Facebook，以用作Facebook广告促销活动中的自定义受众。 下面是如何设置它。

1. 转到Marketo **管理员**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. 转到 **LaunchPoint**，单击 **新建** 选择 **新服务**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. 输入 **显示名称** 为您的服务选择 **Facebook自定义受众** 服务 **服务** 下拉菜单。

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. 在同一浏览器中打开新选项卡，然后转到 [facebook.com](https://www.facebook.com/). 使用您要用于集成的帐户登录Facebook。

   >[!CAUTION]
   >
   >为了让Marketo跨多个广告管理器帐户发送受众，您在以下步骤中授权的Facebook用户需要有权访问 *全部* 这些账户中。

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. 登录Facebook后，返回Marketo。 单击 **授权**.

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >您 _必须_ 使用Facebook Business Manager帐户，以便您的自定义受众集成正常工作。 要了解如何设置Business Manager帐户，请参阅 [Facebook帮助](https://www.facebook.com/business/help/1710077379203657).

1. 如果出现提示，请单击 **确定** 接受将Marketo应用程序安装到Facebook中。

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. 你现在被授权了！ 选择匹配模式并单击 **创建**.

   >[!NOTE]
   >
   >**基本匹配** 仅使用电子邮件地址。 **高级匹配** 使用另外七个字段（这会增加匹配率）进行更多转化。 但是，如果贵公司的隐私政策不允许共享其他字段，或者如果您的数据不包含这些字段，请选择“基本匹配”。

   ![](assets/fb-custom-adv-matching-hands.png)

   干得好！ 您现在可以转到Marketo中的任何静态或智能列表，并将受众数据发送到Facebook。

   >[!CAUTION]
   >
   >你走之前，一定要 [接受Facebook的自定义受众条款](https://www.facebook.com/ads/manage/customaudiences/tos.php) 在你的Facebook账户里！ 否则，受众更新将失败。

>[!MORELIKETHIS]
>
>* [在Facebook中创建自定义受众](/help/marketo/product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md)
>
>* [设置Facebook潜在客户广告](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)

