---
unique-page-id: 27656223
description: 为Professional Edition客户安装Salesforce自定义- Marketo文档——产品文档
title: 为Professional Edition客户安装Salesforce自定义
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---


# 为Professional Edition客户安装Salesforce自定义{#install-salesforce-customization-for-professional-edition-customers}

使用Salesforce Professional Edition的客户必须按照以下步骤安装自定义。

>[!PREREQUISITES]
>
>* 销售连接管理员需要连接其Salesforce和销售连接帐户。
>* 使用的Salesforce实例需要有空间来安装十三个自定义活动字段。


## 安装{#installation}

1. 在Sales Connect中，单击右上角的齿轮图标，然后选择&#x200B;**设置**。

   ![](assets/one-4.png)

1. 在“管理员设置”下，单击&#x200B;**Salesforce**。

   ![](assets/two-4.png)

1. 验证是否已连接到您的Salesforce帐户。

   >[!CAUTION]
   >
   >如果已连接，您将看到绿色的“安装”按钮。 **请勿** 单击此按钮，请改为继续执行步骤4。

1. 登录到您连接的Salesforce帐户，然后单击[此链接](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t0b000001oWEZ)。
1. 您将被发送到Sales Connect安装页面。

   ![](assets/install-package.png)

1. 选择要为以下用户安装自定义项的用户：仅限管理员、所有用户或特定用户档案。
1. 单击&#x200B;**安装**&#x200B;按钮以安装自定义。
1. 要确认安装成功，请登录您的Salesforce帐户。
1. 单击“**安装程序**”，在搜索栏中搜索“已安装的包”，然后单击“已安装的包”。****

   您将在此处看到Marketo Sales Connect自定义。

   要在Salesforce实例中配置Sales Connect，请按照安装指南第7页“配置SALES ENGAGE SALESFORCE包”部分中的步骤开始。

   >[!NOTE]
   >
   >Sales Engage是Sales Connect的以前名称。

## 参考线{#guides}

[Salesforce Classic安装指南](http://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf)

[Salesforce Lightning安装指南](http://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf)
