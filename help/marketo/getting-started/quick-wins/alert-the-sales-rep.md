---
unique-page-id: 2359424
description: 提醒销售代表- Marketo Docs —— 产品文档
title: 提醒销售代表
translation-type: tm+mt
source-git-commit: 09dbd3a141fed0525aec8bf1ca6d141be2a6ce46
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 0%

---


# 提醒销售代表 {#alert-the-sales-rep}

## 任务：当某人填写您网站上的表单时，提醒销售代表 {#mission-alert-the-sales-rep-when-a-person-fills-out-a-form-on-your-web-site}

要自动向销售代表发送提醒电子邮件，您只需要一封提醒电子邮件和一封电子邮件活动。 下面介绍如何实现。

>[!NOTE]
>
>**FYI**
>
>Marketo现在正在所有订阅实现语言标准化，因此您可能会在订阅和docs.marketo.com中看到潜在客户／潜在客户。 这些术语的含义是相同的；它不影响文章说明。 还有一些其他变化。 [了解更多](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

>[!NOTE]
>
>**先决条件**
>
>* [登陆页表单](landing-page-with-a-form.md)

>



## 第1步：创建警报电子邮件 {#step-create-an-alert-email}

1. 转到“营销 **活动** ”区域。

   ![](assets/one-5.png)

1. 选 **择您** 在登陆页中用Form [quick win创建的My Asset](landing-page-with-a-form.md) ，然后在New（新建）下 **单** 击New **Local Asset**。

   ![](assets/two-6.png)

1. 单击“ **电子邮件**”。

   ![](assets/three-5.png)

1. **将电子邮件命** 名为“我的电子邮件警报”，选择一个模板，然后单击“ **创建**”。

   ![](assets/four-4.png)

1. 输入您 **希望销售团**&#x200B;队查看 **的“发件人名**&#x200B;称”、“ **发件人电子邮件”、“回复至**” **** 和“主题”。

   ![](assets/five-5.png)

1. 多次单击可编辑电子邮件文本。

   ![](assets/six-5.png)

1. 键入电子邮件内容。

   ![](assets/seven-6.png)

1. 将光标放在要插入人员联系信息的位置，然后单击“插入 **令牌** ”图标。

   ![](assets/eight-4.png)

1. 查找并选择令牌 `{{SP_Send_Alert_Info}}` , **然后** 单击 **插入**。

   ![](assets/image2014-9-24-13-3a10-3a0.png)

   >[!NOTE]
   >
   >{{SP_Send_Alert_Info}}是警报电子邮件的特殊令牌。 请参 [阅使用发送警报信息令牌](../../product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md) ，了解更多信息。

1. 单击 **保存**。

   ![](assets/ten-5.png)

1. 关闭电子邮件编辑器选项卡／窗口。

   ![](assets/eleven-5.png)

1. 在“电 **子邮件操作** ”下 **单击“批准**”。

   ![](assets/twelve-4.png)

## 第2步：创建警报触发器活动 {#step-create-an-alert-trigger-campaign}

1. 选择 **之前创建** 的“我的项目 **”，然后在“**新建”**下单击“**&#x200B;新建智能活动”。

   ![](assets/image2014-9-24-13-3a14-3a17.png)

1. **将活动** 命名为“我的警报活动”，然后单击“ **创建**”。

   ![](assets/image2014-9-24-13-3a14-3a28.png)

1. 在“智 **能列表** ”选项卡下，查找并 **将“填充表单”触发** 器拖动到画布上。

   ![](assets/image2014-9-24-13-3a14-3a43.png)

1. 选择我们之前创建的表单。

   ![](assets/image2014-9-24-13-3a14-3a58.png)

1. 在“ **流** ”选项卡下，查找并 **将“发送警报** ”流动操作拖至画布。

   ![](assets/image2014-9-24-13-3a15-3a10.png)

1. 选择 **之前创建的** “我的警报电子邮件”, **并保留“发送至****”作**&#x200B;为销售所有者。

   ![](assets/eighteen-1.png)

1. 在“收件人其他电子邮件”字 **段中键入您的电子邮件** 地址。

   ![](assets/nineteen-2.png)

1. 转到“ **计划** ”选项卡，单击“**激活**”按钮。

   ![](assets/twenty-2.png)

   >[!TIP]
   >
   >
   >将“资 **格规** 则 **”设置为** 每次(通过编辑智能活动)，以允许同一人多次触发警报。

1. 单击 **确认屏** 上的激活。

   ![](assets/twenty-one-1.png)

## 第3步：测试！ {#step-test-it-out}

1. 选择您的登陆页，然后单击 **视图批准页面**。

   ![](assets/image2014-9-24-13-3a17-3a8.png)

   >[!NOTE]
   >
   >**提醒**
   >
   >
   >别忘了批准登陆页;他们直到获得批准才上线。

1. 填写表单，然后单击“ **提交**”。

   ![](assets/image2014-9-24-13-3a17-3a41.png)

1. 您应该很快会收到您的电子邮件。 验证一切正常后，请从“发送警报”流中删除您的电子邮件地址（请参阅上面的步骤2.7）。

   >[!NOTE]
   >
   >单击Market **中的** “人员信息”选项卡以查看联系信息。

## 任务完成！ {#mission-complete}

<br> 

[◄任务7:个性化电子邮件](personalize-an-email.md)[任务9:更新潜在客户数据►](update-person-data.md)