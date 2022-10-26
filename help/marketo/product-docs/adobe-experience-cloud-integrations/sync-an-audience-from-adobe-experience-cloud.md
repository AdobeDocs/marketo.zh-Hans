---
description: 从Adobe Experience Cloud同步受众 — Marketo文档 — 产品文档
title: 从Adobe Experience Cloud同步受众
exl-id: 2288ee01-2c2e-4f33-b5c9-da3a431c1816
source-git-commit: 492f21f090dc2478271172cf7db470e16f202366
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---

# 从Adobe Experience Cloud同步受众 {#sync-an-audience-from-adobe-experience-cloud}

>[!NOTE]
>
>Marketo实例的HIPAA就绪部署无法使用此集成。

>[!PREREQUISITES]
>
>[设置Adobe组织映射](/help/marketo/product-docs/adobe-experience-cloud-integrations/set-up-adobe-organization-mapping.md){target=&quot;_blank&quot;}

## 如何同步受众 {#how-to-sync-an-audience}

1. 在My Marketo中，单击 **数据库** 拼贴。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-1.png)

1. 单击 **新建** 下拉框并选择 **从Experience Cloud受众同步**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-2.png)

1. 单击 **受众库文件夹** 下拉菜单，然后选择所需的源文件夹。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-3.png)

1. 选择 **受众名称**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-4.png)

1. 对于目标，您可以选择现有列表，或键入新列表的名称。 在本例中，我们正在创建一个新的。 单击 **同步** 完成时。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-5.png)

1. 单击 **确定**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-6.png)

## 常见问题解答 {#faq}

**Cookie同步如何工作？**

为您的Marketo订阅启用Cookie同步后，Marketo的munchkin.js将尝试捕获并存储在集成设置期间指定的Adobe IMS组织的AdobeECID，并将这些ECID与相应的Marketo Cookie标识符匹配。 这样，Marketo的匿名用户配置文件便能够通过AdobeECID进行扩充。

还需要进一步的步骤来将匿名用户配置文件与潜在客户配置文件关联，潜在客户配置文件使用纯文本电子邮件进行标识。 这到底是如何工作的 [此处描述](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md){target=&quot;_blank&quot;}。

**Marketo中的列表大小为何与Adobe中的列表大小不同？**

如果我们无法将ECID Cookie ID关联到Marketo中的已知人员，则人员也不会进行同步。

**这是一次性同步吗？**

您只需启动同步一次。 之后，记录将自动同步。 初始同步可能最长需要24小时；今后，新记录将在2-3小时内同步。
