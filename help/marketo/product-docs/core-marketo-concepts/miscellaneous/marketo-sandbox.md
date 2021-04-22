---
unique-page-id: 11386358
description: Marketo沙箱 — Marketo文档 — 产品文档
title: Marketo沙箱
exl-id: c040fac6-2290-4de5-b27d-2c7cb28f6e30
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# Marketo沙箱{#marketo-sandbox}

Marketo沙箱是在生产环境中实施之前用于测试目的的附加实例。

>[!AVAILABILITY]
>
>并非所有客户都购买了此功能。 有关详细信息，请联系您的客户成功经理。

如果Marketo沙箱已同步到您的生产实例，则无法同步到常规CRM。 使用CRM的沙箱进行同步，并执行与原始同步相同的所有步骤。

## 沙箱的注意事项{#things-to-know-about-sandboxes}

* 在Customer Success Manager设置沙箱并向您发送邀请后，您必须使用与Marketo生产实例不同的电子邮件地址进行登录。
* 如果要添加用户，则此过程与在生产中添加用户的过程[相同。 ](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md#create-users)同样，如果他们已经有了Marketo登录名，则必须使用其他电子邮件地址。
* Marketo沙箱将开始为空，但具有与生产实例相同的功能。
* 如果您在沙箱中创建了项目并希望将其移动到生产，则可以执行[项目导入](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md)。
* 沙箱会受到限制，因此生产实例不会受到测试环境的不利影响。 每次活动运行最多可发送30封电子邮件。

>[!CAUTION]
>
>我们当前不支持Marketo Dynamics Sync的沙箱刷新。 如果需要刷新Dynamics CRM沙箱，则需要新的Marketo沙箱。 有关更多详细信息，请联系您的客户成功经理。

## 实例复制{#instance-copy}

您可以提交支持案例，请求一次性实例副本以填充沙箱。 但是，实例副本不会引入&#x200B;_everything_。 有关详细信息，请咨询[Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support)。

>[!NOTE]
>
>* 如果源实例已与Microsoft Dynamics集成，则不支持&#x200B;****&#x200B;实例复制。
>* 如果要更改本机CRM，则需要一个新的Marketo实例，并且无法复制到新Marketo实例的实例。 相反，请与Marketo支持部门一起探索“导入项目”功能。

