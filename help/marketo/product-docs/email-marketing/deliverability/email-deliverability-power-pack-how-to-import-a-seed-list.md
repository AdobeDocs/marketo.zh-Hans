---
unique-page-id: 10099077
description: 了解如何将种子列表导入Marketo Engage实例。
title: 电子邮件可投放性功能包 — 如何导入种子列表
exl-id: a4782611-2556-43bf-802b-afeb332eafcd
feature: Deliverability
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# 电子邮件可投放性功能包：如何导入种子列表 {#email-deliverability-power-pack-how-to-import-a-seed-list}

种子列表是多个邮箱提供商(包括Google应用程序、Hotmail、Yahoo！等)的电子邮件帐户列表，用于估计收件箱投放率与垃圾邮件文件夹投放率。 以下是将该列表导入Marketo Engage实例的步骤。

>[!IMPORTANT]
>
>本文适用于目前拥有活跃珠穆朗玛峰订阅的用户。 如果您使用Inbox Tracker by Bird （以前称为MessageBird），则可以在此处[找到您的教程](/help/marketo/product-docs/email-marketing/deliverability/inbox-tracker/inbox-tracker-tutorials.md){target="_blank"}。

## 导入种子列表 {#import-a-seed-list}

1. 在“我的Marketo”中，选择&#x200B;**[!UICONTROL Deliverability Tools]**。

   ![](assets/email-deliverability-power-pack-1.png)

1. 将会打开[!DNL Everest]应用程序。 在左侧导航中，单击&#x200B;**[!UICONTROL In-Flight]**&#x200B;并选择&#x200B;**[!UICONTROL Inbox Placement]**。

   ![](assets/email-deliverability-power-pack-2.png)

1. 单击&#x200B;**[!UICONTROL Manage Seed List]**&#x200B;选项卡。

   ![](assets/email-deliverability-power-pack-3.png)

1. 单击&#x200B;**[!UICONTROL Actions]**&#x200B;下拉菜单并选择&#x200B;**[!UICONTROL Download: One Per Line]**。

   ![](assets/email-deliverability-power-pack-4.png)

   >[!NOTE]
   >
   >如果您希望[!DNL Everest]为您优化列表，请使用种子列表优化器（位于页面顶部）。

1. 导出后，该列表将在浏览器的下载文件夹中显示为.txt文件。 检索它，然后将其作为静态列表[导入](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)到您的Marketo实例中。

   ![](assets/email-deliverability-power-pack-5.png)

   >[!TIP]
   >
   >请确保以易于查找的方式命名您的列表。

   >[!CAUTION]
   >
   >您每月获得的这些收件箱投放活动数量有限。 要查看你获得的数量，请查看[!UICONTROL Subscription]中[!UICONTROL Account Settings] > [!UICONTROL Subscription]下的[!DNL Everest]部分。 要获取更多信息，请联系您的Marketo销售代表。

## 获取新种子列表 {#acquiring-new-seedlists}

您的种子列表每月可能会发生更改。 请务必定期登录Email Deliverability Power Pack并检查您的种子列表的状态。 添加新地址或需要您这端的更新时，将通过应用程序左下角的通知图标向您发出警报。

在Marketo中创建静态列表后，您可以开始向其发送以测试电子邮件的收件箱位置。
