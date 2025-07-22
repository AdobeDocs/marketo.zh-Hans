---
unique-page-id: 14352475
description: 在活动历史记录中安装Sales Connect事件字段 — Marketo文档 — 产品文档
title: 在活动历史记录中安装Sales Connect事件字段
exl-id: c1bdb5a6-04f0-4579-84b6-33f4a301128f
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 2%

---

# 在活动历史记录中安装Sales Connect事件字段 {#install-sales-connect-event-fields-on-activity-history}

将Enterprise包安装到[!DNL Salesforce]中后，就可以将[!UICONTROL Sales Connect]事件字段安装到活动历史记录部分。 [!UICONTROL Sales Connect]事件字段包括查看次数、点击次数和促销活动数等信息。 这样，您就可以将电子邮件相关信息直接导入到[!DNL Salesforce]中。

执行这些步骤时，请确保与[!DNL Salesforce]管理员组成团队。 在此示例中，我们将这些字段安装到&#x200B;**潜在客户页面布局**&#x200B;上。 您还可以将字段安装到Contact 、 Account和Opportunity页面布局中。 请记住，在将电子邮件记录到“帐户”和“机会”时，您将需要通过电子邮件将您作为联系人角色关联的联系人。

1. 单击 **[!UICONTROL Setup]**。
1. 单击 **[!UICONTROL Customize]**。
1. 单击 **[!UICONTROL Leads]**。
1. 单击 **[!UICONTROL Page Layouts]**。
1. 单击要更改的页面布局旁边的&#x200B;**[!UICONTROL Edit]**。

   >[!NOTE]
   >
   >[!DNL Sales Connect]将为您安装一些页面布局，但如果您已有默认页面布局，您的团队将希望在该处安装它。 如果您不想使用[!DNL Sales Connect]页面布局，可以将其删除。

1. 向下滚动到[!UICONTROL Activity History]部分。
1. 单击要编辑的扳手。
1. 选择要包含在[!UICONTROL Sales Connect]部分中的[!UICONTROL Activity History]字段。 如果此处未显示[!UICONTROL Sales Connect]字段，则说明您可能安装了错误的[!DNL Salesforce]包。
1. 单击&#x200B;**[!UICONTROL Add]**&#x200B;将所需字段移过来。
1. 单击 **[!UICONTROL OK]**。
1. 单击 **[!UICONTROL Save]**。

   您的用户现在可以在[!DNL Salesforce]中查看有关其电子邮件的重要信息和更新！
