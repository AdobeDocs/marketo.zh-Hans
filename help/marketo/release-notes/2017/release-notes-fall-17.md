---
unique-page-id: 12983280
description: 发行说明 — 1917年秋季 — Marketo文档 — 产品文档
title: 发行说明 — 2017年秋季
exl-id: 329022e6-f388-4ff9-9724-62aeed76c0b9
source-git-commit: cbfa6110e85c185a5b65342052f168d9715f2f6a
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 0%

---

# 发行说明：’17年秋季 {#release-notes-fall}

’17年秋季版本中包含以下功能。 查看您的Marketo版本以了解功能的可用性。

请单击标题链接以查看每项功能的详细文章。 注意：此版本中包含的某些功能没有相关文章。 如果一个主题具有多个子标题，则链接会放置在该位置。

## 系统可靠性 {#system-reliability}

我们进一步改进了Marketo核心基础设施，包括更好的顺序、更少的不匹配以及改进Munchkin稳定性。

## SFDC同步性能 {#sfdc-sync-performance}

利用Marketo和Salesforce之间更丰富、更快的同步。 需要对帐户或潜在客户进行批量更新的数据更改可以拆分为并行队列以避免积压日志。 事件和任务现在的同步速度也提高了50%。

## Analytics性能改进 {#analytics-performance-improvements}

最近的基础架构改进增加了Marketo报告和分析工具内的正常运行时间和稳定性，使您能够更快地构建临时报告。

## [收件人时区](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md) {#recipient-time-zone}

利用此新功能，您现在可以按当地时区保留和发送电子邮件。 可以将电子邮件和参与计划配置为按收件人的时区发送，从而无需创建多个计划 — 发送一次，Marketo会自动保留电子邮件直到到正确的当地时间。 提升电子邮件量度，观察本地实践，并在全球使用单个程序节省时间。

![](assets/image2017-11-29-8-3a45-3a47.png)

>[!NOTE]
>
>如果您尚未对电子邮件和参与项目启用收件人时区，请不要惊慌！ 我们正在逐步向所有客户启用此功能。

## [按区段查看示例电子邮件](/help/marketo/product-docs/email-marketing/general/creating-an-email/send-a-sample-email.md) {#review-sample-emails-by-segment}

Marketo新增了一个选项，用于在发送示例电子邮件以供审阅时选取区段。 您不再需要手动确定潜在客户属于哪个区段，从而更轻松地向不同区段发送包含动态内容的电子邮件。

## [linkedIn Lead Gen自定义问题](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md) {#linkedin-lead-gen-custom-questions}

自定义您的LinkedIn潜在客户生成表单，以收集自定义潜在客户属性。 现在，您最多可以在每个表单中提出三个自定义问题，从单行文本输入或多选题中进行选择，然后映射回Marketo潜在客户字段。

## Slack集成 {#slack-integration}

我们发布了两项功能，作为新Slack集成的一部分：

* 系统通知：获取有关Marketo实例中重要事件的Slack通知，例如有关当前促销活动状态以及任何需要立即注意的问题的警报。
* 有趣的时刻：当Marketo Insight由销售帐户中的已知个人触发时，可以通过Slack通知潜在客户所有者。 通知包括潜在客户信息以及有关销售帐户的详细信息。

## ABM增强功能 {#abm-enhancements}

**[显示无联系人的帐户](https://docs.marketo.com/x/fKCt)**

Marketo ABM现在无需联系人即可同步并显示CRM帐户。 包括没有以前销售或营销历史记录的新帐户，并通过将后续潜在客户匹配到帐户来跟踪进度。

## ContentAI Analytics {#contentai-analytics}

**[新的ABM帐户列表过滤器](https://docs.marketo.com/x/1BPG)**

查看和比较ABM帐户列表中的内容性能，以优化现有内容。 ContentAI会向您显示：

* 查看的热门内容
* 顶部转换内容
* 基于AI的营销活动建议内容

## Web个性化增强功能 {#web-personalization-enhancements}

**[Web促销活动的令牌](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

令牌现在可在Web营销活动中使用。 利用令牌提供个性化的消息和内容，以提高您的Web营销活动参与度。

![](assets/image2017-11-16-11-3a25-3a7.png)

**[在Web Campaign编辑器中设计Studio图像](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

在Marketo中跨多个渠道重复使用创意资产和图像，从而节省时间。

![](assets/image2017-11-16-11-3a26-3a10.png)

## 集成  {#integration}

**[电子邮件预览API](https://developers.marketo.com/rest-api/assets/emails/)**

您现在可以在Marketo之外远程预览电子邮件，从而简化电子邮件内容本地化流程并减少错误。

**[替换HTML API](https://developers.marketo.com/rest-api/assets/emails/)**

开发人员可以远程更新电子邮件资产的HTML内容，以便在单个系统中工作以维护资产。
