---
solution: Marketo Engage
product: marketo
title: 使用高级HTML编辑器编辑电子邮件模板
description: 了解如何在Marketo Engage Email Designer中查看和编辑原始HTML源代码，包括护栏、访问步骤和关键限制。
level: Intermediate
feature: Email Designer
exl-id: b030e56a-de70-4b0d-9788-04a01235cffb
source-git-commit: 2b638c3945d6b28379655596d2c5c878d842e60e
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# 使用高级HTML编辑器编辑电子邮件模板 {#advanced-html-mode}

高级HTML模式允许您直接从[!DNL Marketo Engage]电子邮件Designer界面查看和编辑电子邮件模板的原始源代码。

此功能允许您直接在源中插入高级表达式。 切换回可视化（桌面）视图后，内容将重新呈现，这样您就可以检查内容的外观，并在任一视图中继续编辑。

## 护栏 {#guardrails}

使用高级HTML编辑器时，以下护栏可保护内容兼容性并设置预期。

* 高级HTML编辑器&#x200B;**不验证**&#x200B;您的代码。 它不会检查语法错误或布局中断。 在保存之前仔细查看您的内容。

* 将来的系统更新可能会覆盖您对默认标记所做的更改。 **您的更改可能不会保留**。

* [!DNL Adobe]支持&#x200B;**无法排除或解决由自定义代码和手动更改导致的**&#x200B;问题。 保留内容的备份，以防您需要还原。

* 您无法在高级HTML视图中模拟内容。 切换到桌面视图以预览您的内容。

* 为确保内容兼容性，**您不能在高级HTML视图中保存**。 准备好保存更改后，切换回“桌面”视图。

## 访问高级HTML模式 {#access-html-mode}

要打开高级HTML编辑器并编辑模板源，请执行以下步骤。

1. 在电子邮件Designer中打开或[创建电子邮件模板](/help/marketo/product-docs/email-marketing/email-designer/email-template-authoring.md#create-an-email-template)。

1. 在&#x200B;_编辑电子邮件模板_&#x200B;屏幕中，单击右上角的HTML按钮。

   ![](assets/advanced-html-mode-1.png){width="800" zoomable="yes"}

1. 首次打开高级HTML编辑器时，会显示一条警告消息。 完成时单击&#x200B;**[!UICONTROL OK]**&#x200B;进行审核。

   ![](assets/advanced-html-mode-2.png)

   >[!NOTE]
   >
   >首次打开高级HTML编辑器时会出现此警告，并且会在每月重置。

1. 此时将显示高级HTML编辑器。

   ![](assets/advanced-html-mode-3.png){width="800" zoomable="yes"}

1. 将所需的更改添加到您的电子邮件内容中。

   >[!WARNING]
   >
   >确保输入正确的HTML和CSS代码，因为没有语法验证过程，并且Adobe支持无法协助进行HTML编辑。

1. 出于兼容性原因，内容模拟和保存在高级HTML视图中不可用。 切换回“桌面”视图以预览内容并保存更改。

   ![](assets/advanced-html-mode-4.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >切换视图时，将保留所做的编辑。
