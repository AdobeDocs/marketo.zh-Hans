---
unique-page-id: 4719291
description: 设置默认人员姓氏和公司名称 — Marketo文档 — 产品文档
title: 设置默认人员姓氏和公司名称
exl-id: 0216fb41-adf0-4ccf-be22-c064e90be65a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 0%

---

# 设置默认人员姓氏和公司名称 {#set-default-person-last-name-and-company-name}

Salesforce要求（最小）其潜在客户和联系人的姓氏和公司名称。 不完整的记录将不会同步到Salesforce。 如果要同步部分记录，则必须为Marketo设置默认值，以便与Salesforce一起使用。

1. 转到 **管理员** 单击 **Salesforce**.

   ![](assets/image2014-12-9-13-3a41-3a58.png)

1. 单击 **编辑同步选项**.

   ![](assets/image2014-12-9-13-3a42-3a6.png)

1. 输入 **默认人员姓氏** 和 **默认人员公司** 然后单击 **保存**.

   ![](assets/sync-options-hands.png)

   >[!NOTE]
   >
   >Marketo仅在记录最初同步到Salesforce时分配默认值，并且仅当任一必填字段为空时才分配默认值。

就这样！ 每次人员缺少姓氏和/或公司名称时，Marketo将在同步记录时添加默认值。
