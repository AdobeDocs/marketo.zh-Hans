---
unique-page-id: 2360368
description: 在Salesforce Enterprise/Unlimited中配置Marketo Sales Insight - Marketo文档 — 产品文档
title: 在Salesforce Enterprise/Unlimited中配置Marketo Sales Insight
exl-id: a33ed396-8d26-403f-b6d8-fe7c55ce76ba
feature: Marketo Sales Insights
source-git-commit: 9d1b18b2aebde00ae715a072580a8f128d07923e
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 0%

---

# 在Salesforce Enterprise/Unlimited中配置Marketo Sales Insight {#configure-marketo-sales-insight-in-salesforce-enterprise-unlimited}

以下是配置Salesforce Enterprise/Unlimited Edition中的Marketo Sales Insight所需的步骤。 我们开始吧。

>[!PREREQUISITES]
>
>[在SalesforceAppExchange中安装Marketo Sales Insight包](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)

>[!NOTE]
>
>**需要管理员权限**

## 在Marketo中配置Sales Insight {#configure-sales-insight-in-marketo}

1. 在Marketo中获取MSI凭据。 转到管理区域并选择 **销售分析**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1.png)

1. 单击 **编辑API配置**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2.png)

1. 输入您选择的API密钥，然后单击 **保存**. 请勿在API密钥中使用&amp;符号。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3.png)

   >[!NOTE]
   >
   >您的API密钥就像您组织的密码，应当是安全的。

1. 单击 **视图** 在Rest API配置面板中填充凭据。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4.png)

1. 您将看到一个确认弹出窗口。 单击 **确定**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5.png)

   >[!TIP]
   >
   >保持这个窗口打开。 稍后在Salesforce中需要此信息。

## 在Salesforce中配置Sales Insight {#configure-sales-insight-in-salesforce}

1. 在Salesforce中，单击 **设置**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6.png)

1. 搜索“远程站点”并选择 **远程站点设置**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7.png)

1. 单击 **新建远程站点**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8.png)

1. 输入远程站点名称（可以类似于“MarketoSoapAPI”）。 输入远程站点URL，它是Marketo中“Soap API配置”面板中的您的Marketo主机URL。 单击 **保存**. 您现在已为Soap API创建了远程站点设置。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9.png)

1. 单击 **新建远程站点** 再来一次。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10.png)

1. 输入远程站点名称（可以是“MarketoAPI”之类的名称）。 输入远程站点URL，它是您在Marketo的Rest API配置面板中的API URL。 单击 **保存**. 您现在已为Rest API创建了远程站点设置。

   >[!NOTE]
   >
   >_您_ 选择您的 **远程站点名称** （此处使用MarketoAPI）。 此 **远程站点URL** 可以在“编辑API配置”对话框的“Marketo主机”字段中找到，该字段位于步骤3“在Marketo中配置Sales Insight”部分。

## 自定义页面布局 {#customize-page-layouts}

1. 单击 **设置**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. 搜索“页面布局”并选择 **页面布局** 下 **潜在客户**.

   ![](assets/image2015-5-28-14-3a58-3a39.png)

1. 单击 **Visualforce页面** 左边。 拖动 **部分** 至自定义链接部分下面的布局。

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. 输入“Marketo Sales Insight”作为 **区域名称**. 选择 **1列** 并单击 **确定**.

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. 拖放 **商机** 到新章节。

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >此框的名称将根据对象类型而变化。 例如，如果您正在修改Contacts的页面布局，则将显示为Contact。

1. 双击 **商机** 您刚刚添加的块。

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. 编辑高度至 **450** 像素并单击 **确定**.

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!NOTE]
   >
   >Check **显示滚动条** 如果您需要访问滚动浏览活动。

   >[!TIP]
   >
   >我们建议将Accounts和Opportunities对象的高度设置为410像素。

1. 单击 **字段** 左边。 然后搜索并拖动 **紧急** 标记到 **Marketo Sales Insight** 布局。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-18.png)

1. 对这些字段也重复上述步骤。

   <table> 
    <tbody> 
     <tr> 
      <td>最后一个有趣的时刻</td> 
     </tr> 
     <tr> 
      <td>上一个有趣时刻的日期</td> 
     </tr> 
     <tr> 
      <td>上一个有趣时刻说明</td> 
     </tr> 
     <tr> 
      <td>上一个有趣时刻源</td> 
     </tr> 
     <tr> 
      <td>上一个有趣时刻类型</td> 
     </tr> 
     <tr> 
      <td>按销售人员列出的最后一次活动</td> 
     </tr> 
     <tr> 
      <td>按销售人员列出的最后一次参与</td> 
     </tr> 
     <tr> 
      <td>MSI联系人ID</td> 
     </tr> 
     <tr> 
      <td>相对分数</td> 
     </tr> 
     <tr> 
      <td>相对得分值</td> 
     </tr> 
     <tr> 
      <td>紧急</td> 
     </tr> 
     <tr> 
      <td>紧急值</td> 
     </tr> 
     <tr> 
      <td>在Marketo中查看</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **保存** 完成后。

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. 重复步骤5 - 7以添加Visualforce页面部分和Sales Insight字段 **联系人**， **帐户** 和 **机会**.

1. 重复步骤8 - 10 ，从下面的列表中添加销售分析字段 **联系人**. 请确保保存所有更改。

<table> 
    <tbody> 
     <tr> 
      <td>最后一个有趣的时刻</td> 
     </tr> 
     <tr> 
      <td>上一个有趣时刻的日期</td> 
     </tr> 
     <tr> 
      <td>上一个有趣时刻说明</td> 
     </tr> 
     <tr> 
      <td>上一个有趣时刻源</td> 
     </tr> 
     <tr> 
      <td>上一个有趣时刻类型</td> 
     </tr> 
     <tr> 
      <td>按销售人员列出的最后Marketo活动</td> 
     </tr> 
     <tr> 
      <td>按销售人员列出的最后一次Marketo参与</td> 
     </tr> 
     <tr> 
      <td>MKTO商机得分</td> 
     </tr> 
     <tr> 
      <td>相对分数</td> 
     </tr> 
     <tr> 
      <td>相对得分值</td> 
     </tr> 
     <tr> 
      <td>销售分析 — 打开联系人完整列表页面</td> 
     </tr> 
     <tr> 
      <td>紧急</td> 
     </tr> 
     <tr> 
      <td>紧急值</td> 
     </tr> 
    </tbody> 
   </table>

## 映射自定义人员字段 {#map-custom-person-fields}

Marketo人员字段需要映射到Salesforce联系人字段，以确保转换正常工作。 具体方法如下。

1. 单击 **设置**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. 在搜索栏中搜索“字段”，然后单击 **字段** 下 **潜在客户**.

   ![](assets/image2015-6-1-9-3a54-3a50.png)

1. 单击 **映射潜在客户字段**.

   ![](assets/image2015-6-1-9-3a58-3a48.png)

1. 单击右侧的下拉菜单以查看 **参与**.

   ![](assets/image2015-6-1-10-3a9-3a53.png)

1. 选择 **Contact.Engagement** 在列表中。

   ![](assets/image2015-6-1-10-3a12-3a11.png)

1. 重复并映射这些字段。

   <table> 
    <tbody> 
     <tr> 
      <th colspan="1" rowspan="1">Marketo人员自定义字段</th> 
      <th colspan="1" rowspan="1">Salesforce联系人自定义字段</th> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>参与</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Engagement</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>相对得分值</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Relative Score值</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>紧急值</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Urginity值</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>上一个有趣时刻的日期</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Last Interest Moment日期</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>上一个有趣时刻说明</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Last有趣时刻说明</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>上一个有趣时刻源</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Last Interest Moment源</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>上一个有趣时刻类型</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Last有趣时刻类型</p></td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **保存** 等你完事了。

## Marketo Sales Insight“配置”选项卡 {#marketo-sales-insight-configuration-tab}

1. 在Salesforce中，单击 **+** 单击选项卡栏末尾的 **Marketo销售分析配置**.

1. 从中的Soap API面板复制凭据 [Marketo的销售分析管理页面](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} 并将其粘贴到“Salesforce销售分析配置”页面的Soap API部分。

1. 从Rest API面板复制凭据于 [Marketo的销售分析管理页面](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} 并将其粘贴到“Salesforce Sales Insight配置”页面的Rest API部分。

   ![](assets/configure-marketo-sales-insight-in-salesforce-enterprise-edition-25.png)

就是这样！ 您应该能够看到Marketo Sales Insight中有关Leads 、 Contacts 、 Accounts和Opportunities的字段。

>[!NOTE]
>
>如果诊断测试失败，您可能需要 [向页面布局添加更多字段](https://nation.marketo.com/docs/DOC-1115){target="_blank"}.

>[!NOTE]
>
>对于客户， Sales Insight将包括所有电子邮件，但只包括最近有趣的时刻、 Web活动和分数更改。

>[!MORELIKETHIS]
>
>* [优先级、紧迫性、相对分数和最佳匹配](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [将Marketo选项卡添加到Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md)
>* [添加对用户档案的销售分析访问权限](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
