---
unique-page-id: 4720257
description: 将Facebook自定义受众添加为LaunchPoint服务- Marketo Docs —— 产品文档
title: 将Facebook自定义受众添加为LaunchPoint服务
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---


# 将Facebook自定义受众添加为LaunchPoint服务{#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**需要管理员权限**

通过此集成，您可以将受众数据从Market发送到静态列表和智能受众到Facebook，以用作Facebook广告活动中的自定义。 下面介绍如何设置。

1. 转到Marketo **Admin**。

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. 转至&#x200B;**LaunchPoint**，单击&#x200B;**新建**&#x200B;并选择&#x200B;**新建服务**。

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. 为您的服务输入&#x200B;**显示名称**，并从&#x200B;**服务**&#x200B;下拉列表中选择&#x200B;**Facebook自定义受众**&#x200B;服务。

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. 在同一浏览器中打开新选项卡并转到[www.facebook.com。](http://www.facebook.com./) 使用要用于集成的帐户登录Facebook。

   >[!CAUTION]
   >
   >为了使Market能够在多个广告管理器帐户中发送受众，您在以下步骤授权的Facebook用户需要有权访问这些帐户的&#x200B;*all*。

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. 登录Facebook后，返回Marketo。 单击&#x200B;**授权**。

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >您&#x200B;*必须*&#x200B;使用Facebook Business Manager帐户，以便您的自定义受众集成能够正常工作。 要了解如何设置Business Manager帐户，请参阅[Facebook帮助](https://www.facebook.com/business/help/1710077379203657)。

1. 如果出现提示，请单击**确定**接受Marketo应用程序安装到Facebook中。

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. 你现在被授权了！ 选择匹配模式，然后单击&#x200B;**创建**。

   >[!NOTE]
   >
   >**基本匹配**&#x200B;仅使用电子邮件地址。**高级** 匹配使用七个附加字段，这增加了匹配率，以便进行更多转换。但是，如果公司的隐私策略不允许共享其他字段，或者数据不包含这些字段，请选择“基本匹配”。

   ![](assets/fb-custom-adv-matching-hands.png)

   干得好！ 您现在可以转到Market中的任何静态或智能列表，并将受众数据发送到Facebook。

   >[!CAUTION]
   >
   >哦，在您离开之前，请务必在您的Facebook帐户中[接受Facebook的自定义受众条款](https://www.facebook.com/ads/manage/customaudiences/tos.php)! 否则，受众更新将失败。

>[!MORELIKETHIS]
>
>* [在Facebook中创建自定义受众](../../../product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md)
   >
   >
* [设置Facebook潜在客户广告](../../../product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)

>



