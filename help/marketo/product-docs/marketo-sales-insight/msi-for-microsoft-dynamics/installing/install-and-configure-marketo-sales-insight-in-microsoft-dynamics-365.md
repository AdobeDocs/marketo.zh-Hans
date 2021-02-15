---
unique-page-id: 3571739
description: 在Microsoft Dynamics 365中安装和配置Marketo Sales Insight - Marketo Docs — 产品文档
title: 在Microsoft Dynamics 365中安装和配置Marketo Sales Insight
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---


# 在Microsoft Dynamics 365 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}中安装和配置Marketo Sales Insight

Marketo Sales Insight是一款绝佳的工具，可让您的销售团队“了解”营销团队拥有的大量数据。 下面介绍如何安装和配置。

>[!PREREQUISITES]
>
>完成Marketo-Microsoft集成。
>
>[下载适用于](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) 您版本的Microsoft Dynamics CRM的正确解决方案。

## 导入解决方案{#import-solution}

1. 登录到[Microsoft Office 365](https://login.microsoftonline.com/)。

   ![](assets/image2015-3-16-15-58-55.png)

1. 单击![—](assets/image2015-3-16-16-1-13.png)菜单并选择&#x200B;**CRM**。

   ![](assets/image2015-3-16-16-0-10.png)

1. 单击![—](assets/image2015-5-13-10-5-8.png)菜单。 在下拉列表中，选择&#x200B;**设置**，然后选择&#x200B;**解决方案**。

   ![](assets/image2015-5-13-10-4-1.png)

   >[!NOTE]
   >
   >在前进之前，您应已安装并配置了[ Marketo解决方案](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md)。

1. 单击&#x200B;**导入**。

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. 在新窗口中，单击&#x200B;**浏览**。 选择您在步骤1](#msi)中下载的[ Marketo Sales Insight解决方案。 单击&#x200B;**下一步**。

   ![](assets/image2015-5-13-15-3a38-3a49.png)

1. 解决方案将上传。 您可以视图包内容（如果需要）。 单击&#x200B;**下一步**。

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. 确保将框&#x200B;**留下，并单击**&#x200B;导入&#x200B;**。**

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. 请随时下载日志文件。 单击&#x200B;**关闭**。

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. 太棒了！ 你现在应该看到解决方案。 如果它不在，请刷新您的屏幕。

   ![](assets/image2015-5-13-15-3a42-3a29.png)

1. 单击&#x200B;**发布所有自定义项**。

   ![](assets/image2015-11-10-11-3a15-3a40.png)

## Connect Marketo和Sales Insight {#connect-marketo-and-sales-insight}

让我们将您的Marketo实例与Dynamics中的Sales Insight绑定。 下面是具体方法：

>[!NOTE]
>
>**需要管理权限**

1. 登录Marketo并转到&#x200B;**Admin**&#x200B;部分。

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. 在&#x200B;**Sales Insight**&#x200B;部分下，单击&#x200B;**编辑API配置**。

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. 复制&#x200B;**Marketo Host**、**API URL**&#x200B;和&#x200B;**API用户Id**，以在后续步骤中使用。 输入您选择的&#x200B;**API密钥**，然后单击&#x200B;**保存**。

   >[!CAUTION]
   >
   >请勿在API密钥中使用&amp;号。

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >以下字段必须与Marketo同步，以使&#x200B;_和Contact_&#x200B;的Sales Insight能够正常工作：
   >
   > * 优先级
   > * 紧急
   > * 相对得分

   >
   >如果缺少其中任何字段，您将在Marketo中看到一条错误消息，其中包含缺少字段的名称。 要解决此问题，请执行[此过程](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md)。

1. 返回至Microsoft Dynamics，单击“设置”旁边的![](assets/image2015-5-13-15-3a49-3a19.png)图标，然后在下拉列表中选择&#x200B;**Marketo API Config**。

   ![](assets/image2015-5-13-16-3a4-3a1.png)

1. 单击&#x200B;**默认配置**。

   ![](assets/image2015-5-13-16-3a5-3a2.png)

1. 输入您从Market复制到之前的信息。

   ![](assets/image2015-5-13-16-3a7-3a6.png)

1. 单击右下角的![](assets/image2015-5-13-16-3a8-3a51.png)图标以保存更改。

## 设置用户访问{#set-user-access}

您需要向用户授予使用Sales Insight的权限。

1. 单击![](assets/image2015-5-13-10-3a5-3a8.png)菜单。 在下拉菜单中，选择&#x200B;**设置**，然后选择&#x200B;**安全**。

   ![](assets/image2015-5-13-16-3a12-3a12.png)

1. 单击&#x200B;**用户**。

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. 选择要授予对Sales Insight访问权限的用户，然后单击&#x200B;**管理角色**。

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. 选择&#x200B;**Marketo Sales Insight**&#x200B;角色，然后单击&#x200B;**确定**。

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   你们该做完！ 最后，要进行测试，请以有权访问Marketo Sales Insight并查看潜在客户或联系人的用户身份登录Dynamics。

   ![](assets/image2015-4-29-15-3a2-3a27.png)

您现在已为您的销售团队释放了Marketo Sales Insight的强大功能。

>[!MORELIKETHIS]
>
>[为潜在客户/联系人记录设置星星和火焰](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
