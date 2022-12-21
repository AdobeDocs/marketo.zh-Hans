---
unique-page-id: 11380774
description: 帐户分数 — Marketo文档 — 产品文档
title: 帐户分数
exl-id: 68fb5f41-f715-4a4d-b4da-9db4dc38d67d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# 帐户分数 {#account-score}

帐户评分是Target帐户管理的重要部分。 它有助于您确定帐户的参与程度。

## 什么是帐户评分？ {#what-is-account-scoring}

这是一种系统化的方法，旨在帮助销售和营销团队识别最有可能购买的公司（包括潜在客户）并排定其优先级。

在复杂的B2B购买流程中，很少有一个人做出购买决策。 通常涉及各种角色，每个角色都有各自的需求。 基于帐户的评分通过从多个潜在客户汇总潜在客户得分并在帐户级别提供得分来考虑这一点。

## 常见示例 {#common-examples}

<table> 
 <tbody>
  <tr>
   <td><strong>帐户参与度分数</strong></td> 
   <td>根据特定目标帐户中人员跨不同渠道（例如电子邮件、Web和广告）跟踪的行为活动，确定参与深度。</td>
  </tr>
  <tr>
   <td><strong>帐户产品兴趣分数</strong></td>
   <td>目标帐户中显示对特定产品内容感兴趣的人员（例如，下载白皮书）。</td> 
  </tr>
  <tr>
   <td><strong>帐户Web参与度分数</strong></td>
   <td>来自目标帐户访问Web渠道的人员。 可以创建相同的分数来测量来自电子邮件、广告或其他渠道的渠道参与度。</td> 
  </tr>
 </tbody>
</table>

## 如何配置帐户分数 {#how-to-configure-account-score}

>[!NOTE]
>
>要计算帐户分数，您首先需要创建潜在客户分数。 Marketo TAM会自动将潜在客户得分汇总到帐户得分。 例如，我们将举两个上述示例(_帐户产品兴趣分数_ 和 _帐户Web参与度分数_)。
>
>首先，创建潜在客户得分字段，以从目标帐户的每个潜在客户中捕获相关详细信息。\
>然后，将这些潜在客户得分分配给其各自的帐户得分：\
>帐户产品兴趣分数= SUM（潜在客户产品兴趣分数）\
>帐户Web参与度分数= SUM（潜在客户Web参与度分数）

>[!NOTE]
>
>用户可以创建多个帐户参与度分数，并将不同的人员分数分配给不同的帐户分数。

配置潜在客户得分后，请按照以下步骤继续操作。

1. 单击 **管理员**.

   ![](assets/one-1.png)

1. 单击 **Target帐户管理**.

   ![](assets/account-score-2.png)

1. 在评分字段中，单击 **编辑**.

   ![](assets/account-score-3.png)

   >[!NOTE]
   >
   >您可以选择 **五** 字段来计算“帐户分数”。

1. 输入帐户分数名称，单击 **选择人员分数** 下拉菜单，然后选择相应的得分。

   ![](assets/four.png)

1. 单击 **+添加** 添加更多分数。

   ![](assets/five.png)

1. 添加所有所需的分数。 单击 **保存** 完成时。

   ![](assets/six.png)
