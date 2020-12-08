---
unique-page-id: 4720257
description: 将Facebook自定义受众添加为LaunchPoint服务- Marketo Docs —— 产品文档
title: 将Facebook自定义受众添加为LaunchPoint服务
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---


# 将Facebook自定义受众添加为LaunchPoint服务 {#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**需要管理员权限**

通过此集成，您可以将受众数据从Market发送到静态列表和智能受众到Facebook，以用作Facebook广告活动中的自定义。 下面介绍如何设置。

1. 转到Marketto **Admin**。

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. 转到 **LaunchPoint**，单击“新 **建”** ，然后选 **择“新建服务**”。

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. 为您的 **服务输入** “显示名称”，并从“服 **务”下拉框中选** 择“Facebook自定义 **受众** ”服务。

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. 在同一浏览器中打开新选项卡并转 [到www.facebook.com。](http://www.facebook.com./) 使用要用于集成的帐户登录Facebook。

   >[!CAUTION]
   >
   >为了使Market能够在多个广告管理者帐户中发送受众，您通过以下步骤授权的Facebook用户需要有权访问 *所* 有这些帐户。

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. 登录Facebook后，返回Marketo。 单击 **授权**。

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >您必 *须使* 用Facebook业务经理帐户，以便您的自定义受众集成能够正常工作。 要了解如何设置业务经理帐户，请参阅Facebook [帮助](https://www.facebook.com/business/help/1710077379203657)。

1. 如果出现提示，请单击**确定**接受Marketo应用程序安装到Facebook中。

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. 你现在被授权了！ 选择匹配模式，然后单击“ **创建**”。

   >[!NOTE]
   >
   >**基本匹配**&#x200B;仅使用电子邮件地址。**“高级匹配** ”使用七个附加字段，这增加了匹配率，以便进行更多转换。 但是，如果公司的隐私策略不允许共享其他字段，或者数据不包含这些字段，请选择“基本匹配”。

   ![](assets/fb-custom-adv-matching-hands.png)

   干得好！ 您现在可以转到Market中的任何静态或智能列表，并将受众数据发送到Facebook。

   >[!CAUTION]
   >
   >哦，在您离开之前，请务必在 [您的Facebook帐户中接受Facebook](https://www.facebook.com/ads/manage/customaudiences/tos.php) 的自定义受众条款！ 否则，受众更新将失败。

>[!NOTE]
>
>**相关文章**
>
>* [在Facebook中创建自定义受众](../../../product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md)
   >
   >
* [设置Facebook潜在客户广告](../../../product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)

>



