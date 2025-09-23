---
description: 将致电原因和致电结果记录到Salesforce - Marketo文档 — 产品文档
title: 将通话原因和通话结果记录到 Salesforce
exl-id: b35acdc2-8ec7-4dec-92b8-58ba7a1ad858
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 4%

---

# 将致电原因和致电结果记录到[!DNL Salesforce] {#log-call-reasons-and-call-outcomes-to-salesforce}

如果您出于报告或可见性的目的，希望将致电结果记录并致电原因[!DNL Salesforce]，则可以为每个创建自定义活动字段。 每个字段必须使用特定的API名称（在[!DNL Salesforce]中称为“字段名称”）。

* 呼叫结果字段名称：mktosales_call_output
* 致电原因字段名称：mktosales_call_reason

要利用这些字段，您首先需要将字段创建为自定义活动字段。 为了使其对用户可见，您需要将其添加到任务对象页面布局。

## [!DNL Salesforce] Classic {#salesforce-classic}

### 在[!DNL Salesforce] Classic中创建自定义活动字段  {#create-custom-activity-field-in-salesforce-classic}

1. 在[!DNL Salesforce]中，单击&#x200B;**[!UICONTROL Setup]**。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-1.png)

1. 在快速查找框中键入“Activities”。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-2.png)

1. 单击 **[!UICONTROL Activity Custom Fields]**。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-3.png)

1. 单击 **[!UICONTROL New]**。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-4.png)

1. 选择数据类型“[!UICONTROL Text]”并单击&#x200B;**[!UICONTROL Next]**。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-5.png)

1. 为自定义字段提供上面定义的字段名称。 字段长度限制为255个字符。 字段标签将是您的销售团队可见的字段，并且可以自定义以满足您团队的需求。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-6.png)

1. 其余设置是可选的。 完成配置后，单击&#x200B;**[!UICONTROL Next]**。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-7.png)

1. 为此字段选择所需的字段级安全设置，然后单击&#x200B;**[!UICONTROL Next]**（下面的图像只是一个示例）。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-8.png)

   >[!NOTE]
   >
   >确保您的[!DNL Sales Connect]用户使用的个人资料可看到该自定义字段，以及您希望它可见的任何其他内容。

1. 选择要将该字段添加到哪些页面布局，然后单击&#x200B;**[!UICONTROL Save]** （或者，您可以单击&#x200B;**[!UICONTROL Save & New]**&#x200B;并重复呼叫原因字段的流程）。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-9.png)

### 在[!DNL Salesforce] Classic中将自定义活动字段添加到任务页面布局 {#add-custom-activity-field-to-task-page-layout-in-salesforce-classic}

>[!NOTE]
>
>如果您没有在上面的步骤9中选择所需的页面布局，则只需执行以下步骤即可。

1. 在[!DNL Salesforce]中，单击&#x200B;**[!UICONTROL Setup]**。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-10.png)

1. 在“快速查找”框中键入“Task”。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-11.png)

1. 单击 **[!UICONTROL Task Page Layouts]**。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-12.png)

1. 单击您想要将此字段添加到的任务页面布局旁的&#x200B;**[!UICONTROL Edit]**。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-13.png)

1. 将该字段拖放到任务页面布局的所需部分。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-14.png)

1. 单击 **[!UICONTROL Save]**。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-15.png)

## [!DNL Salesforce]闪电 {#salesforce-lightning}

### 在[!DNL Salesforce]闪电中创建自定义活动字段 {#create-custom-activity-field-in-salesforce-lightning}

1. 在[!DNL Salesforce]中，单击右上角的齿轮图标并选择&#x200B;**[!UICONTROL Setup]**。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-16.png)

1. 单击 **[!UICONTROL Object Manager]**。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-17.png)

1. 在快速查找框中键入“[!UICONTROL Activity]”。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-18.png)

1. 单击&#x200B;**[!UICONTROL Activity]**&#x200B;标签。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-19.png)

1. 单击 **[!UICONTROL Fields & Relationships]**。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-20.png)

1. 单击 **[!UICONTROL New]**。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-21.png)

### 在[!DNL Salesforce]闪电中向任务页面布局添加自定义活动字段 {#add-custom-activity-field-to-task-page-layout-in-salesforce-lightning}

1. 在[!DNL Salesforce]中，单击右上角的齿轮图标并选择&#x200B;**[!UICONTROL Setup]**。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-22.png)

1. 单击 **[!UICONTROL Object Manager]**。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-23.png)

1. 在快速查找框中键入“[!UICONTROL Task]”。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-24.png)

1. 单击&#x200B;**[!UICONTROL Task]**&#x200B;标签。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-25.png)

1. 单击 **[!UICONTROL Page Layouts]**。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-26.png)

1. 单击要将此字段添加到的任务页面布局。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-27.png)

1. 将该字段拖放到任务页面布局的所需部分。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-28.png)

1. 单击 **[!UICONTROL Save]**。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-29.png)

>[!MORELIKETHIS]
>
>[在活动历史记录上安装Sales Connect事件字段](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/install-sales-connect-event-fields-on-activity-history.md)
