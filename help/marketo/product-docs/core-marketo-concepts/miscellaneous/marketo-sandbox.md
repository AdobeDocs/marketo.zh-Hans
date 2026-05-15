---
unique-page-id: 11386358
description: 了解用于生产前测试的Marketo Engage沙盒。 使用沙盒实例在不影响生产的情况下进行测试。
title: Marketo 沙盒
exl-id: c040fac6-2290-4de5-b27d-2c7cb28f6e30
TQID: https://experienceleague.adobe.com/Cb1H0PKG-G0c4FkIcjI-erNzR0dwRtj7TwfqtwhFFMI
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: e2290edd-b061-4880-9d79-dee306cf5aa9id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: eddd9b14-83bd-4ff4-9072-54a4a484abb7id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 306
ht-degree: 3%

---

# Marketo 沙盒 {#marketo-sandbox}

Marketo Engage沙盒是在生产环境中实施之前用于测试目的的附加实例。

>[!AVAILABILITY]
>
>并非每个人都购买了此功能。 有关详细信息，请联系Adobe客户团队（您的客户经理）。

如果Marketo沙盒已同步到您的生产实例，则无法将其同步到您的常规CRM。 使用CRM的沙盒进行同步，并执行与原始同步相同的所有步骤。

## 关于沙盒的注意事项 {#things-to-know-about-sandboxes}

* 如果要添加用户，该过程与[在生产环境中添加用户](/help/marketo/product-docs/administration/users-and-roles/add-or-remove-a-user.md#add-a-user)的过程相同。 同样，如果他们已具有Marketo登录信息，则必须使用其他电子邮件地址。
* 您的Marketo沙盒最初将是空的，但具有与生产实例相同的可用功能。
* 如果您在沙盒中创建程序并希望将其移至生产环境，则可以执行[程序导入](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md)。
* 沙盒会被限制，以便生产实例不会受到测试环境的不利影响。 每次营销活动运行最多可发送20封电子邮件。

>[!CAUTION]
>
>目前不支持Marketo Dynamics _或_ Salesforce同步的沙盒刷新。 如果您需要刷新CRM沙盒，则需要新的Marketo沙盒。 有关详细信息，请联系Adobe客户团队（您的客户经理）。

## 实例复制 {#instance-copy}

您可以提交支持案例，请求一次性实例副本以填充沙盒。 但是，实例副本不会带来&#x200B;_所有_。 有关详细信息，请联系[Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support)。

>[!NOTE]
>
>如果您更改本机CRM，则需要新的Marketo实例，并且无法将实例复制到新的Marketo实例。 相反，请与Marketo支持人员一起探索导入程序功能。
