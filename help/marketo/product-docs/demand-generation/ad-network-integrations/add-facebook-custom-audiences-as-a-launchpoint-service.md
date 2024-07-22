---
unique-page-id: 4720257
description: 将Facebook自定义受众添加为LaunchPoint服务 — Marketo文档 — 产品文档
title: 将Facebook自定义受众添加为LaunchPoint Service
exl-id: 5c5b5c80-fd0f-482a-8163-6eef3dbcb236
feature: Integrations
source-git-commit: bebf61037f37a06b40b4d9c1df872f1cf62a1403
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---

# 将Facebook自定义受众添加为LaunchPoint Service {#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**需要管理员权限**

利用此集成，您可以将受众数据从Marketo Engage静态列表和智能列表发送到Facebook，以在Facebook广告促销活动中用作自定义受众。 下面是设置方法。

1. 转到Marketo **[!UICONTROL 管理员]**。

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. 转到&#x200B;**[!UICONTROL LaunchPoint]**，单击&#x200B;**[!UICONTROL 新建]**，然后选择&#x200B;**[!UICONTROL 新建服务]**。

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. 为您的服务输入&#x200B;**[!UICONTROL 显示名称]**，然后从&#x200B;**[!UICONTROL 服务]**&#x200B;下拉列表中选择&#x200B;**[!UICONTROL Facebook自定义受众]**&#x200B;服务。

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. 在同一浏览器中打开一个新选项卡，然后转到[facebook.com](https://www.facebook.com/){target="_blank"}。 使用要用于集成的帐户登录Facebook。

   >[!CAUTION]
   >
   >为了使Marketo能够跨多个Ad Manager帐户发送受众，您在以下步骤中授权的Facebook用户需要有权访问这些帐户中的&#x200B;*所有*。

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. 登录Facebook后，请返回Marketo。 单击&#x200B;**[!UICONTROL 授权]**。

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >您&#x200B;_必须_&#x200B;使用Facebook Business Manager帐户才能使自定义受众集成正常工作。 要了解如何设置Business Manager帐户，请参阅[Facebook帮助](https://www.facebook.com/business/help/1710077379203657){target="_blank"}。

1. 如果出现提示，请单击&#x200B;**[!UICONTROL 确定]**&#x200B;接受Marketo应用程序安装到Facebook中。

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. 您现在已获得授权！ 选择匹配模式并单击&#x200B;**[!UICONTROL 创建]**。

   >[!NOTE]
   >
   >**基本匹配**&#x200B;仅使用电子邮件地址。 **高级匹配**&#x200B;使用七个额外的字段，这些字段提高了匹配率，从而提高了转化率。 但是，如果贵公司的隐私政策不允许共享其他字段，或者您的数据不包含这些字段，请选择“基本匹配”。

   ![](assets/fb-custom-adv-matching-hands.png)

   做得好！您现在可以转到Marketo中的任何静态列表或智能列表，并将受众数据发送到Facebook。

   >[!CAUTION]
   >
   >哦，开始之前，请确保在您的Facebook帐户中[接受Facebook的自定义受众条款](https://www.facebook.com/ads/manage/customaudiences/tos.php){target="_blank"}！ 否则，受众更新将失败。

>[!MORELIKETHIS]
>
>* [在Facebook中创建自定义受众](/help/marketo/product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md){target="_blank"}
>
>* [设置Facebook潜在客户广告](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md){target="_blank"}
