---
unique-page-id: 2360368
description: 了解如何在Salesforce Enterprise/Unlimited版本中配置Marketo Sales Insight。
title: 在Salesforce Enterprise/Unlimited中配置Marketo Sales Insight
exl-id: a33ed396-8d26-403f-b6d8-fe7c55ce76ba
feature: Marketo Sales Insights
source-git-commit: 3cbefabe80778b0502eaecd733b5732fd9003316
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 0%

---

# 在Salesforce Enterprise/Unlimited中配置Marketo Sales Insight {#configure-marketo-sales-insight-in-salesforce-enterprise-unlimited}

完成以下步骤，在Salesforce Enterprise/Unlimited版本中配置Marketo Sales Insight。

>[!PREREQUISITES]
>
>[在SalesforceAppExchange中安装Marketo Sales Insight包](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)

>[!NOTE]
>
>**需要管理员权限。**

## 在Marketo Engage中配置Sales Insight {#configure-sales-insight-in-marketo}

1. 若要在Marketo Engage中获取Marketo Sales Insight凭据，请转到&#x200B;**[!UICONTROL 管理员]**&#x200B;区域并选择&#x200B;**[!UICONTROL Sales Insight]**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1.png)

1. 单击&#x200B;**[!UICONTROL 编辑API配置]**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2.png)

1. 输入您选择的API密钥，然后单击&#x200B;**[!UICONTROL 保存]**。 请勿在API密钥中使用&amp;符号(`&`)。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3.png)

   >[!NOTE]
   >
   >您的API密钥与组织的密码类似，应当是安全的。

1. 要填充凭据，请在&#x200B;_[!UICONTROL Rest API配置]_&#x200B;面板中单击&#x200B;**[!UICONTROL 查看]**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4.png)

1. 如果看到确认对话框，请单击&#x200B;**[!UICONTROL 确定]**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5.png)

   >[!TIP]
   >
   >保持这个窗口打开。 稍后您需要此信息才能配置Salesforce。

## 在Salesforce中配置Sales Insight {#configure-sales-insight-in-salesforce}

1. 在Salesforce中，单击&#x200B;**[!UICONTROL 设置]**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6.png)

1. 搜索“远程站点”并选择&#x200B;**[!UICONTROL 远程站点设置]**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7.png)

1. 单击&#x200B;**[!UICONTROL 新建远程站点]**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8.png)

1. 输入远程站点名称（它可以类似于`MarketoSoapAPI`）。 输入远程站点URL，它是Marketo Engage _[!UICONTROL Soap API配置]_&#x200B;面板中的Marketo主机URL。 单击&#x200B;**[!UICONTROL 保存]**。 您现在已为Soap API创建了远程站点设置。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9.png)

1. 再次单击&#x200B;**[!UICONTROL 新建远程站点]**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10.png)

1. 输入远程站点名称（它可以类似于`MarketoAPI`）。 输入远程站点URL，它是Marketo Engage _[!UICONTROL Rest API配置]_&#x200B;面板中的API URL。 单击&#x200B;**[!UICONTROL 保存]**。 您现在已为Rest API创建了远程站点设置。

   >[!NOTE]
   >
   >_您_&#x200B;选择您的&#x200B;**[!UICONTROL 远程站点名称]** （此处使用了`MarketoAPI`）。 **[!UICONTROL 远程站点URL]**&#x200B;位于“在Marketo中配置Sales Insight in Marketo”部分步骤3中“编辑API配置”对话框的“主机”字段中。

## 授予Sales Insight用户配置文件对标准Salesforce对象的访问权限 {#grant-sales-insight-users-profile-access}

由于Salesforce安全增强，AppExchange包无法再向标准对象授予权限，必须从Salesforce用户的配置文件向相关的Salesforce对象授予访问权限。 要授予所需的权限，请执行以下步骤。

1. 单击&#x200B;**[!UICONTROL 设置]**。

1. 在快速查找中搜索“配置文件”。

1. 单击Salesforce用户正在使用的配置文件旁边的&#x200B;**[!UICONTROL 编辑]**。

1. 在&#x200B;_[!UICONTROL 标准对象权限]_&#x200B;部分下，启用以下对象的&#x200B;**[!UICONTROL 读取]**&#x200B;访问权限：[!UICONTROL 潜在客户]、[!UICONTROL 联系人]、[!UICONTROL 帐户]和[!UICONTROL 机会]。

1. 单击&#x200B;**[!UICONTROL 保存]**。

## 自定义页面布局 {#customize-page-layouts}

1. 单击&#x200B;**[!UICONTROL 设置]**。

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. 搜索“页面布局”并选择&#x200B;**[!UICONTROL 潜在客户]**&#x200B;下的&#x200B;**[!UICONTROL 页面布局]**。

   ![](assets/image2015-5-28-14-3a58-3a39.png)

1. 单击左侧的&#x200B;**[!UICONTROL Visualforce页面]**。 将&#x200B;**[!UICONTROL 节]**&#x200B;拖到&#x200B;_[!UICONTROL 自定义链接]_&#x200B;节下的布局。

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. 输入“Marketo Sales Insight”作为&#x200B;**[!UICONTROL 节名称]**，选择&#x200B;**[!UICONTROL 1 — 列]**，然后单击&#x200B;**[!UICONTROL 确定]**。

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. 将&#x200B;**[!UICONTROL 潜在客户]**&#x200B;拖放到新分区中。

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >此框的名称会根据对象类型而更改。 例如，如果您正在修改“联系人”的页面布局，则会显示“联系人”。

1. 双击刚刚添加的&#x200B;**[!UICONTROL 潜在客户]**&#x200B;块。

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. 将高度编辑为&#x200B;**450**&#x200B;像素，然后单击&#x200B;**[!UICONTROL 确定]**。

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!NOTE]
   >
   >如果需要访问滚动条活动，请选中&#x200B;**[!UICONTROL 显示滚动条]**。

   >[!TIP]
   >
   >Accounts和Opportunities对象的建议高度为410像素。

1. 单击左侧的&#x200B;**[!UICONTROL 字段]**。 然后搜索&#x200B;**[!UICONTROL Urgency]**&#x200B;标签并将其拖动到&#x200B;**[!UICONTROL Marketo Sales Insight]**&#x200B;布局中。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-18.png)

1. 对这些字段也重复上述步骤。

   * 最后一个有趣的时刻
   * 上一个有趣时刻的日期
   * 上一个有趣时刻说明
   * Source上一个有趣的时刻
   * 上一个有趣时刻类型
   * 按销售人员列出的最后一次活动
   * 按销售人员列出的最后一次参与
   * MSI联系人ID
   * 相对分数
   * 相对得分值
   * 紧急
   * 紧急值
   * 在Marketo中查看

1. 完成后单击&#x200B;**[!UICONTROL 保存]**。

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. 重复步骤5 - 7以添加&#x200B;**[!UICONTROL 联系人]**、**[!UICONTROL 帐户]**&#x200B;和&#x200B;**[!UICONTROL Opportunity]**&#x200B;的Visualforce页面部分和Sales Insight字段。

1. 重复步骤8至10，为&#x200B;**[!UICONTROL 联系人]**&#x200B;添加这些Sales Insight字段。 请确保保存所有更改。

   * 最后一个有趣的时刻
   * 上一个有趣时刻的日期
   * [!UICONTROL 上一个有趣时刻描述]
   * [!UICONTROL 最近有趣的时刻Source]
   * [!UICONTROL 上一个有趣的时刻类型]
   * [!UICONTROL 上次Marketo活动（按销售人员列出）]
   * [!UICONTROL 销售人员的最近一次Marketo参与]
   * [!UICONTROL MKTO潜在客户得分]
   * [!UICONTROL 相对分数]
   * [!UICONTROL 相对分数值]
   * [!UICONTROL 销售分析] — 打开联系人完整列表页
   * [!UICONTROL 急迫性]
   * [!UICONTROL 紧急值]

## 映射自定义人员字段 {#map-custom-person-fields}

Marketo人员字段必须映射到Salesforce联系人字段，以确保转换正常工作。 按照以下步骤映射它们。

1. 单击&#x200B;**[!UICONTROL 设置]**。

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. 在搜索栏中搜索“字段”，然后单击&#x200B;**[!UICONTROL 潜在客户]**&#x200B;下的&#x200B;**[!UICONTROL 字段]**。

   ![](assets/image2015-6-1-9-3a54-3a50.png)

1. 单击&#x200B;**[!UICONTROL 映射潜在客户字段]**。

   ![](assets/image2015-6-1-9-3a58-3a48.png)

1. 单击&#x200B;**[!UICONTROL 参与]**&#x200B;右侧的下拉菜单。

   ![](assets/image2015-6-1-10-3a9-3a53.png)

1. 在列表中选择&#x200B;**[!UICONTROL Contact.Engagement]**。

   ![](assets/image2015-6-1-10-3a12-3a11.png)

1. 重复并映射这些字段。

   | Marketo人员自定义字段 | Salesforce联系人自定义字段 |
   |--- |--- |
   | `Engagement` | `Contact.Engagement` |
   | `Relative Score Value` | `Contact.Relative Score Value` |
   | `Urgency Value` | `Contact.Urgency Value` |
   | `Last Interesting Moment Date` | `Contact.Last Interesting Moment Date` |
   | `Last Interesting Moment Desc` | `Contact.Last Interesting Moment Desc` |
   | `Last Interesting Moment Source` | `Contact.Last Interesting Moment Source` |
   | `Last Interesting Moment Type` | `Contact.Last Interesting Moment Type` |

1. 完成后，单击&#x200B;**[!UICONTROL 保存]**。

## Marketo Sales Insight “配置”选项卡 {#marketo-sales-insight-configuration-tab}

1. 在Salesforce中，单击选项卡栏末尾的&#x200B;**+**，然后单击&#x200B;**[!UICONTROL Marketo Sales Insight配置]**。

1. 从[Marketo的Sales Insight Admin页](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"}中的Soap API面板复制凭据，并将其粘贴到Salesforce Sales Insight配置页的Soap API部分。

1. 从[Marketo的Sales Insight Admin页](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"}中的Rest API面板复制凭据，并将其粘贴到Salesforce Sales Insight配置页的Rest API部分。

   ![](assets/configure-marketo-sales-insight-in-salesforce-enterprise-edition-25.png)

您应该能够看到Marketo Sales Insight中有关Leads 、 Contacts 、 Accounts和Opportunities的字段。

>[!NOTE]
>
>如果诊断测试失败，[向页面布局添加更多字段](https://nation.marketo.com:443/t5/knowledgebase/how-to-repair-marketo-sales-insight-setup-configuration-problems/ta-p/248218){target="_blank"}可能会修复此问题。

>[!NOTE]
>
>对于客户， Sales Insight包括所有电子邮件，但只包括最近有趣的时刻、 Web活动和分数更改。

>[!MORELIKETHIS]
>
>* [优先级、紧迫性、相对分数和最佳匹配](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [将Marketo选项卡添加到Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md)
>* [添加销售分析访问用户档案](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
