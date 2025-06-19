---
solution: Marketo Engage
product: marketo
title: 垃圾邮件杀手
description: 此处显示文本
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
source-git-commit: bfa1bc900c2adc263e634a81440b77bef2976d3b
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 3%

---

# 垃圾邮件杀手 {#spam-assassin}

在Marketo Engage中使用SpamAssassin，您可以测试电子邮件内容并查看ISP/邮箱提供商将其标记为垃圾邮件的可能性。

SpamAssassin会分析您的内容并根据各种标准分配分数。 得分越低越好。保持低分很重要，因为发送高分电子邮件可能会对您的总体可投放性产生负面影响。

## 访问垃圾邮件报告 {#access-the-spam-report}

1. 在“模拟”屏幕中，单击&#x200B;**垃圾邮件报告**&#x200B;按钮。

屏幕快照

1. 生成垃圾邮件报告。

屏幕快照

1. 检查每个项目的得分和描述。

>[!IMPORTANT]
>
>如果总体分数高于5，则您的电子邮件可能会在投放时被阻止或标记为垃圾邮件。

1. 如果您认为分数过高，请在Email Designer中编辑您的内容，然后重新运行垃圾邮件报表，直到分数为您想要的位置。

屏幕快照

>[!NOTE]
>
>垃圾邮件分数通过SpamAssassin获得，而规则不归Adobe所有。 有关这些规则的更多详细信息，请参阅[SpamAssassin文档](https://spamassassin.apache.org/#_blank)。 可以在此处[&#128279;](https://spamassassin.apache.org/old/tests_3_0_x.html?utm_source=chatgpt.com)查看错误的完整列表。
