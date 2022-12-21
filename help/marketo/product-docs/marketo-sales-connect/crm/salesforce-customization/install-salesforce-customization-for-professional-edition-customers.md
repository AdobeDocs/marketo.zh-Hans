---
unique-page-id: 27656223
description: 为专业版客户安装Salesforce自定义 — Marketo文档 — 产品文档
title: 为Professional Edition客户安装Salesforce自定义
exl-id: dc004a28-b580-4449-9fde-e744681ac53a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# 为Professional Edition客户安装Salesforce自定义 {#install-salesforce-customization-for-professional-edition-customers}

使用Salesforce Professional Edition的客户必须按照这些步骤来安装自定义设置。

>[!PREREQUISITES]
>
>* Sales Connect管理员需要连接其Salesforce和Sales Connect帐户。
>* 使用的Salesforce实例需要有空间才能安装十三个自定义活动字段。


## 安装 {#installation}

1. 在Sales Connect中，单击右上角的齿轮图标，然后选择 **设置**.

   ![](assets/one-4.png)

1. 在“管理员设置”下，单击 **Salesforce**.

   ![](assets/two-4.png)

1. 验证您是否已连接到Salesforce帐户。

   >[!CAUTION]
   >
   >如果已连接，您将看到绿色的“安装”按钮。 **不要** 单击此按钮，改为继续执行步骤4。

1. 登录到您连接到的Salesforce帐户，然后单击 [此链接](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t0b000001oWEZ).
1. 您将被发送到Sales Connect安装页面。

   ![](assets/install-package.png)

1. 选择要为以下项安装自定义设置的用户：仅限管理员、所有用户或特定用户档案。
1. 单击 **安装** 按钮以安装自定义设置。
1. 要确认安装成功，请登录到您的Salesforce帐户。
1. 单击 **设置**，在搜索栏中搜索“已安装的包”，然后单击 **已安装的包**.

   您将在此处看到Marketo Sales Connect自定义设置。

   要在Salesforce实例中配置Sales Connect，请按照《安装指南》第7页中“配置SALES ENGAGE SALESFORCE包”部分开始的步骤操作。

   >[!NOTE]
   >
   >Sales Engage是Sales Connect的先前名称。

## 指南 {#guides}

[适用于Salesforce Classic的安装指南](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf)

[Salesforce Lightning安装指南](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf)
