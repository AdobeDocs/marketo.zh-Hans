---
unique-page-id: 2359646
description: 配置表单渐进式分析 — Marketo文档 — 产品文档
title: 配置表单渐进式分析
exl-id: 72afe3dc-0688-45ec-ab70-4dc9accf4fc8
feature: Forms
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---

# 配置表单渐进式分析 {#configure-form-progressive-profiling}

简短表格很好！ 当某人返回表单时，您可以显示新字段并逐步填写访客资料。 具体方法如下。

>[!NOTE]
>
>要使此功能正常工作，请确保对可见字段启用表单预填充，对隐藏字段启用[禁用](/help/marketo/product-docs/demand-generation/forms/form-fields/disable-pre-fill-for-a-form-field.md)。

1. 转到&#x200B;**营销活动**。

   ![](assets/ma-1.png)

1. 选择您的表单并单击&#x200B;**编辑表单**。

   ![](assets/image2014-9-15-12-3a31-3a20.png)

1. 在&#x200B;**表单设置**&#x200B;下，单击&#x200B;**设置**。

   ![](assets/image2014-9-15-12-3a31-3a29.png)

1. 将&#x200B;**Progressive Profiling**&#x200B;设置为&#x200B;**Enabled**。

   ![](assets/image2014-9-15-12-3a31-3a47.png)

1. 好，现在让我们配置它。 转到&#x200B;**字段详细信息**。

   ![](assets/image2014-9-15-12-3a31-3a55.png)

1. 拖放渐进式配置文件集中的所有字段。

   ![](assets/image2014-9-15-12-3a32-3a3.png)

1. 移动完所有字段后，它应该如下所示：

   ![](assets/image2014-9-15-12-3a32-3a12.png)

   >[!NOTE]
   >
   >**Progressive Profiling**&#x200B;框之外的字段将始终显示在表单中，即使已填写也是如此。

1. 选择&#x200B;**Progressive Profiling**&#x200B;框。

   ![](assets/image2014-9-15-12-3a32-3a19.png)

   >[!CAUTION]
   >
   >在Progressive Profiling中使用必填字段时要小心。 如果访客在之前提交其他字段的数据后输入新的电子邮件地址（这将创建新人员），这些字段仍可留空，因为它们将在最新表单上被禁止。

1. 现在，选择您希望用户在任何给定时间从&#x200B;**Progressive Profiling**&#x200B;框中查看多少空白字段。

   ![](assets/image2014-9-15-12-3a32-3a26.png)

   >[!NOTE]
   >
   >如果您选择&#x200B;**数字** **/** **空白** **字段**&#x200B;作为1，则访客第一次看到此表单时将看到以下内容：
   >
   >* 名字（空）
   >* 姓氏（空）
   >* 电子邮件地址（空）
   >* 电话号码（空）
   >
   >如果他们填写了每个字段，那么在第二次访问时，将会看到：
   >
   >* 名字（预填）
   >* 姓氏（预填）
   >* 电子邮件地址（预填）
   >* 手机号码（空）
   >
   >假设他们填写了手机号码，那么他们第三次访问时将会看到：
   >
   >* 名字（预填）
   >* 姓氏（预填）
   >* 电子邮件地址（预填）
   >* 国家/地区（空）

1. 单击&#x200B;**完成**。

   ![](assets/image2014-9-15-12-3a33-3a35.png)

1. 单击&#x200B;**批准并关闭**。

   ![](assets/image2014-9-15-12-3a33-3a45.png)

做得好！ 你刚才做的工作会有所收获。

尝试使用此功能并确保进行测试。 它非常先进，但你可以用这种方式让表单变得非常动态。
