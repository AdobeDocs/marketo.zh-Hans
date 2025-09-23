---
unique-page-id: 2359424
description: 提醒销售代表 — Marketo文档 — 产品文档
title: 通知销售代表
exl-id: 4ad7d7b8-ee1e-4605-b4e0-e72a7e573c05
feature: Getting Started
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 8%

---

# 通知销售代表 {#alert-the-sales-rep}

## 任务：当某人填写您网站上的表单时提醒销售代表 {#mission-alert-the-sales-rep-when-a-person-fills-out-a-form-on-your-web-site}

要自动向销售代表发送警报电子邮件，您只需要一封警报电子邮件和一封电子邮件促销活动。 下面是操作方法。

>[!PREREQUISITES]
>
>[带有表单的登陆页面](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}

## 步骤1：创建警报电子邮件 {#step-create-an-alert-email}

1. 进入 **[!UICONTROL Marketing Activities]** 区域。

   ![](assets/alert-the-sales-rep-1.png)

1. 选择您在&#x200B;**登录页中使用表单**&#x200B;快速入选创建的[我的项目](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}，然后在&#x200B;**[!UICONTROL New]**&#x200B;下单击&#x200B;**[!UICONTROL New Local Asset]**。

   ![](assets/alert-the-sales-rep-2.png)

1. 单击 **[!UICONTROL Email]**。

   ![](assets/alert-the-sales-rep-3.png)

1. **将电子邮件命名为“我的电子邮件警报”**，选择一个模板并单击&#x200B;**[!UICONTROL Create]**。

   ![](assets/alert-the-sales-rep-4.png)

1. 输入您希望销售团队查看的&#x200B;**发件人姓名**、**发件人电子邮件**、**[!UICONTROL Reply-to]**&#x200B;和&#x200B;**[!UICONTROL Subject]**。

   ![](assets/alert-the-sales-rep-5.png)

1. 双击以编辑电子邮件文本。

   ![](assets/alert-the-sales-rep-6.png)

1. 键入电子邮件内容。

   ![](assets/alert-the-sales-rep-7.png)

1. 将光标放在要插入人员联系信息的位置，然后单击&#x200B;**插入令牌**&#x200B;图标。

   ![](assets/alert-the-sales-rep-8.png)

1. 查找并选择`{{SP_Send_Alert_Info}}` **[!UICONTROL Token]**&#x200B;并单击&#x200B;**[!UICONTROL Insert]**。

   ![](assets/alert-the-sales-rep-9.png)

   >[!NOTE]
   >
   >{{SP_Send_Alert_Info}}是警报电子邮件的特殊令牌。 请参阅[使用发送警报信息令牌](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target="_blank"}{target="_blank"}了解更多信息。

1. 单击 **[!UICONTROL Save]**。

   ![](assets/alert-the-sales-rep-10.png)

1. 点击 **[!UICONTROL Email Actions]** 下拉菜单，并选择 **[!UICONTROL Approve and Close]**。

   ![](assets/alert-the-sales-rep-11.png)

## 步骤2：创建警报触发器营销活动 {#step-create-an-alert-trigger-campaign}

1. 选择之前创建的&#x200B;**我的程序**，然后在&#x200B;**[!UICONTROL New]**&#x200B;下单击&#x200B;**[!UICONTROL New Smart Campaign]**。

   ![](assets/alert-the-sales-rep-12.png)

1. **将**&#x200B;营销活动命名为“我的警报营销活动”，然后单击&#x200B;**[!UICONTROL Create]**。

   ![](assets/alert-the-sales-rep-13.png)

1. 在&#x200B;**[!UICONTROL Smart List]**&#x200B;选项卡下，找到&#x200B;**[!UICONTROL Fills Out Form]**&#x200B;触发器并将其拖动到画布。

   ![](assets/alert-the-sales-rep-14.png)

1. 选择我们之前创建的表单。

   ![](assets/alert-the-sales-rep-15.png)

1. 在&#x200B;**[!UICONTROL Flow]**&#x200B;选项卡下，找到&#x200B;**[!UICONTROL Send Alert]**&#x200B;流量操作并将其拖动到画布。

   ![](assets/alert-the-sales-rep-16.png)

1. 选择&#x200B;**[!UICONTROL My Alert Email]**&#x200B;之前创建，并将&#x200B;**[!UICONTROL Send To]**&#x200B;保留为&#x200B;**[!UICONTROL Sales Owner]**。

   ![](assets/alert-the-sales-rep-17.png)

1. 在&#x200B;**[!UICONTROL To Other Emails]**&#x200B;字段中键入您的电子邮件地址。

   ![](assets/alert-the-sales-rep-18.png)

1. 转到&#x200B;**[!UICONTROL Schedule]**&#x200B;选项卡并单击&#x200B;**[!UICONTROL Activate]**&#x200B;按钮。

   ![](assets/alert-the-sales-rep-19.png)

   >[!TIP]
   >
   >将&#x200B;**[!UICONTROL Qualification Rules]**&#x200B;设置为&#x200B;**[!UICONTROL every time]**（通过编辑Smart Campaign）以允许同一人员多次触发警报。

1. 在确认屏幕中点击 **[!UICONTROL Activate]**。

   ![](assets/alert-the-sales-rep-20.png)

## 第3步：测试！ {#step-test-it-out}

1. 选择您的登陆页面并单击&#x200B;**[!UICONTROL View Approved Page]**。

   ![](assets/alert-the-sales-21.png)

   >[!NOTE]
   >
   >不要忘记批准登陆页面；在获得批准之前，登陆页面不会启用。

1. 填写表单并单击&#x200B;**[!UICONTROL Submit]**。

   ![](assets/alert-the-sales-22.png)

1. 您很快就会收到电子邮件。 验证所有功能均可正常使用后，从“发送警报”流程中删除您的电子邮件地址（请参阅上面的步骤2.7）。

   >[!NOTE]
   >
   >单击Marketo中的&#x200B;**[!UICONTROL Person Info]**&#x200B;选项卡以查看联系信息。

## 任务完成！ {#mission-complete}

<br> 

[◄任务7：个性化电子邮件](/help/marketo/getting-started/quick-wins/personalize-an-email.md)

[任务9：更新人员数据►](/help/marketo/getting-started/quick-wins/update-person-data.md)
