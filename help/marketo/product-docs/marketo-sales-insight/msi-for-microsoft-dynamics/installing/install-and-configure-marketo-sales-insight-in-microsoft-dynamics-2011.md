---
unique-page-id: 3571735
description: 在Microsoft Dynamics 2011中安装和配置Marketo Sales Insight - Marketo Docs —— 产品文档
title: 在Microsoft Dynamics 2011中安装和配置Marketo Sales Insight
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---


# 在Microsoft Dynamics 2011中安装和配置Marketo Sales Insight {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight是您的销售团队的绝佳工具。 以下是如何在Microsoft Dynamics 2011内部部署中安装和配置该应用程序的分步说明。

>[!PREREQUISITES]
>
>完成[Marketo-Microsoft集成](http://docs.marketo.com/x/DoA2)。
>
>[下载适用于](http://docs.marketo.com/x/LoJo) 您版本的Microsoft Dynamics CRM的正确解决方案。

## 导入解决方案{#import-solution}

1. 登录Microsoft Dynamics CRM。 单击左下方菜单中的&#x200B;**设置**。

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. 在树中选择&#x200B;**解决方案**。

   ![](assets/image2015-5-4-10-3a41-3a56.png)

1. 单击&#x200B;**导入**(![](assets/image2015-5-4-10-3a45-3a44.png))。

   ![](assets/image2015-5-4-10-3a42-3a38.png)

   >[!NOTE]
   >
   >**提醒**
   >
   >
   >在前进之前，您应已安装[并配置](install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2011.md) Marketo解决方案。

1. 单击&#x200B;**浏览**。 选择您[downloaded](download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md)的Marketo Sales Insight解决方案。 单击&#x200B;**下一步**。

   ![](assets/image2015-5-4-10-3a55-3a15.png)

1. 验证解决方案的详细信息，然后单击&#x200B;**下一步**。

   ![](assets/image2015-5-4-10-3a57-3a31.png)

1. 确保选中SDK消息选项。 单击&#x200B;**下一步**。

   ![](assets/image2015-5-4-11-3a43-3a37.png)

1. 现在，请等待导入完成。

   ![](assets/image2015-5-4-11-3a0-3a58.png)

1. 单击&#x200B;**关闭**。

   ![](assets/crmhand.png)

1. Marketo Sales Insight现在将显示在解决方案列表中。 耶！

   ![](assets/image2015-5-4-11-3a2-3a37.png)

1. 选择Marketo Sales Insight，然后单击&#x200B;**发布所有自定义项**(![](assets/image2015-5-4-11-3a7-3a8.png))。

   ![](assets/image2015-5-4-11-3a8-3a27.png)

## Connect Marketo和Sales Insight {#connect-marketo-and-sales-insight}

>[!NOTE]
>
>**需要管理员权限**

1. 登录到Marketo并单击&#x200B;**管理**。

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. 在**Sales Insight **部分下，单击&#x200B;**编辑API配置**。

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. 复制&#x200B;**Marketo主机**、**API URL**&#x200B;和&#x200B;**API用户Id**，以在后续步骤中使用。 输入您选择的&#x200B;**API密钥**，然后单击&#x200B;**SAVE**。

   >[!CAUTION]
   >
   >请勿在API密钥中使用&amp;符。

   ![](assets/image2015-5-4-11-3a16-3a3.png)

   >[!NOTE]
   >
   >*Lead和Contact*&#x200B;的以下字段必须与Marketo同步，才能使Sales Insight正常工作：
   >
   >    
   >    
   >    * 优先级
   >    * 紧急
   >    * 相对得分

   >    
   >    
   >如果这些字段中有任何一个缺失，您将在Marketo中看到一条错误消息，其中包含缺失字段的名称。 要解决此问题，请执行[此过程](../../../../product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md)。

1. 返回动态，选择&#x200B;**设置**。

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. 在树中选择&#x200B;**Marketo API Config**。

   ![](assets/image2015-5-4-11-3a22-3a41.png)

1. 单击&#x200B;**默认配置**。

   ![](assets/image2015-5-4-11-3a26-3a10.png)

1. 输入您从Market获取到的早期信息。

   ![](assets/image2015-5-4-11-3a27-3a16.png)

1. 单击&#x200B;**保存。**

   ** ![](assets/image2015-5-4-11-3a28-3a13.png)

   **

## 设置用户访问权限{#set-user-access}

设置用户角色，以授予特定用户对Sales Insight的访问权限。

1. 选择&#x200B;**设置**。

   ![](assets/image2015-5-4-11-3a30-3a54.png)

1. 在树中选择&#x200B;**管理**。

   ![](assets/image2015-5-4-11-3a31-3a39.png)

1. 单击&#x200B;**用户**。

   ![](assets/image2015-5-4-11-3a32-3a25.png)

1. 选择要授予访问权限的用户，然后单击&#x200B;**管理角色**。

   ![](assets/image2015-5-4-11-3a35-3a8.png)

1. 选择&#x200B;**Marketo Sales Insight**&#x200B;角色，然后单击&#x200B;**确定**。

   ![](assets/image2015-5-4-11-3a36-3a59.png)

   就这样！ 所有具有访问权限的用户现在都可以查看潜在客户／联系人详细信息视图中的销售分析部分。

   ![](assets/image2015-5-4-11-3a39-3a23.png)

   恭喜。 您现在已释放了Marketo Sales Insight的力量。

>[!MORELIKETHIS]
>
>[为潜在客户／联系人记录设置星星和火焰](http://docs.marketo.com/x/BICMAg)

