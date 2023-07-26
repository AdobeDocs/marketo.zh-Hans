---
description: 了解目标跟踪和预计注册 — Marketo文档 — 产品文档
title: 了解目标跟踪和预计注册
exl-id: 110768f4-46ed-4951-96b2-a97813d7b257
feature: Predictive Audiences
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '986'
ht-degree: 0%

---

# 了解目标跟踪和预计注册 {#understanding-goal-tracking-and-projected-registrations}

下面是如何跟踪目标进度并了解Marketo的预测的。

>[!PREREQUISITES]
>
>要访问其中的大多数功能，请确保启用 [下一代切换](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md){target="_blank"} 用于事件程序。

>[!NOTE]
>
>在Marketo Classic Experience中创建事件程序时，事件开始日期当前默认为事件创建日期。 由于预计注册会考虑事件开始日期之前经过的时间，因此如果开始日期和创建日期相同（除非有意设置），则这些数字可能不准确。

## 目标跟踪和预计注册

1. 有关目标跟踪的详细信息，请参阅 **[!UICONTROL 报表]** 选项卡。 在这一具体例子中，迄今有150名注册成员，而目标为200名(75%)。

   ![](assets/understanding-goal-tracking-and-projected-registrations-1.png)

您还将看到您的 **[!UICONTROL 预计]** 注册。 将鼠标悬停在信息图标上可查看按可能性区段划分此数字的细分。

![](assets/understanding-goal-tracking-and-projected-registrations-2.png)

>[!NOTE]
>
>在活动开始之前，“已参加”和“更高”图表将一直为空。

如果未启用切换开关，下面显示了它在Marketo类UI中的显示方式：

![](assets/understanding-goal-tracking-and-projected-registrations-3.png)

1. 单击图表切换开关可按注册可能性切换到成员细分。 您将看到每个区段的当前注册百分比与过去计划中该区段的平均百分比的比较。

   ![](assets/understanding-goal-tracking-and-projected-registrations-4.png)

所有成员（已注册和未注册）均根据其注册可能性进行分类。 将鼠标悬停在信息图标上可查看这些可能性类别的定义方式。

![](assets/understanding-goal-tracking-and-projected-registrations-5.png)

>[!NOTE]
>
>预测数字每24小时更新一次，直到事件发生的那天为止。 任何成员列为 _正在处理_ 将被包含在下一个计算周期中。

## 类似计划

您可以通过查看类似程序在过去中的执行情况，深入了解当前事件。 此部分向您显示过去6个月内多达5个类似的计划，以及符合以下条件的成员数量/百分比 _已注册_ 或更高。

在计算类似程序时，我们特别包括以下因素：

* 项目类型
* 项目频道
* 受众规模
* 项目标记
* 从事件创建到事件开始的时间
* 事件持续时间

  ![](assets/understanding-goal-tracking-and-projected-registrations-6.png)

## 推荐

在报告页面顶部，您可以根据自己的进度找到由AI/ML驱动的推荐。 请定期回来查看以获取有用的提示和见解！

![](assets/understanding-goal-tracking-and-projected-registrations-7.png)

## 人员级别预测

单击 **[!UICONTROL 成员]** 选项卡查看您的所有计划成员。 将鼠标悬停在 **[!UICONTROL 注册可能性]** 或 **[!UICONTROL 出席可能性]** 栏查看精确的百分比和分类。 然后，您可以对特定类别中的成员（例如，“不太可能”注册类别中的每个人）执行操作，并明确定向这些成员，以便潜在地提高您的注册数量。

![](assets/understanding-goal-tracking-and-projected-registrations-8.png)

>[!NOTE]
>
>个人可能性会考虑40多个人员因素，包括个人资料属性、人员活动以及过去受邀/注册/参加的活动。

## 常见问题解答

**问：什么是区段？**

A：可能注册的值介于0到100之间。 每个活动计划成员都可获得0-100之间的似然值。

我们将似然值分为三个部分：

* 注册的可能性大于50% =极有可能的区段
* 注册的可能性大于25%到&lt;50% =可能的区段
* 注册的可能性&lt;25% =可能性较低的区段

当一个人获得注册的可能性时，预测将属于这些区段之一（每个身为项目成员的人都将属于这些区段之一）。 例如，如果根据可能性预测某个活动项目拥有1000名成员，则这1000名成员将被分发到 _很有可能_， _可能_，或 _不太可能_ 区段。

因此，属于“极有可能”区段的用户更有可能注册该事件。

转化为注册用户=已注册区段中的人员数除以属于该区段的人数（例如，如果100人属于极有可能的区段，并且其中60人注册，则转化率为60%）。

要注册的转化百分比将遵循以下模式：可能性>可能性>可能性。

**问：如何使用洞察？**

答：最佳做法包括以下内容：

i.您创建一个项目，然后智能营销活动使用“大于X”的预测过滤器，这会产生一定数量的人员（假设1000人），并且您运行该营销活动。

二、 24小时后，在 [!UICONTROL 报表] 选项卡，您可以查看根据注册当前受邀所有人员值的可能性计算的预计注册。

三、 如果预计注册次数少于目标，则必须邀请更多人员。 此时，您可以看到一些见解，其中说明了阈值在过去项目中是否有效。

![](assets/understanding-goal-tracking-and-projected-registrations-9.png)

四、 您可以使用该阈值创建新的Smart Campaign以邀请更多人员。

v.如果您想要了解为什么显示预计数量，可以在任意时间点切换以查看各区段之间的受众分布及其过去的转化率，并将这些转化率应用于当前受众（请参阅下面的屏幕快照）。

**问：什么是按注册区段图？**

答案：三个栏，每个栏代表一个区段（可能性高，可能性高，可能性低）。

**紫色虚线：** 在该区段中注册的平均会话率，基于以往的类似计划。

**蓝色条形：** 该区段中所有人员的注册百分比。

![](assets/understanding-goal-tracking-and-projected-registrations-10.png)

例如，假设有100个人可能注册了50%以上的用户，而这100个人中有60个人可能注册。 转化率很可能为60%。 因此，添加到该计划的所有成员都获得注册值的可能性，然后将其放入区段，并根据每个区段注册的人数计算转化率。

**问：“已注册和更高”是什么意思？**

A：被列为已注册人员或具有相等或更高步骤编号的任何其他身份的人员。

您可以为事件程序创建新的进度状态，但我们会将这些状态映射到标准状态。 考虑将某人从受邀人中移往提醒人的情况，这是比登记更高的一步。 此用户也将被视为已注册并显示在目标跟踪中。

![](assets/understanding-goal-tracking-and-projected-registrations-11.png)

**问：如何计算预计注册数？**

答：请参见下文。

![](assets/understanding-goal-tracking-and-projected-registrations-12.png)
