---
title: 模型健康与数据有效性
description: 模型健康与数据有效性
exl-id: b14ec648-be1c-467b-b41d-2c53d74e25ea
source-git-commit: 41a51afde7942d6973a01636810bc5862d023e99
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---

# 模型健康与数据有效性

模型的性能取决于输入数据的质量和完整性。 查看每种可能性AI模型的主要影响因素。 另请参阅导致事件注册次数增加/减少、事件出席或取消订阅的主要因素。

>[!NOTE]
>
>标记有(+)的行为对预测产生积极影响（反之亦然）。

下面是如何评估模型健康状况。

导航到 **[!UICONTROL Models and Data Health]** 部分 **[!UICONTROL Predictive Audiences]** 在 **[!UICONTROL Admin]** Marketo Classic地区。 在此，您将看到所有模型及其状态。

![图像1](/help/sky/assets/predictive-audiences/model-health-and-data-validity/model-health-and-data-validity-1.png)

* **培训状态**:指示您的模型是否在积极培训（改进预测）。 每两周自动进行一次培训。 任何 _处理_ 可能需要长达24小时才能完成。 对于任意 _失败_ 模型，请联系 [Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support).
* **评分状态**:指示您的模型是否正在主动计算程序成员的预测（可能性百分比）。
* **性能**：根据数据完整性和数据质量对模型运行状况进行分类（请参阅下文）。
* **数据完整性**:存在/完成的数据属性的百分比。
* **数据质量**:包含良好可用数据的属性的百分比。
