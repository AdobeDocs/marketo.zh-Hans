---
unique-page-id: 37355602
description: 在Marketo Dynamics Online中安装和配置Microsoft Sales Insight - Marketo文档 — 产品文档
title: 在Microsoft Dynamics Online中安装和配置Marketo Sales Insight
exl-id: 3b58b109-96f9-427e-be5c-a8db270ffe69
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# 在Microsoft Dynamics Online中安装和配置Marketo Sales Insight {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online}

Marketo Sales Insight是一款非常棒的工具，可为您的销售团队提供一个了解营销团队拥有的大量数据的“窗口”。 以下是如何在Microsoft Dynamics Online中安装和配置该组件的。

>[!PREREQUISITES]
>
>完成Marketo-Microsoft集成。
>
>[下载适用于您的Microsoft Dynamics CRM版本的正确解决方案](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md)。

## 导入解决方案 {#import-solution}

>[!NOTE]
>
>如果您使用的是统一界面，请在下面的步骤1之前，单击右上角的“设置”图标，然后选择&#x200B;**高级设置**。

1. 在Microsoft Dynamics CRM下，单击&#x200B;**设置**。

   ![](assets/image2014-12-12-9-3a4-3a56-1.png)

1. 在“设置”下，单击&#x200B;**自定义项**。

   ![](assets/image2015-4-29-14-3a22-3a1-1.png)

1. 单击&#x200B;**解决方案**。

   ![](assets/image2014-12-12-9-3a5-3a17-1.png)

   >[!NOTE]
   >
   >在继续下一步之前，您应该已经安装和配置了Marketo解决方案。

1. 单击&#x200B;**导入**。

   ![](assets/image2014-12-12-9-3a5-3a27-1.png)

1. 在新窗口中，单击&#x200B;**浏览**。

   ![](assets/image2014-12-12-9-3a5-3a36-1.png)

1. 在您的计算机上，查找并安装刚刚下载的解决方案。

1. 单击&#x200B;**下一步**。

   ![](assets/seven.png)

1. 将上传解决方案。 您可以查看文件包的内容（如果需要）。 单击&#x200B;**下一步**。

   ![](assets/image2014-12-12-9-3a6-3a10-1.png)

1. 确保选中此框并单击&#x200B;**导入**。

   ![](assets/image2014-12-12-9-3a6-3a19-1.png)

1. 欢迎下载日志文件，然后单击&#x200B;**关闭**。

   ![](assets/image2014-12-12-9-3a6-3a29-1.png)

1. 太棒了！ 您现在应该看到解决方案。 如果不存在，请刷新屏幕。

   ![](assets/eleven.png)

1. 单击&#x200B;**Publish自定义**。

   >[!NOTE]
   >
   >确保启用全局MS Dynamics同步。

## 连接Marketo和Sales Insight {#connect-marketo-and-sales-insight}

让我们将您的Marketo实例关联到Dynamics中的Sales Insight。 方法如下：

>[!NOTE]
>
>**需要管理员权限**

1. 登录Marketo并转到&#x200B;**管理员**&#x200B;部分。

   ![](assets/image2014-12-12-9-3a6-3a50-1.png)

1. 在“销售分析”部分下，单击&#x200B;**编辑API配置**。

   ![](assets/image2014-12-12-9-3a7-3a0-1.png)

1. 复制&#x200B;**Marketo主机**、**API URL**&#x200B;和&#x200B;**API用户ID**&#x200B;以便在以后的步骤中使用。 输入您选择的API密钥，然后单击&#x200B;**保存**。

   >[!CAUTION]
   >
   >请勿在API密钥中使用&amp;符号。

   ![](assets/image2014-12-12-9-3a7-3a9-1.png)

   >[!NOTE]
   >
   >以下字段必须与&#x200B;_潜在客户和联系人_&#x200B;的Marketo同步，Sales Insight才能正常工作：
   >
   >* 优先级
   >* 紧急
   >* 相对分数
   >
   >如果缺少这些字段中的任何一个，您将在Marketo中看到一条错误消息，其中包含缺少的字段的名称。 若要解决此问题，请执行[此过程](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md)。

1. 返回Microsoft Dynamics，转到&#x200B;**设置**。

   ![](assets/image2014-12-12-9-3a7-3a25-1.png)

1. 在&#x200B;**设置**&#x200B;下，单击&#x200B;**Marketo API配置**。

   ![](assets/image2014-12-12-9-3a7-3a34-1.png)

1. 单击&#x200B;**新建**。

   ![](assets/image2014-12-12-9-3a8-3a8-1.png)

1. 输入您之前从Marketo获取的信息，然后单击&#x200B;**保存**。

   ![](assets/image2014-12-12-9-3a8-3a17-1.png)

## 启用同步 {#enable-sync}

1. 在Marketo中，单击&#x200B;**管理员**。

   ![](assets/enable-one.png)

1. 在集成下，选择&#x200B;**Microsoft Dynamics**。

   ![](assets/enable-two.png)

1. 单击&#x200B;**启用同步**。

   ![](assets/enable-three.png)

1. 单击字段同步详细信息旁边的&#x200B;**编辑**。

   ![](assets/enable-four.png)

1. 这将&#x200B;_自动_&#x200B;选择以前禁用的MSI字段（紧急程度、相对分数和优先级）。 只需单击&#x200B;**保存**&#x200B;即可开始同步数据。

   ![](assets/enable-five.png)

## 设置用户访问权限 {#set-user-access}

最后，您必须授予特定用户使用Marketo Sales Insight的权限。

1. 转到&#x200B;**设置**。

   ![](assets/image2014-12-12-9-3a8-3a34-1.png)

1. 转到&#x200B;**安全性**。

   ![](assets/image2015-4-29-14-3a56-3a33-1.png)

1. 单击&#x200B;**用户**。

   ![](assets/image2015-4-29-14-3a57-3a46-1.png)

1. 选择要授予Sales Insight访问权限的用户，然后单击&#x200B;**管理角色**。

   ![](assets/image2015-4-29-14-3a59-3a31-1.png)

1. 选择Marketo Sales Insight角色，然后单击&#x200B;**确定**。

   ![](assets/image2014-12-12-9-3a9-3a22-1.png)

   你应该都做完了！ 最后，要进行测试，请以有权访问Marketo Sales Insight的用户身份登录Dynamics，并查看潜在客户或联系人。

   ![](assets/image2015-4-29-15-3a2-3a27-1.png)

>[!MORELIKETHIS]
>
>[为潜在客户/联系人记录设置星星和火焰](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
