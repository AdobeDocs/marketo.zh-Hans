---
description: 人员帐户同步常见问题解答 — Marketo文档 — 产品文档
title: 人员帐户同步常见问题解答
exl-id: b77bb44f-94d0-40b2-9955-9636421ac468
feature: Veeva CRM
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# 人员帐户同步常见问题解答 {#person-account-sync-faq}

Marketo Engage将整个数据库与人员帐户类型记录的[!DNL Veeva]同步。 同步后，它将等待5分钟，然后每天、全天再次同步。

可在[!DNL Veeva]中设置人员帐户以满足您组织的需求。

>[!NOTE]
>
>我们仅将“专业”级别帐户同步为个人帐户。

**什么是个人帐户？**

人员帐户与[!DNL Veeva] CRM中的帐户对象非常相似。 但是，人员帐户对帐户字段和联系人字段均具有访问权限。

**将人员帐户同步到Marketo后会出现什么情况？**

人员帐户作为公司和人员同步到Marketo。

>[!NOTE]
>
>人员帐户的自定义字段将会复制到Marketo中的公司和人员。

**如何区分业务帐户和人员帐户？**

使用智能列表中的“Is Person”帐户筛选器将人员帐户与标准业务帐户分开。

**我应该将哪个电子邮件字段用于人员帐户？**

人员帐户有两个电子邮件字段。 在您的表单中使用“电子邮件地址”字段（不是人员电子邮件地址）来确保Marketo的重复数据消除和其他电子邮件处理正常工作。

## 同步方向 {#sync-direction}

人员帐户的联系人相关字段的同步是双向的。 如果您在[!DNL Veeva] CRM或Marketo中对联系人进行了更改，则您的更新将同时反映在这两个系统中。 帐户上的字段仅在一个方向上同步，从[!DNL Veeva] CRM到Marketo。

**如果在两个系统中同时更改人员帐户上的Contact字段会怎样？**

我们会做得很好，让[!DNL Veeva] CRM获胜。 然而，这种数据冲突很少发生。

**记录的潜在客户或联系人类型是否与[!DNL Veeva] CRM同步？**

[!DNL Veeva] CRM只真正处理人员帐户对象，并且还有业务帐户。 传统CRM类型的Lead、Contacts和Opportunity实际上并未在传统[!DNL Veeva] CRM系统中使用。 这些连接器可在[!DNL Veeva] CRM中创建，但官方不支持使用此连接器。

**我能否在Marketo中将某人转换为联系人？**

不支持，因为与[!DNL Veeva] CRM同步不支持潜在客户和联系人类型。 因此，不支持转换。

**我可以手动强制同步联系人吗？**

否，由于联系人不是独立的记录类型，因此不支持将人员同步到[!DNL Veeva]。

**每个标准字段是否都会同步到Marketo？**

否，并非所有标准字段都有用。 所有自定义字段都可以成为同步的一部分。

>[!NOTE]
>
>Marketo将仅同步您的Marketo同步用户有权访问的字段。

**Marketo是否会遵守[!DNL Veeva]验证规则？**

是，如果存在冲突，我们会将结果记录到商机的活动日志中。

>[!MORELIKETHIS]
>
>* [默认 [!DNL Veeva] 字段映射](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping.md){target="_blank"}
>* [正在同步呼叫和呼叫关键消息](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
