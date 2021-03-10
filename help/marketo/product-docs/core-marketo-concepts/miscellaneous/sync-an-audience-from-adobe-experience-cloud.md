---
description: 从Adobe Experience Cloud同步受众- Marketo Docs — 产品文档
title: 从Adobe Experience Cloud同步受众
translation-type: tm+mt
source-git-commit: 05c2e89222f9316241a3929642998bddb02ff7a5
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 0%

---


# 从Adobe Experience Cloud {#sync-an-audience-from-adobe-experience-cloud}同步受众

>[!NOTE]
>
>Marketo实例的HIPAA就绪部署无法使用此集成。

>[!PREREQUISITES]
>
>[设置Adobe Experience Cloud受众共享](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/set-up-adobe-experience-cloud-audience-sharing.md)

## 如何同步受众{#how-to-sync-an-audience}

1. 在My Marketo中，单击&#x200B;**Database**&#x200B;拼贴。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-1.png)

1. 单击&#x200B;**新建**&#x200B;下拉框，然后选择&#x200B;**从Experience Cloud受众**&#x200B;同步。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-2.png)

1. 单击&#x200B;**受众库文件夹**&#x200B;下拉框并选择所需的来源文件夹。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-3.png)

1. 选择&#x200B;**受众名称**。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-4.png)

1. 对于目标，您可以选择现有列表，或键入新目标的名称。 在此示例中，我们将创建新的。 完成后，单击&#x200B;**同步**。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-5.png)

1. 单击&#x200B;**确定**。

   ![](assets/sync-an-audience-from-adobe-experience-cloud-6.png)

## 常见问题解答{#faq}

**Cookie同步是如何工作的？**

为您的Marketo订阅启用Cookie同步后，Marketo的munchkin.js将尝试为您在集成设置过程中指定的AdobeIMS组织捕获和存储AdobeECID，并将这些ECID与相应的Marketo Cookie标识符匹配。 这使Marketo的匿名用户用户档案能够丰富AdobeECID。

需要进一步将匿名用户用户档案关联到潜在客户用户档案，该潜在客户使用纯文本电子邮件进行标识。 ](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md)中具体介绍了这种方法的工作方式。[

**为什么Marketo中的列表大小与Adobe中的不同？**

如果我们无法将ECID Cookie ID绑定到Marketo中的已知人，则用户也不会同步。

**这是一次性同步吗？**

您只需启动同步一次。 之后，记录将自动同步。 初始同步最长可能需要24小时；今后，新记录将在2-3小时内同步。
