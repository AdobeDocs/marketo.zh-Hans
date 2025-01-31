---
description: 销售分析操作管理员设置指南 — Marketo文档 — 产品文档
title: 《 Sales Insight Actions管理员设置指南》
exl-id: 339d518d-445b-4634-ab81-92c9d5541927
feature: Sales Insight Actions
source-git-commit: 1f228323c18204149630a7cb77d6ae0a88b425e3
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---

# 《 Sales Insight Actions管理员设置指南》 {#sales-insight-actions-admin-setup-guide}

>[!NOTE]
>
>Marketo Sales Insight Actions是一个基于Web的应用程序，它通过[Marketo Sales Insight包](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}专门与Salesforce CRM集成。 它有时称为“Marketo Sales”，或简称为“Actions”。

>[!PREREQUISITES]
>
>* 与Adobe客户团队（您的客户经理）确认已为您的Marketo Engage启用MSI操作(如果您没有客户经理，请联系[Marketo支持](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"})。
>* 必须设置您的Marketo/Salesforce同步。

<table>
 <tr>
  <th>角色</th>
  <th>步骤</th>
 </tr>
 <tr>
  <td>Marketo管理员</td>
  <td>设置Marketo Sales帐户</td>
 </tr>
 <tr>
  <td>Marketo管理员或<br/>Salesforce管理员</td>
  <td>将Marketo Sales帐户连接到Salesforce</td>
 </tr>
 <tr>
  <td>Marketo管理员</td>
  <td>将Marketo Sales帐户连接到Marketo</td>
 </tr>
 <tr>
  <td>Marketo管理员</td>
  <td>启动从Marketo到Marketo销售帐户的数据同步</td>
 </tr>
 <tr>
  <td>Marketo管理员</td>
  <td>邀请用户使用MSI操作</td>
 </tr>
 <tr>
  <td>Salesforce管理员</td>
  <td>在Salesforce中安装/升级MSI包</td>
 </tr>
 <tr>
  <td>Salesforce管理员</td>
  <td>在Salesforce中配置MSI-Actions</td>
 </tr>
</table>

## 设置Marketo销售帐户 {#set-up-marketo-sales-account}

1. 在Marketo中，单击&#x200B;**管理员**。

   ![](assets/msi-actions-admin-guide-1.png)

   >[!NOTE]
   >
   >如果您在集成信息卡上未看到客户端ID和客户端密钥，请通过邀请第一个用户激活您的操作实例，您会看到客户端ID和客户端密钥出现。

1. 单击&#x200B;**销售分析**，然后单击&#x200B;**操作配置**。 从要邀请的Marketo管理员列表中选择并单击&#x200B;**发送邀请**。

   ![](assets/msi-actions-admin-guide-2.png)

用户将收到一封电子邮件，其中包含访问该帐户的步骤。

>[!NOTE]
>
>其他用户将不会通过Marketo添加，而是通过Sales Account User Management页面添加。 [单击此处](/help/marketo/product-docs/marketo-sales-connect/admin/invite-users.md){target="_blank"}了解有关添加其他用户的更多信息。

## 将Marketo Sales帐户连接到Salesforce {#connect-marketo-sales-account-to-salesforce}

1. 在您的Marketo Sales帐户中，单击齿轮图标并选择&#x200B;**设置**。

   ![](assets/msi-actions-admin-guide-3.png)

1. 在“管理员设置”下，单击&#x200B;**Salesforce**。

   ![](assets/msi-actions-admin-guide-4.png)

1. 在“连接和自定义项”选项卡中，单击&#x200B;**连接**。

   ![](assets/msi-actions-admin-guide-5.png)

1. 单击&#x200B;**确定**。

   ![](assets/msi-actions-admin-guide-6.png)

如果您已登录Salesforce，则会连接到网络。 否则，系统将要求您登录。

## 将Marketo连接到您的Sales Apps帐户 {#connect-marketo-to-your-sales-apps-account}

1. 在您的Marketo Sales帐户中，单击齿轮图标并选择&#x200B;**设置**。

   ![](assets/msi-actions-admin-guide-7.png)

1. 在“管理员设置”下，单击&#x200B;**Marketo**。

   ![](assets/msi-actions-admin-guide-8.png)

1. 单击&#x200B;**连接**。 然后，将连接您的帐户。

   ![](assets/msi-actions-admin-guide-9.png)

>[!NOTE]
>
>如果未连接，请从Marketo Sales Insight的“Actions Config”选项卡复制凭据，并将它们粘贴到“Setup”选项卡中。

## 启动数据同步 {#initiate-data-sync}

通过Sales Insight Actions的数据统一字段同步，系统可以将人员信息从您的Marketo Engage数据库提取到Sales Insight Actions数据库中，使您的人员数据保持最新，并确保在Marketo和Salesforce中将活动记录到正确的记录中。

>[!CAUTION]
>
>启动数据同步后，您应该&#x200B;**不应**&#x200B;删除您的Sales Insight Actions实例上的原始用户。 这是第一个邀请所发送到的用户。

1. 在Marketo中，单击&#x200B;**管理员**。

   ![](assets/msi-actions-admin-guide-10.png)

1. 单击&#x200B;**销售分析**。

   ![](assets/msi-actions-admin-guide-11.png)

1. 单击&#x200B;**操作配置**&#x200B;选项卡。 在操作字段同步卡中，单击&#x200B;**同步**。

   ![](assets/msi-actions-admin-guide-12.png)

1. 您将看到将同步的字段预览。 单击&#x200B;**开始同步**。

   ![](assets/msi-actions-admin-guide-13.png)

Marketo和Salesforce中存在的人员记录将同步到您的Marketo Sales Apps帐户。

>[!NOTE]
>
>要了解有关Sales Insight Actions、Marketo和Salesforce之间人员和活动数据如何同步的更多信息，请[单击此处](/help/marketo/product-docs/marketo-sales-insight/actions/admin/sync-sales-action-data-with-marketo-and-salesforce.md){target="_blank"}。

## 邀请个人用户执行MSI操作 {#invite-individual-users-to-msi-actions}

1. 在您的Marketo Sales帐户中，单击齿轮图标并选择&#x200B;**设置**。

   ![](assets/msi-actions-admin-guide-14.png)

1. 在“管理员设置”下，选择&#x200B;**用户管理**。

   ![](assets/msi-actions-admin-guide-15.png)

1. 单击&#x200B;**操作**&#x200B;并选择&#x200B;**邀请用户**。

   ![](assets/msi-actions-admin-guide-16.png)

1. 输入电子邮件地址并单击&#x200B;**邀请**。

   ![](assets/msi-actions-admin-guide-17.png)

>[!NOTE]
>
>默认情况下，所有新成员都将添加到“所有人”团队中。

您将收到一条确认消息。

## 通过CSV邀请用户执行MSI操作 {#invite-users-via-csv-to-msi-actions}

1. 在您的Marketo Sales帐户中，单击齿轮图标并选择&#x200B;**设置**。

   ![](assets/msi-actions-admin-guide-18.png)

1. 在“管理员设置”下，选择&#x200B;**用户管理**。

   ![](assets/msi-actions-admin-guide-19.png)

1. 单击&#x200B;**操作**&#x200B;并选择&#x200B;**通过CSV邀请用户**。

   ![](assets/msi-actions-admin-guide-20.png)

1. 在计算机上浏览CSV，选择它，然后单击&#x200B;**下一步**。

   ![](assets/msi-actions-admin-guide-21.png)

1. 确认字段已正确映射，然后单击&#x200B;**邀请**。

   ![](assets/msi-actions-admin-guide-22.png)

发送邀请后，您将收到一条确认消息。

>[!NOTE]
>
>完成此操作后，您可以升级现有的MSI包，或安装新的MSI包，然后转到[在Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/sales-insight-actions-configuration-in-salesforce.md){target="_blank"}中配置MSI操作。
