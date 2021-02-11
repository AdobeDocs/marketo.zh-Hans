---
unique-page-id: 14746188
description: 与Salesforce同步取消订阅——营销文档——产品文档
title: 与Salesforce同步取消订阅
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---


# 与Salesforce {#syncing-unsubscribes-with-salesforce}同步取消订阅

## 取消订阅同步到Salesforce {#requirements-for-unsubscribes-to-sync-to-salesforce}的要求

* 必须启用取消订阅同步（用于夜间同步）
* 字选择退出段必须安装在Salesforce中
* Sales Connect中的人员记录必须具有Salesforce ID

**取消订阅推送**

在Sales Connect中收集取消订阅时，我们会实时将其推送到Salesforce并更新您选选择退出定要同步的任一字段。 如果您已禁用Salesforce同步，我们仍会将取消订阅推送到电子邮件选择退出。

**取消订阅同步**

启用取消订阅同步后（下面的步骤3），您将打开晚间同步。 在太平洋标准时间晚上8:00左右，每天进行一次同步。 它将MSE/ToutApp中的所有未订阅与Salesforce中选择退出的字段双向同步。

## 配置与Salesforce的取消订阅同步{#configure-unsubscribe-sync-to-salesforce}

用户可以决定是要将其取消订阅与Marketo还可以同步的选择退出标准电子邮件字段同步，还是可以与Marketo销售字段同步选择退出，以便能够区分销售取消订阅和营销取消订阅。

1. 转至[Web应用程序](https://toutapp.com/login)，单击齿轮图标并选择&#x200B;**设置**。

   ![](assets/one-1.png)

1. 在“管理设置”下，选择&#x200B;**取消订阅**。

   ![](assets/two-2.png)

1. 单击&#x200B;**同步到Salesforce**，然后启用晚间同步。

   ![](assets/three-2.png)

1. 选择要同步到的字段。

   ![](assets/4.png)

   | 字段 | 说明 |
   |---|---|
   | **同步到Salesforce字选择退出段** | 默认情况下，选中此项后，仅更新Salesforce选择退出字段。 |
   | **同步到Marketo销售字选择退出段** | 如果要将“销售”和“市场营销”分开取消订阅，请选择此选项以更新其他[“市场选择退出营销”字段。](#msoo) |

## 在页选择退出面布局{#installing-the-opt-out-field-in-the-page-layout}中安装字段

**电子邮件选择退出**

电选择退出子邮件是Salesforce中可从Salesforce安装的标准字段。 您必须是Salesforce管理员才能安装它。

1. 转到[Salesforce.com](https://salesforce.com)并登录。

   ![](assets/five-1.png)

1. 单击您的用户名，然后选择&#x200B;**Setup**。

   ![](assets/six-1.png)

1. 在“快速查找”框中，搜索联系人或潜在客户。 在此方案中，我们将字段安装到“联系人”页面布局，但您将要为两个人记录安装。

   ![](assets/seven-1.png)

1. 选择&#x200B;**页面布局**。

   ![](assets/eight-1.png)

1. 选择要添加字段的页面布局旁的&#x200B;**编辑**。

   ![](assets/nine.png)

1. 选择&#x200B;**字段**。

   ![](assets/ten.png)

1. 将电子邮件拖选择退出放到页面布局中。

   ![](assets/11.png)

1. 单击&#x200B;**保存**。

   ![](assets/twelve.png)

## 营销人选择退出员销售{#marketo-sales-opt-out}

“Marketo Sales”选择退出字段是自定义字段，对于已安装Marketo Sales Connect自定义项的用户可用。

成功将Marketo Sales Connect自定义项安装到Salesforce后，您将看到可供您使用的选择退出Marketo Sales字段。
