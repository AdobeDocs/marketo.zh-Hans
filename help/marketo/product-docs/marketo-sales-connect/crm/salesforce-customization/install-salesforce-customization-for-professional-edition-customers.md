---
unique-page-id: 27656223
description: 为Professional Edition客户安装 [!DNL Salesforce] 自定义 — Marketo文档 — 产品文档
title: 安装Professional Edition客户的 [!DNL Salesforce] 自定义
exl-id: dc004a28-b580-4449-9fde-e744681ac53a
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%

---

# 安装Professional Edition客户的[!DNL Salesforce]自定义 {#install-salesforce-customization-for-professional-edition-customers}

具有[!DNL Salesforce] Professional Edition的客户必须按照这些步骤安装自定义。

>[!PREREQUISITES]
>
>* [!DNL Sales Connect]管理员需要连接其[!DNL Salesforce]和[!DNL Sales Connect]帐户。
>* [!DNL Salesforce]使用的实例需要空间来安装13个自定义活动字段。

## 安装 {#installation}

1. 在[!DNL Sales Connect]中，单击右上角的齿轮图标，然后选择&#x200B;**[!UICONTROL Settings]**。

   ![](assets/one-4.png)

1. 在[!UICONTROL Admin Settings]下，单击&#x200B;**[!UICONTROL Salesforce]**。

   ![](assets/two-4.png)

1. 验证是否已连接到[!DNL Salesforce]帐户。

   >[!CAUTION]
   >
   >如果您已连接，则会看到绿色的“[!UICONTROL Install]”按钮。 **不要**&#x200B;单击此按钮，改为继续执行步骤4。

1. 登录到您连接到的[!DNL Salesforce]帐户，然后单击[此链接](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t0b000001oWEZ)。
1. 您将被发送到[!DNL Sales Connect]安装页面。

   ![](assets/install-package.png)

1. 选择要为其安装自定义设置的用户：仅限管理员、所有用户或特定配置文件。
1. 单击&#x200B;**[!UICONTROL Install]**&#x200B;按钮安装自定义设置。
1. 要确认安装成功，请登录到您的[!DNL Salesforce]帐户。
1. 单击&#x200B;**[!UICONTROL Setup]**，在搜索栏中搜索“已安装的包”，然后单击&#x200B;**[!UICONTROL Installed Packages]**。

   您将在其中看到Marketo Sales Connect自定义设置。

   为了在[!DNL Sales Connect]实例中配置[!DNL Salesforce]，请按照《安装指南》第7页的“配置SALES ENGAGE SALESFORCE包”一节中的步骤操作。

   >[!NOTE]
   >
   >[!DNL Sales Engage]是[!DNL Sales Connect]的前一个名称。

## 指南 {#guides}

《Salesforce Classic安装指南》[&#128279;](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf)

Salesforce Lightning的[安装指南](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf)
