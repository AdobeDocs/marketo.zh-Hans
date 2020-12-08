---
unique-page-id: 13796466
description: Sales Connect快速入门- Marketo Docs —— 产品文档
title: 销售连接入门
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '638'
ht-degree: 0%

---


# 销售连接入门 {#getting-started-with-sales-connect}

如果您希望观看这些步骤而不是阅读它们，请直接跳到下面的 [视频说明](#video)。

>[!NOTE]
>
>**可用性**
>
>并非所有客户都购买了此功能。 有关更多信息，请联系您的客户成功经理。

## 您需要的入门 {#what-you-need-to-get-started}

* 营销订阅
* 销售连接订阅
* Salesforce订阅（启用API调用和Apex类）

## 您需要开始的人 {#who-you-need-to-get-started}

* Marketo管理员用户
* 销售Connect管理员用户
* Salesforce管理员
* Sales Connect用户

## 销售Connect管理员 {#sales-connect-admins}

您将收到一封来自Marketo的电子邮件，其中包含重置密码的链接。 创建新密码后，请登录Sales Connect。

要完成设置，您必须执行以下操作：

* [连接销售连接和销售人员](#sfdc)
* [在将Sales Connect与Marketo连接之前获取凭据](#acquire)
* [Connect Sales Connect与Marketo](#mkto)
* [邀请／配置用户](#IPU)

（可选）您还可以：

* [在沙箱中测试销售连接](#sandbox)

## 将您的Sales Connect帐户连接到Salesforce {#connect-your-sales-connect-account-to-salesforce}

要将您的Sales Connect帐户以管理员或非管理员身份连接到您的Salesforce帐户，请按照本文中的 [步骤操作](http://docs.marketo.com/x/JwDb)。

>[!NOTE]
>
>您连接的Salesforce实例必须与已（或将）连接到Marketo的实例相同。

## 在将Sales Connect与Marketo连接之前获取凭据 {#acquiring-credentials-prior-to-connecting-sales-connect-with-marketo}

您需要从Marketo中获取一组凭据。 以后，Sales Connect管理员将使用这些凭据将Marketo与Sales Connect连接。

1. 在Marketo中，单击“管 **理员**”。

   ![](assets/one.png)

1. 在树中，单击“销 **售连接”**。

   ![](assets/two.png)

1. 选择以下Marketo凭据并将其发送给您的Sales Connect管理员：Munchkin ID、Client ID、Client Secret。

   ![](assets/3.jpg)

   >[!NOTE]
   >
   >复制并粘贴上述信息时，请确保未添加任何空格。

## 将销售连接到Marketo {#connect-sales-connect-to-marketo}

1. 在Sales Connect中，单击齿轮图标，然后选择“ **设置**”。

   ![](assets/four.png)

1. 在“管理员设置”下，选 **择Marketo**。

   ![](assets/eight.png)

1. 输入Marketo管理员提供的Marketo凭据，然后单击 **Connect**。

   ![](assets/credentials.png)

## 邀请／配置用户 {#invite-provision-users}

如果您的帐户（以前从ToutApp）上已有任何用户，他们将显示在Sales Connect的“Marketo” **部分的** “团队访问”选项卡中。

您可以通过此页面将您的团队配置为Marketo Sales Connect用户。 如果您从未使用过ToutApp，或尚未邀请用户，请按照本文中的步 [骤操作](http://docs.marketo.com/display/TOUT/Invite+Team+Members)。

>[!CAUTION]
>
>在将Sales Connect与Marketo连接后，请等待十分钟，然后再执行这些步骤。

1. 选择一个或多个用户，然后单击“ **连接**”。

   >[!NOTE]
   >
   >在邀请用户时，您只能进行一次工作区分配。 设置完毕后，您必须断开用户连接才能更改它。

   ![](assets/users.png)

1. 如果您的营销订阅启用了工作区，您将能够批量为每个用户或一组用户分配工作区。 如果未选择任何工作区，我们将将其分配到默认营销工具工作区。

   ![](assets/nine.jpg)

1. 单击“工作区”(Workspace)下拉框，选择所需的工作区，然后单击“ **连接**”。

   ![](assets/ten.png)

   >[!NOTE]
   >
   >如果要添加新用户，请转到“管理设置”的“团队管理”部分，然后单击“邀请 **用户** ”按钮。

您可以从“团队管理”页面添加用户，然后按照上述步骤连接他们。

## 在沙箱中测试销售连接 {#test-sales-connect-in-your-sandbox}

对于希望使用Marketo Sales Connect测试其Marketo Sandbox的团队，可以根据请求设置额外的Sales Connect帐户。 这仅适用于已购买Marketo Sandbox的客户，或将其作为其Marketo捆绑包的一部分的客户。 如果您对获取沙箱感兴趣，请与您的Marketo客户经理联系。

>[!NOTE]
>
>不能将具有相同电子邮件ID的Sales Connect帐户配置到多个实例。 这意味着，如果您希望有一个额外的Sales Connect帐户来测试Marketo沙箱实例，您需要在每个帐户中使用不同的电子邮件ID。

## 视频说明 {#video-instructions}

`<iframe width="630" height="470" src="//play.vidyard.com/w5RY7iMPpEfUYQ4Fp8WUKR.html?v=3.1.1" frameborder="0" allowfullscreen></iframe>`
