---
unique-page-id: 4720257
description: 将Facebook自定义受众添加为LaunchPoint服务 — Marketo Docs — 产品文档
title: 将Facebook自定义受众添加为LaunchPoint服务
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 0%

---


# 将Facebook自定义受众添加为LaunchPoint服务{#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**需要管理权限**

通过此集成，您可以将受众数据从Market发送到静态列表和智能，并将其用作Facebook广告活动中的自定义受众。 下面是设置方法。

1. 转至Marketo **Admin**。

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. 转至&#x200B;**LaunchPoint**，单击&#x200B;**新建**&#x200B;并选择&#x200B;**新建服务**。

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. 为您的服务输入&#x200B;**显示名称**，然后从&#x200B;**服务**&#x200B;下拉菜单中选择&#x200B;**Facebook自定义受众**&#x200B;服务。

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. 在同一浏览器中打开新选项卡并转到[facebook.com](https://www.facebook.com/)。 使用要用于集成的帐户登录Facebook。

   >[!CAUTION]
   >
   >为了Market能够在多个广告管理器帐户中发送受众，您在以下步骤授权的Facebook用户需要有权访问这些帐户的&#x200B;*所有*。

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. 登录Facebook后，返回Marketo。 单击&#x200B;**授权**。

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >您&#x200B;_必须_&#x200B;使用Facebook Business Manager帐户，以便您的自定义受众集成正常工作。 要了解如何设置Business Manager帐户，请参阅[Facebook帮助](https://www.facebook.com/business/help/1710077379203657)。

1. 如果出现提示，请单击&#x200B;**确定**&#x200B;接受Marketo应用程序安装到Facebook中。

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. 你现在被授权了！ 选择匹配模式，然后单击&#x200B;**创建**。

   >[!NOTE]
   >
   >**基本匹** 配仅使用电子邮件地址。**高级** 匹配使用七个附加字段，可提高匹配率以实现更多转换。但是，如果公司的隐私策略不允许共享其他字段，或者您的数据不包括这些字段，请选择“基本匹配”。

   ![](assets/fb-custom-adv-matching-hands.png)

   干得好！ 您现在可以转到Marketo中的任何静态或智能列表，并将受众数据发送到Facebook。

   >[!CAUTION]
   >
   >哦，在您离开之前，请务必在您的Facebook帐户中[接受Facebook的自定义受众条款](https://www.facebook.com/ads/manage/customaudiences/tos.php)! 否则，受众更新将失败。

>[!MORELIKETHIS]
>
>* [在Facebook中创建自定义受众](/help/marketo/product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md)
   >
   >
* [设置Facebook潜在客户广告](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)

