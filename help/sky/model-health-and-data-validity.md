---
title: 模型健康与数据有效性
description: 模型健康与数据有效性
exl-id: b14ec648-be1c-467b-b41d-2c53d74e25ea
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 0%

---

# 模型健康与数据有效性

<br> 

模型的性能取决于输入数据的质量和完整性。 下面介绍如何评估模型的健康。

导航到Marketo Classic **[!UICONTROL Admin]**&#x200B;区域&#x200B;**[!UICONTROL Predictive Audiences]**&#x200B;下的&#x200B;**[!UICONTROL Models and Data Health]**&#x200B;部分。 在此，您将看到所有模型及其状态。

![图像1](/help/sky/assets/predictive-audiences/model-health-and-data-validity/model-health-and-data-validity-1.png)

* **培训状态**:指示您的模型是否在积极培训（改进预测）。每两周自动进行一次培训。 任何&#x200B;_Processing_&#x200B;型号可能需要24小时才能完成。 对于任何&#x200B;_Failed_&#x200B;型号，请联系[Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support)。
* **评分状态**:指示您的模型是否在主动计算项目成员的预测（似然百分比）。
* **性能**：根据数据完整性和数据质量对模型运行状况进行分类（请参阅下文）。
* **数据完整性**:存在/完成的数据属性百分比。
* **数据质量**:包含良好可用数据的属性的百分比。
