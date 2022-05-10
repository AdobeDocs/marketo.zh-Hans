---
description: 人员帐户同步常见问题解答 — Marketo文档 — 产品文档
title: 人员帐户同步常见问题解答
exl-id: b77bb44f-94d0-40b2-9955-9636421ac468
source-git-commit: bb020cba0bb0cb65761e15cba05147b6e9fffe50
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 0%

---

# 人员帐户同步常见问题解答 {#person-account-sync-faq}

Marketo Engage会将整个数据库与Veeva同步，以获得人员帐户类型的记录。 同步后，需要等待5分钟，然后每天再次同步。

可以在Veeva中设置人员帐户，以满足贵组织的需求。

>[!NOTE]
>
>我们仅将“专业”层帐户同步为“人员帐户”。

**什么是个人帐户？**

人员帐户与Veeva CRM中的帐户对象非常相似。 但是，个人帐户同时具有帐户字段和联系字段的访问权限。

**当人员帐户同步到Marketo时，会出现什么情况？**

人员帐户以公司和人员身份同步到Marketo。

>[!NOTE]
>
>人员帐户的自定义字段会复制到Marketo中的公司和人员。

**如何区分业务帐户和人员帐户？**

在智能列表中使用“是人员”帐户筛选器可将人员帐户与标准业务帐户分开。

**我应该将哪个电子邮件字段用于个人帐户？**

个人帐户有两个电子邮件字段。 使用表单中的“电子邮件地址”字段（而非人员电子邮件地址），可确保Marketo的重复数据删除和其他电子邮件处理正常工作。

## 同步方向 {#sync-direction}

人员帐户的联系人相关字段的同步是双向的。 如果您在Veva CRM或Marketo中对联系人进行了更改，则您的更新将反映在两个系统中。 帐户上的字段仅在一个方向上同步，从Veeva CRM到Marketo。

**如果同时在两个系统中对人员帐户上的“联系人”字段进行了更改，该怎么办？**

我们会很好，让维娃客户关系公司赢。 但这种数据冲突很少发生。

**潜在客户或联系人类型的记录是否与Veeva CRM同步？**

Veeva CRM仅真正处理人员帐户对象，还具有业务帐户。 传统的CRM类型的潜在客户、联系人和机会在传统的Veeva CRM系统中并没有真正使用。 这些组件可以在Veeva CRM中创建，但使用此连接器不会正式支持它们。

**我能将人员转换为Marketo中的联系人吗？**

不支持，因为与Veeva CRM同步的潜在客户和联系人类型不受支持。 因此，不支持转换。

**我能否手动强制同步联系人？**

否，由于“联系人”不是独立类型的记录，因此不支持将人员同步到Veeva。

**每个标准字段是否都同步到Marketo?**

不，并非所有标准字段都有用。 所有自定义字段都可以包含在同步中。

>[!NOTE]
>
>Marketo将仅同步Marketo同步用户有权访问的字段。

**Marketo会遵守Veeva验证规则吗？**

是的，如果发生冲突，我们将在潜在客户的活动日志中记录结果。

>[!MORELIKETHIS]
>
>* [默认Veeva字段映射](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping.md){target=&quot;_blank&quot;}
>* [正在同步呼叫和呼叫密钥消息](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target=&quot;_blank&quot;}

