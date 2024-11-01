---
unique-page-id: 3571844
description: Microsoft Dynamics同步 — Opportunity同步 — Marketo文档 — 产品文档
title: Microsoft Dynamics同步 — 机会同步
exl-id: dcb72f28-c980-4183-8473-a1e5ad0c8d3c
feature: Microsoft Dynamics
source-git-commit: 9a130e0b2ec84b638adf37188b65b565b090fe1b
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 0%

---

# Microsoft Dynamics同步：机会同步 {#microsoft-dynamics-sync-opportunity-sync}

对Dynamics同步的Marketo Engage功能非常强大。 下面是机会同步的所有详细信息。

## 两个系统之间的机会详细信息如何保持同步？ {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

机会同步是一种方式 — Dynamics到Marketo。 如果您在Dynamics中更改了业务机会，您的更新将反映在Marketo中。

## 我可以使用Marketo在Dynamics中创建机会吗？ {#can-i-create-an-opportunity-in-dynamics-using-marketo}

否，您必须在Dynamics中创建机会，该机会会自动同步到Marketo。

## 哪些字段将同步到Marketo？ {#what-fields-will-sync-to-marketo}

您可以[选择要在安装过程中同步的字段](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"}。

## 客户/联系人如何与业务机会关联？ {#how-is-an-account-contact-associated-with-an-opportunity}

可以通过两种方式将联系人/客户关联到Opportunity ：

* 在创建业务机会时，可以设置Contact （要联系的表单上的查找字段）和/或Account （要联系的表单上的查找字段）。 在任一情况下，这些值都存储在Dynamics的潜在客户(customerid)字段中。 此字段未显示在机会表单上，但可从设置添加。 此字段只能包含1个值，即联系人或帐户。 Marketo执行以下操作：

   * 如果设置了联系人值并且帐户为空，则Marketo将创建一个`opportunitycontactrole`并将商机上的帐户设置为联系人的帐户。 如果联系人没有帐户，此字段将留空。
   * 如果设置了account值并且contact留空，则Marketo将只为该帐户设置商机上的帐户。
   * 如果同时设置了这两个值，则Dynamics会选择帐户作为customerid的值，因此其行为将与上面相同。


* 通过利益干系人： Dynamics使用连接从机会创建页面将机会连接到利益干系人。 为此，我们将为每个新利益相关者创建一个`opportunitycontactrole`记录。
