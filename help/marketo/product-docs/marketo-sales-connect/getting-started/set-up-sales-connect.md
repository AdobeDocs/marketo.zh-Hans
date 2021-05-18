---
description: 设置Sales Connect - Marketo Docs — 产品文档
title: 设置销售连接
source-git-commit: b491f476c4facc6343559a0acf5d5527e9afc618
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# 设置Sales Connect {#set-up-sales-connect}

此文档将指导您完成设置新Sales Connect实例的初始步骤。 其中一些步骤需要以Marketo管理员、Salesforce管理员和Sales Connect管理员身份访问。 请按照以下指南完成实例设置。

## 访问您的新Marketo Sales Connect帐户{#accessing-your-new-marketo-sales-connect-account}

如果您已购买Marketo Sales Connect，则将从Marketo的管理员部分设置对您的实例的访问权限。 单击此处查看有关Marketo管理员如何设置对新实例的访问权限的说明。

![](assets/set-up-sales-connect-1.png)

## 邀请和管理用户{#inviting-and-managing-users}

从Marketo设置您的Marketo Sales Connect帐户并邀请您的第一个管理员用户后，该管理员用户可以从Marketo Sales Connect用户管理页面邀请其他用户。 [单](/help/marketo/product-docs/marketo-sales-connect/admin/invite-users.md) 击此处查看如何从用户管理页面邀请用户。

![](assets/set-up-sales-connect-2.png)

## 正在连接到Salesforce {#connecting-to-salesforce}

所有用户都需要单独连接到Salesforce，以便向Salesforce启用日志销售活动(如电子邮件、呼叫和任务)。 但是，作为管理员连接到Salesforce时，您将有机会为整个团队配置活动日志记录设置，以便全局日志记录设置将应用于所有Sales Connect用户。

要将您的Sales Connect实例以管理员或非管理员身份连接到您的Salesforce实例，请按照[本文](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/connect-your-sales-connect-account-to-salesforce.md)中的步骤操作。

![](assets/set-up-sales-connect-3.png)

## 连接到Marketo {#connecting-to-marketo}

连接到Marketo将使您的销售者能够利用营销自动化和营销洞察的强大力量来开展他们的潜在客户工作。 以下功能要求您设置与Marketo的集成。

* 与销售商共享[营销活动](/help/marketo/product-docs/marketo-sales-connect/marketo/make-a-campaign-visible-to-sales-connect-users.md)
* 将[有趣的时刻](/help/marketo/product-docs/marketo-sales-connect/marketo/interesting-moments-in-msc.md)推送到实时动态消息
* 将销售活动记录到Marketo

要进一步了解如何连接到Marketo并授予销售用户访问该连接的权限，请单击此处。

## 正在安装Salesforce自定义包{#installing-salesforce-customization-package}

确保成功启用销售的部分原因是，在其主工作区中拥有适当的功能。 Sales Connect自定义包允许从Salesforce访问参与功能和关键销售活动属性。

要了解有关安装Sales Connect自定义[的详细信息，请单击此处](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/sales-connect-customizations-for-crm.md)。

## 在沙箱{#testing-in-sandbox}中测试

对于要使用其Marketo沙箱测试Marketo Sales Connect的团队，可以根据请求设置一个额外的Sales Connect帐户。 这仅适用于购买了Marketo沙箱的客户，或将其作为Marketo捆绑包的一部分的客户。 如果您对获取沙箱感兴趣，请与您的Marketo客户经理联系。

>[!NOTE]
>
>不能将具有相同电子邮件ID的Sales Connect帐户配置到多个实例。 这意味着，如果您想要拥有一个额外的Sales Connect帐户以使用Marketo沙箱实例进行测试，则需要在每个帐户中使用不同的电子邮件ID。

>[!MORELIKETHIS]
[管理员权限](/help/marketo/product-docs/marketo-sales-connect/admin/user-access-details.md)>
>
