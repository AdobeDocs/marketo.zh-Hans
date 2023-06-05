---
description: 连接到Outlook - Marketo文档 — 产品文档
title: 连接到Outlook
source-git-commit: 2538bd5973eb3372352c3ddbada6521911f9fc33
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 0%

---

# 连接到Outlook {#connect-to-outlook}

了解如何将Sales Insight Actions帐户与Outlook连接。

>[!NOTE]
>
>每个用户都需要从其Marketo Sales帐户连接到Outlook。

## 正在连接到Outlook Online {#connecting-to-outlook-online}

连接到Outlook意味着您将获得回复跟踪、对Outlook投放渠道的访问权限、在Outlook中计划电子邮件的能力以及发送合规性。

1. 在Marketo Sales中，单击齿轮图标并选择 **设置**.

   ![](assets/connect-to-outlook-1.png)

1. 在我的帐户下，选择 **电子邮件设置**.

   ![](assets/connect-to-outlook-2.png)

1. 单击 **电子邮件连接** 选项卡。

   ![](assets/connect-to-outlook-3.png)

1. 单击 **开始使用**.

   ![](assets/connect-to-outlook-4.png)

1. 选择 **我使用Outlook发送电子邮件** 并单击 **下一个**.

   ![](assets/connect-to-outlook-5.png)

1. 选择您正在使用的Outlook版本，然后单击 **下一个**. 在本例中，我们选择了Outlook Online。

   ![](assets/connect-to-outlook-6.png)

   <table> 
    <tbody>
     <tr>
      <td><strong>Outlook联机</strong></td> 
      <td>也称为Exchange Online</td> 
     </tr>
     <tr>
      <td><strong>Exchange On-premise</strong></td> 
      <td>包括Exchange 2013和2016</td> 
     </tr>
    </tbody>
   </table>

   >[!NOTE]
   >
   >Marketo目前不支持Exchange混合帐户。

1. 单击 **确定**.

   ![](assets/connect-to-outlook-7.png)

1. 如果您未登录Outlook，请输入您的登录信息并单击 **下一个**. 如果是，请选择想要连接的帐户，然后单击 **下一个**. 在本例中，我们已经登录。

   ![](assets/connect-to-outlook-8.png)

1. 单击 **接受**.

   ![](assets/connect-to-outlook-9.png)

   您可以使用此连接来跟踪电子邮件，也可以将其用作投放渠道。

   >[!NOTE]
   >
   >Outlook Online (Office365)强制执行其自身的发送限制。 [在此处了解详情](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md#email-provider-limits).

## 连接到Exchange On-Premise {#connecting-to-exchange-on-premise}

连接到Exchange内部部署意味着您将获得回复跟踪、对Outlook投放渠道的访问权限、在Outlook中计划电子邮件的能力以及发送合规性。

1. 在Marketo Sales中，单击齿轮图标并选择 **设置**.

   ![](assets/connect-to-outlook-10.png)

1. 在我的帐户下，选择 **电子邮件设置**.

   ![](assets/connect-to-outlook-11.png)

1. 单击 **电子邮件连接** 选项卡。

   ![](assets/connect-to-outlook-12.png)

1. 单击 **开始使用**.

   ![](assets/connect-to-outlook-13.png)

1. 选择 **我使用Outlook发送电子邮件** 并单击 **下一个**.

   ![](assets/connect-to-outlook-14.png)

1. 选择您正在使用的Outlook版本，然后单击 **下一个**. 在此示例中，我们选择了Exchange On-premise。

   ![](assets/connect-to-outlook-15.png)

   <table> 
    <tbody>
     <tr>
      <td><strong>Outlook联机</strong></td> 
      <td>也称为Exchange Online</td> 
     </tr>
     <tr>
      <td><strong>Exchange On-premise</strong></td> 
      <td>包括Exchange 2013和2016</td> 
     </tr>
    </tbody>
   </table>

1. 输入您的凭据，然后单击 **Connect**.

   ![](assets/connect-to-outlook-16.png)

   >[!NOTE]
   >
   >如果您在Exchange版本下拉列表中关闭自动发现，则需要向IT部门询问Exchange URL。

   您可以使用此连接来跟踪电子邮件，也可以将其用作投放渠道。

   >[!NOTE]
   >
   >在使用Exchange内部部署时，您的IT团队将建立您的电子邮件发送限制。

## 正在获取连接到Outlook Online的权限 {#getting-permission-to-connect-to-outlook-online}

您可能需要与IT团队合作，以获得允许Marketo Sales连接到Outlook Online帐户(Microsoft 365)的权限。

>[!NOTE]
>
>通知管理您的Microsoft 365帐户的IT团队，需要访问的应用程序是“Marketo Sales Connect”。

根据您的IT团队的偏好和当前配置，最好咨询他们如何授予访问权限。 下面是一些有助于指导对话的文章。

* 全局同意： [适用于Microsoft 365管理员的集成应用程序和Azure AD](https://learn.microsoft.com/en-us/microsoft-365/enterprise/integrated-apps-and-azure-ads?view=o365-worldwide){target="_blank"}
* 用户同意： [配置用户如何同意应用程序](https://learn.microsoft.com/en-us/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal&amp;pivots=portal){target="_blank"}
* 管理员同意： [配置管理员同意工作流](https://learn.microsoft.com/en-us/microsoft-365/admin/misc/user-consent?source=recommendations&amp;view=o365-worldwide){target="_blank"}
* 打开或关闭用户同意： [在Microsoft 365中管理用户对应用程序的同意](https://learn.microsoft.com/en-us/microsoft-365/admin/misc/user-consent?source=recommendations&amp;view=o365-worldwide){target="_blank"}
* 使用Microsoft Defender进行管理： [管理OAuth应用程序](https://learn.microsoft.com/en-us/defender-cloud-apps/manage-app-permissions){target="_blank"}
