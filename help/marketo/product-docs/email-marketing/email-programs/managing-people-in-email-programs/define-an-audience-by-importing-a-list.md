---
unique-page-id: 1900597
description: 通过导入列表定义受众 — Marketo文档 — 产品文档
title: 通过导入列表定义受众
exl-id: 9a63f4a5-1d76-4671-9622-19eb368d196f
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 1%

---

# 通过导入列表定义受众 {#define-an-audience-by-importing-a-list}

>[!PREREQUISITES]
>
>[为电子邮件程序创建电子邮件](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)

创建电子邮件程序后，您会希望告诉该程序要将电子邮件发送给谁。 您可以通过 [创建智能列表](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) 或通过导入列表。 下面介绍如何通过导入列表来完成此操作。

>[!NOTE]
>
>只有在电子邮件程序未获批准时，才能定义受众。
>
>正在导入的任何日期/时间字段都将被视为中央时间。 如果您的日期/时间字段位于不同的时区，则可以使用Excel公式将其转换为中部时间（美国/芝加哥）。

1. 转到 **营销活动**.

   ![](assets/login-marketing-activities-1.png)

1. 选择您的电子邮件程序，然后单击受众拼贴下的导入列表。

   ![](assets/importlist.png)

1. 将打开列表导入窗口，单击 **浏览** ，然后选择要导入的文件。 选择人员列表后，单击 **下一个**.

   ![](assets/importlist1.png)

   >[!CAUTION]
   >
   >确保列表已编码为UTF-8、UTF-16、Shift-JIS或EUC-JP，且文件大小不超过50MB。

1. 验证文件中的字段是否已正确映射，然后单击 **下一个**.

   ![](assets/image2014-9-12-11-3a10-3a7.png)

   >[!TIP]
   >
   >Marketo将记住将来导入的映射！

1. 输入 **名称** ，单击 **导入**.

   ![](assets/image2014-9-12-11-3a10-3a13.png)

1. 完成导入后，返回到主程序选项卡。 你会看到有多少人有资格。

   ![](assets/myemailprogram-1.jpg)

>[!NOTE]
>
>**条件**
>
>你注意到被阻止的号码了吗？ 此数字是符合条件的人员的子集，表示无法发送此电子邮件的人员，因为他们是：
>
>* 退订
>* 营销暂停
>* 列入阻止列表
>* 电子邮件无效
>* 空电子邮件
>
>单击号码可查看阻止发送邮件的详细人员列表。
>
>使用 ![—](assets/image2014-10-23-16-3a32-3a36-1.png) 按钮 **受众** 拼贴，以查看有多少人有资格根据智能列表条件接收电子邮件。 从人员数字中减去阻止的数字，以获取接收电子邮件的总人数。

>[!TIP]
>
>您无需等待列表导入完成。 你愿意的话可以继续工作。

太棒了！ 现在，该选择一封已有的电子邮件，或者创建一封新电子邮件发送给这些人员。

>[!MORELIKETHIS]
>
>* [选择现有电子邮件](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/choose-an-existing-email.md)
>* [为电子邮件程序创建电子邮件](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)

