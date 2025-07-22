---
unique-page-id: 7513865
description: 在Marketo 2015中安装和配置Microsoft Dynamics Sales Insight - Marketo文档 — 产品文档
title: 在Microsoft Dynamics 2015中安装和配置Marketo Sales Insight
exl-id: 26c1f02c-c910-445d-8560-0b37961eadcb
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 1%

---

# 在[!DNL Marketo Sales Insight]中安装和配置[!DNL Microsoft Dynamics 2015] {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight是一款非常棒的工具，可为您的销售团队提供一个了解营销团队拥有的数据财富的“窗口”。 以下是如何在[!DNL Microsoft Dynamics 2015]中安装和配置它

>[!PREREQUISITES]
>
>完成Marketo-Microsoft集成。
>
>[为您的](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md)版本下载正确的解决方案[!DNL Microsoft Dynamics CRM]。

## 导入解决方案 {#import-solution}

好，现在可以将[!DNL Marketo Sales Insight]解决方案导入[!DNL Microsoft Dynamics]了。 方法如下：

1. 在[!UICONTROL Microsoft Dynamics CRM]下，单击&#x200B;**[!UICONTROL Settings]**。

   ![](assets/image2014-12-12-9-3a4-3a56.png)

1. 在[!UICONTROL SETTINGS]下，单击&#x200B;**[!UICONTROL Customizations]**。

   ![](assets/image2015-4-29-14-3a22-3a1.png)

1. 单击 **[!UICONTROL Solutions]**。

   ![](assets/image2014-12-12-9-3a5-3a17.png)

   >[!NOTE]
   >
   >在继续下一步之前，您应该已经安装和配置了Marketo解决方案。

1. 单击 **[!UICONTROL Import]**。

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. 在新窗口中，单击&#x200B;**[!UICONTROL Browse]**。

   ![](assets/image2014-12-12-9-3a5-3a36.png)

1. 查找并选择您在上面下载的解决方案。

   ![](assets/image2014-12-12-9-3a5-3a45.png)

1. 单击 **[!UICONTROL Next]**。

   ![](assets/image2014-12-12-9-3a5-3a55.png)

1. 将上传解决方案。 您可以查看文件包的内容（如果需要）。 单击 **[!UICONTROL Next]**。

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. 确保保持选中此框并单击&#x200B;**[!UICONTROL Import]**。

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. 欢迎下载日志文件，然后单击&#x200B;**[!UICONTROL Close]**。

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. 太棒了！ 您现在应该看到解决方案。 如果不存在，请刷新屏幕。

   ![](assets/image2014-12-12-9-3a6-3a40.png)

## 连接Marketo和Sales Insight {#connect-marketo-and-sales-insight}

让我们在[!DNL Sales Insight]中将您的Marketo实例关联到[!DNL Dynamics]。 方法如下：

>[!NOTE]
>
>需要管理员权限。

1. 登录Marketo并转到&#x200B;**[!UICONTROL Admin]**&#x200B;部分。

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. 在[!UICONTROL Sales Insight]部分下，单击&#x200B;**[!UICONTROL Edit API Configuration]**。

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. 复制&#x200B;**[!UICONTROL Marketo Host]**、**[!UICONTROL API URL]**&#x200B;和&#x200B;**[!UICONTROL API User Id]**&#x200B;以供稍后步骤使用。 输入您选择的API密钥，然后单击&#x200B;**[!UICONTROL Save]**。

   >[!CAUTION]
   >
   >请勿在API密钥中使用&amp;符号。

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >以下字段必须与Marketo同步，*潜在客户和联系人*&#x200B;才能使[!DNL Sales Insight]正常工作：
   >
   >* 优先级
   >* 紧急
   >* 相对分数
   >
   >如果缺少这些字段中的任何一个，您将在Marketo中看到一条错误消息，其中包含缺少的字段的名称。 若要解决此问题，请执行[此过程](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md)。

1. 返回[!DNL Microsoft Dynamics]，转到&#x200B;**[!UICONTROL Settings]**。

   ![](assets/image2014-12-12-9-3a7-3a25.png)

1. 在&#x200B;**[!UICONTROL Settings]**&#x200B;下，单击&#x200B;**[!UICONTROL Marketo API Config]**。

   ![](assets/image2014-12-12-9-3a7-3a34.png)

1. 单击 **[!UICONTROL New]**。

   ![](assets/image2014-12-12-9-3a8-3a8.png)

1. 输入您之前从Marketo中获取的信息，然后单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/image2014-12-12-9-3a8-3a17.png)

## 设置用户访问权限 {#set-user-access}

最后，您必须授予特定用户使用Marketo Sales Insight的权限。

1. 转到&#x200B;**[!UICONTROL Settings]**。

   ![](assets/image2014-12-12-9-3a8-3a34.png)

1. 转到&#x200B;**[!UICONTROL Security]**。

   ![](assets/image2015-4-29-14-3a56-3a33.png)

1. 单击 **[!UICONTROL Users]**。

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. 选择要授予[!DNL Sales Insight]访问权限的用户，然后单击&#x200B;**[!UICONTROL Manage Roles]**。

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. 选择[!DNL Marketo Sales Insight]角色并单击&#x200B;**[!UICONTROL OK]**。

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   你应该都做完了！ 最后，要进行测试，请以有权访问[!DNL Dynamics]的用户身份登录[!DNL Marketo Sales Insight]并查看潜在客户或联系人。

   ![](assets/image2015-4-29-15-3a2-3a27.png)

您现在已为销售团队解锁[!DNL Marketo Sales Insight]的强大功能。

>[!MORELIKETHIS]
>
>[为潜在客户/联系人记录设置星星和火焰](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
