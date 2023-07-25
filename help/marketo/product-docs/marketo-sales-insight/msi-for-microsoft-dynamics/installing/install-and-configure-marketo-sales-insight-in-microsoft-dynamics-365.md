---
unique-page-id: 3571739
description: 在Marketo Dynamics 365中安装和配置Microsoft Sales Insight - Marketo文档 — 产品文档
title: 在Microsoft Dynamics 365中安装和配置Marketo Sales Insight
exl-id: c1f06b8c-48fd-4015-9502-7c9693632589
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 在Microsoft Dynamics 365中安装和配置Marketo Sales Insight {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight是一个非常棒的工具，可为您的销售团队提供一个窗口，让您了解营销团队拥有的大量数据。 以下是如何安装和配置的。

>[!PREREQUISITES]
>
>完成Marketo-Microsoft集成。
>
>[下载正确的解决方案](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) 适用于您的Microsoft Dynamics CRM版本。

## 导入解决方案 {#import-solution}

1. 登录 [Microsoft Office 365](https://login.microsoftonline.com/).

   ![](assets/image2015-3-16-15-58-55.png)

1. 单击 ![—](assets/image2015-3-16-16-1-13.png) 菜单并选择 **CRM**.

   ![](assets/image2015-3-16-16-0-10.png)

1. 单击 ![—](assets/image2015-5-13-10-5-8.png) 菜单。 在下拉菜单中，选择 **设置**，然后选择 **解决方案**.

   ![](assets/image2015-5-13-10-4-1.png)

   >[!NOTE]
   >
   >您应该已经拥有 [已安装和配置Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md) 在继续下一步之前。

1. 单击 **导入**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. 在新窗口中，单击 **浏览**. 选择 [您在步骤1下载的Marketo Sales Insight解决方案](#msi). 单击 **下一个**.

   ![](assets/image2015-5-13-15-3a38-3a49.png)

1. 将上传解决方案。 您可以根据需要查看包内容。 单击 **下一个**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. 请务必离开此框 **已选中** 并单击 **导入**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. 欢迎您随时下载日志文件。 单击&#x200B;**关闭**。

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. 太棒了！ 您现在应该可以看到解决方案。 如果不存在，请刷新屏幕。

   ![](assets/image2015-5-13-15-3a42-3a29.png)

1. 单击 **发布所有自定义项**.

   ![](assets/image2015-11-10-11-3a15-3a40.png)

## 连接Marketo和Sales Insight {#connect-marketo-and-sales-insight}

让我们将您的Marketo实例关联到Dynamics中的Sales Insight。 方法如下：

>[!NOTE]
>
>**需要管理员权限**

1. 登录Marketo并转到 **管理员** 部分。

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. 在 **销售分析** 部分，单击 **编辑API配置**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. 复制 **Marketo主机**， **API URL** 和 **API用户ID** 以便在后续步骤中使用。 输入 **API密钥** ，然后单击 **保存**.

   >[!CAUTION]
   >
   >请勿在API密钥中使用&amp;符号。

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >以下字段必须与Marketo同步 _潜在客户和联系人_ 让Sales Insight发挥作用：
   >
   > * 优先级
   > * 紧急
   > * 相对分数
   >
   >如果缺少其中任何字段，您将在Marketo中看到一条错误消息，其中包含缺少的字段的名称。 要解决此问题，请执行 [此过程](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. 返回到Microsoft Dynamics，单击 ![](assets/image2015-5-13-15-3a49-3a19.png) 图标，然后选择 **Marketo API配置** 在下拉菜单中。

   ![](assets/image2015-5-13-16-3a4-3a1.png)

1. 单击 **默认配置**.

   ![](assets/image2015-5-13-16-3a5-3a2.png)

1. 输入您之前从Marketo复制的信息。

   ![](assets/image2015-5-13-16-3a7-3a6.png)

1. 单击 ![](assets/image2015-5-13-16-3a8-3a51.png) 图标以保存更改。

## 设置用户访问权限 {#set-user-access}

您需要授予用户使用Sales Insight的权限。

1. 单击 ![](assets/image2015-5-13-10-3a5-3a8.png) 菜单。 在下拉菜单中，选择 **设置**，然后选择 **安全性**.

   ![](assets/image2015-5-13-16-3a12-3a12.png)

1. 单击 **用户**.

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. 选择要向授予Sales Insight访问权限的用户，然后单击 **管理角色**.

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. 选择 **Marketo Sales Insight** 角色并单击 **确定**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   你该做完了！ 最后，要进行测试，请以有权访问Marketo Sales Insight的用户身份登录Dynamics，并查看潜在客户或联系人。

   ![](assets/image2015-4-29-15-3a2-3a27.png)

您现在已为销售团队解锁了Marketo Sales Insight的强大功能。

>[!MORELIKETHIS]
>
>[为潜在客户/联系人记录设置星星和火焰](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
