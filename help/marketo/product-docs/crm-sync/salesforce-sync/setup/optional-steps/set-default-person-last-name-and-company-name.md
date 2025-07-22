---
unique-page-id: 4719291
description: 设置默认人员姓名和公司名称 — Marketo文档 — 产品文档
title: 设置默认人员姓氏和公司名称
exl-id: 0216fb41-adf0-4ccf-be22-c064e90be65a
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '127'
ht-degree: 0%

---

# 设置默认人员姓氏和公司名称 {#set-default-person-last-name-and-company-name}

[!DNL Salesforce]需要其潜在客户和联系人的姓氏和公司名称（最小）。 未完成的记录将不会同步到[!DNL Salesforce]。 如果要同步部分记录，必须设置Marketo的默认值以与[!DNL Salesforce]一起使用。

1. 转到&#x200B;**[!UICONTROL Admin]**&#x200B;并单击&#x200B;**[!DNL Salesforce]**。

   ![](assets/image2014-12-9-13-3a41-3a58.png)

1. 单击 **[!UICONTROL Edit Sync Options]**。

   ![](assets/image2014-12-9-13-3a42-3a6.png)

1. 输入&#x200B;**[!UICONTROL Default person last name]**&#x200B;和&#x200B;**[!UICONTROL Default person company]**，然后单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/sync-options-hands.png)

   >[!NOTE]
   >
   >仅当最初将记录同步到Salesforce时，并且仅当任一必填字段为空时，Marketo Engage才会分配默认值。

就是这样！ 每次人员缺少姓氏和/或公司名称时，Marketo都会在记录同步过程中添加默认值。
