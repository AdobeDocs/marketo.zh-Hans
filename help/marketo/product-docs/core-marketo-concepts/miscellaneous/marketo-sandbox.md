---
unique-page-id: 11386358
description: Marketo沙盒 — Marketo文档 — 产品文档
title: Marketo沙盒
exl-id: c040fac6-2290-4de5-b27d-2c7cb28f6e30
source-git-commit: c2dc3c337cb5ea1446a2ebd6233f570025d1d986
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Marketo沙盒 {#marketo-sandbox}

Marketo沙盒是在生产环境中实施之前用于测试的额外实例。

>[!AVAILABILITY]
>
>并非所有客户都购买了此功能。 有关详细信息，请联系您的客户成功经理。

如果Marketo沙盒已经与您的生产实例同步，则该沙盒无法同步到常规CRM。 使用CRM的沙盒进行同步，并执行与原始同步相同的所有步骤。

## 沙箱注意事项 {#things-to-know-about-sandboxes}

* 在客户成功经理设置沙盒并向您发送邀请后，您必须使用与Marketo生产实例不同的电子邮件地址进行登录。
* 如果要添加用户，则该过程与 [在生产中添加用户](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md#create-users). 同样，如果用户已经登录Marketo，则必须使用其他电子邮件地址。
* 您的Marketo沙盒将以空开始，但其功能与生产实例相同。
* 如果在沙盒中创建项目并希望将其移动到生产环境，则可以执行 [程序导入](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md).
* 沙箱受到限制，因此生产实例不会受到测试环境的不利影响。 每个营销活动运行最多可发送20封电子邮件。

>[!CAUTION]
>
>我们当前不支持对Marketo Dynamics同步进行沙盒刷新。 如果您需要刷新Dynamics CRM沙盒，则需要新的Marketo沙盒。 有关更多详细信息，请联系您的客户成功经理。

## 实例复制 {#instance-copy}

您可以提交支持案例，请求一次性实例副本以填充您的沙盒。 实例副本将不会提交 _一切_&#x200B;但是。 请咨询 [Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support) 以了解详细信息。

>[!NOTE]
>
>如果您要更改本机CRM，则需要一个新的Marketo实例，并且将无法复制到新Marketo实例的实例。 请与Marketo支持团队合作，探索导入计划功能。
