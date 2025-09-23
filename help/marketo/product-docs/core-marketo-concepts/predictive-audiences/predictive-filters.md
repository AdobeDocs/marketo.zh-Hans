---
description: 预测过滤器 — Marketo文档 — 产品文档
title: 预测型过滤器
exl-id: 27736b80-cd8b-455d-9d73-c17d492d0906
feature: Predictive Audiences
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# 预测型过滤器 {#predictive-filters}

作为预测受众的一部分，Marketo在智能营销活动的智能列表中提供一组基于AI/ML的过滤器。

![图像1](assets/predictive-filters-1.png)

>[!NOTE]
>
>“可能参加”和“可能注册”过滤器只能在“事件程序”中使用。 “取消订阅的可能性”、“项目成员的相似程度”和“智能列表成员的相似程度”可用于所有项目类型。

## 出席的可能性 {#likelihood-to-attend}

此筛选器用于有效地缩小受众范围。 这有助于您定位和邀请具有较高&#x200B;**可能参加**&#x200B;您的网络研讨会或活动的潜在客户。 请注意，您的“参加计划的可能性”将是您当前的活动计划。

![图像2](assets/predictive-filters-2.png)

## 注册的可能性 {#likelihood-to-register}

与&#x200B;_参加_&#x200B;的可能性过滤器类似，使用此过滤器可缩小受众范围，并定位具有较高&#x200B;**注册率**&#x200B;以用于网络研讨会或活动的潜在客户。

![图像三](assets/predictive-filters-3.png)

## 取消订阅的可能性 {#likelihood-to-unsubscribe}

该功能会根据受众在接下来的两周内取消订阅的可能性高低来过滤受众。 您可以使用此功能以不同方式更有效地定位高疲劳线索。 取消订阅阈值是动态的，并且由AI模型驱动，该模型考虑多个属性，包括数据库中的提前期和潜在客户活动。

![图像四](assets/predictive-filters-4.png)

>[!NOTE]
>
>参加/注册/取消订阅过滤器的可能性必须与其他标准过滤器结合使用。

## 项目成员的相似对象/智能列表成员的相似对象 {#lookalike-of-members}

这两个筛选器可帮助您通过定位与其他项目或智能列表成员相似的其他潜在客户来扩展当前受众。 相似人群拓展过滤器考虑了50多种因素，包括商机属性、电子邮件活动、Web活动和参与。

单击&#x200B;**[!UICONTROL Add Constraint]**&#x200B;为所选计划的成员选择成功标准。

单击&#x200B;**+**&#x200B;图标可轻松将多个程序/智能列表添加到一个筛选器中。

![图像五](assets/predictive-filters-5.png)

## 注意事项 {#things-to-note}

* 即使是在启用预测过滤器之前创建父项目，您也可以将预测过滤器应用于智能营销活动。
* 预测过滤器不可用于触发营销活动。
* 不支持克隆或移动包含预测过滤器的营销活动。
* 一个智能列表中最多可以使用5个预测过滤器。
* 如果Marketo Engage在评估预测过滤器时遇到错误，则营销活动运行将自动中止，并且您将在Marketo通知中心收到通知。
* 预测过滤器当前的输入限制为100万符合条件的人员。
* 您最多可以拥有50个具有预测过滤器的活动项目。
