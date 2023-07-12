---
description: 从Adobe Experience Cloud同步受众 — Marketo文档 — 产品文档
title: 从Adobe Experience Cloud同步受众
exl-id: 2288ee01-2c2e-4f33-b5c9-da3a431c1816
source-git-commit: dd4fb7dfc92580c58da70d603b6d92bd8f64493c
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# 从Adobe Experience Cloud同步受众 {#sync-an-audience-from-adobe-experience-cloud}

>[!NOTE]
>
>Marketo实例的适用于HIPAA的部署无法使用此集成。

>[!PREREQUISITES]
>
>[设置Adobe组织映射](/help/marketo/product-docs/adobe-experience-cloud-integrations/set-up-adobe-organization-mapping.md){target="_blank"}

## 如何同步受众 {#how-to-sync-an-audience}

1. 在“我的Marketo”中，单击 **[!UICONTROL 数据库]** 图块。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-1.png)

1. 单击 **[!UICONTROL 新]** 下拉菜单并选择 **[!UICONTROL 从Experience Cloud受众同步]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-2.png)

1. 单击 **[!UICONTROL 受众库文件夹]** 下拉列表，然后选择所需的原始文件夹。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-3.png)

1. 选择 **[!UICONTROL 受众名称]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-4.png)

1. 对于目标，您可以选择现有列表，也可以键入新列表的名称。 在本例中，我们将创建一个新实例。 单击 **[!UICONTROL 同步]** 完成时。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-5.png)

1. 单击 **[!UICONTROL 确定]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-6.png)

## 常见问题解答 {#faq}

**Cookie同步如何工作？**

为您的Marketo订阅启用Cookie同步后，Marketo的munchkin.js将尝试捕获和存储您在集成设置期间指定的Adobe IMS组织的AdobeECID，并将这些ECID与相应的Marketo Cookie标识符匹配。 这使得Marketo的匿名用户配置文件可以利用AdobeECID丰富内容。

还需要执行进一步的步骤以将匿名用户配置文件与潜在客户配置文件相关联，后者使用纯文本电子邮件进行标识。 具体操作方式 [此处对此进行了说明](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md){target="_blank"}.

**Marketo中的列表大小为何与Adobe中的列表大小不同？**

如果我们无法将ECID Cookie ID关联到Marketo中的已知人员，则人员也不会进行同步。

**这是一次性同步吗？**

您只需启动同步一次。 之后，记录将自动同步。 初始同步最长可能需要24小时；以后，新记录将在2-3小时内同步。
