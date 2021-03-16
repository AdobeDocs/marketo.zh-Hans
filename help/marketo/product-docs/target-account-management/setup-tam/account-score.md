---
unique-page-id: 11380774
description: 帐户分数 — Marketo Docs — 产品文档
title: 帐户分数
translation-type: tm+mt
source-git-commit: 9f88e7cebc5e9d0d4491d65d332ccfdd9a31c395
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---


# 帐户分数{#account-score}

帐户评分是目标帐户管理的重要部分。 它可以帮助您确定帐户的参与程度。

## 什么是帐户评分？{#what-is-account-scoring}

这是一种系统化方法，旨在帮助销售和营销团队确定最可能进行购买的公司(包括潜在客户)并确定其优先级。

在复杂的B2B购买流程世界中，很少有个人做出购买决策。 参与的角色往往各不相同，每个角色都有自己的需求。 基于帐户的评分通过从多个潜在客户中汇总潜在客户得分并在帐户级别提供得分来考虑这一点。

## 常见示例{#common-examples}

<table> 
 <tbody>
  <tr>
   <td><strong>帐户参与分数</strong></td> 
   <td>根据特定目标帐户中人员跨不同渠道（例如电子邮件、Web和广告）跟踪的行为活动，实现深度参与。</td>
  </tr>
  <tr>
   <td><strong>帐户产品兴趣分数</strong></td>
   <td>目标帐户中显示对特定产品内容感兴趣的人员（例如下载白皮书）。</td> 
  </tr>
  <tr>
   <td><strong>帐户Web参与分数</strong></td>
   <td>来自目标帐户的访问Web渠道的人员。 可以创建相同的分数来衡量来自电子邮件、广告或其他渠道的渠道参与度。</td> 
  </tr>
 </tbody>
</table>

## 如何配置帐户分数{#how-to-configure-account-score}

>[!NOTE]
>
>要计算帐户分数，您首先需要创建潜在客户分数。 Marketo TAM会自动将潜在客户得分聚合到帐户得分。 作为示例，我们将举两个以上示例（_帐户产品兴趣分数_&#x200B;和&#x200B;_帐户Web参与分数_）。
>
>首先，创建从目标帐户的每个潜在客户捕获相关详细信息的潜在客户得分字段。\
>然后，将这些潜在客户分数分配给各自的帐户分数：\
>帐户产品兴趣得分= SUM（潜在客户产品兴趣得分）\
>帐户Web参与分数= SUM（潜在客户Web参与分数）

>[!NOTE]
>
>用户可以创建多个帐户参与分数，并为不同的帐户分数分配不同的人员分数。

配置潜在客户得分后，请按照以下步骤继续。

1. 单击&#x200B;**管理员**。

   ![](assets/one-1.png)

1. 单击&#x200B;**目标帐户管理**。

   ![](assets/account-score-2.png)

1. 在“评分字段”中，单击&#x200B;**编辑**。

   ![](assets/account-score-3.png)

   >[!NOTE]
   >
   >您最多可以选择&#x200B;**五个**&#x200B;字段来计算帐户分数。

1. 输入帐户分数名称，单击&#x200B;**选择人员分数**&#x200B;下拉框并选择相应的分数。

   ![](assets/four.png)

1. 单击&#x200B;**+Add**&#x200B;可添加更多分数。

   ![](assets/five.png)

1. 添加所有所需的分数。 完成后，单击&#x200B;**保存**。

   ![](assets/six.png)
