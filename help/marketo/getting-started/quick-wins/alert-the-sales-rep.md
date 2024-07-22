---
unique-page-id: 2359424
description: 提醒销售代表 — Marketo文档 — 产品文档
title: 提醒销售代表
exl-id: 4ad7d7b8-ee1e-4605-b4e0-e72a7e573c05
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# 提醒销售代表 {#alert-the-sales-rep}

## 任务：当某人填写您网站上的表单时提醒销售代表 {#mission-alert-the-sales-rep-when-a-person-fills-out-a-form-on-your-web-site}

要自动向销售代表发送警报电子邮件，您只需要一封警报电子邮件和一封电子邮件促销活动。 下面是操作方法。

>[!PREREQUISITES]
>
>带有表单的[登陆页面](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}

## 步骤1：创建警报电子邮件 {#step-create-an-alert-email}

1. 转到&#x200B;**[!UICONTROL 营销活动]**&#x200B;区域。

   ![](assets/alert-the-sales-rep-1.png)

1. 选择您在[登录页中使用表单](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}快速入选创建的&#x200B;**我的项目**，然后在&#x200B;**[!UICONTROL 新建]**&#x200B;下单击&#x200B;**[!UICONTROL 新建本地资产]**。

   ![](assets/alert-the-sales-rep-2.png)

1. 单击&#x200B;**[!UICONTROL 电子邮件]**。

   ![](assets/alert-the-sales-rep-3.png)

1. **将电子邮件命名为“我的电子邮件警报”**，选择一个模板并单击&#x200B;**[!UICONTROL 创建]**。

   ![](assets/alert-the-sales-rep-4.png)

1. 输入您希望销售团队查看的&#x200B;**发件人姓名**、**发件人电子邮件**、**[!UICONTROL 回复]**&#x200B;和&#x200B;**[!UICONTROL 主题]**。

   ![](assets/alert-the-sales-rep-5.png)

1. 双击以编辑电子邮件文本。

   ![](assets/alert-the-sales-rep-6.png)

1. 键入电子邮件内容。

   ![](assets/alert-the-sales-rep-7.png)

1. 将光标放在要插入人员联系信息的位置，然后单击&#x200B;**插入令牌**&#x200B;图标。

   ![](assets/alert-the-sales-rep-8.png)

1. 查找并选择`{{SP_Send_Alert_Info}}` **[!UICONTROL 令牌]**&#x200B;并单击&#x200B;**[!UICONTROL 插入]**。

   ![](assets/alert-the-sales-rep-9.png)

   >[!NOTE]
   >
   >{{SP_Send_Alert_Info}}是警报电子邮件的特殊令牌。 请参阅[使用发送警报信息令牌](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target="_blank"}{target="_blank"}了解更多信息。

1. 单击&#x200B;**[!UICONTROL 保存]**。

   ![](assets/alert-the-sales-rep-10.png)

1. 单击&#x200B;**[!UICONTROL 电子邮件操作]**&#x200B;下拉列表，然后选择&#x200B;**[!UICONTROL 批准并关闭]**。

   ![](assets/alert-the-sales-rep-11.png)

## 步骤2：创建警报触发器营销活动 {#step-create-an-alert-trigger-campaign}

1. 选择之前创建的&#x200B;**我的项目**，然后在&#x200B;**[!UICONTROL 新建]**&#x200B;下单击&#x200B;**[!UICONTROL 新建Smart Campaign]**。

   ![](assets/alert-the-sales-rep-12.png)

1. **将营销活动命名为**&#x200B;我的警报营销活动，然后单击&#x200B;**[!UICONTROL 创建]**。

   ![](assets/alert-the-sales-rep-13.png)

1. 在&#x200B;**[!UICONTROL 智能列表]**&#x200B;选项卡下，找到&#x200B;**[!UICONTROL 填写表单]**&#x200B;触发器并将其拖动到画布。

   ![](assets/alert-the-sales-rep-14.png)

1. 选择我们之前创建的表单。

   ![](assets/alert-the-sales-rep-15.png)

1. 在&#x200B;**[!UICONTROL 流]**&#x200B;选项卡下，找到&#x200B;**[!UICONTROL 发送警报]**&#x200B;流操作并将其拖动到画布。

   ![](assets/alert-the-sales-rep-16.png)

1. 选择&#x200B;**[!UICONTROL 我的警报电子邮件]**，并保留&#x200B;**[!UICONTROL 发送至]**&#x200B;作为&#x200B;**[!UICONTROL 销售所有者]**。

   ![](assets/alert-the-sales-rep-17.png)

1. 在&#x200B;**[!UICONTROL 至其他电子邮件]**&#x200B;字段中键入您的电子邮件地址。

   ![](assets/alert-the-sales-rep-18.png)

1. 转到&#x200B;**[!UICONTROL 计划]**&#x200B;选项卡，然后单击&#x200B;**[!UICONTROL 激活]**&#x200B;按钮。

   ![](assets/alert-the-sales-rep-19.png)

   >[!TIP]
   >
   >每次&#x200B;]**将**[!UICONTROL &#x200B;资格规则&#x200B;]**设置为**[!UICONTROL （通过编辑Smart Campaign），以允许同一人员多次触发警报。

1. 在确认屏幕上单击&#x200B;**[!UICONTROL 激活]**。

   ![](assets/alert-the-sales-rep-20.png)

## 第3步：测试！ {#step-test-it-out}

1. 选择您的登陆页面，然后单击&#x200B;**[!UICONTROL 查看已批准的页面]**。

   ![](assets/alert-the-sales-21.png)

   >[!NOTE]
   >
   >不要忘记批准登陆页面；在获得批准之前，登陆页面不会启用。

1. 填写表单，然后单击&#x200B;**[!UICONTROL 提交]**。

   ![](assets/alert-the-sales-22.png)

1. 您很快就会收到电子邮件。 验证所有功能均可正常使用后，从“发送警报”流程中删除您的电子邮件地址（请参阅上面的步骤2.7）。

   >[!NOTE]
   >
   >单击Marketo中的&#x200B;**[!UICONTROL 人员信息]**&#x200B;选项卡以查看联系信息。

## 任务完成！ {#mission-complete}

<br> 

[◄ Mission 7：个性化电子邮件](/help/marketo/getting-started/quick-wins/personalize-an-email.md)

[任务9：更新人员数据►](/help/marketo/getting-started/quick-wins/update-person-data.md)
