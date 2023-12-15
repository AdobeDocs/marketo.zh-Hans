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

1. 转到Marketo **[!UICONTROL 管理员]**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. 转到 **[!UICONTROL 启动点]**，单击 **[!UICONTROL 新建]** 并选择 **[!UICONTROL 新建服务]**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. 输入 **[!UICONTROL 显示名称]** ，然后选择 **[!UICONTROL facebook自定义受众]** 来自的服务 **[!UICONTROL 服务]** 下拉菜单。

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. 在同一浏览器中打开新选项卡，然后转到 [facebook.com](https://www.facebook.com/){target="_blank"}. 使用要用于集成的帐户登录Facebook。

   >[!CAUTION]
   >
   >为了使Marketo能够跨多个Ad Manager帐户发送受众，您在以下步骤中授权的Facebook用户需要有权访问 *所有* 这些账号的。

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. 登录Facebook后，请返回Marketo。 单击 **[!UICONTROL 授权]**.

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >您 _必须_ 使用Facebook Business Manager帐户以使您的自定义受众集成正常工作。 要了解如何设置业务经理帐户，请参阅 [facebook帮助](https://www.facebook.com/business/help/1710077379203657){target="_blank"}.

1. 如果出现提示，请单击 **[!UICONTROL 确定]** ，以接受将Marketo应用程序安装到Facebook中。

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. 您现在已获得授权！ 选择匹配模式并单击 **[!UICONTROL 创建]**.

   >[!NOTE]
   >
   >**基本匹配** 仅使用电子邮件地址。 **高级匹配** 使用七个额外的字段，这会提高匹配率，以实现更多转化。 但是，如果贵公司的隐私政策不允许共享其他字段，或者您的数据不包含这些字段，请选择“基本匹配”。

   ![](assets/fb-custom-adv-matching-hands.png)

   做得好！您现在可以转到Marketo中的任何静态列表或智能列表，并将受众数据发送到Facebook。

   >[!CAUTION]
   >
   >在你走之前，请确保 [接受Facebook的自定义受众术语](https://www.facebook.com/ads/manage/customaudiences/tos.php){target="_blank"} 在您的Facebook帐户中！ 否则，受众更新将失败。

>[!MORELIKETHIS]
>
>* [在Facebook中创建自定义受众](/help/marketo/product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md){target="_blank"}
>
>* [设置Facebook潜在客户广告](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md){target="_blank"}
