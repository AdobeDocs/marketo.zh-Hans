---
unique-page-id: 3571739
description: 在Microsoft Dynamics 365中安装和配置Marketo Sales Insight - Marketo Docs —— 产品文档
title: 在Microsoft Dynamics 365中安装和配置Marketo Sales Insight
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 0%

---


# 在Microsoft Dynamics 365中安装和配置Marketo Sales Insight {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight是一款绝佳的工具，可让您的销售团队“了解”营销团队所拥有的大量数据。 下面介绍如何安装和配置。

>[!NOTE]
>
>**先决条件**
>
>完成 [Marketo-Microsoft集成](http://docs.marketo.com/x/E4A2)。
>
>[下载适用于您的](http://docs.marketo.com/x/LoJo) Microsoft Dynamics CRM版本的正确解决方案。

## 导入解决方案 {#import-solution}

1. 登录到 [Microsoft Office 365](https://login.microsoftonline.com/)。

   ![](assets/image2015-3-16-15-58-55.png)

1. 单击“- ![”](assets/image2015-3-16-16-1-13.png) 菜单并选 **择CRM**。

   ![](assets/image2015-3-16-16-0-10.png)

1. 单击— ![菜](assets/image2015-5-13-10-5-8.png) 单。 在下拉框中，选择设 **置**，然后选择 **解决方案**。

   ![](assets/image2015-5-13-10-4-1.png)

   >[!NOTE]
   >
   >**提醒**
   >
   >
   >在前进之前， [您应已安装并配置Marketo解](../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md) 决方案。

   单击“导入”。
   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. 在新窗口中，单击“浏 **览”**。 选择您 [在步骤1中下载的Marketo Sales Insight解决方案](#msi)。 单击“ **下一步**”。

   ![](assets/image2015-5-13-15-3a38-3a49.png)

1. 解决方案将上传。 您可以视图包内容（如果喜欢）。 单击“ **下一步**”。

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. 确保选中该框 **并单** 击“ **Import**”。

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. 请随时下载日志文件。 单击 **关闭**。

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. 太棒了！ 您应该立即看到解决方案。 如果它不在，请刷新您的屏幕。

   ![](assets/image2015-5-13-15-3a42-3a29.png)

1. 单击“ **发布所有自定义**”。

   ![](assets/image2015-11-10-11-3a15-3a40.png)

## Connect Marketo和Sales Insight {#connect-marketo-and-sales-insight}

让我们将您的Marketo实例绑定到Dynamics中的Sales Insight。 下面是具体方法：

>[!NOTE]
>
>**需要管理员权限**

1. 登录Marketo并转到“管理 **员** ”部分。

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. 在Sales Insight **部分** ，单击 **编辑API配置**。

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. 复制 **Marketto主机**、 **API URL** 和API **用户Id** ，以便在后续步骤中使用。 输入您 **选择的API密钥** ，然后单击 **保存**。

   >[!CAUTION]
   >
   >请勿在API密钥中使用&amp;符。

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >以下字段必须与Marketo同步，以 *便潜在客户和销售分析联* 系人都能正常工作：
   >
   > * 优先级
   > * 紧急
   > * 相对得分

   >
   >如果这些字段中有任何一个缺失，您将在Marketo中看到一条错误消息，其中包含缺失字段的名称。 要解决此问题，请执 [行此过程](../../../../product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md)。

1. 返回至Microsoft Dynamics，单击“设置” ![](assets/image2015-5-13-15-3a49-3a19.png) 旁边的图标，然后在下拉 **列表中选择** “Marketo API Config”。

   ![](assets/image2015-5-13-16-3a4-3a1.png)

1. 单击 **默认配置**。

   ![](assets/image2015-5-13-16-3a5-3a2.png)

1. 输入您从Market复制到早期版本的信息。

   ![](assets/image2015-5-13-16-3a7-3a6.png)

1. 单击 ![](assets/image2015-5-13-16-3a8-3a51.png) 右下角的图标以保存更改。

## 设置用户访问权限 {#set-user-access}

您需要向用户授予使用Sales Insight的权限。

1. 单击菜 ![](assets/image2015-5-13-10-3a5-3a8.png) 单。 在下拉菜单中，选 **择设置**，然后选择 **安全性**。

   ![](assets/image2015-5-13-16-3a12-3a12.png)

1. 单击“ **用户**”。

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. 选择要授予对Sales Insight访问权限的用户，然后单击管理 **角色**。

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. 选择Marketo **Sales Insight角色** ，然后单击 **确定**。

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   你们应该全部完成！ 最后，要进行测试，请以有权访问Marketo Sales Insight并查看潜在客户或联系人的用户身份登录Dynamics。

   ![](assets/image2015-4-29-15-3a2-3a27.png)

您现在已为您的销售团队解锁了Marketo Sales Insight的强大功能。

>[!NOTE]
>
>**相关文章**
>
>[为潜在客户／联系人记录设置星星和火焰](http://docs.marketo.com/x/BICMAg)