---
unique-page-id: 1147108
description: 导入程序 — Marketo文档 — 产品文档
title: 导入项目群
exl-id: 15e23e38-a24b-45b3-89a9-ffec85649f4a
feature: Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 0%

---

# 导入项目群 {#import-a-program}

程序可以从一个Marketo订阅导入到另一个订阅。 例如，您可以在沙盒中创建程序，然后将其导入您的实时订阅。 此外，您还可以从Marketo程序库导入预建程序。

## 导入项目群 {#importing-a-program}

1. 转到 **营销活动。**

   ![](assets/import-a-program-1.png)

1. 单击 **新** 下拉菜单。 选择 **导入程序**.

   ![](assets/import-a-program-2.png)

   >[!NOTE]
   >
   >程序导入仅适用于启用了导入程序权限角色的用户。 详细了解 [管理用户角色和权限](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md).
   >
   >要将沙盒帐户连接到您的实时订阅，请联系 [Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support).

1. 选择Marketo **订阅** 以及要导入的程序。 单击 **下一个**.

   ![](assets/import-a-program-3.png)

1. 指定 **Campaign文件夹** 对于导入的程序。 单击 **下一个。**

   ![](assets/import-a-program-4.png)

   >[!NOTE]
   >
   >确保 **使用默认冲突** 已选择规则。 将程序导入具有相同名称的资产实例时，需要冲突规则。

1. 选择所需的冲突详细信息，然后单击 **下一个**.

   ![](assets/import-a-program-5.png)

   >[!NOTE]
   >
   >将使用自定义流程步骤或从“流程步骤服务”派生的“智能列表”规则的程序导入到目标实例中，其中存在多个兼容的服务提供程序，系统将提示导入用户将步骤或规则分配给目标实例中的正确服务提供程序。

1. 预览详细信息和 **导入** 程序。

   ![](assets/import-a-program-6.png)

导入完成后，您将收到一封电子邮件确认函。

>[!NOTE]
>
>您需要重新计划导入的批量营销活动并激活触发器营销活动。 系统会自动停用营销活动计划，并触发导入项目中的营销活动。

## 程序导入期间对外部资产的影响 {#impact-on-external-assets-during-program-imports}

项目使用外部资产，如电子邮件模板、登陆页面模板、图像、表单、令牌和项目标记。 您可以配置如何处理登陆页面模板和项目标记，而Marketo会自动管理其余的模板和项目标记。

**电子邮件/登陆页面模板：** 电子邮件/登陆页面模板将导入到Design Studio中。 您可以使用冲突规则来配置存在同名模板时的行为。 使用默认规则时，如果存在同名模板，则会将一个数字附加到模板中。 例如，如果您已经有一个名为“标准模板”的模板，则新模板将名为“标准模板 — 1”。

**登陆页面/Forms：** 如果Design Studio中存在同名的表单或登陆页面，则仍会导入这些表单或登陆页面，但会在其名称后附加一个数字（例如：登陆页面 — 1）。

**图像：** 登陆页面使用的图像会导入到设计工作室中，除非存在具有相同名称的图像。

**令牌：** 在导入过程中，位于项目之外的令牌将会转换为本地令牌。

>[!CAUTION]
>
>程序导入不支持图像类型我的令牌。 如果导入了图像类型为我的令牌的程序， **否** 令牌将通过。

**项目标记：** 您可以使用冲突规则来控制如何处理目标帐户中不存在的程序标记。 使用默认规则将创建程序标记，或者您可以选择忽略标记。

>[!CAUTION]
>
>导入项目时，包含以下内容的电子邮件/登陆页面 [动态内容](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md) 将被跳过。
