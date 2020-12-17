---
unique-page-id: 2359424
description: 提醒销售代表- Marketo Docs —— 产品文档
title: 提醒销售代表
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---


# 提醒销售代表{#alert-the-sales-rep}

## 任务：当某人填写您网站上的表单{#mission-alert-the-sales-rep-when-a-person-fills-out-a-form-on-your-web-site}时，提醒销售代表

要自动向销售代表发送提醒电子邮件，您只需要一封提醒电子邮件和一封电子邮件活动。 下面介绍如何实现。

>[!PREREQUISITES]
>
>[登陆页表单](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)

## 第1步：创建警报电子邮件{#step-create-an-alert-email}

1. 转至&#x200B;**营销活动**&#x200B;区域。

   ![](assets/one-5.png)

1. 选择您在[项目中以Form](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)快速赢取创建的&#x200B;**我的登陆页**，然后在&#x200B;**新建**&#x200B;下单击&#x200B;**新建本地资产**。

   ![](assets/two-6.png)

1. 单击&#x200B;**电子邮件**。

   ![](assets/three-5.png)

1. **将电** 子邮件命名为“我的电子邮件警报”，选择一个模板，然后单击 **创建**。

   ![](assets/four-4.png)

1. 输入您希望销售团队看到的&#x200B;**From Name**、**From Email**、**Reply-to**&#x200B;和&#x200B;**Subject**。

   ![](assets/five-5.png)

1. 多次单击可编辑电子邮件文本。

   ![](assets/six-5.png)

1. 键入电子邮件内容。

   ![](assets/seven-6.png)

1. 将光标放在要插入人员联系信息的位置，然后单击&#x200B;**插入令牌**&#x200B;图标。

   ![](assets/eight-4.png)

1. 查找并选择`{{SP_Send_Alert_Info}}` **令牌**，然后单击&#x200B;**插入**。

   ![](assets/image2014-9-24-13-3a10-3a0.png)

   >[!NOTE]
   >
   >{{SP_Send_Alert_Info}}是警报电子邮件的特殊令牌。 请参阅[使用发送警报信息令牌](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md)了解更多信息。

1. 单击&#x200B;**保存**。

   ![](assets/ten-5.png)

1. 关闭电子邮件编辑器选项卡／窗口。

   ![](assets/eleven-5.png)

1. 在&#x200B;**电子邮件操作**&#x200B;下，单击&#x200B;**批准**。

   ![](assets/twelve-4.png)

## 第2步：创建警报触发器活动{#step-create-an-alert-trigger-campaign}

1. 选择“以前创建的&#x200B;**我的项目**”，然后在“新建”下单击“新建智能活动&#x200B;**”。******

   ![](assets/image2014-9-24-13-3a14-3a17.png)

1. **将活动** 命名为“我的警报活动”，然后单击“ **创建”**。

   ![](assets/image2014-9-24-13-3a14-3a28.png)

1. 在&#x200B;**智能列表**&#x200B;选项卡下，找到并将&#x200B;**填充表单**&#x200B;触发器拖动到画布。

   ![](assets/image2014-9-24-13-3a14-3a43.png)

1. 选择我们之前创建的表单。

   ![](assets/image2014-9-24-13-3a14-3a58.png)

1. 在&#x200B;**Flow**&#x200B;选项卡下，找到并将&#x200B;**发送警报**&#x200B;流动操作拖动到画布。

   ![](assets/image2014-9-24-13-3a15-3a10.png)

1. 选择之前创建的&#x200B;**我的警报电子邮件**，将&#x200B;**发送到**&#x200B;保留为&#x200B;**销售所有者**。

   ![](assets/eighteen-1.png)

1. 在&#x200B;**收件人其他电子邮件**&#x200B;字段中键入您的电子邮件地址。

   ![](assets/nineteen-2.png)

1. 转到&#x200B;**计划**&#x200B;选项卡并单击&#x200B;**激活**&#x200B;按钮。

   ![](assets/twenty-2.png)

   >[!TIP]
   >
   >每次&#x200B;**(通过编辑智能活动)将**&#x200B;资格规则&#x200B;**设置为**（通过编辑智能），允许同一人多次触发警报。

1. 单击确认屏幕上的&#x200B;**激活**。

   ![](assets/twenty-one-1.png)

## 第3步：测试！{#step-test-it-out}

1. 选择您的登陆页并单击&#x200B;**视图批准页面**。

   ![](assets/image2014-9-24-13-3a17-3a8.png)

   >[!NOTE]
   >
   >别忘了批准登陆页;他们直到获得批准才上线。

1. 填写表单，然后单击&#x200B;**提交**。

   ![](assets/image2014-9-24-13-3a17-3a41.png)

1. 您应该很快会收到您的电子邮件。 验证一切正常后，请从“发送警报”流中删除您的电子邮件地址（请参阅上面的步骤2.7）。

   >[!NOTE]
   >
   >单击Market中的&#x200B;**人员信息**&#x200B;选项卡以查看联系信息。

## 任务完成！{#mission-complete}

<br> 

[◄任务7:个性化电子邮件](personalize-an-email.md)

[任务9:更新潜在客户数据►](update-person-data.md)
