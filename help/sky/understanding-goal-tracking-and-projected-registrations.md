---
title: 了解目标跟踪和预测注册
description: 了解目标跟踪和预计注册
exl-id: 65064cbd-2ed7-45d5-aab9-4fc865e2bed6
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '969'
ht-degree: 0%

---

# 了解目标跟踪和预计注册

<br> 

在[设置事件目标](/help/sky/setting-event-goals.md)并通过[智能活动](/help/sky/create-a-smart-campaign.md)发出邀请后，下面将介绍如何跟踪目标进度并了解Marketo的预测。

>[!NOTE]
>
>在Marketo Classic中创建事件项目时，事件开始日期当前默认为事件创建日期。 由于预计的注册会考虑事件开始日期之前的时间，因此，如果开始日期和创建日期相同（除非有意设置），则这些数字可能不准确。

## 目标跟踪和预计注册

1. 您可以在事件项目的&#x200B;**[!UICONTROL Reports]**&#x200B;选项卡中找到目标跟踪详细信息。 在这一具体例子中，到目前为止有150名注册成员，而目标是200(75%)。

   ![图像1](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-1.png)

您还将看到您的&#x200B;**[!UICONTROL Projected]**&#x200B;注册。 将鼠标悬停在“信息”图标上，可查看按“可能性”区段划分的此数字。

![图2](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-2.png)

>[!NOTE]
>
>“已出席”和“更高”图表在事件日之前将保持为空。

1. 单击“图表”切换按钮，按注册可能性切换到成员划分。 您会看到每个区段的当前注册百分比，与过去项目该区段的平均百分比相比。

   ![图3](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-3.png)

所有成员（已注册且尚未注册）均根据其注册可能性进行分类。 将鼠标悬停在“信息”图标上可查看如何定义这些似然类别。

![图4](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-4.png)

>[!NOTE]
>
>预测数字在事件日之前每24小时更新一次。 列为&#x200B;_Processing_&#x200B;的所有成员都将包含在下一个计算周期中。

## 类似项目

您可以通过查看过去执行的类似事件来深入了解当前项目。 此部分显示了过去6个月中最多5个类似项目，其中&#x200B;_已注册_&#x200B;或更高成员的数量/百分比。

在计算类似项目时，我们包括以下因素：

* 项目类型
* 项目渠道
* 受众大小
* 项目标签
* 从事件创建到事件开始的持续时间
* 事件持续时间

   ![图像5](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-5.png)

## Recommendations

在“报告”页面顶部，您可以根据您的进度找到AI/ML驱动的推荐。 定期回访，获取有用的提示和洞察！

![图6](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-6.png)

## 个人级预测

单击&#x200B;**[!UICONTROL Members]**&#x200B;选项卡以视图您的所有项目成员。 将鼠标悬停在&#x200B;**[!UICONTROL Registration Likelihood]**&#x200B;或&#x200B;**[!UICONTROL Attendance Likelihood]**&#x200B;栏上可查看确切百分比和分类。 然后，您可以对特定类别中的成员(例如，“不太可能”中的每个成员进行注册类别)采取操作，具体来说就是目标他们以潜在地增加您的注册号。

![图七](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-7.png)

>[!NOTE]
>
>个人可能性考虑了40多个人因素，包括用户档案属性、人员活动和过去的受邀/注册/出席活动。

## 常见问题解答

**问：什么是区段？**

答：可能要注册的值为0到100。 每个是事件项目成员的人都将获得0到100之间的可能性值。

我们将似然值分为三个细分：

* 注册的可能性>50% =极有可能的区段
* 注册的可能性>25%到&lt;50% =可能的区段
* 注册的可能性&lt;25% =不太可能的区段

当一个人有可能注册时，预测就会归入其中一个细分(每个项目成员都会归入其中一个细分)。 例如，如果事件项目基于似然预测有1000个成员，则这些1000将分发到&#x200B;_Highly Pacibility_、_Pocibility_&#x200B;或&#x200B;_Less Pocibility_&#x200B;区段。

因此，属于“极有可能”部分的人员注册事件的机率更高。

转换为注册=区段中注册的人数除以属于该区段的人数(例如，如果100人属于“极有可能”区段，而其中60人属于注册，则转化率为60%)。

将%转换为注册将遵循以下模式：极有可能>可能>不可能。

**问：如何使用洞察？**

答：最佳做法包括：

我。您创建一个项目，然后智能活动使用“大于X”的预测过滤器，这将导致特定数量的人（例如1000人）并运行活动。

ii. 24小时后，在[!UICONTROL Reports]选项卡中，您可以看到根据注册当前受邀人员的值的可能性计算出的预计注册。

iii. 如果预计的注册数低于目标数，您必须邀请更多人。 此时，您可以看到一些洞察，告诉您过去项目的阈值是什么。

![图像8](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-8.png)

iv. 您可以使用该阈值创建新的智能活动以邀请更多人。

v.如果您希望了解投影数目显示的原因，您可以随时切换以查看各区段的受众分布、过去的转化率，并将这些转化率应用到当前受众（请参阅下面的截图）。

**问：什么是“按注册划分的区段”图？**

答：三个条，每个条代表一个区段（极有可能、极可能、极不可能）。

**紫色虚线：根** 据过去的类似项目，在该区段中注册的平均对话率。

**蓝条：该** 区段中所有人员的注册百分比。

![图9](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-9.png)

例如，假设100人有可能注册超过50%，而100人中有60人注册。 极有可能实现60%的转化率。 因此，添加到项目的所有成员都获得注册值的可能性，然后将它们放入区段中，并根据每个区段转化率中注册的人数计算这些值。

**问：“注册和更高”是什么意思？**

答：列为已注册的人员，或具有等于或更高步骤号的任何其他状态。

您可以为事件项目创建新的晋升状态，但我们会将这些状态映射为标准状态。 以某人从被邀请转到被提醒的情况为例，这比注册要高。 此人也将被视为已注册并显示在目标跟踪中。

![图10](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-10.png)

**问：如何计算预计的注册？**

答：请参见下文。

![图11](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-11.png)
