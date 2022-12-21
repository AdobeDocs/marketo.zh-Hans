---
unique-page-id: 45416698
description: 发行说明 — 2020年7月 — Marketo文档 — 产品文档
title: 发行说明 — 2020年7月
exl-id: 3c9b1f1d-961c-4bf8-8b99-37b483230506
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 0%

---

# 发行说明：’20年7月 {#release-notes-july}

’20年7月版包含以下功能。 查看您的Marketo版本以了解功能的可用性。

>[!AVAILABILITY]
>
>请注意，根据您当前的包，带有星号的项目( ![（星号）](assets/yellow-star.png))可能需要购买值附加组件。 请联系您的Marketo Engage代表以了解更多信息。

**_季度版本_** 将在 **2020年7月31日**.

## 管理 {#administration}

* **[字段管理中的“使用者”导出](/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md)**:管理员现在可以将选定字段的所有“使用者”资产链接导出到CSV文件。 此增强功能可帮助管理员和非管理员清除未使用的字段。 此外，现在还可以在新的浏览器选项卡或窗口中打开资产。

## Account-Based Marketing {#account-based-marketing}

![（星号）](assets/yellow-star.png)

* **更新了用于帐户分析的UI**:通过在单个屏幕中简化所有步骤，简化“帐户分析”中目标帐户列表的创建。

<br> 

**_在整个季度发布_**

以下功能处于非季度周期，将在未来几个月内发布。

* **Forms服务**:我们引入了更强大的表单字段语法验证功能，以及使用新的登陆页面安全域功能阻止常见机器人模式的功能。 阻止机器人模式可减少垃圾邮件表单提交并提高数据库质量。

>[!NOTE]
>
>增强表单字段语法验证的完整推出已推迟到2021年1月版之后。

* **增加了资产API URI大小限制**:在删除“_method”参数之前，统一资源标识符(URI)大小限制将从8KB增加到65KB。 执行长查询字符串时，此大小限制的增加将使数据更容易传递。 删除“_method”参数是即将进行的安全升级的一部分。

## 销售分析 {#sales-insight}

![（星号）](assets/yellow-star.png)

* **[为集成了非本机Salesforce CRM的客户启用了Sales Insight](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md) （测试版）**:将非本机Salesforce CRM集成的Marketo Engage客户现在可以使用Sales Insight帮助其销售团队了解、排定优先级并与最投入的商机和机会进行互动，从而实现智能销售和更快的交易。

## Sales Connect {#sales-connect}

![（星号）](assets/yellow-star.png)

* **[增强了销售呼叫的双方同意：](/help/marketo/product-docs/marketo-sales-connect/phone/two-party-consent-settings.md)** 管理员现在可以更好地控制呼叫记录配置。 [启用呼叫录制](/help/marketo/product-docs/marketo-sales-connect/phone/enable-call-recording.md) 确保您遵守双方同意法。 自动通知正在录制的呼叫，并激活要在呼叫之前播放的音频剪辑。

<br> 

## 公告和弃用 {#announcements-deprecations}

* **删除资产API“_method”参数**:2020年9月之后，Asset API端点将不再接受“_method”在POST正文中传递查询参数以绕过URI长度限制。 为了适应需要此参数的请求，资产API的URI限制将从8KB增加到65KB。
* **[Munchkin Associate Lead](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**:在此版本的Munchkin JavaScript客户端版本159中，我们将开始弃用Munchkin Associate Lead方法。 如果调用，您将收到一则警告，指示将来版本中将删除该方法。 删除该方法后，该方法将不再起作用，尝试使用该方法将失败。 最近使用此方法的Marketo Engage客户将单独收到其使用通知。
* **支持Internet Explorer**:如前所述，Marketo Engage对Internet Explorer 11的支持将在 **2020年7月31日**. 我们将继续支持Google Chrome、Mozilla Firefox、Apple Safari和Microsoft Edge。
* **天空默认体验**:此版本中将删除管理员或用户将Marketo Sky设置为默认体验的选项，以便为主用户体验的更新做准备。 计划在今年晚些时候更新的主要体验的更多详细信息将在7月提供。 将Marketo Sky设置为默认体验或已获得Marketo Sky访问权限的用户，可以继续从“我的Marketo”主页上的拼贴中访问Marketo Sky。
* **EdgeHTML（非Chromium）Microsoft Edge支持**:Marketo Engage2020年底将不再支持Microsoft Edge的EdgeHTML版本。 从2021年1月1日开始，我们将仅支持最新的Chromium版本的Microsoft Edge。
