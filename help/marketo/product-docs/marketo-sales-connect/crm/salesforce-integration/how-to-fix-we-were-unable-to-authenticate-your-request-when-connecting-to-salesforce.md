---
unique-page-id: 14352484
description: 如何修复连接到Salesforce时“我们无法验证您的请求” — Marketo文档 — 产品文档
title: 如何修复连接到Salesforce时“我们无法验证您的请求”的问题
exl-id: ddd49064-f584-4490-8d45-29cf61ed3ebe
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 3%

---

# 如何修复连接到[!DNL Salesforce]时“我们无法验证您的请求” {#how-to-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

如果您在尝试将[!DNL Sales Connect]连接到[!DNL Salesforce]时收到错误消息“我们无法验证您的请求”，则您的访问[!DNL Salesforce]的API可能会受到限制。 与您的[!DNL Salesforce]管理员确认以下事项。

## 在用户权限中启用API {#enable-api-in-user-permissions}

1. 让[!DNL Salesforce]管理员登录SFDC。
1. 选择 **[!UICONTROL Setup]**。
1. 选择 **[!UICONTROL Manage Users]**。
1. 选择 **[!UICONTROL Profiles]**。
1. 查找ToutApp用户所属的配置文件，然后单击&#x200B;**[!UICONTROL Edit]**。
1. 向下滚动到&#x200B;**[!UICONTROL Administrative Permissions]**&#x200B;并确保选中&#x200B;**[!UICONTROL API Enabled]**。

## 检查[!DNL Salesforce]是否阻止[!DNL Sales Connect]连接 {#check-if-salesforce-is-blocking-sales-connect-from-connecting}

1. 让[!DNL Salesforce]管理员登录SFDC。
1. 选择 **[!UICONTROL Setup]**。
1. 选择 **[!UICONTROL Manage Apps]**。
1. 选择 **[!UICONTROL Connected Apps OAuth Usage]**。
1. 确保[!DNL Sales Connect]旁边显示“[!UICONTROL Block]”。 如果您看到“[!UICONTROL Unblock]”，请单击按钮以取消阻止[!DNL Sales Connect]访问[!DNL Salesforce]。
