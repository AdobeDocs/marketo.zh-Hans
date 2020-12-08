---
unique-page-id: 5472678
description: 导入非拉丁字符列表- Marketo Docs —— 产品文档
title: 导入非拉丁字符列表
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---


# 导入非拉丁字符列表 {#import-a-non-latin-characters-list}

尝试导入不是英语的文件？ 当您用Excel打开列表时，它看上去很完美。

![](assets/image2015-2-10-9-3a34-3a57.png)

但是，将其导入Marketo时，您可能会发现非英语字符的拾取不正确。

![](assets/image2015-2-10-9-3a35-3a49.png)

这是因为Market无法正确保存文件以识别所有非拉丁字符。 好消息是，您可以遵循一些简单的步骤来修复它。

1. 从 **Excel的“文件** ”菜 **单中选** 择“另存为……”。

   ![](assets/image2015-2-10-9-3a46-3a44.png)

1. 选 **择UTF-16 Unicode文本(.txt)作为** “格式 **”选项** 。 这将按照Marketo显示文件的方式对文件进行编码。

   ![](assets/image2015-2-10-9-3a48-3a7.png)

   >[!NOTE]
   >
   >Marketo还支持UTF-8、Shift-JIS或EUC-JP。

1. Excel将新文件另存为扩展名为。txt的文本文件。 但它也会将文件中的所有逗号转换为选项卡。 我们得把它改回来。

   >[!TIP]
   >
   >如果您使用Windows，则可 **以使** 用记事本打开文 **本文件** ，如果您使用Mac，则可以使用TextEdit打开文本文件。

   ![](assets/image2015-2-10-9-3a51-3a41.png)

1. 从文档中选择一个选项卡并复制它。

   ![](assets/image2015-2-10-9-3a55-3a53.png)

1. 从“ **编辑”菜单中选择“查找并替换** ... **”** 。

   ![](assets/image2015-2-10-9-3a59-3a8.png)

   >[!TIP]
   >
   >对于Windows用户，等效的操作是： **“编辑”>“替换……”**

1. 将您在步骤4中复制的选项卡粘贴到第一个（要替换）框中，然后在第二个（替换为）框中键入逗号。 然后单击“ **全部**”。

   ![](assets/image2015-2-10-10-3a8-3a53.png)

1. 看，所有逗号都回来了，我们准备开始了。

   ![](assets/image2015-2-10-10-3a14-3a45.png)

1. 将新文件导入Marketo，此时应正确显示信息。

   ![](assets/image2015-2-10-10-3a16-3a9.png)

   >[!NOTE]
   >
   >导入的任何日期／时间字段均视为中央时间。 如果日期／时间字段位于其他时区，则可使用Excel公式将其转换为中时（美国／芝加哥）。

我们知道这很奇怪，但是很管用。 导入快乐！