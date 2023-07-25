---
unique-page-id: 4719291
description: 设置默认人员姓氏和公司名称 — Marketo文档 — 产品文档
title: 设置默认人员姓氏和公司名称
exl-id: 0216fb41-adf0-4ccf-be22-c064e90be65a
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 0%

---

# 设置默认人员姓氏和公司名称 {#set-default-person-last-name-and-company-name}

Salesforce要求其Leads和Contacts具有（最低）姓氏和公司名称。 未完成的记录将不会同步到Salesforce。 如果要同步部分记录，必须设置Marketo的默认值以与Salesforce一起使用。

1. 转到 **管理员** 并单击 **Salesforce**.

   ![](assets/image2014-12-9-13-3a41-3a58.png)

1. 单击 **编辑同步选项**.

   ![](assets/image2014-12-9-13-3a42-3a6.png)

1. 输入 **默认人员姓氏** 和 **默认人员公司** 然后单击 **保存**.

   ![](assets/sync-options-hands.png)

   >[!NOTE]
   >
   >仅当记录最初同步到Salesforce时，且仅当任一必填字段为空时，Marketo才分配默认值。

就是这样！ 每次人员缺少姓氏和/或公司名称时，Marketo都会在记录同步时添加默认值。
