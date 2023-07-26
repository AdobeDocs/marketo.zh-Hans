---
unique-page-id: 3571735
description: 在Marketo Dynamics 2011中安装和配置Microsoft Sales Insight - Marketo文档 — 产品文档
title: 在Microsoft Dynamics 2011中安装和配置Marketo Sales Insight
exl-id: 40622dcc-7129-4392-95dc-ca829c15c3a6
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 0%

---

# 在Microsoft Dynamics 2011中安装和配置Marketo Sales Insight {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight是您销售团队的一个非常棒的工具。 以下分步说明如何在Microsoft Dynamics 2011内部部署中安装和配置内部部署。

>[!PREREQUISITES]
>
>完成Marketo-Microsoft集成。
>
>[下载正确的解决方案](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) 适用于您的Microsoft Dynamics CRM版本。

## 导入解决方案 {#import-solution}

1. 登录到Microsoft Dynamics CRM。 单击 **设置** ，位于左下角菜单中。

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. 选择 **解决方案** 在树上。

   ![](assets/image2015-5-4-10-3a41-3a56.png)

1. 单击 **导入** ( ![](assets/image2015-5-4-10-3a45-3a44.png))。

   ![](assets/image2015-5-4-10-3a42-3a38.png)

   >[!NOTE]
   >
   >您应该已经拥有 [已安装并配置](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2011.md) Marketo解决方案。

1. 单击 **浏览**. 为您选择Marketo Sales Insight解决方案 [已下载](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md). 单击 **下一个**.

   ![](assets/image2015-5-4-10-3a55-3a15.png)

1. 验证解决方案的详细信息，然后单击 **下一个**.

   ![](assets/image2015-5-4-10-3a57-3a31.png)

1. 确保选中SDK消息选项。 单击 **下一个**.

   ![](assets/image2015-5-4-11-3a43-3a37.png)

1. 现在等待导入完成。

   ![](assets/image2015-5-4-11-3a0-3a58.png)

1. 单击&#x200B;**关闭**。

   ![](assets/crmhand.png)

1. Marketo Sales Insight现在将显示在解决方案列表中。 好耶！

   ![](assets/image2015-5-4-11-3a2-3a37.png)

1. 选择Marketo Sales Insight ，然后单击 **发布所有自定义项** ( ![](assets/image2015-5-4-11-3a7-3a8.png))。

   ![](assets/image2015-5-4-11-3a8-3a27.png)

## 连接Marketo和Sales Insight  {#connect-marketo-and-sales-insight}

>[!NOTE]
>
>**需要管理员权限**

1. 登录Marketo并单击 **管理员**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. 在 **销售分析** 部分单击 **编辑API配置**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. 复制 **Marketo主机**， **API URL**、和 **API用户ID** 以便在以后的步骤中使用。 输入 **API密钥** ，然后单击 **保存**.

   >[!CAUTION]
   >
   >请勿在API密钥中使用&amp;符号。

   ![](assets/image2015-5-4-11-3a16-3a3.png)

   >[!NOTE]
   >
   >以下字段必须与Marketo同步， _潜在客户和联系人_ 让Sales Insight发挥作用：
   >
   >* 优先级
   >* 紧急
   >* 相对分数
   >
   >如果缺少这些字段中的任何一个，您将在Marketo中看到一条错误消息，其中包含缺少的字段的名称。 要解决此问题，请执行 [此过程](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. 返回到Dynamics，选择 **设置**.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. 选择 **Marketo API配置** 在树上。

   ![](assets/image2015-5-4-11-3a22-3a41.png)

1. 单击 **默认配置**.

   ![](assets/image2015-5-4-11-3a26-3a10.png)

1. 输入您之前从Marketo获取的信息。

   ![](assets/image2015-5-4-11-3a27-3a16.png)

1. 单击 **保存**.

   ![](assets/image2015-5-4-11-3a28-3a13.png)

## 设置用户访问权限 {#set-user-access}

设置用户角色以授予特定用户访问Sales Insight的权限。

1. 选择 **设置**.

   ![](assets/image2015-5-4-11-3a30-3a54.png)

1. 选择 **管理** 在树上。

   ![](assets/image2015-5-4-11-3a31-3a39.png)

1. 单击 **用户**.

   ![](assets/image2015-5-4-11-3a32-3a25.png)

1. 选择要向其授予访问权限的用户，然后单击 **管理角色**.

   ![](assets/image2015-5-4-11-3a35-3a8.png)

1. 选择 **Marketo Sales Insight** 角色并单击 **确定**.

   ![](assets/image2015-5-4-11-3a36-3a59.png)

   就是这样！ 现在，所有有权访问的用户都可以在潜在客户/联系人详细信息视图中查看销售分析部分。

   ![](assets/image2015-5-4-11-3a39-3a23.png)

   恭喜！ 您现在已释放了Marketo Sales Insight的强大功能。

>[!MORELIKETHIS]
>
>[为潜在客户/联系人记录设置星星和火焰](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
