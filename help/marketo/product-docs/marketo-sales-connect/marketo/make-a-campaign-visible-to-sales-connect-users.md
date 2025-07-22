---
unique-page-id: 14745655
description: 使营销活动对Sales Connect用户可见 — Marketo文档 — 产品文档
title: 使营销活动对Sales Connect用户可见
exl-id: 1fde53e3-2764-4e4b-897f-635b78534133
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '96'
ht-degree: 2%

---

# 使营销活动对[!DNL Sales Connect]用户可见 {#make-a-campaign-visible-to-sales-connect-users}

只有当营销活动可见时，才能共享它们。 以下是具体操作方法。

1. 选择（或创建）要共享的Campaign。

   ![](assets/make-a-marketing-campaign-visible-msc-1.png)

1. 单击&#x200B;**[!UICONTROL Smart List]**&#x200B;选项卡。

   ![](assets/make-a-marketing-campaign-visible-msc-2.png)

1. 添加[!UICONTROL Campaign is Requested]触发器。

   ![](assets/make-a-marketing-campaign-visible-msc-3.png)

1. 对于源，请选择“[!UICONTROL is]”**[!UICONTROL Web Service API]**。

   ![](assets/make-a-marketing-campaign-visible-msc-4.png)

1. 单击&#x200B;**[!UICONTROL Flow]**&#x200B;选项卡。

   ![](assets/make-a-marketing-campaign-visible-msc-5.png)

1. 添加[!UICONTROL Interesting Moment]流程操作。

   ![](assets/make-a-marketing-campaign-visible-msc-6.png)

1. 对于 [!UICONTROL Type]，选择 **[!UICONTROL Web]**。

   ![](assets/make-a-marketing-campaign-visible-msc-7.png)

1. 在[!UICONTROL Description]框中，向您的销售团队写入一条消息。 在此示例中，我们使用令牌指定填写的表单。

   ![](assets/make-a-marketing-campaign-visible-msc-8.png)

1. 单击&#x200B;**[!UICONTROL Schedule]**&#x200B;选项卡，然后单击&#x200B;**[!UICONTROL Activate]**&#x200B;营销活动。

   ![](assets/make-a-marketing-campaign-visible-msc-9.png)
