---
unique-page-id: 12983280
description: 发行说明 — ’17年秋季 — Marketo文档 — 产品文档
title: 发行说明 — 1917年秋季
exl-id: 329022e6-f388-4ff9-9724-62aeed76c0b9
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 0%

---

# 发行说明：’17年秋{#release-notes-fall}

’17年秋季版包含以下功能。 查看您的Marketo版本以了解功能可用性。

请单击标题链接，以视图每种功能的详细文章。 注意：此版本中包含的部分功能没有相关文章。 如果一个主题有多个子标题，则链接将放在该位置。

## 系统可靠性{#system-reliability}

我们对核心Marketo基础架构做了进一步改进，包括更好的顺序、更少的不匹配和提高Munchkin的稳定性。

## SFDC同步性能{#sfdc-sync-performance}

充分利用Marketo和Salesforce之间更丰富、更快的同步。 需要对帐户或潜在客户进行批量更新的数据更改可以拆分为并行队列以避免积压日志。 事件和任务现在同步速度提高了50%。

## 分析性能改进{#analytics-performance-improvements}

最近基础架构改进优惠提高了Marketo报告和分析工具中的正常运行时间和稳定性，使您能够更快地构建临时报告。

## [收件人时区](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md) {#recipient-time-zone}

利用此新功能，您现在可以根据当地时区保存和发送电子邮件。 可以将电子邮件和参与项目配置为在收件人的时区内发送，无需创建多个项目 — 发送一次，Marketo将自动保留电子邮件，直到正确的本地时间。 全球使用单一项目，提升电子邮件指标、观察本地实践并节省时间。

![](assets/image2017-11-29-8-3a45-3a47.png)

>[!NOTE]
>
>如果您还无法为电子邮件和参与项目启用收件人时区，请勿恐慌！ 我们正在逐步向所有客户启用此功能。

## [按区段查看示例电子邮件](/help/marketo/product-docs/email-marketing/general/creating-an-email/send-a-sample-email.md) {#review-sample-emails-by-segment}

Marketo在发送示例电子邮件以供审阅时，有一个新选项可选择区段。 您不再需要手动确定潜在客户属于哪个区段，从而更轻松地向不同区段发送包含动态内容的电子邮件。

## [linkedIn Lead Gen自定义问题](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md) {#linkedin-lead-gen-custom-questions}

自定义LinkedIn潜在客户生成表单以收集自定义潜在客户属性。 现在，您最多可以为每个表单提出三个自定义问题，从单行文本输入或多选题中进行选择，然后映射回Marketo潜在客户字段。

## [Slack集成](/help/marketo/product-docs/administration/additional-integrations/add-slack-as-a-launchpoint-service.md) {#slack-integration}

我们发布了两个功能，作为新Slack集成的一部分：

* 系统通知：获取有关Marketo实例中重要事件的Slack通知，如有关当前活动状态和任何需要立即注意的问题的警告。
* 有趣的时刻：当Marketo Insight由销售帐户中的已知个人触发时，潜在客户所有者可以通过Slack获得通知。 通知包括潜在客户信息以及有关销售帐户的详细信息。

## ABM增强{#abm-enhancements}

**[显示没有联系人的帐户](https://docs.marketo.com/x/fKCt)**

Marketo ABM现在无需联系人即可同步和显示CRM帐户。 包括没有以前销售或营销历史的新帐户，并通过将后续潜在客户匹配到帐户来跟踪进度。

## ContentAI分析{#contentai-analytics}

**[新的ABM帐户列表过滤器](https://docs.marketo.com/x/1BPG)**

视图和比较ABM帐户列表中的内容性能，以优化现有内容。 ContentAI向您展示：

* 查看的内容
* 顶部转换的内容
* 面向营销活动的基于人工智能的建议内容

## Web个性化增强{#web-personalization-enhancements}

**[Web活动令牌](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

现在可在Web活动中使用令牌。 利用令牌提供个性化消息和内容，提高Web活动的参与度。

![](assets/image2017-11-16-11-3a25-3a7.png)

**[在Web活动编辑器中设计Studio图像](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

在Marketo中跨多个渠道重复使用创意资源和图像，从而节省时间。

![](assets/image2017-11-16-11-3a26-3a10.png)

## 集成{#integration}

**[电子邮件预览API](https://developers.marketo.com/rest-api/assets/emails/)**

您现在可以远程预览Marketo以外的电子邮件，简化电子邮件内容本地化流程并减少错误。

**[替换HTML API](https://developers.marketo.com/rest-api/assets/emails/)**

开发人员可以远程更新电子邮件资源的HTML内容，使他们能够在单个系统中工作以维护资源。
