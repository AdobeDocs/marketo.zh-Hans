---
unique-page-id: 4720257
description: 添加 [!DNL Facebook] 自定义受众作为 [!DNL LaunchPoint] 服务 — Marketo文档 — 产品文档
title: 将 [!DNL Facebook] 自定义受众添加为 [!DNL LaunchPoint] 服务
exl-id: 5c5b5c80-fd0f-482a-8163-6eef3dbcb236
feature: Integrations
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 1%

---

# 将[!DNL Facebook]自定义受众添加为[!DNL LaunchPoint]服务 {#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**需要管理员权限**

通过此集成，您可以将受众数据从Marketo静态列表和智能列表发送到[!DNL Facebook]，以在[!DNL Facebook]广告营销活动中用作自定义受众。 下面是设置方法。

1. 转到Marketo **[!UICONTROL Admin]**。

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. 转到&#x200B;**[!UICONTROL LaunchPoint]**，单击&#x200B;**[!UICONTROL New]**&#x200B;并选择&#x200B;**[!UICONTROL New Service]**。

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. 为您的服务输入&#x200B;**[!UICONTROL Display Name]**，然后从&#x200B;**[!UICONTROL Facebook Custom Audiences]**&#x200B;下拉列表中选择&#x200B;**[!UICONTROL Service]**&#x200B;服务。

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. 在同一浏览器中打开一个新选项卡，然后转到[facebook.com](https://www.facebook.com/)。 使用要用于集成的帐户登录[!DNL Facebook]。

   >[!CAUTION]
   >
   >为了使Marketo能够跨多个广告管理器帐户发送受众，您在以下步骤中授权的[!DNL Facebook]用户需要有权访问这些帐户中的&#x200B;*所有*&#x200B;帐户。

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. 登录[!DNL Facebook]后，返回Marketo。 单击 **[!UICONTROL Authorize]**。

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >您&#x200B;_必须_&#x200B;使用[!DNL Facebook] Business Manager帐户才能使您的自定义受众集成正常工作。 要了解如何设置Business Manager帐户，请参阅[[!DNL Facebook] 帮助](https://www.facebook.com/business/help/1710077379203657)。

1. 如果出现提示，请单击&#x200B;**[!UICONTROL OK]**&#x200B;接受Marketo应用程序安装到[!DNL Facebook]中。

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. 您现在已获得授权！ 选择匹配模式并单击&#x200B;**[!UICONTROL Create]**。

   >[!NOTE]
   >
   >**[!UICONTROL Basic Matching]**&#x200B;仅使用电子邮件地址。 **[!UICONTROL Advanced Matching]**&#x200B;使用七个额外的字段，这会增加匹配率，以获得更多转化。 但是，如果贵公司的隐私政策不允许共享其他字段，或者您的数据不包含这些字段，请选择[!UICONTROL Basic Matching]。

   ![](assets/fb-custom-adv-matching-hands.png)

   做得好！您现在可以转到Marketo中的任何静态列表或智能列表，并将受众数据发送到[!DNL Facebook]。

   >[!CAUTION]
   >
   >哦，开始之前，请确保在您的[帐户中 [!DNL Facebook]接受](https://www.facebook.com/ads/manage/customaudiences/tos.php)的自定义受众条款[!DNL Facebook]！ 否则，受众更新将失败。

>[!MORELIKETHIS]
>
>* [在 [!DNL Facebook]](/help/marketo/product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md)中创建自定义受众
>
>* [设置 [!DNL Facebook] 潜在客户广告](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)
