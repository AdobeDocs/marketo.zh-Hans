---
unique-page-id: 1900597
description: 通过导入列表定义受众 — Marketo文档 — 产品文档
title: 通过导入列表定义受众
exl-id: 9a63f4a5-1d76-4671-9622-19eb368d196f
feature: Email Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 15%

---

# 通过导入列表定义受众 {#define-an-audience-by-importing-a-list}

>[!PREREQUISITES]
>
>[为电子邮件程序创建电子邮件](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)

创建电子邮件程序后，您将需要告诉它要将电子邮件发送到的收件人。 您可以通过[创建智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)或导入列表来执行此操作。 以下是如何通过导入列表来实现此目的。

>[!NOTE]
>
>仅当电子邮件程序未获批准时，定义受众才能正常工作。
>
>导入的所有日期/时间字段将视为中部时间（Central Time）。如果您的日期/时间字段为其他时区，可以使用 Excel 公式将其转换为中部时间（美国/芝加哥）。

1. 转到&#x200B;**[!UICONTROL Marketing Activities]**。

   ![](assets/login-marketing-activities-1.png)

1. 选择您的电子邮件程序，然后单击&#x200B;**[!UICONTROL Import List]**&#x200B;图块下的&#x200B;**[!UICONTROL Audience]**。

   ![](assets/importlist.png)

1. 列表导入窗口打开，单击&#x200B;**[!UICONTROL Browse]**&#x200B;并选择要导入的文件。 选择人员列表后，单击&#x200B;**[!UICONTROL Next]**。

   ![](assets/importlist1.png)

   >[!CAUTION]
   >
   >确保列表编码为UTF-8、UTF-16、Shift-JIS或EUC-JP，并且文件大小不超过50MB。

1. 验证文件中的字段是否已正确映射，然后单击&#x200B;**[!UICONTROL Next]**。

   ![](assets/image2014-9-12-11-3a10-3a7.png)

   >[!TIP]
   >
   >Marketo将记住映射以供将来导入！

1. 为您的列表输入&#x200B;**[!UICONTROL Name]**&#x200B;并单击&#x200B;**[!UICONTROL Import]**。

   ![](assets/image2014-9-12-11-3a10-3a13.png)

1. 导入完成后，返回主项目选项卡。 你将看到有多少人有资格参加比赛。

   ![](assets/myemailprogram-1.jpg)

>[!NOTE]
>
>**定义**
>
>你注意到被阻止的号码了吗？ 此数字是合格人员的子集，表示由于以下原因无法发送此电子邮件的人员：
>
>* 已取消订阅
>* 营销暂停
>* 已列入阻止列表
>* 电子邮件无效
>* 空电子邮件
>
>单击此号码可获取阻止发送邮件的人员的详细列表。
>
>使用![磁贴上的](assets/image2014-10-23-16-3a32-3a36-1.png)—**[!UICONTROL Audience]**&#x200B;按钮查看有多少人有资格根据智能列表条件接收电子邮件。 从人员编号中减去阻止的编号，即可获得接收电子邮件的总人数。

>[!TIP]
>
>您不必等待列表导入完成。 如果你愿意，你可以继续工作。

太棒了！ 现在该选择现有电子邮件或创建新电子邮件以发送给这些人员了。

>[!MORELIKETHIS]
>
>* [选择现有电子邮件](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/choose-an-existing-email.md)
>* [为电子邮件程序创建电子邮件](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)
