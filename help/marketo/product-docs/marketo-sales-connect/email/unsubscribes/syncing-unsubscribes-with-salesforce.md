---
unique-page-id: 14746188
description: 取消订阅与Salesforce同步 — Marketo文档 — 产品文档
title: 正在与Salesforce同步取消订阅
exl-id: 1694d7bf-d2f6-4950-8a3e-c7d89c37b276
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# 正在与Salesforce同步取消订阅 {#syncing-unsubscribes-with-salesforce}

## 取消订阅同步到Salesforce的要求 {#requirements-for-unsubscribes-to-sync-to-salesforce}

* 必须启用取消订阅同步（用于夜间同步）
* “选择退出”字段必须安装在Salesforce中
* Sales Connect中的人员记录必须具有Salesforce ID

**推送取消订阅**

在Sales Connect中收集到取消订阅时，我们会将其实时推送到Salesforce，并更新您选择与之同步的任何一个选择退出字段。 如果您禁用了Salesforce同步，我们仍会将取消订阅推送至电子邮件选择退出。

**取消订阅同步**

启用取消订阅同步后（下面的步骤3），您将打开夜间同步。 同步在PST晚上8:00左右每天执行一次。 它将Marketo Sales中的所有取消订阅与Salesforce中的选择退出字段进行双向同步。

## 配置取消订阅同步到Salesforce {#configure-unsubscribe-sync-to-salesforce}

用户可以决定是希望与Marketo也可以同步的标准电子邮件选择退出字段同步其取消订阅内容，还是可以与Marketo销售人员选择退出字段同步，以便区分销售人员取消订阅和营销人员取消订阅内容。

1. 转到 [Web应用程序](https://toutapp.com/login)，单击齿轮图标并选择 **设置**.

   ![](assets/one-1.png)

1. 在管理设置下，选择 **取消订阅**.

   ![](assets/two-2.png)

1. 单击 **正在同步到Salesforce**，然后启用nightly sync。

   ![](assets/three-2.png)

1. 选择要同步到的字段。

   ![](assets/4.png)

   | 字段 | 描述 |
   |---|---|
   | **同步到Salesforce选择退出字段** | 默认情况下处于选中状态，只会更新Salesforce选择退出字段。 |
   | **同步到“Marketo销售人员选择退出”字段** | 如果要区分销售和营销取消订阅，请选择此选项以更新其他 [Marketo Sales Opt Out字段。](#msoo) |

## 在页面布局中安装选择退出字段 {#installing-the-opt-out-field-in-the-page-layout}

**电子邮件选择退出**

电子邮件选择退出是Salesforce中的一个标准字段，可从Salesforce安装。 您必须是Salesforce管理员才能安装该软件。

1. 转到 [Salesforce.com](https://salesforce.com) 并登录。

   ![](assets/five-1.png)

1. 单击您的用户名并选择 **设置**.

   ![](assets/six-1.png)

1. 在快速查找框中，搜索Contact或Lead。 在此方案中，我们将字段安装到联系人页面布局，但您希望为两个人员记录都安装。

   ![](assets/seven-1.png)

1. 选择 **页面布局**.

   ![](assets/eight-1.png)

1. 选择 **编辑** 在页面布局旁边，您可以添加字段。

   ![](assets/nine.png)

1. 选择 **字段**.

   ![](assets/ten.png)

1. 将电子邮件选择退出拖放到页面布局中。

   ![](assets/11.png)

1. 单击 **保存**.

   ![](assets/twelve.png)

## Marketo销售人员选择退出 {#marketo-sales-opt-out}

Marketo Sales Opt Out字段是一个自定义字段，可供安装了Marketo Sales Connect Customizations的用户使用。

成功将Marketo Sales Connect Customizations安装到Salesforce中后，您将看到可供您使用的Marketo Sales Opt Out字段。
