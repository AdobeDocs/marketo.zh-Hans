---
unique-page-id: 1900597
description: 通过导入受众- Marketo Docs —— 产品文档定义列表
title: 通过导入受众定义列表
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---


# 通过导入受众{#define-an-audience-by-importing-a-list}定义列表

>[!PREREQUISITES]
>
>[创建电子邮件项目](../../../../product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)

创建电子邮件项目后，您会希望告诉它要将电子邮件发送给谁。 可通过[创建智能列表](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)或导入列表来执行此操作。 下面介绍如何通过导入列表来完成此操作。

>[!NOTE]
>
>只有在未批准电子邮件受众时，才能定义项目。
>
>导入的任何日期／时间字段均视为中央时间。 如果日期／时间字段位于其他时区，则可使用Excel公式将其转换为中时（美国／芝加哥）。

1. 转到&#x200B;**营销活动**。

   ![](assets/login-marketing-activities-1.png)

   选择您的电子邮件项目，然后单击受众拼贴下的“导入列表”。
   ![](assets/importlist.png)

1. 列表导入窗口将打开，单击&#x200B;**浏览**&#x200B;并选择要导入的文件。 选择人员列表后，单击“下一步”。
1. ![](assets/importlist1.png)

   >[!CAUTION]
   >
   >确保列表是以UTF-8、UTF-16、Shift-JIS或EUC-JP编码，且文件大小不超过50MB。

   验证文件中的字段映射是否正确，然后单击“下一步”。
   ![](assets/image2014-9-12-11-3a10-3a7.png)

   >[!TIP]
   >
   >Marketo将记住将来导入的映射！

1. 为您的列表输入&#x200B;**名称**&#x200B;并单击&#x200B;**导入**。

   ![](assets/image2014-9-12-11-3a10-3a13.png)

1. 完成导入后，返回主项目选项卡。 你会看到有多少人有资格。

   ![](assets/myemailprogram-1.jpg)

>[!NOTE]
>
>**定义**
>
>你注意到被阻止的号码了吗？ 此数字是合格人员的子集，表示无法发送此电子邮件的人员，因为他们：
>
>* 取消订阅
>* 营销已暂停
>* 列入阻止列表
>* 电子邮件无效
>* 空电子邮件

>
>
单击号码，详细列表邮件中阻止的人员。
>
>使用&#x200B;**受众**&#x200B;拼贴上的![—](assets/image2014-10-23-16-3a32-3a36-1.png)按钮，查看有多少人有资格根据智能列表条件接收电子邮件。 从“人员”号中减去“被阻止”号以获得接收电子邮件的总人数。

>[!TIP]
>
>您不必等待列表导入完成。 如果你愿意，你可以继续工作。

太棒了！ 现在，是时候选择已有的电子邮件或创建新电子邮件发送给这些人了。

>[!MORELIKETHIS]
>
>* [选择现有电子邮件](../../../../product-docs/email-marketing/email-programs/email-program-actions/choose-an-existing-email.md)
>* [创建电子邮件项目](../../../../product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)

>



