---
unique-page-id: 2360335
description: 列表从不受信任的源导入过程中块字段更新- Marketo文档——产品文档
title: 从不受信任的源导入列表期间块字段更新
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---


# 从不受信任的源{#block-field-updates-during-list-import-from-untrusted-sources}导入列表期间块字段更新

您可以比其他列表更信任某些数据。 有时，您有可疑数据，如果字段为空，但如果存在现有值，则希望获取该数据。 您可以通过阻止关键字段的字段更新来完成此操作。

>[!NOTE]
>
>**需要管理员权限**

## 阻止来自不受信任的源的字段更新{#blocking-field-updates-from-untrusted-sources}

1. 转至&#x200B;**Admin**&#x200B;并单击&#x200B;**字段管理**。

   ![](assets/image2014-9-19-9-3a38-3a38.png)

1. 找到所需字段，选择它，然后在&#x200B;**字段操作**&#x200B;下，单击&#x200B;**块字段更新**。

   ![](assets/image2014-9-19-9-3a39-3a40.png)

1. 选中&#x200B;**列表导入不受信任的源**&#x200B;并单击&#x200B;**应用**。

   ![](assets/blockupdates.png)

>[!TIP]
>
>通过同时检查&#x200B;**列表导入信任源**，可以保证字段免受所有列表的信任和不信任。

对于要避免不受信任的列表的任何其他字段，请重复上述步骤。

## 运行不受信任的列表导入{#running-an-untrusted-list-import}

1. 运行列表导入时，如果希望在上一步中设置的所有字段都安全，请务必选择**不受信任**。

   ![](assets/importpersondetails.jpg)

有关导入列表的详细说明，请参阅[导入People](../../../getting-started/quick-wins/import-a-list-of-people.md)的列表。

干得好！ 现在您知道如何保护密钥字段免受不可信列表的侵害。
