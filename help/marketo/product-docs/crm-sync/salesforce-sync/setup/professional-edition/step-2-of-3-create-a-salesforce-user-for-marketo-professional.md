---
unique-page-id: 3571797
description: 第2步（共3步） — 创建Salesforce用户以使用Marketo（专业） - Marketo文档 — 产品文档
title: 第2步（共3步） — 创建Marketo的Salesforce用户（专业）
exl-id: 7eb4bf89-b6e4-45e0-adee-e2976cb01dd3
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---

# 第2步（共3步）：为Marketo (Professional)创建[!DNL Salesforce]用户 {#step-of-create-a-salesforce-user-for-marketo-professional}

>[!NOTE]
>
>这些步骤必须由Salesforce管理员完成。

>[!PREREQUISITES]
>
>[第1步（共3步）：将Marketo字段添加到Salesforce (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md){target="_blank"}

在本文中，您将使用[!DNL Salesforce]页面布局自定义字段权限，并创建Marketo-[!DNL Salesforce]同步用户。

## 设置页面布局 {#set-page-layouts}

[!DNL Salesforce]专业人员设置具有页面布局的字段级辅助功能，而不是[!DNL Salesforce]企业/无限配置文件的辅助功能。 执行以下步骤将允许Marketo同步用户更新自定义字段。

1. 在导航搜索栏中键入“[!UICONTROL page layouts]”而不按&#x200B;**[!UICONTROL Enter]**，然后单击&#x200B;**[!UICONTROL Page Layout]**&#x200B;下的&#x200B;**[!UICONTROL Leads]**。

   ![](assets/image2016-2-26-12-3a58-3a32.png)

1. 单击“潜在客户布局”旁边的&#x200B;**[!UICONTROL Edit]**。

   ![](assets/image2016-2-26-13-3a2-3a46.png)

1. 单击并将新&#x200B;**[!UICONTROL Section]**&#x200B;拖到页面布局中。

   ![](assets/image2014-12-9-12-3a56-3a40.png)

1. 输入&#x200B;**[!UICONTROL Section Name]**&#x200B;的“Marketo”并单击&#x200B;**[!UICONTROL OK]**。

   ![](assets/image2014-12-9-12-3a56-3a52.png)

1. 单击并将字段&#x200B;**[!UICONTROL Acquisition Date]**&#x200B;拖入&#x200B;**Marketo**&#x200B;部分。

   ![](assets/image2014-12-9-12-3a57-3a0.png)

1. 对以下字段重复上述步骤：

   * [!UICONTROL Acquisition Program]
   * [!UICONTROL Acquisition Program Id]
   * [!UICONTROL Email Opt Out]
   * [!UICONTROL Inferred City]
   * [!UICONTROL Inferred Company]
   * [!UICONTROL Inferred Country]
   * [!UICONTROL Inferred Metropolitan Area]
   * [!UICONTROL Inferred Phone Area Code]
   * [!UICONTROL Inferred Postal Code]
   * [!UICONTROL Inferred State Region]
   * [!UICONTROL Lead Score]
   * [!UICONTROL Original Referrer]
   * [!UICONTROL Original Search Engine]
   * [!UICONTROL Original Search Phrase]
   * [!UICONTROL Original Source Info]
   * [!UICONTROL Original Source Type]

   >[!NOTE]
   >
   >这些字段需要在页面布局中，以便Marketo能够对其执行读/写操作。

   >[!TIP]
   >
   >通过向下拖动到页面的右侧，为字段创建两列。 您可以将字段从一侧移动到另一侧，以平衡列长度。

1. 添加完字段后单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/image2014-12-9-12-3a57-3a10.png)

1. 对Salesforce **[!UICONTROL Contact Page Layout]**&#x200B;重复上述所有步骤。

   ![](assets/image2016-2-26-13-3a10-3a1.png)

1. 完成&#x200B;**[!UICONTROL Save]**&#x200B;后请记得单击&#x200B;**[!UICONTROL Contact Page Layout]**。

   ![](assets/image2014-12-9-12-3a57-3a30.png)

   >[!NOTE]
   >
   >确保已将&#x200B;**[!UICONTROL All-Day Event]**&#x200B;字段添加到&#x200B;**[!UICONTROL Event Page Layout]**。

## 创建同步用户 {#create-sync-user}

Marketo需要凭据才能访问[!DNL Salesforce]。 最好是通过执行以下步骤创建的专用用户来完成此操作。

>[!NOTE]
>
>如果贵组织没有额外的Salesforce许可证，则可以将现有营销用户与系统管理员配置文件结合使用。

1. 在导航搜索栏中输入“用户”，然后单击&#x200B;**[!UICONTROL Users]**&#x200B;下的&#x200B;**[!UICONTROL Manage Users]**。

   ![](assets/image2014-12-9-12-3a57-3a42.png)

1. 单击 **[!UICONTROL New User]**。

   ![](assets/image2014-12-9-12-3a58-3a1.png)

1. 填写必填字段，选择&#x200B;**[!UICONTROL User License: Salesforce]**，设置&#x200B;**[!UICONTROL Profile: System Administrator]**，选中&#x200B;**[!UICONTROL Marketing User]**&#x200B;并单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/image2014-12-9-12-3a58-3a11.png)

   >[!TIP]
   >
   >确保您输入的电子邮件地址有效。 您需要以同步用户身份登录才能重置密码。

太棒了！ 现在，您拥有了一个帐户，Marketo可使用该帐户连接到[!DNL Salesforce]。 我们开始吧。

>[!MORELIKETHIS]
>
>[第3步（共3步）：连接Marketo和Salesforce（专业）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-3-of-3-connect-marketo-and-salesforce-professional.md){target="_blank"}
