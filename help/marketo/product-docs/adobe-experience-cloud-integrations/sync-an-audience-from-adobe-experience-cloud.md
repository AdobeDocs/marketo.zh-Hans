---
description: 从Adobe Experience Cloud同步受众 — Marketo文档 — 产品文档
title: 从Adobe Experience Cloud同步受众
exl-id: 2288ee01-2c2e-4f33-b5c9-da3a431c1816
feature: Integrations
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '275'
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

1. 在“我的Marketo”中，单击&#x200B;**[!UICONTROL 数据库]**&#x200B;磁贴。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-1.png)

1. 单击&#x200B;**[!UICONTROL 新建]**&#x200B;下拉列表，然后选择&#x200B;**[!UICONTROL 从Experience Cloud受众同步]**。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-2.png)

1. 单击&#x200B;**[!UICONTROL 受众库文件夹]**&#x200B;下拉列表，然后选择所需的原始文件夹。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-3.png)

1. 选择&#x200B;**[!UICONTROL 受众名称]**。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-4.png)

1. 对于目标，您可以选择现有列表，也可以键入新列表的名称。 在本例中，我们将创建一个新实例。 完成后单击&#x200B;**[!UICONTROL 同步]**。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-5.png)

1. 单击&#x200B;**[!UICONTROL 确定]**。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-6.png)

## 常见问题 {#faq}

**Cookie同步如何工作？**

为您的Marketo订阅启用Cookie同步后，Marketo的munchkin.js将尝试为您在集成设置期间指定的Adobe IMS组织捕获和存储AdobeECID，并将这些ECID与相应的Marketo Cookie标识符匹配。 这使得Marketo的匿名用户档案能够利用AdobeECID丰富内容。

还需要执行进一步的步骤，以将匿名用户配置文件关联到潜在客户配置文件，该潜在客户配置文件使用纯文本电子邮件进行标识。 此处介绍了[的工作方式](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md){target="_blank"}。

**为什么Marketo中的列表大小与Adobe中的列表大小不同？**

如果我们无法将ECID Cookie ID绑定到Marketo中的已知人员，则人员也不会进行同步。

**这是一次性同步吗？**

您只需启动同步一次。 之后，记录将自动同步。 初始同步最多可能需要24小时；以后，新记录将在2-3小时内同步。
