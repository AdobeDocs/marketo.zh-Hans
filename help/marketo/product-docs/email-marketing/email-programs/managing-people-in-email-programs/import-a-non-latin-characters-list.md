---
unique-page-id: 5472678
description: 导入非拉丁文字符列表 — Marketo文档 — 产品文档
title: 导入非拉丁字符列表
exl-id: 11519e2c-ab01-4164-8ce3-0717e4c13ae6
feature: Email Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 15%

---

# 导入非拉丁字符列表 {#import-a-non-latin-characters-list}

正在尝试导入非英文的文件？ 当您用Excel打开列表时，它看起来完美无缺。

![](assets/image2015-2-10-9-3a34-3a57.png)

但是，将其导入Marketo时，您可能会发现未正确提取非英语字符。

![](assets/image2015-2-10-9-3a35-3a49.png)

这是因为文件未正确保存，以便Marketo识别所有非拉丁字符。 好消息是，您可以按照一些简单的步骤来修复此问题。

1. 从Excel的&#x200B;**[!UICONTROL Save As]菜单中选择**...**[!UICONTROL File]**。

   ![](assets/image2015-2-10-9-3a46-3a44.png)

1. 选择&#x200B;**[!UICONTROL UTF-16 Unicode Text (.txt)]**&#x200B;作为&#x200B;**[!UICONTROL Format]**&#x200B;选项。 这将以Marketo显示文件的方式对文件进行编码。

   ![](assets/image2015-2-10-9-3a48-3a7.png)

   >[!NOTE]
   >
   >Marketo还支持UTF-8、Shift-JIS或EUC-JP。

1. Excel会将新文件另存为扩展名为.txt的文本文件。 但它也会将文件中的所有逗号转换为制表符。 我们得把它改回来。

   >[!TIP]
   >
   >如果您使用Windows，可以使用&#x200B;**[!DNL Notepad]**&#x200B;打开文本文件；如果您使用Mac，可以使用&#x200B;**[!DNL TextEdit]**&#x200B;打开文本文件。

   ![](assets/image2015-2-10-9-3a51-3a41.png)

1. 从文档中选择一个选项卡并复制它。

   ![](assets/image2015-2-10-9-3a55-3a53.png)

1. 从&#x200B;**[!UICONTROL Find and Replace]菜单中选择**...**[!UICONTROL Edit]**。

   ![](assets/image2015-2-10-9-3a59-3a8.png)

   >[!TIP]
   >
   >Windows用户的等效操作为： **[!UICONTROL Edit]> [!UICONTROL Replace]...**

1. 将您在步骤4中复制的选项卡粘贴到第一个（要替换的）框中，并在第二个（替换为）框中键入逗号。 然后单击&#x200B;**[!UICONTROL All]**。

   ![](assets/image2015-2-10-10-3a8-3a53.png)

1. 好了，所有逗号都恢复了，我们准备好了。

   ![](assets/image2015-2-10-10-3a14-3a45.png)

1. 将新文件导入Marketo，此时信息应会正确显示。

   ![](assets/image2015-2-10-10-3a16-3a9.png)

   >[!NOTE]
   >
   >导入的所有日期/时间字段将视为中部时间（Central Time）。如果您的日期/时间字段为其他时区，可以使用 Excel 公式将其转换为中部时间（美国/芝加哥）。

我们知道这很奇怪，但它管用。 祝您进口顺利！
