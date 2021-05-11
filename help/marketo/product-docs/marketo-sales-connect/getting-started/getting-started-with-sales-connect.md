---
unique-page-id: 13796466
description: Sales Connect快速入门 — Marketo Docs — 产品文档
title: Sales Connect入门
exl-id: 8c5b1f65-449c-4304-b904-fc6442a47e5a
translation-type: tm+mt
source-git-commit: 20ccc6ba2b26b869776ed88ed6fe76a67f74400a
workflow-type: tm+mt
source-wordcount: '624'
ht-degree: 0%

---

# Sales Connect {#getting-started-with-sales-connect}入门

如果您希望观看这些步骤而不是阅读它们，请直接跳到](#video)下面的[视频说明。

>[!AVAILABILITY]
>
>并非所有客户都购买了此功能。 有关更多信息，请联系您的客户成功经理。

## 您需要入门的内容{#what-you-need-to-get-started}

* Marketo 订阅
* Sales Connect订阅
* Salesforce订阅（启用API调用和Apex类）

## 您需要从谁开始{#who-you-need-to-get-started}

* Marketo Admin用户
* Sales Connect管理员用户
* Salesforce管理员
* Sales Connect用户

## Sales Connect管理员{#sales-connect-admins}

您将收到一封来自Marketo的电子邮件，其中包含重置密码的链接。 创建新口令后，请登录Sales Connect。

要完成设置，您必须执行以下操作：

* [连接Sales Connect和Salesforce](#connect-your-sales-connect-account-to-salesforce)
* [在将Sales Connect与Marketo连接之前获取凭据](#acquiring-credentials-prior-to-connecting-sales-connect-with-marketo)
* [Connect Sales Connect与Marketo](#connect-sales-connect-to-marketo)
* [邀请/设置用户](#invite-provision-users)

（可选）您还可以：

* [在沙箱中测试销售连接](#test-sales-connect-in-your-sandbox)

## 将您的Sales Connect帐户连接到Salesforce {#connect-your-sales-connect-account-to-salesforce}

要将您的Sales Connect帐户以管理员或非管理员身份连接到您的Salesforce帐户，请按照[本文](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/connect-your-sales-connect-account-to-salesforce.md)中的步骤操作。

>[!NOTE]
>
>您所连接的Salesforce实例必须与已（或将）连接到Marketo的实例相同。

## 在将Sales Connect与Marketo{#acquiring-credentials-prior-to-connecting-sales-connect-with-marketo}连接之前获取凭据

您需要从Marketo中获取一组凭据。 以后，销售连接管理员将使用这些凭据将Marketo与销售连接连接。

1. 在Marketo中，单击&#x200B;**Admin**。

   ![](assets/one.png)

1. 在树中，单击&#x200B;**Sales Connect**。

   ![](assets/two.png)

1. 选择以下Marketo凭据并将其发送给您的Sales Connect管理员：Munchkin ID、客户端ID、客户端机密。

   ![](assets/3.jpg)

   >[!NOTE]
   >
   >复制并粘贴上述信息时，请确保未添加空格。

## 将Sales Connect连接到Marketo {#connect-sales-connect-to-marketo}

1. 在Sales Connect中，单击齿轮图标，然后选择&#x200B;**设置**。

   ![](assets/four.png)

1. 在“管理设置”下，选择&#x200B;**Marketo**。

   ![](assets/eight.png)

1. 输入Marketo管理员提供的Marketo凭据，然后单击&#x200B;**Connect**。

   ![](assets/credentials.png)

## 邀请/设置用户{#invite-provision-users}

如果您的帐户（以前来自ToutApp）上已存在任何用户，他们将显示在Sales Connect的Marketo部分的&#x200B;**团队访问**&#x200B;选项卡中。

您可以通过此页面将您的团队设置为Marketo Sales Connect用户。 如果您从未使用过ToutApp，或尚未邀请用户，请按照[本文](/help/marketo/product-docs/marketo-sales-connect/admin/invite-users.md)中的步骤操作。

>[!CAUTION]
>
>在将Sales Connect与Marketo连接后，请等待十分钟，然后再执行这些步骤。

1. 选择一个或多个用户，然后单击&#x200B;**Connect**。

   >[!NOTE]
   >
   >在邀请用户时，您只能进行一次工作区分配。 设置完毕后，您必须断开用户连接才能更改它。

   ![](assets/users.png)

1. 如果您的Marketo订阅启用了工作区，您可以批量将工作区分配给每个用户或一组用户。 如果未选择任何工作区，我们会将它们分配给默认Marketo工作区。

   ![](assets/nine.jpg)

1. 单击“工作区”(Workspace)下拉框，选择所需的工作区，然后单击&#x200B;**Connect**。

   ![](assets/ten.png)

   >[!NOTE]
   >
   >如果要添加新用户，请转到“管理设置”的“团队管理”部分，然后单击&#x200B;**邀请用户**&#x200B;按钮。

您可以从“团队管理”页面添加更多用户，然后按照上述步骤与他们连接。

## 在沙箱{#test-sales-connect-in-your-sandbox}中测试Sales Connect

对于要使用其Marketo沙箱测试Marketo Sales Connect的团队，可以根据请求设置一个额外的Sales Connect帐户。 这仅适用于购买了Marketo沙箱的客户，或将其作为Marketo捆绑包的一部分的客户。 如果您对获取沙箱感兴趣，请与您的Marketo客户经理联系。

>[!NOTE]
>
>不能将具有相同电子邮件ID的Sales Connect帐户配置到多个实例。 这意味着，如果您想要拥有一个额外的Sales Connect帐户以使用Marketo沙箱实例进行测试，则需要在每个帐户中使用不同的电子邮件ID。
