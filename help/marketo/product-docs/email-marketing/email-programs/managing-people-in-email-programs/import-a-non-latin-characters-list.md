---
unique-page-id: 5472678
description: 导入非拉丁文字符列表 — Marketo文档 — 产品文档
title: 导入非拉丁文字符列表
exl-id: 11519e2c-ab01-4164-8ce3-0717e4c13ae6
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 0%

---

# 导入非拉丁文字符列表 {#import-a-non-latin-characters-list}

正在尝试导入非英文的文件？ 当您用Excel打开列表时，它看起来完美无缺。

![](assets/image2015-2-10-9-3a34-3a57.png)

但是，将其导入Marketo时，您可能会发现未正确提取非英语字符。

![](assets/image2015-2-10-9-3a35-3a49.png)

这是因为文件未正确保存，以便Marketo识别所有非拉丁字符。 好消息是，您可以按照一些简单的步骤来修复此问题。

1. 从Excel的&#x200B;**文件**&#x200B;菜单中选择&#x200B;**另存为……**。

   ![](assets/image2015-2-10-9-3a46-3a44.png)

1. 选择&#x200B;**UTF-16 Unicode文本(.txt)**&#x200B;作为&#x200B;**格式**&#x200B;选项。 这将以Marketo显示文件的方式对文件进行编码。

   ![](assets/image2015-2-10-9-3a48-3a7.png)

   >[!NOTE]
   >
   >Marketo还支持UTF-8、Shift-JIS或EUC-JP。

1. Excel会将新文件另存为扩展名为.txt的文本文件。 但它也会将文件中的所有逗号转换为制表符。 我们得把它改回来。

   >[!TIP]
   >
   >如果您使用Windows，可以使用&#x200B;**记事本**&#x200B;打开文本文件；如果您使用Mac，则可以使用&#x200B;**TextEdit**&#x200B;打开文本文件。

   ![](assets/image2015-2-10-9-3a51-3a41.png)

1. 从文档中选择一个选项卡并复制它。

   ![](assets/image2015-2-10-9-3a55-3a53.png)

1. 从&#x200B;**编辑**&#x200B;菜单中选择&#x200B;**查找和替换……**。

   ![](assets/image2015-2-10-9-3a59-3a8.png)

   >[!TIP]
   >
   >Windows用户的等效操作为： **编辑>替换……**

1. 将您在步骤4中复制的选项卡粘贴到第一个（要替换的）框中，并在第二个（替换为）框中键入逗号。 单击&#x200B;**全部**。

   ![](assets/image2015-2-10-10-3a8-3a53.png)

1. 好了，所有逗号都恢复了，我们准备好了。

   ![](assets/image2015-2-10-10-3a14-3a45.png)

1. 将新文件导入Marketo，此时信息应会正确显示。

   ![](assets/image2015-2-10-10-3a16-3a9.png)

   >[!NOTE]
   >
   >正在导入的任何日期/时间字段都将被视为中部时间。 如果您的日期/时间字段位于不同的时区，则可以使用Excel公式将其转换为中部时间（美洲/芝加哥）。

我们知道这很奇怪，但它管用。 祝您进口顺利！
