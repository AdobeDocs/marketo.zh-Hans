---
title: 了解目标跟踪和预测注册
description: 了解目标跟踪和预计注册
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '969'
ht-degree: 0%

---


# 了解目标跟踪和预计注册

<br> 

在[设置事件目标](/help/sky/setting-event-goals.md)并通过[智能活动](/help/sky/create-a-smart-campaign.md)发送邀请后，下面将介绍如何跟踪目标进度并了解Marketo的预测。

>[!NOTE]
>
>在Marketo Classic中创建事件项目时，事件开始日期当前默认为事件创建日期。 由于预计注册会考虑事件开始日期之前的时间，因此如果开始日期和创建日期相同（除非有意设置），则这些数字可能不准确。

## 目标跟踪和预计注册

1. 您可以在事件项目的&#x200B;**[!UICONTROL Reports]**&#x200B;选项卡中找到目标跟踪详细信息。 在这一具体例子中，到目前为止有150名注册成员，而目标是200(75%)。

   ![图像1](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-1.png)

您还会看到您的&#x200B;**[!UICONTROL Projected]**&#x200B;注册。 将指针悬停在信息图标上，可按似然区段查看此数字的细分。

![图像2](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-2.png)

>[!NOTE]
>
>“已出席”和“更高”图表在事件日之前将保持为空。

1. 单击“图表”切换以按注册可能性切换到成员细分。 您将看到每个区段的当前注册百分比，与过去项目该区段的平均百分比相比。

   ![图3](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-3.png)

所有成员（已注册且尚未注册）均根据其注册可能性进行分类。 将指针悬停在“信息”图标上，查看如何定义这些似然类别。

![图像4](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-4.png)

>[!NOTE]
>
>预测数字每24小时更新一次，直到事件日。 列为&#x200B;_处理_&#x200B;的所有成员都将包括在下一个计算周期中。

## 类似项目

您可以通过查看过去的相似事件执行情况来深入了解当前项目。 此部分显示过去6个月中最多5个类似项目，其成员数／百分比为&#x200B;_Registered_&#x200B;或更高。

在计算相似项目时，我们包括以下因素：

* 项目类型
* 项目渠道
* 受众大小
* 项目标记
* 从事件创建到事件开始的持续时间
* 事件持续时间

   ![图像5](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-5.png)

## Recommendations

在“报告”页面顶部，您可以根据您的进度找到AI/ML驱动的推荐。 定期回访，获取有用的提示和见解！

![图6](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-6.png)

## 人员级预测

单击&#x200B;**[!UICONTROL Members]**&#x200B;选项卡以视图所有项目成员。 将鼠标悬停在&#x200B;**[!UICONTROL Registration Likelihood]**&#x200B;或&#x200B;**[!UICONTROL Attendance Likelihood]**&#x200B;栏上可查看确切百分比和分类。 然后，您可以对特定类别中的成员(例如，“不太可能”中的每个成员注册类别)采取操作，并特别是目标他们以潜在地增加您的注册号码。

![图像七](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-7.png)

>[!NOTE]
>
>个人可能性考虑了40多个人员因素，包括用户档案属性、人员活动和过去受邀／注册／参加的活动。

## 常见问题解答

**问：什么是区段？**

答：可能要注册的值为0到100。 每个事件项目的成员都会得到0-100的可能性值。

我们将似然值分为三个细分：

* 注册的可能性>50% =高可能区段
* 注册的可能性>25%到&lt;50% =可能区段
* 注册的可能性&lt;25% =可能性较小的区段

当某人有可能注册时，预测将属于其中一个细分(每个项目成员都属于其中一个细分)。 例如，如果事件项目根据似然预测有1000个成员，则这些1000将分发到&#x200B;_Highly Pocibity_、_Pocibity_&#x200B;或&#x200B;_Less Pocibity_&#x200B;区段。

因此，属于“极可能性”部分的用户注册事件的机率更高。

转换为注册人数=区段中注册人数除以属于该区段的人员人数(例如，如果100人属于“极可能”区段，其中60人注册，则转化率为60%)。

将%转换为注册模式：极可能性>可能性>不太可能。

**问：如何使用洞察？**

答：最佳做法包括：

我。您创建项目，然后智能活动使用“大于X”的预测过滤器，这将导致特定人数（例如1000人）并运行活动。

ii. 24小时后，在[!UICONTROL Reports]选项卡中，您可以看到根据注册当前受邀人员的值的可能性计算出的预计注册。

iii. 如果预计的注册数少于目标数，您必须邀请更多人员。 此时，您可以看到一些洞察，告诉您过去项目的阈值是什么。

![图像8](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-8.png)

iv. 您可以创建具有此阈值的新智能活动来邀请更多人。

v.在任何时间点，如果您想要了解显示预计数字的原因，您可以切换以查看受众在区段间的分布情况、过去的转化率，以及将这些转化率应用于当前受众（请参阅下面的截图）。

**问：什么是“按注册划分的区段”图？**

答：三个条，每个条代表一个区段（极可能、极可能、极不可能）。

**紫色虚线：根** 据过去的类似项目，在该区段中注册的平均对话率。

**蓝色条：** 该区段中所有人的注册百分比。

![图像9](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-9.png)

例如，假设100人有可能注册超过50%，而注册的100人中有60人。 转化率很可能为60%。 因此，添加到项目的所有成员都获得注册值的可能性，然后将其放入区段中，并根据每个区段转化率中注册的人数计算这些值。

**问：“注册和更高”是什么意思？**

答：列为已注册的人员，或具有等于或更高步骤编号的任何其他状态。

您可以为事件项目创建新晋升状态，但我们会映射那些具有标准状态的状态。 请考虑某人从被邀请转到被提醒的情况，这比注册要高。 此人也将被视为已注册并在目标跟踪中显示。

![图像十](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-10.png)

**问：如何计算预计注册？**

答：请参见下文。

![图11](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-11.png)
