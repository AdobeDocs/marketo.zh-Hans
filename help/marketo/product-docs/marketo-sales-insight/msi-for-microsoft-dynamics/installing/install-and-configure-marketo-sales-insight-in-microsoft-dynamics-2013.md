---
unique-page-id: 3571737
description: 在Microsoft Dynamics 2013中安装和配置Marketo Sales Insight - Marketo Docs —— 产品文档
title: 在Microsoft Dynamics 2013中安装和配置Marketo Sales Insight
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 0%

---


# 在Microsoft Dynamics 2013中安装和配置Marketo Sales Insight {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight是一款绝佳的工具，可让您的销售团队“了解”营销团队所拥有的丰富数据。 下面介绍如何安装和配置它。

>[!PREREQUISITES]
>
>完成 [Marketo-Microsoft集成](http://docs.marketo.com/x/EIA2)。
>
>[下载适用于您的](http://docs.marketo.com/x/LoJo) Microsoft Dynamics CRM版本的正确解决方案。

## 导入解决方案 {#import-solution}

好，现在是时候将Marketo Sales Insight解决方案导入Microsoft Dynamics了。

1. 在Microsoft **Dynamics CRM下** ，单 **击设置**。

   ![](assets/image2014-12-12-9-3a4-3a56.png)

1. 在“设 **置**”下，单 **击“自定义**”。

   ![](assets/image2014-12-12-9-3a5-3a6.png)

1. 单击“ **解决方案**”。

   ![](assets/image2014-12-12-9-3a5-3a17.png)

   >[!NOTE]
   >
   >**提醒**
   >
   >
   >在前进之前，您应已安装并配置Marketo

1. 单击“ **导入**”。

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. 在新窗口中，单击“浏 **览”**。

   ![](assets/image2014-12-12-9-3a5-3a36.png)

1. 查找并选择您在上面下载的解决方案。

   ![](assets/image2014-12-12-9-3a5-3a45.png)

1. 单击“ **下一步**”。

   ![](assets/image2014-12-12-9-3a5-3a55.png)

1. 解决方案将上传。 您可以视图包内容（如果喜欢）。 单击“ **下一步**”。

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. 确保选中该框并单击“导 **入”**。

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. 请随时下载日志文件。 单击 **关闭**。

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. 太棒了！ 您应该立即看到解决方案。 如果它不在，请刷新您的屏幕。

   ![](assets/image2014-12-12-9-3a6-3a40.png)

## Connect Marketo和Sales Insight {#connect-marketo-and-sales-insight}

让我们将您的Marketo实例绑定到Dynamics中的Sales Insight。

>[!NOTE]
>
>需要管理员权限。

1. 登录到Marketo并转到“管理 **员** ”部分。

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. 在Sales Insight **部分下** ，单 **击Edit API Configuration**。

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. 复制 **Marketto主机**、 **API URL**&#x200B;和API **用户Id** ，以便在以后的步骤中使用。 输入您 **选择的API密钥** ，然后单击 **保存**。

   >[!CAUTION]
   >
   >请勿在API密钥中使用&amp;符。

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >以下字段必须与Marketo同步，以 *便潜在客户和销售分析联* 系人都能正常工作：
   >
   >    
   >    
   >    * 优先级
   >    * 紧急
   >    * 相对得分

   >    
   >    
   >如果这些字段中有任何一个缺失，您将在Marketo中看到一条错误消息，其中包含缺失字段的名称。 要解决此问题，请执 [行此过程](../../../../product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md)。

1. 返回Microsoft Dynamics，转至“设 **置”**。

   ![](assets/image2014-12-12-9-3a7-3a25.png)

1. 在“ **设置**”下， **单击“Marketo API Config**”。

   ![](assets/image2014-12-12-9-3a7-3a34.png)

1. 单击 **新建**。

   ![](assets/image2014-12-12-9-3a8-3a8.png)

1. 输入您从Market转到之前的信息，然后单击“保 **存”**。

   ![](assets/image2014-12-12-9-3a8-3a17.png)

## 设置用户访问权限 {#set-user-access}

最后，您可以授予特定用户访问Marketo Sales Insight的权限。

1. 转到“ **设置**”。

   ![](assets/image2014-12-12-9-3a8-3a34.png)

1. 单击“ **用户**”。

   ![](assets/image2014-12-12-9-3a8-3a42.png)

1. 选择要授予对Sales Insight访问权限的用户，然后单击管理 **角色**。

   ![](assets/image2014-12-12-9-3a9-3a13.png)

1. 选择Marketo **Sales Insight角色** ，然后单击 **确定**。

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   你们应该全部完成！ 最后，要进行测试，请以有权访问Marketo Sales Insight并查看潜在客户或联系人的用户身份登录Dynamics。

   ![](assets/image2014-12-12-9-3a9-3a31.png)

您现在已为您的销售团队解锁了Marketo Sales Insight的强大功能。

>[!NOTE]
>
>**相关文章**
>
>[为潜在客户／联系人记录设置星星和火焰](http://docs.marketo.com/x/BICMAg)

