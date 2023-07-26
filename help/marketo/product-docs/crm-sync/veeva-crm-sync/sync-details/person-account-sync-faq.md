---
description: 人员帐户同步常见问题解答 — Marketo文档 — 产品文档
title: 人员帐户同步常见问题解答
exl-id: b77bb44f-94d0-40b2-9955-9636421ac468
feature: Veeva CRM
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# 人员帐户同步常见问题解答 {#person-account-sync-faq}

Marketo Engage会将您的整个数据库与Veeva同步，以获取人员帐户类型的记录。 同步后，它将等待5分钟，然后每天、全天再次同步。

可在Veeva中设置人员帐户，以满足贵组织的需求。

>[!NOTE]
>
>我们仅将“专业”级别帐户同步为个人帐户。

**什么是个人帐户？**

人员帐户与Veeva CRM中的帐户对象非常相似。 但是，人员帐户对帐户字段和联系人字段均具有访问权限。

**将人员帐户同步到Marketo后会发生什么情况？**

人员帐户作为公司和人员同步到Marketo。

>[!NOTE]
>
>人员帐户的自定义字段将会复制到Marketo中的公司和人员。

**如何区分业务帐户和个人帐户？**

使用智能列表中的“Is Person”帐户筛选器将人员帐户与标准业务帐户分开。

**个人帐户应使用哪个电子邮件字段？**

人员帐户有两个电子邮件字段。 在您的表单中使用“电子邮件地址”字段（不是人员电子邮件地址）来确保Marketo的重复数据消除和其他电子邮件处理正常工作。

## 同步方向 {#sync-direction}

人员帐户的联系人相关字段的同步是双向的。 如果您在Veeva CRM或Marketo中更改了联系人，则您的更新将反映在这两个系统中。 帐户上的字段仅在一个方向上同步，从Veeva CRM到Marketo。

**如果两个系统中同时更改了人员帐户上的Contact字段，该怎么办？**

我们会很友善，让Veeva CRM获胜。 然而，这种数据冲突很少发生。

**Lead或Contact类型的记录是否与Veeva CRM同步？**

Veeva CRM实际只处理人员帐户对象，并且还有业务帐户。 传统的CRM类型的Lead 、 Contacts和Opportunity在传统的Veeva CRM系统中实际上并未使用。 这些连接器可在Veeva CRM中创建，但不正式支持使用此连接器。

**能否在Marketo中将人员转换为联系人？**

不支持，因为不支持将潜在客户和联系人类型与Veeva CRM同步。 因此，不支持转换。

**我可以手动强制同步联系人吗？**

否，由于联系人不是独立的记录类型，因此不支持将人员同步到Veeva。

**每个标准字段是否都会同步到Marketo？**

否，并非所有标准字段都有用。 所有自定义字段都可以成为同步的一部分。

>[!NOTE]
>
>Marketo将仅同步您的Marketo同步用户有权访问的字段。

**Marketo是否会遵守Veeva验证规则？**

是，如果存在冲突，我们会将结果记录到商机的活动日志中。

>[!MORELIKETHIS]
>
>* [默认Veeva字段映射](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping.md){target="_blank"}
>* [同步呼叫和呼叫关键消息](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
