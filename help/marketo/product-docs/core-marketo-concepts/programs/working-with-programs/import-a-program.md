---
unique-page-id: 1147108
description: 导入程序 — Marketo文档 — 产品文档
title: 导入项目群
exl-id: 15e23e38-a24b-45b3-89a9-ffec85649f4a
feature: Programs
source-git-commit: 0adb780ea1622d12b8daafc502fd6a9151757ad3
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---

# 导入项目群 {#import-a-program}

程序可以从一个Marketo Engage订阅导入到另一个订阅。 例如，您可以在沙盒中创建程序，然后将其导入您的实时订阅。 此外，您还可以从[Marketo程序库](/help/marketo/product-docs/core-marketo-concepts/programs/program-library/program-import-library-overview.md){target="_blank"}导入预建程序。

>[!CAUTION]
>
>如果程序具有包含“自定义对象已更新”触发器的智能列表，将导致导入失败。 在执行以下列出的步骤之前，请从所有智能列表中删除此触发器。

## 导入项目群 {#importing-a-program}

1. 转到&#x200B;**[!UICONTROL 营销活动]**。

   ![](assets/import-a-program-1.png)

1. 单击&#x200B;**[!UICONTROL 新建]**&#x200B;下拉列表并选择&#x200B;**[!UICONTROL 导入程序]**。

   ![](assets/import-a-program-2.png)

   >[!NOTE]
   >
   >* “程序导入”仅适用于启用了导入程序权限的角色的用户。 了解有关[管理用户角色和权限的详细信息](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target="_blank"}。
   >
   >* 要将沙盒帐户连接到您的实时订阅，请联系[Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}。

1. 选择要导入的Marketo **[!UICONTROL 订阅]**&#x200B;和程序。 单击&#x200B;**[!UICONTROL 下一步]**。

   ![](assets/import-a-program-3.png)

1. 为导入的程序指定&#x200B;**[!UICONTROL Campaign文件夹]**。 单击&#x200B;**[!UICONTROL 下一步]**。

   ![](assets/import-a-program-4.png)

   >[!NOTE]
   >
   >确保选择&#x200B;**[!UICONTROL 使用默认冲突]**&#x200B;规则。 将项目导入具有相同名称的实例时，需要冲突规则。

1. 选择所需的冲突详细信息，然后单击&#x200B;**[!UICONTROL 下一步]**。

   ![](assets/import-a-program-5.png)

   >[!NOTE]
   >
   >将使用自定义流程步骤或从“流程步骤服务”派生的智能列表规则的程序导入到目标实例中，其中存在多个兼容服务提供程序，将提示导入用户将步骤或规则分配给目标实例中的正确服务提供程序。

1. 预览详细信息并&#x200B;**[!UICONTROL 导入]**&#x200B;程序。

   ![](assets/import-a-program-6.png)

导入完成后，您将收到一封电子邮件确认。

>[!NOTE]
>
>您需要重新计划导入的批量营销活动并激活触发器营销活动。 系统会自动停用营销活动计划，并触发导入项目中的营销活动。

## 程序导入期间对外部Assets的影响 {#impact-on-external-assets-during-program-imports}

项目使用外部资产，如电子邮件模板、登陆页面模板、图像、表单、令牌和项目标记。 您可以配置如何处理登陆页面模板和项目标记，而Marketo会自动管理其余的模板。

**电子邮件/登陆页面模板：**&#x200B;电子邮件/登陆页面模板已导入到Design Studio中。 您可以使用冲突规则配置同名模板存在时的行为。 使用默认规则时，如果存在具有相同名称的数字，则会向模板附加数字。 例如，如果您已经有一个名为“标准模板”的模板，则新模板将命名为“标准模板 — 1”。

**登陆页面/Forms：**&#x200B;如果Design Studio中存在同名的表单或登陆页面，则仍会导入这些表单或登陆页面，但会在其名称后附加一个数字（例如：登陆页面 — 1）。

**图像：**&#x200B;登陆页面使用的图像已导入到设计工作室中，除非存在具有相同名称的图像。

在导入过程中，**令牌：**&#x200B;位于项目之外的令牌将转换为本地令牌。

>[!CAUTION]
>
>程序导入不支持图像类型我的令牌。 如果导入了图像类型为我的令牌的程序，则将通过&#x200B;_no_&#x200B;令牌。

**程序标记：**&#x200B;您可以使用冲突规则来控制如何处理目标帐户中不存在的程序标记。 使用默认规则将创建程序标记，或者您可以选择忽略标记。

>[!CAUTION]
>
>导入项目时，将跳过包含[动态内容](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md){target="_blank"}的电子邮件/登陆页面。
