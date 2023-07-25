---
unique-page-id: 1147114
description: 项目群成员自定义字段令牌 — Marketo文档 — 产品文档
title: 项目群成员自定义字段令牌
exl-id: 3046dec8-b885-4b08-baa9-896bcf3594b2
feature: Tokens
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# 项目群成员自定义字段令牌 {#program-member-custom-field-tokens}

## 项目群成员自定义字段的令牌支持 {#token-support-for-program-member-custom-fields}

在程序成员自定义字段功能的背面，对令牌框架中的程序成员自定义字段的支持正在扩展。

PMCF令牌将在令牌家族的成员域下受支持。

成员令牌用于项目群成员范围内的字段。 截至当前状态，还使用成员令牌插入来自综合服务合作伙伴的唯一值。 `{{member.webinar url}}` 令牌会自动解析服务提供商生成的人员的唯一确认URL。 {{member.registration code}} 解析为服务提供商提供的注册码。

>[!NOTE]
>
>* 项目群成员自定义字段只能在项目群上下文中使用。
>* 项目群成员自定义字段令牌不能在以下位置使用：电子邮件标头、等待步骤中的日期令牌或代码片段。
>* 成员令牌不支持项目群成员状态。

## 在Assets中使用项目群成员自定义字段令牌 {#using-program-member-custom-field-tokens-in-assets}

您可以将项目群成员自定义字段令牌插入电子邮件、登陆页面、短信、推送通知和Webhook中。

**电子邮件**

1. 选择所需的电子邮件并单击 **编辑草稿**.

   ![](assets/program-member-custom-field-tokens-1.png)

1. 单击插入令牌图标。

   ![](assets/program-member-custom-field-tokens-2.png)

1. 查找并选择所需的程序成员自定义字段令牌，输入默认值，然后单击 **插入**.

   ![](assets/program-member-custom-field-tokens-3.png)

1. 单击 **保存**.

   ![](assets/program-member-custom-field-tokens-4.png)

>[!NOTE]
>
>别忘了批准您的电子邮件。

**登陆页面**

1. 选择您的登陆页面并单击 **编辑草稿**.

   ![](assets/program-member-custom-field-tokens-5.png)

   >[!NOTE]
   >
   >登陆页面设计器将在新窗口中打开。

1. 双击要向其添加令牌的富文本框。

   ![](assets/program-member-custom-field-tokens-6.png)

1. 单击您希望令牌所在的位置，然后单击插入令牌图标。

   ![](assets/program-member-custom-field-tokens-7.png)

1. 查找并选择所需的令牌。

   ![](assets/program-member-custom-field-tokens-8.png)

1. 输入默认值并单击 **插入**.

   ![](assets/program-member-custom-field-tokens-9.png)

1. 单击 **保存**.

   ![](assets/program-member-custom-field-tokens-10.png)

**短信**

1. 选择所需的短信并单击 **编辑草稿**.

   ![](assets/program-member-custom-field-tokens-11.png)

1. 单击 **`{{ Token`** 按钮。

   ![](assets/program-member-custom-field-tokens-12.png)

1. 查找并选择所需的项目群成员自定义字段令牌。 输入默认值，然后单击“插入”。

   ![](assets/program-member-custom-field-tokens-13.png)

1. 单击短信操作下拉列表并选择 **批准并关闭**.

   ![](assets/program-member-custom-field-tokens-14.png)

**推送通知**

1. 选择所需的推送通知并单击 **编辑草稿**.

   ![](assets/program-member-custom-field-tokens-15.png)

1. 单击 **推送通知**.

   ![](assets/program-member-custom-field-tokens-16.png)

1. 单击编辑器中的消息，然后单击 `{{` 按钮以获取令牌选择器。

   ![](assets/program-member-custom-field-tokens-17.png)

1. 查找并选择所需的项目群成员自定义字段令牌。 输入默认值并单击 **插入**.

   ![](assets/program-member-custom-field-tokens-18.png)

1. 单击 **完成** 保存并退出(或 **下一个** ，以首先查看)。

   ![](assets/program-member-custom-field-tokens-19.png)

>[!NOTE]
>
>如果程序成员的程序成员自定义字段没有值，则令牌将被默认值替换（如果已提供）。

## 在营销活动中使用项目成员自定义字段令牌 {#using-program-member-custom-field-tokens-in-campaigns}

项目群成员自定义字段令牌可用于以下位置：

* 创建任务
* 在Microsoft中创建任务
* 有趣的时刻
* 更改数据值流操作
* Webhook
