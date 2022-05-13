---
description: Sales Insight Actions管理指南 — Marketo文档 — 产品文档
title: Sales Insight Actions管理指南
exl-id: 339d518d-445b-4634-ab81-92c9d5541927
source-git-commit: 451b5cd8e11045de56ebf57c2b2312813d5d5668
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 0%

---

# Sales Insight Actions管理指南 {#sales-insight-actions-admin-guide}

>[!PREREQUISITES]
>
>* 与您的Marketo成功经理确认已为您的客户成功帐户启用MSI操作(如果您没有CSM，请联系 [Marketo支持](https://nation.marketo.com/t5/support/ct-p/Support){target=&quot;_blank&quot;})。
>* 必须设置您的Marketo/Salesforce同步。


<table>
 <tr>
  <th>角色</th>
  <th>步骤</th>
 </tr>
 <tr>
  <td>Marketo管理员</td>
  <td>设置Marketo销售帐户</td>
 </tr>
 <tr>
  <td>Marketo管理员或 <br/>Salesforce管理员</td>
  <td>将Marketo销售帐户连接到Salesforce</td>
 </tr>
 <tr>
  <td>Marketo管理员</td>
  <td>将Marketo销售帐户连接到Marketo</td>
 </tr>
 <tr>
  <td>Marketo管理员</td>
  <td>启动从Marketo到Marketo销售帐户的数据同步</td>
 </tr>
 <tr>
  <td>Marketo管理员</td>
  <td>邀请用户使用MSI-Actions</td>
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

1. 在Marketo中，单击 **管理员**.

   ![](assets/msi-actions-admin-guide-1.png)

1. 单击 **销售分析**，则 **操作配置**. 从Marketo管理员列表中选择以邀请并单击 **发送邀请**.

   ![](assets/msi-actions-admin-guide-2.png)

用户将收到一封电子邮件，其中包含获取帐户访问权限的步骤。

>[!NOTE]
>
>其他用户将不会通过Marketo添加，而是通过销售帐户用户管理页面添加。 [单击此处](/help/marketo/product-docs/marketo-sales-connect/admin/invite-users.md){target=&quot;_blank&quot;}以了解有关添加其他用户的更多信息。

## 将Marketo销售帐户连接到Salesforce {#connect-marketo-sales-account-to-salesforce}

1. 在您的Marketo Sales帐户中，单击齿轮图标，然后选择 **设置**.

   ![](assets/msi-actions-admin-guide-3.png)

1. 在“管理员设置”下，单击 **Salesforce**.

   ![](assets/msi-actions-admin-guide-4.png)

1. 在连接和自定义选项卡中，单击 **连接**.

   ![](assets/msi-actions-admin-guide-5.png)

1. 单击 **确定**.

   ![](assets/msi-actions-admin-guide-6.png)

如果您已登录Salesforce，则将连接您。 如果没有，你将被要求登录。

## 将Marketo连接到您的销售应用程序帐户 {#connect-marketo-to-your-sales-apps-account}

1. 在您的Marketo Sales帐户中，单击齿轮图标，然后选择 **设置**.

   ![](assets/msi-actions-admin-guide-7.png)

1. 在“管理员设置”下，单击 **Marketo**.

   ![](assets/msi-actions-admin-guide-8.png)

1. 单击 **connect**. 然后，您的帐户将连接。

   ![](assets/msi-actions-admin-guide-9.png)

>[!NOTE]
>
>如果未连接，请复制Marketo Sales Insight“操作配置”选项卡中的凭据，并将其粘贴到设置选项卡中。

## 启动数据同步 {#initiate-data-sync}

Sales Insight Actions的Marketo Engage统一字段同步使系统能够将人员信息从您的Sales Insight Actions数据库中提取到Sales Insight Actions数据库中，保持人员数据为最新，并确保活动记录到Marketo和Salesforce中的正确记录中。

>[!CAUTION]
>
>启动数据同步后，您应 **not** 删除Sales Insight Actions实例上的原始用户。 这是将第一个邀请发送到的用户。

1. 在Marketo中，单击 **管理员**.

   ![](assets/msi-actions-admin-guide-10.png)

1. 单击 **销售分析**.

   ![](assets/msi-actions-admin-guide-11.png)

1. 单击 **操作配置** 选项卡。 在操作字段同步卡中，单击 **同步**.

   ![](assets/msi-actions-admin-guide-12.png)

1. 您将看到将同步的字段预览。 单击 **开始同步**.

   ![](assets/msi-actions-admin-guide-13.png)

Marketo和Salesforce中存在的人员记录将同步到您的Marketo销售应用程序帐户。

>[!NOTE]
>
>要进一步了解Sales Insight Actions、Marketo和Salesforce之间人员和活动数据如何同步， [单击此处](/help/marketo/product-docs/marketo-sales-insight/actions/admin/actions-data-sync-faq.md){target=&quot;_blank&quot;}。

## 邀请个人用户执行MSI操作 {#invite-individual-users-to-msi-actions}

1. 在您的Marketo Sales帐户中，单击齿轮图标，然后选择 **设置**.

   ![](assets/msi-actions-admin-guide-14.png)

1. 在“管理员设置”下，选择 **用户管理**.

   ![](assets/msi-actions-admin-guide-15.png)

1. 单击 **操作** 选择 **邀请用户**.

   ![](assets/msi-actions-admin-guide-16.png)

1. 输入电子邮件地址并单击 **邀请**.

   ![](assets/msi-actions-admin-guide-17.png)

>[!NOTE]
>
>默认情况下，所有新成员都将添加到“每个人”团队。

您将收到确认消息。

## 通过CSV邀请用户执行MSI操作 {#invite-users-via-csv-to-msi-actions}

1. 在您的Marketo Sales帐户中，单击齿轮图标，然后选择 **设置**.

   ![](assets/msi-actions-admin-guide-18.png)

1. 在“管理员设置”下，选择 **用户管理**.

   ![](assets/msi-actions-admin-guide-19.png)

1. 单击 **操作** 选择 **通过CSV邀请用户**.

   ![](assets/msi-actions-admin-guide-20.png)

1. 在您的计算机上浏览CSV，选择它，然后单击 **下一个**.

   ![](assets/msi-actions-admin-guide-21.png)

1. 确认字段已正确映射，然后单击 **邀请**.

   ![](assets/msi-actions-admin-guide-22.png)

发送邀请后，您将收到确认消息。

>[!NOTE]
>
>完成此操作后，您可以升级现有MSI包，或安装新包并转到 [在Salesforce中配置MSI操作](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-configuration/sales-insight-actions-configuration-in-salesforce.md){target=&quot;_blank&quot;}。
