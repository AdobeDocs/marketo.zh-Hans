---
unique-page-id: 1147114
description: 计划成员自定义字段令牌 — Marketo文档 — 产品文档
title: 程序成员自定义字段令牌
exl-id: 3046dec8-b885-4b08-baa9-896bcf3594b2
source-git-commit: 30f56d93dfd5a600ef3ea75d352ede12c6104940
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# 程序成员自定义字段令牌 {#program-member-custom-field-tokens}

## 程序成员自定义字段的令牌支持 {#token-support-for-program-member-custom-fields}

在程序成员自定义字段功能的后面，正在扩展对令牌框架中程序成员自定义字段的支持。

令牌系列的成员域将支持PMCF令牌。

成员令牌用于属于程序成员范围的字段。 自当前状态起，成员令牌还用于插入来自集成服务合作伙伴的唯一值。 `{{member.webinar url}}` 令牌会自动解析由服务提供商生成的人员的唯一确认URL。 {{member.registration code}} 解析为服务提供商提供的注册代码。

>[!NOTE]
>
>* 程序成员自定义字段只能在程序的上下文中使用。
>* 程序成员自定义字段令牌不能在中使用：电子邮件预标头、等待步骤中的日期令牌或代码片段。
>* 成员令牌中不支持程序成员状态。


## 在资产中使用项目成员自定义字段令牌 {#using-program-member-custom-field-tokens-in-assets}

您可以将项目成员自定义字段令牌插入电子邮件、登陆页、短信、推送通知和Webhook。

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
>不要忘记批准您的电子邮件。

**登陆页面**

1. 选择您的登陆页面并单击 **编辑草稿**.

   ![](assets/program-member-custom-field-tokens-5.png)

   >[!NOTE]
   >
   >登陆页面设计器将在新窗口中打开。

1. 双击要将令牌添加到的富文本框。

   ![](assets/program-member-custom-field-tokens-6.png)

1. 单击令牌所在的位置，然后单击插入令牌图标。

   ![](assets/program-member-custom-field-tokens-7.png)

1. 查找并选择所需的令牌。

   ![](assets/program-member-custom-field-tokens-8.png)

1. 输入默认值并单击 **插入**.

   ![](assets/program-member-custom-field-tokens-9.png)

1. 单击 **保存**.

   ![](assets/program-member-custom-field-tokens-10.png)

**短信**

1. 选择所需的短信，然后单击 **编辑草稿**.

   ![](assets/program-member-custom-field-tokens-11.png)

1. 单击 **`{{ Token`** 按钮。

   ![](assets/program-member-custom-field-tokens-12.png)

1. 查找并选择所需的程序成员自定义字段令牌。 输入默认值，然后单击“插入”。

   ![](assets/program-member-custom-field-tokens-13.png)

1. 单击短信操作下拉列表，然后选择 **批准并关闭**.

   ![](assets/program-member-custom-field-tokens-14.png)

**推送通知**

1. 选择所需的推送通知并单击 **编辑草稿**.

   ![](assets/program-member-custom-field-tokens-15.png)

1. 单击 **推送通知**.

   ![](assets/program-member-custom-field-tokens-16.png)

1. 单击编辑器中的消息，然后单击 `{{` 按钮以获取令牌选择器。

   ![](assets/program-member-custom-field-tokens-17.png)

1. 查找并选择所需的程序成员自定义字段令牌。 输入默认值并单击 **插入**.

   ![](assets/program-member-custom-field-tokens-18.png)

1. 单击 **完成** 保存并退出(或 **下一个** 先审阅)。

   ![](assets/program-member-custom-field-tokens-19.png)

>[!NOTE]
>
>如果程序成员的程序成员自定义字段没有值，则如果已提供该令牌，则将用默认值替换该令牌。

## 在营销活动中使用项目成员自定义字段令牌 {#using-program-member-custom-field-tokens-in-campaigns}

程序成员自定义字段令牌可用于：

* 创建任务
* 在Microsoft中创建任务
* 有趣的时刻
* 更改数据值流操作
* Webhooks
