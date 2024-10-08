---
description: 参与度映射选项卡 — Marketo文档 — 产品文档
title: “参与图”选项卡
exl-id: 8c4d076a-d8aa-44ff-b538-ca6a6778697a
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '949'
ht-degree: 0%

---

# “参与图”选项卡 {#engagement-map-tab}

参与度图通过一系列触发器、过滤器和流量卡表示。 单击每个卡片将显示其他信息。

触发器概述：此信息卡显示促销活动中的触发器数量。 单击此图标将显示每个触发器的卡片，以及包含以下信息的滑出面板：

* 触发器所属的营销活动
* 触发器名称列表
* 编辑触发器

  ![](assets/engagement-map-tab-1.png)

触发器详细信息：此信息卡显示触发器名称。 单击此图标将显示一个滑出面板，其中包含以下信息：

* 触发器所属的营销活动
* 与触发器关联的约束列表
* 编辑触发器

筛选器：单击此卡片将显示一个弹出面板，其中显示以下信息：

* 过滤器所属的营销活动
* 符合筛选条件的估计人数
* 筛选器及其相应限制的列表
* 编辑筛选器

  ![](assets/engagement-map-tab-3.png)

流程步骤：如果流程步骤包含选项，则此卡将显示流程步骤的名称。 单击此图标将显示一个滑出面板，其中包含以下信息：

* 流程步骤所属的活动
* 与流程步骤关联的选择条件列表
* 编辑流程步骤

流程步骤：如果流程步骤&#x200B;_不_&#x200B;包含任何选项，则此卡片将显示与流程步骤关联的属性。 单击此图标将显示一个滑出面板，其中包含以下信息：

* 流程步骤所属的活动
* 与流程步骤关联的属性列表
* 编辑流程步骤

  ![](assets/engagement-map-tab-5.png)

## 执行和请求营销活动的流程步骤 {#flow-step-for-execute-and-request-campaigns}

* 如果执行或请求营销活动流量步骤不包含任何选项，则信息卡将显示营销活动的名称。 单击卡片将显示一个弹出面板，其中包含以下信息：

   * 流程步骤所属的活动
   * 编辑流程步骤
   * 与流程步骤关联的属性列表
   * “查看列表”按钮，这将打开使用特定请求/执行营销活动的营销活动列表

>[!NOTE]
>
>您可以从主营销策划中编辑流量步骤。 要编辑嵌套营销活动，您必须通过滑出面板中的链接导航到该营销活动。

* 如果执行或请求Campaign流程步骤包含多个选项，则单击卡片将显示一个弹出面板，其中包含以下信息：

   * 流程步骤所属的活动
   * 与流程步骤关联的选择条件列表
   * 编辑流程步骤

* 如果执行或请求营销活动包含选项，则单击流量卡片将会展开并显示各个卡片中的所有选项。 单击&#x200B;_选择_&#x200B;卡将展开与特定选择关联的营销活动，并显示包含以下信息的滑出面板：

   * 选择所属的营销活动
   * 编辑选项
   * 与流程步骤关联的选择条件列表
   * 查看列表，这将打开使用特定请求/执行营销活动的营销活动列表

  ![](assets/engagement-map-tab-10.png)

## 可视化嵌套的执行活动 {#visualizing-a-nested-execute-campaign}

执行与父营销活动系列运行的营销活动。 符合可执行营销活动资格的人完成该营销活动的所有流程步骤，然后返回到主营销活动以继续执行此营销活动的流程步骤。

以下是智能营销活动“营销活动A”的示例，其中包括执行营销活动流程步骤。 将“营销活动A”视为您的主要营销活动。

![](assets/engagement-map-tab-11.png)

1. 单击执行营销活动流量卡会展开以显示“营销活动B”的详细信息。
1. “营销活动B”包括将受众拆分为两个组的过滤器：合格受众和未合格受众。
1. 符合条件的受众将执行与“促销活动B”相关的流程步骤。
1. 所有受众（无论是否合格）都将返回到“营销活动A”并进入下一个流程步骤。

   ![](assets/engagement-map-tab-12.png)

您可以单击“促销活动B”中的“执行促销活动流程”步骤，该步骤将展开以显示与每个选择关联的选择卡和促销活动。

![](assets/engagement-map-tab-13.png)

## 可视化请求营销活动 {#visualizing-request-campaign}

请求营销活动与父营销活动并行运行。 符合请求营销活动条件的人员完成该营销活动的所有流量步骤，然后退出该营销活动。 同时，同一组人员将执行主营销活动中的流量步骤。

以下是智能营销活动“营销活动A”的示例，其中包括请求营销活动流程步骤。 将“营销活动A”视为您的主要营销活动。

![](assets/engagement-map-tab-14.png)

1. 单击请求营销活动流量卡将展开以显示“营销活动B”的详细信息
1. “营销活动B”包括将受众拆分为两个组的过滤器：合格受众和未合格受众。
1. 符合条件的受众将执行与“促销活动B”相关的流程步骤。
1. 同时，所有受众将转移到“营销活动A”中的下一个流量步骤。

   ![](assets/engagement-map-tab-15.png)

如果任何流量步骤包含其他请求营销活动，您可以深入了解嵌套营销活动，方法是单击流量卡查看营销活动的详细信息。

![](assets/engagement-map-tab-16.png)

以下是包含选项的请求营销活动的示例。

![](assets/engagement-map-tab-17.png)

## 错误处理 {#error-handling}

智能列表和流程步骤中的错误将通过信息卡中的红色图标突出显示。 此外，相应的错误消息将反映在滑出面板中。

智能列表和流量步骤中的警告将通过信息卡中的橙色图标突出显示。 此外，相应的警告消息将反映在滑出面板中。

以下是“选择”卡中的警告示例，该警告显示在“执行Campaign”流程步骤卡、滑出面板和默认选择卡中。

![](assets/engagement-map-tab-18.png)

>[!NOTE]
>
>警告是需要审查的建议，但并不表示Smart Campaign中有错误。

**筛选器卡片中的错误可能包括：**

* 智能列表中发生错误，导致无法显示符合条件的受众

* 筛选器逻辑中有错误

* 一个或多个过滤器中的约束（或缺少约束）出错

  ![](assets/engagement-map-tab-20.png)

>[!NOTE]
>
>在单击展开嵌套营销活动之前，不会显示嵌套营销活动中的错误。
