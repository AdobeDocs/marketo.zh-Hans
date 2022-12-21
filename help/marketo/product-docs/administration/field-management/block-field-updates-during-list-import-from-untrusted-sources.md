---
unique-page-id: 2360335
description: 从不受信任的源导入列表期间块字段更新 — Marketo文档 — 产品文档
title: 从不受信任的源导入列表期间块字段更新
exl-id: 0fd59f0c-6cb9-442c-937b-da18a4466873
source-git-commit: 2776969be44ba1a3d795e99986d10cf0470fb9e9
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---

# 从不受信任的源导入列表期间块字段更新 {#block-field-updates-during-list-import-from-untrusted-sources}

您可以比其他列表更信任某些列表中的数据。 有时，您拥有可疑数据，如果字段为空，但如果存在现有值，则希望获取该数据。 您可以通过阻止关键字段上的字段更新来实现此目的。

>[!NOTE]
>
>**需要管理员权限**

## 阻止来自不受信任的源的字段更新 {#blocking-field-updates-from-untrusted-sources}

1. 转到 **管理员** 的上界。

   ![](assets/blocking-field-updates-from-untrusted-sources-1.png)

1. 单击 **字段管理**.

   ![](assets/blocking-field-updates-from-untrusted-sources-2.png)

1. 找到所需的字段，将其选中，然后在 **字段操作**，单击 **块字段更新**.

   ![](assets/blocking-field-updates-from-untrusted-sources-3.png)

1. 检查 **列表导入不受信任的源** 单击 **应用**.

   ![](assets/blocking-field-updates-from-untrusted-sources-4.png)

>[!TIP]
>
>通过检查 **列表导入受信任源**.

对要避免受不信任列表影响的任何其他字段重复上述步骤。

## 运行不受信任的列表导入 {#running-an-untrusted-list-import}

1. 运行列表导入时，请务必选择 **不受信任** 如果您希望上一步中设置的所有字段都安全。

   ![](assets/blocking-field-updates-from-untrusted-sources-5.png)

有关导入列表的详细说明，请参阅 [导入人员列表](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md).

干得好！ 现在，您可以了解如何避免密钥字段受到不受信任的列表的影响。
