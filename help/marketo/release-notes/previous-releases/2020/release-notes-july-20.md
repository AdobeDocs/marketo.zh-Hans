---
unique-page-id: 45416698
description: 发行说明 — 2020年7月 — Marketo文档 — 产品文档
title: 发行说明 — 2020年7月
exl-id: 3c9b1f1d-961c-4bf8-8b99-37b483230506
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 0%

---

# 发行说明： 2020年7月 {#release-notes-july}

2020年7月版中包含以下功能。 查看Marketo版本以了解功能可用性。

>[!AVAILABILITY]
>
>请注意，根据您当前的包，带星号( ![(star)](assets/yellow-star.png))可能需要购买附加值。 请联系您的Marketo Engage代表以了解更多信息。

**_季度版本_** 以下功能将发布于 **2020年7月31日**.

## 管理 {#administration}

* **[字段管理中的“使用者”导出](/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md)**：管理员现在可以将选定字段的所有“使用者”资产链接导出到CSV文件。 此增强功能可以帮助管理员和非管理员清除未使用的字段。 此外，现在还可以在新的浏览器选项卡或窗口中打开资产。

## Account-Based Marketing {#account-based-marketing}

![(star)](assets/yellow-star.png)

* **更新了帐户分析的UI**：通过简化步骤在单个屏幕中完成，简化“帐户分析”中目标帐户列表的创建。

<br> 

**_整个季度发布_**

以下功能属于非季度周期，将在未来几个月发布。

* **Forms服务**：我们将推出更强大的表单字段语法验证功能，并能够使用新的安全域阻止常见的机器人模式，以实现登陆页面功能。 阻止机器人模式可以减少垃圾邮件表单提交并改善数据库质量。

>[!NOTE]
>
>已推迟到2021年1月版之后全面推出增强型表单字段语法验证。

* **增加了资源API URI大小限制**：统一资源标识符(URI)大小限制在删除“_method”参数之前从8 KB增加到65 KB。 执行长查询字符串时，增加此大小限制将允许数据更轻松地传递。 即将进行的安全升级中包含删除“_method”参数。

## 销售分析 {#sales-insight}

![(star)](assets/yellow-star.png)

* **[为具有非本机Salesforce CRM集成的客户启用了Sales Insight](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md) (Beta)**：现在，通过非本机Salesforce CRM集成Marketo Engage客户可以使用Sales Insight帮助其销售团队了解、优先考虑最活跃的销售线索和机会并与之交互，以实现智能销售和更快的交易。

## Sales Connect {#sales-connect}

![(star)](assets/yellow-star.png)

* **[增强了销售呼叫的双方同意：](/help/marketo/product-docs/marketo-sales-connect/phone/two-party-consent-settings.md)** 管理员现在可以更好地控制呼叫记录配置。 [启用通话录制](/help/marketo/product-docs/marketo-sales-connect/phone/enable-call-recording.md) 确保遵守两方同意法。 自动通知正在录制的呼叫，并激活要在呼叫前播放的音频剪辑。

<br> 

## 公告和弃用 {#announcements-deprecations}

* **资产API“_method”参数删除**： 2020年9月之后，Asset API端点将不再接受“_method”在POST正文中传递查询参数以绕过URI长度限制。 为了适应需要此参数的请求，资源API的URI限制将从8 KB增加到65 KB。
* **[Munchkin关联潜在客户](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**：在此版本的Munchkin JavaScript客户端版本159中，我们将开始弃用Munchkin Associate Lead方法。 如果调用，您将收到一则警告，指示将在未来版本中删除该方法。 删除后，该方法将无法再正常使用，并且尝试使用它将失败。 最近使用此方法的Marketo Engage客户将单独收到有关其使用的通知。
* **支持Internet Explorer**：如之前宣布的，对Internet Explorer 11的Marketo Engage支持结束于 **2020年7月31日**. 我们将继续支持Google Chrome、Mozilla Firefox、Apple Safari和Microsoft Edge。
* **天空默认体验**：在此版本中，将删除管理员或用户将Marketo Sky设置为默认体验的选项，为更新主用户体验做准备。 有关主要体验更新的更多详细信息计划在今年晚些时候发布，将于7月发布。 已将Marketo Sky设置为默认体验或已授予Marketo Sky访问权限的用户可以继续从“我的Marketo”主页上的图块访问Marketo Sky。
* **EdgeHTML（非Chromium） Microsoft Edge支持**：从2020年底开始，Marketo Engage将不再支持Microsoft Edge的EdgeHTML版本。 从2021年1月1日开始，我们将仅支持最新的Chromium版本的Microsoft Edge。
