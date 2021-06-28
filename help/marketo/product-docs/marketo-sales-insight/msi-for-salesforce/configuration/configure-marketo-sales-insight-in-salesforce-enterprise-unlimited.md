---
unique-page-id: 2360368
description: 在Salesforce企业/无限制 — Marketo文档 — 产品文档中配置Marketo销售分析
title: 在Salesforce企业/无限制中配置Marketo Sales Insight
exl-id: a33ed396-8d26-403f-b6d8-fe7c55ce76ba
source-git-commit: 2e0590d576e5f3ff5ae5e49854a33f04f74a6616
workflow-type: tm+mt
source-wordcount: '824'
ht-degree: 0%

---

# 在Salesforce企业/无限制中配置Marketo Sales Insight {#configure-marketo-sales-insight-in-salesforce-enterprise-unlimited}

以下是在Salesforce企业版/无限制版中配置Marketo Sales Insight时需要执行的步骤。 我们开始吧。

>[!PREREQUISITES]
>
>* [在SalesforceAppExchange中安装Marketo Sales Insight包](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)


>[!NOTE]
**需要管理员权限**

## 在Marketo中配置Sales Insight {#configure-sales-insight-in-marketo}

1. 在Marketo中获取您的MSI凭据。 转到“管理员”区域，然后选择&#x200B;**Sales Insight**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1.png)

1. 单击&#x200B;**编辑API配置**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2.png)

1. 输入您选择的API密钥，然后单击&#x200B;**Save**。 请勿在API密钥中使用与号(&amp;)。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3.png)

   >[!NOTE]
   您的API密钥类似于组织的密码，应该是安全的。

1. 单击“Rest API配置”面板中的&#x200B;**查看**&#x200B;以填充凭据。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4.png)

1. 您将看到确认弹出窗口。 单击&#x200B;**确定**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5.png)

   >[!TIP]
   保持此窗口打开。 您稍后在Salesforce中将需要此信息。

## 在Salesforce中配置销售分析 {#configure-sales-insight-in-salesforce}

1. 在Salesforce中，单击&#x200B;**设置**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6.png)

1. 搜索“远程站点”并选择&#x200B;**远程站点设置**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7.png)

1. 单击&#x200B;**新建远程站点**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8.png)

1. 输入远程站点名称（可以是类似于“MarketoSoapAPI”的内容）。 从Marketo的Soap API配置面板中输入远程站点URL，即您的Marketo主机URL。 单击&#x200B;**Save**。 您现在已为Soap API创建远程站点设置。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9.png)

1. 再次单击&#x200B;**新建远程站点**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10.png)

1. 输入远程站点名称（可以是类似于“MarketoAPI”的内容）。 输入远程站点URL，即Marketo中Rest API配置面板中的API URL。 单击&#x200B;**Save**。 您现在已为Rest API创建了远程站点设置。

   >[!NOTE]
   __ 选择您的 **远程站点名称** （此处使用的是MarketoAPI）。**远程站点URL**&#x200B;可在“在Marketo中配置销售分析”部分步骤3的“编辑API配置”对话框的“Marketo主机”字段中找到。

## 自定义页面布局 {#customize-page-layouts}

1. 单击&#x200B;**Setup**。

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. 搜索“页面布局”并选择&#x200B;**Lead**&#x200B;下的&#x200B;**页面布局**。

   ![](assets/image2015-5-28-14-3a58-3a39.png)

1. 单击左侧的&#x200B;**可视化强制页面**。 将&#x200B;**Section**&#x200B;拖到“自定义链接”部分下的布局中。

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. 输入“Marketo Sales Insight”作为&#x200B;**节名称**。 选择&#x200B;**1-Column**&#x200B;并单击&#x200B;**确定**。

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. 将&#x200B;**Lead**&#x200B;拖放到新部分中。

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   此框的名称将根据对象类型进行更改。 例如，如果您修改“联系人”的页面布局，则会显示“联系人”。

1. 双击您刚才添加的&#x200B;**Lead**&#x200B;块。

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. 编辑高度至&#x200B;**450**&#x200B;像素并单击&#x200B;**确定**。

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!TIP]
   我们建议Accounts和Opportunitys对象的高度为410像素。

1. 单击左侧的&#x200B;**字段**。 然后，搜索并将&#x200B;**Engagement**&#x200B;标签拖动到&#x200B;**Marketo Sales Insight**&#x200B;布局中。

   ![](assets/image2015-5-22-16-3a32-3a46.png)

1. 对这些字段重复上述步骤。

   <table> 
    <tbody> 
     <tr> 
      <td colspan="1">参与度</td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>相对分数值</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>紧急价值</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>最后有趣的时刻日期</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>最后一个有趣的时刻</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>最后有趣的时刻来源</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>最后有趣的时刻类型</p></td> 
     </tr> 
    </tbody> 
   </table>

1. 完成后，单击&#x200B;**保存**。

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. 重复此过程，为&#x200B;**Contact**、**Account**&#x200B;和&#x200B;**Opportunity**&#x200B;添加Visualforce页面部分和Sales Insight字段。

1. 重复步骤5-7，为联系人、帐户和机会添加Visualforce页面部分。 然后，重复步骤8-10，为&#x200B;**Contact**&#x200B;添加Sales Insight字段。 请确保在进行任何更改后进行保存。

## 映射自定义人员字段 {#map-custom-person-fields}

Marketo人员字段需要映射到Salesforce联系字段，以确保转换正常工作。 这是方法。

1. 单击&#x200B;**Setup**。

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. 在搜索栏中搜索“fields”，然后单击&#x200B;**Leads**&#x200B;下的&#x200B;**Fields**。

   ![](assets/image2015-6-1-9-3a54-3a50.png)

1. 单击&#x200B;**映射潜在客户字段**。

   ![](assets/image2015-6-1-9-3a58-3a48.png)

1. 单击&#x200B;**Engagement**&#x200B;右侧的下拉菜单。

   ![](assets/image2015-6-1-10-3a9-3a53.png)

1. 在列表中选择&#x200B;**Contact.Engagement**。

   ![](assets/image2015-6-1-10-3a12-3a11.png)

1. 重复并映射这些字段。

   <table> 
    <tbody> 
     <tr> 
      <th colspan="1" rowspan="1">Marketo人员自定义字段</th> 
      <th colspan="1" rowspan="1">Salesforce联系人自定义字段</th> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>参与度</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Engagement</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>相对分数值</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Relative Score值</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>紧急价值</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Urgency值</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>最后有趣的时刻日期</p></td> 
      <td colspan="1" rowspan="1"><p>联系人。最后一个有趣的时刻日期</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>最后一个有趣的时刻</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Last Interest Moment Desc</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>最后有趣的时刻来源</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Last Interest Moment Source</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>最后有趣的时刻类型</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Last Interest Moment Type</p></td> 
     </tr> 
    </tbody> 
   </table>

1. 完成后，单击&#x200B;**Save**。

## Marketo Sales Insight配置 {#marketo-sales-insight-config}

1. 单击&#x200B;**+**，然后选择&#x200B;**Marketo Sales Insight配置**。

   ![](assets/image2014-9-24-17-3a37-3a45.png)

1. 选中&#x200B;**启用Marketo API**。 然后，在Marketo Admin](#set-up-marketo-sales-insight)中填写[ API配置信息。 完成后，单击&#x200B;**保存更改**。

   ![](assets/image2014-9-24-17-3a38-3a0.png)

   >[!NOTE]
   如果诊断测试失败，您可能需要[向页面布局](https://nation.marketo.com/docs/DOC-1115)添加更多字段。

就这样！ 您应该能够看到“潜在客户”、“联系人”、“帐户”和“业务机会”的“Marketo销售分析”字段。

![](assets/twenty-six.png)

>[!NOTE]
对于帐户，Sales Insight将包含所有电子邮件，但只包含最近的有趣时刻、Web活动和得分变化。

## 访问Marketo Sales Insight {#access-marketo-sales-insight}

1. 在Salesforce中，单击选项卡栏末尾的&#x200B;**+**，然后单击&#x200B;**Marketo Sales Insight配置**。

1. 选中&#x200B;**启用Marketo API**&#x200B;复选框。

1. 从Marketo的“销售分析管理”页面的Soap API面板复制凭据，并将凭据粘贴到“Salesforce销售分析配置”页面的Soap API部分。

1. 从Marketo的“销售分析管理”页面的Rest API面板中复制凭据，并将其粘贴到“Salesforce销售分析配置”页面的Rest API部分。

   ![](assets/access-msi.png)

>[!MORELIKETHIS]
* [优先级、紧急性、相对得分和最佳押注](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
* [将Marketo Sales Insight选项卡和按钮添加到Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/bulk-actions/add-marketo-sales-insight-tab-and-buttons-to-salesforce.md)
* [为团队设置销售分析](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/setting-up-sales-insight-for-your-team.md)

