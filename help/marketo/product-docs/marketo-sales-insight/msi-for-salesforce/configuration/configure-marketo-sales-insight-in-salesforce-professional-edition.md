---
unique-page-id: 3571743
description: 了解如何在Marketo Professional Edition中配置Salesforce Sales Insight。
title: 在Marketo Professional Edition中配置Salesforce Sales Insight
exl-id: fae63560-0bb3-46a9-94a3-cc27c1aa363e
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '672'
ht-degree: 1%

---

# 在[!DNL Marketo Sales Insight] Professional Edition中配置[!DNL Salesforce] {#configure-marketo-sales-insight-in-salesforce-professional-edition}

完成以下步骤以配置Salesforce Professional Edition中的Marketo Sales Insight 。

>[!PREREQUISITES]
>
>* 在[!DNL Salesforce] Professional Edition中安装Marketo。
>
>* 在[AppExchange [!DNL Marketo Sales Insight] 中 [!DNL Salesforce] 安装](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}包

>[!NOTE]
>
>**需要管理员权限。**

## 在Marketo Engage中配置Sales Insight {#configure-sales-insight-in-marketo}

1. 要通过您的Marketo帐户获取Marketo Sales Insight凭据，请打开一个新的浏览器窗口。

1. 转到&#x200B;**[!UICONTROL Admin]**&#x200B;区域并选择&#x200B;**[!UICONTROL Sales Insight]**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1-1.png)

1. 单击 **[!UICONTROL Edit API Configuration]**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2-1.png)

1. 输入您选择的API密钥，然后单击&#x200B;**[!UICONTROL Save]**。 请勿在API密钥中使用&amp;符号(`&`)。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3-1.png)

   >[!NOTE]
   >
   >您的API密钥与组织的密码类似，应当是安全的。

1. 要填充凭据，请单击&#x200B;**[!UICONTROL View]**&#x200B;面板中的&#x200B;_[!UICONTROL Rest API Configuration]_。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4-1.png)

1. 当看到确认对话框时，单击&#x200B;**[!UICONTROL OK]**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5-1.png)

## 在[!DNL Salesforce]中配置Sales Insight {#configure-sales-insight-in-salesforce}

1. 在Salesforce中，单击&#x200B;**[!UICONTROL Setup]**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6-1.png)

1. 搜索“远程站点”并选择&#x200B;**[!UICONTROL Remote Site Settings]**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7-1.png)

1. 单击 **[!UICONTROL New Remote Site]**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8-1.png)

1. 输入远程站点名称（它可以类似于`MarketoSoapAPI`）。 输入远程站点URL，它是Marketo Engage中“Soap API配置”面板中的您的Marketo主机URL。 单击&#x200B;**[!UICONTROL Save]**。 您现在已为Soap API创建了远程站点设置。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9-1.png)

1. 再次单击&#x200B;**[!UICONTROL New Remote Site]**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10-1.png)

1. 输入远程站点名称（可以是“MarketoRestAPI”之类的名称）。 输入远程站点URL，它是您在Marketo的Rest API配置面板中的API URL。 单击&#x200B;**[!UICONTROL Save]**。 您现在已为Rest API创建了远程站点设置。

## 授予Sales Insight用户配置文件对标准Salesforce对象的访问权限 {#grant-sales-insight-users-profile-access}

由于Salesforce安全增强，AppExchange包无法再向标准对象授予权限，必须从Salesforce用户的配置文件向相关的Salesforce对象授予访问权限。 按照以下步骤授予所需权限。

1. 单击 **[!UICONTROL Setup]**。

1. 在快速查找中搜索“配置文件”。

1. 单击Salesforce用户正在使用的配置文件旁边的&#x200B;**[!UICONTROL Edit]**。

1. 在“标准对象权限”部分下，启用以下对象的读取权限：潜在客户、联系人、帐户和机会。

1. 单击 **[!UICONTROL Save]**。

## 自定义页面布局 {#customize-page-layouts}

1. 单击 **[!UICONTROL Setup]**。

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. 搜索“页面布局”并选择&#x200B;**[!UICONTROL Page Layout]**&#x200B;下的&#x200B;**[!UICONTROL Leads]**。

   ![](assets/image2015-5-28-14-3a58-3a39-1.png)

1. 单击左侧的&#x200B;**[!UICONTROL Visualforce Pages]**。 将&#x200B;**[!UICONTROL Section]**&#x200B;拖到“自定义链接”部分下面的布局中。

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. 输入“Marketo Sales Insight”作为&#x200B;**[!UICONTROL Section Name]**。 选择&#x200B;**[!UICONTROL 1-Column]**&#x200B;并单击&#x200B;**[!UICONTROL OK]**。

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. 将&#x200B;**[!UICONTROL Lead]**&#x200B;拖放到新分区中。

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >此框的名称会根据对象类型而更改。 例如，如果您正在修改“联系人”的页面布局，则会显示“联系人”。

1. 双击刚刚添加的&#x200B;**[!UICONTROL Lead]**&#x200B;块。

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. 将高度编辑为450像素，然后单击&#x200B;**[!UICONTROL OK]**。

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!NOTE]
   >
   >如果需要访问滚动浏览活动，请选中&#x200B;**[!UICONTROL Show scrollbars]**。

   >[!TIP]
   >
   >Accounts和Opportunities对象的建议高度为410像素。

1. 单击左侧的&#x200B;**[!UICONTROL Fields]**。 然后搜索&#x200B;**[!UICONTROL Engagement]**&#x200B;标签并将其拖到&#x200B;**[!UICONTROL Marketo Sales Insight]**&#x200B;布局中。

   ![](assets/image2015-5-22-16-3a32-3a46-1.png)

1. 对以下字段重复上述步骤：

   * [!UICONTROL Engagement]
   * [!UICONTROL Relative Score Value]
   * [!UICONTROL Urgency Value]
   * [!UICONTROL Last Interesting Moment Date]
   * [!UICONTROL Last Interesting Moment Desc]
   * [!UICONTROL Last Interesting Moment Source]
   * [!UICONTROL Last Interesting Moment Type]

1. 完成后单击 **[!UICONTROL Save]**。

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. 要为&#x200B;**[!UICONTROL Contact]**、**[!UICONTROL Account]**&#x200B;和&#x200B;**[!UICONTROL Opportunity]**&#x200B;添加Visualforce页面部分，请重复步骤5至7。

1. 重复步骤8 - 10以添加&#x200B;**[!UICONTROL Contact]**&#x200B;的Sales Insight字段。 请确保在进行任何更改后进行保存。

## 映射自定义人员字段 {#map-custom-person-fields}

Marketo人员字段必须映射到Salesforce联系人字段，以确保转换正常工作。 按照以下步骤映射它们。

1. 单击 **[!UICONTROL Setup]**。

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. 在搜索栏中搜索“字段”，然后单击&#x200B;**[!UICONTROL Fields]**&#x200B;下的&#x200B;**[!UICONTROL Leads]**。

   ![](assets/image2015-6-1-9-3a54-3a50-1.png)

1. 单击 **[!UICONTROL Map Lead Fields]**。

   ![](assets/image2015-6-1-9-3a58-3a48-1.png)

1. 单击&#x200B;**[!UICONTROL Engagement]**&#x200B;右侧的下拉菜单。

   ![](assets/image2015-6-1-10-3a9-3a53-1.png)

1. 在列表中选择&#x200B;**[!UICONTROL Contact.Engagement]**。

   ![](assets/image2015-6-1-10-3a12-3a11-1.png)

1. 同时重复并映射这些字段。

   | Marketo人员自定义字段 | Salesforce联系人自定义字段 |
   |--- |--- |
   | `Engagement` | `Contact.Engagement` |
   | `Relative Score Value` | `Contact.Relative Score Value` |
   | `Urgency Value` | `Contact.Urgency Value` |
   | `Last Interesting Moment Date` | `Contact.Last Interesting Moment Date` |
   | `Last Interesting Moment Desc` | `Contact.Last Interesting Moment Desc` |
   | `Last Interesting Moment Source` | `Contact.Last Interesting Moment Source` |
   | `Last Interesting Moment Type` | `Contact.Last Interesting Moment Type` |

   {style="table-layout:auto"}

1. 完成后，单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/image2014-9-24-17-3a37-3a17.png)

## Marketo Sales Insight的“配置”选项卡 {#marketo-sales-insight-configuration-tab}

1. 在Salesforce中，单击选项卡栏末尾的&#x200B;**+**，然后单击&#x200B;**[!UICONTROL Marketo Sales Insight Config]**。

1. 从[Marketo的Sales Insight Admin页](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"}中的Soap API面板复制凭据，并将其粘贴到Salesforce Sales Insight配置页的Soap API部分中。

1. 从&#x200B;**[!UICONTROL Rest API]** Marketo的Sales Insight管理页面[中的](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"}面板复制凭据，并将其粘贴到Salesforce Sales Insight配置页面的Rest API部分。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-27.png)

您应该能够看到Marketo Sales Insight中的Leads 、 Contacts 、 Accounts和Opportunities字段。

>[!NOTE]
>
>如果诊断测试失败，[向页面布局添加更多字段](https://nation.marketo.com/t5/knowledgebase/how-to-repair-marketo-sales-insight-setup-configuration-problems/ta-p/248218){target="_blank"}可能会修复此问题。

>[!NOTE]
>
>对于客户，Sales Insight包括所有电子邮件，但只包括最近有趣的时刻、Web活动和分数更改。

>[!MORELIKETHIS]
>
>* [优先级、紧迫性、相对分数和最佳匹配](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md){target="_blank"}
>* [将Marketo选项卡添加到 [!DNL Salesforce]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md){target="_blank"}
>* [添加Sales Insight访问用户档案的权限](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
