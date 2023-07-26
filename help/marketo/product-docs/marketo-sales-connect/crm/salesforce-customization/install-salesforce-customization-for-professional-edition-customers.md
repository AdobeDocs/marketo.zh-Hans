---
unique-page-id: 27656223
description: 安装面向Professional Edition客户的Salesforce Customization - Marketo文档 — 产品文档
title: 为Professional Edition客户安装Salesforce Customization
exl-id: dc004a28-b580-4449-9fde-e744681ac53a
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# 为Professional Edition客户安装Salesforce Customization {#install-salesforce-customization-for-professional-edition-customers}

拥有Salesforce Professional Edition的客户必须按照以下步骤安装自定义。

>[!PREREQUISITES]
>
>* Sales Connect管理员需要连接他们的Salesforce和Sales Connect帐户。
>* 使用的Salesforce实例需要具有空间来安装十三个自定义活动字段。

## 安装 {#installation}

1. 在Sales Connect中，单击右上角的齿轮图标，然后选择 **设置**.

   ![](assets/one-4.png)

1. 在管理设置下，单击 **Salesforce**.

   ![](assets/two-4.png)

1. 验证您是否连接到Salesforce帐户。

   >[!CAUTION]
   >
   >如果已连接，您将看到绿色的“安装”按钮。 **不要** 单击此按钮，改为继续执行步骤4。

1. 登录到您连接的Salesforce帐户，然后单击 [此链接](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t0b000001oWEZ).
1. 您将被发送到Sales Connect安装页面。

   ![](assets/install-package.png)

1. 选择要为其安装自定义设置的用户：仅限管理员、所有用户或特定配置文件。
1. 单击 **安装** 按钮以安装自定义。
1. 要确认安装成功，请登录到您的Salesforce帐户。
1. 单击 **设置**，在搜索栏中搜索“已安装的包”，然后单击 **已安装的包**.

   您将在其中看到Marketo Sales Connect自定义设置。

   要在Salesforce实例中配置Sales Connect，请按照《安装指南》第7页的“配置SALES ENGAGE SALESFORCE包”一节中所述的步骤操作。

   >[!NOTE]
   >
   >Sales Engage是以前的Sales Connect名称。

## 指南 {#guides}

[Salesforce Classic安装指南](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf)

[Salesforce Lightning安装指南](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf)
