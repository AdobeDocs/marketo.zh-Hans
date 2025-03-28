---
unique-page-id: 3571737
description: 在Marketo Dynamics 2013中安装和配置Microsoft Sales Insight - Marketo文档 — 产品文档
title: 在Microsoft Dynamics 2013中安装和配置Marketo Sales Insight
exl-id: 290db451-47a6-4cfa-a36f-bc12ef7d3482
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 0%

---

# 在Microsoft Dynamics 2013中安装和配置Marketo Sales Insight {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight是一款非常棒的工具，可为您的销售团队提供一个了解营销团队拥有的大量数据的“窗口”。 下面是如何安装和配置它的。

>[!PREREQUISITES]
>
>完成Marketo-Microsoft集成。
>
>[下载适用于您的Microsoft Dynamics CRM版本的正确解决方案](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md)。

## 导入解决方案 {#import-solution}

好，现在可以将Marketo Sales Insight解决方案导入Microsoft Dynamics了。

1. 在&#x200B;**Microsoft Dynamics CRM**&#x200B;下，单击&#x200B;**设置**。

   ![](assets/image2014-12-12-9-3a4-3a56.png)

1. 在&#x200B;**设置**&#x200B;下，单击&#x200B;**自定义项**。

   ![](assets/image2014-12-12-9-3a5-3a6.png)

1. 单击&#x200B;**解决方案**。

   ![](assets/image2014-12-12-9-3a5-3a17.png)

   >[!NOTE]
   >
   >在继续下一步之前，您应该已经安装和配置了Marketo

1. 单击&#x200B;**导入**。

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. 在新窗口中，单击&#x200B;**浏览**。

   ![](assets/image2014-12-12-9-3a5-3a36.png)

1. 查找并选择您在上面下载的解决方案。

   ![](assets/image2014-12-12-9-3a5-3a45.png)

1. 单击&#x200B;**下一步**。

   ![](assets/image2014-12-12-9-3a5-3a55.png)

1. 将上传解决方案。 您可以查看文件包的内容（如果需要）。 单击&#x200B;**下一步**。

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. 确保选中此框并单击&#x200B;**导入**。

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. 您可以随时下载日志文件。 单击&#x200B;**关闭**。

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. 太棒了！ 您现在应该看到解决方案。 如果不存在，请刷新屏幕。

   ![](assets/image2014-12-12-9-3a6-3a40.png)

## 连接Marketo和Sales Insight {#connect-marketo-and-sales-insight}

让我们将您的Marketo实例关联到Dynamics中的Sales Insight。

>[!NOTE]
>
>需要管理员权限。

1. 登录到Marketo，然后转到&#x200B;**管理员**&#x200B;部分。

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. 在&#x200B;**销售分析**&#x200B;部分下，单击&#x200B;**编辑API配置**。

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. 复制&#x200B;**Marketo主机**、**API URL**&#x200B;和&#x200B;**API用户ID**&#x200B;以便在以后的步骤中使用。 输入您选择的&#x200B;**API密钥**，然后单击&#x200B;**保存**。

   >[!CAUTION]
   >
   >请勿在API密钥中使用&amp;符号。

   ![](assets/image2014-12-12-9-3a7-3a9.png)

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

   ![](assets/image2014-12-12-9-3a7-3a25.png)

1. 在&#x200B;**设置**&#x200B;下，单击&#x200B;**Marketo API配置**。

   ![](assets/image2014-12-12-9-3a7-3a34.png)

1. 单击&#x200B;**新建**。

   ![](assets/image2014-12-12-9-3a8-3a8.png)

1. 输入您之前从Marketo获取的信息，然后单击&#x200B;**保存**。

   ![](assets/image2014-12-12-9-3a8-3a17.png)

## 设置用户访问权限 {#set-user-access}

最后，您还可以为特定用户提供访问Marketo Sales Insight的权限。

1. 转到&#x200B;**设置**。

   ![](assets/image2014-12-12-9-3a8-3a34.png)

1. 单击&#x200B;**用户**。

   ![](assets/image2014-12-12-9-3a8-3a42.png)

1. 选择要授予Sales Insight访问权限的用户，然后单击&#x200B;**管理角色**。

   ![](assets/image2014-12-12-9-3a9-3a13.png)

1. 选择&#x200B;**Marketo销售分析**&#x200B;角色，然后单击&#x200B;**确定**。

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   你应该都做完了！ 最后，要进行测试，请以有权访问Marketo Sales Insight的用户身份登录到Dynamics，然后查看潜在客户或联系人。

   ![](assets/image2014-12-12-9-3a9-3a31.png)

您现在已为销售团队解锁了Marketo Sales Insight的强大功能。

>[!MORELIKETHIS]
>
>[为潜在客户/联系人记录设置星星和火焰](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
