---
unique-page-id: 3571743
description: 在Salesforce专业版 — Marketo文档 — 产品文档中配置Marketo Sales Insight
title: 在Salesforce专业版中配置Marketo Sales Insight
translation-type: tm+mt
source-git-commit: ed9399396c82a3b2fb93c83ffdaa1dc7b0827306
workflow-type: tm+mt
source-wordcount: '905'
ht-degree: 0%

---


# 在Salesforce专业版{#configure-marketo-sales-insight-in-salesforce-professional-edition}中配置Marketo Sales Insight

以下是在Salesforce Professional Edition中配置Marketo Sales Insight时需要执行的步骤。 我们开始吧。

>[!PREREQUISITES]
>
>* 在您的Salesforce专业版中安装Marketo。
   >
   >
* [在SalesforceAppExchange中安装Marketo Sales Insight包](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)


>[!NOTE]
>
>**需要管理权限**

## 在Marketo {#configure-sales-insight-in-marketo}中配置Sales Insight

1. 打开新的浏览器窗口，从您的Marketo帐户获取Marketo Sales Insight凭据。
1. 转至“管理员”区域，然后选择&#x200B;**Sales Insight**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1-1.png)

1. 单击&#x200B;**编辑API配置**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2-1.png)

1. 输入您选择的API密钥，然后单击&#x200B;**保存**。 请勿在API密钥中使用&amp;号。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3-1.png)

   >[!NOTE]
   >
   >您的API密钥类似于组织的密码，应该是安全的。

1. 单击“Rest API配置”面板中的&#x200B;**视图**&#x200B;以填充凭据。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4-1.png)

1. 您将看到一个确认弹出窗口。 单击&#x200B;**确定**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5-1.png)

## 在Salesforce中配置Sales Insight {#configure-sales-insight-in-salesforce}

1. 在Salesforce中，单击&#x200B;**Setup**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6-1.png)

1. 搜索“远程站点”并选择&#x200B;**“远程站点设置”**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7-1.png)

1. 单击&#x200B;**新建远程站点**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8-1.png)

1. 输入远程站点名称（可以是“MarketoSoapAPI”）。 在Marketo的“Soap API配置”面板中输入远程站点URL，该URL是您的Marketo主机URL。 单击&#x200B;**保存**。 您现在已为Soap API创建了远程站点设置。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9-1.png)

1. 再次单击&#x200B;**新建远程站点**。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10-1.png)

1. 输入远程站点名称（可以是“MarketoRestAPI”）。 输入远程站点URL，该URL是Marketo中“Rest API配置”面板中的API URL。 单击&#x200B;**保存**。 您现在已为Rest API创建远程站点设置。

## 设置Marketo Sales Insight {#set-up-marketo-sales-insight}

1. 登录到您的Marketo实例，然后单击&#x200B;**管理**。

   ![](assets/login-admin-1.png)

1. 单击&#x200B;**Sales Insight**。

   ![](assets/image2015-5-22-15-3a12-3a33-1.png)

1. 单击&#x200B;**编辑API配置**。

   ![](assets/image2015-5-22-15-3a15-3a0-1.png)

1. 输入&#x200B;**API密钥**，然后单击&#x200B;**保存**。

   >[!CAUTION]
   >
   >请勿在API密钥中使用&amp;号。

   ![](assets/image2015-5-27-16-3a36-3a56-1.png)

   >[!TIP]
   >
   >保持窗口打开。 您以后需要在Salesforce中使用此信息。

1. 返回至Salesforce，单击&#x200B;**Setup**。

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. 搜索“远程站点”，然后单击&#x200B;**安全控件**&#x200B;下的&#x200B;**远程站点设置**。

   ![](assets/image2014-9-24-17-3a25-3a52.png)

1. 单击&#x200B;**新建远程站点**。

   ![](assets/image2014-9-24-17-3a26-3a6.png)

1. 输入&#x200B;**远程站点名称**&#x200B;和&#x200B;**远程站点URL**，然后单击&#x200B;**保存**。

   ![](assets/remote-site-1.png)

   >[!NOTE]
   >
   >选择&#x200B;**远程站点名称**（此处使用MarketoAPI）。 在步骤4的“编辑API配置”对话框的“Marketo主机”字段中，可以找到&#x200B;**远程站点URL**。

## 自定义页面布局{#customize-page-layouts}

1. 单击&#x200B;**Setup**。

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. 搜索“页面布局”并在&#x200B;**Leads**&#x200B;下选择&#x200B;**页面布局**。

   ![](assets/image2015-5-28-14-3a58-3a39-1.png)

1. 单击左侧的&#x200B;**Visualforce页面**。 将&#x200B;**Section**&#x200B;拖至“自定义链接”部分下的布局。

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. 输入“Marketo Sales Insight”作为&#x200B;**节名称**。 选择&#x200B;**1-Column**&#x200B;并单击&#x200B;**确定**。

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. 将&#x200B;**潜在客户**&#x200B;拖放到新部分中。

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >此框的名称将根据对象类型而更改。 例如，如果您正在修改“联系人”的页面布局，则该布局将显示“联系人”。

1. 多次单击刚刚添加的&#x200B;**Lead**&#x200B;块。

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. 编辑高度至&#x200B;**450**&#x200B;像素，然后单击&#x200B;**确定**。

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!TIP]
   >
   >我们建议Accounts和Opportunity对象的高度为410像素。

1. 单击左侧的&#x200B;**字段**。 然后，搜索并将&#x200B;**Engagement**&#x200B;标签拖至&#x200B;**Marketo Sales Insight**&#x200B;布局中。

   ![](assets/image2015-5-22-16-3a32-3a46-1.png)

1. 对这些字段重复上述步骤。

<table> 
 <tbody> 
  <tr> 
   <td colspan="1">参与</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>相对得分值</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>紧急值</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>最后有趣的时刻</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>最后有趣的时刻</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>最后有趣的时刻</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>最后有趣的时刻类型</p></td> 
  </tr> 
 </tbody> 
</table>

1. 完成后，单击&#x200B;**保存**。

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. 重复此过程，为&#x200B;**Contact**、**Account**&#x200B;和&#x200B;**Opportunity**&#x200B;添加Visualforce页面部分和Sales Insight字段。
1. 重复步骤5-7，为Contact、Account和Opportunity添加Visualforce页面部分。 然后，重复步骤8-10，为&#x200B;**Contact**&#x200B;添加Sales Insight字段。 请务必在更改后保存。

## 映射自定义人员字段{#map-custom-person-fields}

需要将Marketo人员字段映射到Salesforce联系人字段，以确保转换正常工作。 下面介绍如何操作。

1. 单击&#x200B;**Setup**。

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. 在搜索栏中搜索“字段”，然后单击&#x200B;**Leads**&#x200B;下的&#x200B;**Fields**。

   ![](assets/image2015-6-1-9-3a54-3a50-1.png)

1. 单击&#x200B;**映射潜在客户字段**。

   ![](assets/image2015-6-1-9-3a58-3a48-1.png)

1. 单击右侧的下拉列表，查看&#x200B;**参与**。

   ![](assets/image2015-6-1-10-3a9-3a53-1.png)

1. 在列表中选择&#x200B;**Contact.Engagement**。

   ![](assets/image2015-6-1-10-3a12-3a11-1.png)

1. 重复这些字段并映射。

<table> 
 <tbody> 
  <tr> 
   <th colspan="1" rowspan="1">Marketo Person自定义字段</th> 
   <th colspan="1" rowspan="1">Salesforce联系人自定义字段</th> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>参与</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Engagement</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>相对得分值</p></td> 
   <td colspan="1" rowspan="1"><p>联系人。相对得分值</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>紧急值</p></td> 
   <td colspan="1" rowspan="1"><p>联系人。紧急值</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>最后有趣的时刻</p></td> 
   <td colspan="1" rowspan="1"><p>联系。最后一个有趣的时刻</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>最后有趣的时刻</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Last Interest Monet Desc</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>最后有趣的时刻</p></td> 
   <td colspan="1" rowspan="1"><p>联系。最后一个有趣的时刻源</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>最后有趣的时刻类型</p></td> 
   <td colspan="1" rowspan="1"><p>联系。最后一个有趣的瞬间类型</p></td> 
  </tr> 
 </tbody> 
</table>

1. 完成后，单击&#x200B;**保存**。

   ![](assets/image2014-9-24-17-3a37-3a17.png)

## Marketo Sales Insight配置{#marketo-sales-insight-config}

1. 单击&#x200B;**+**，然后选择&#x200B;**Marketo Sales Insight Config**。

   ![](assets/image2014-9-24-17-3a37-3a45.png)

1. 选中&#x200B;**启用Marketo API**。 然后，在Marketo Admin](#set-up-marketo-sales-insight)中填写[ API配置信息。 完成后，单击&#x200B;**保存更改**。

   ![](assets/image2014-9-24-17-3a38-3a0.png)

   >[!NOTE]
   >
   >如果诊断测试失败，您可能需要[向页面布局](https://nation.marketo.com/docs/DOC-1115)添加更多字段。

就这样！ 您应该能够看到Lead 、 Contacts 、 Accounts和Opportunity的Marketo Sales Insight字段。

![](assets/twenty-six-1.png)

>[!NOTE]
>
>对于帐户，Sales Insight将包含所有电子邮件，但只包括最近的有趣时刻、Web活动和得分更改。

## 访问Marketo Sales Insight {#access-marketo-sales-insight}

1. 在Salesforce中，单击选项卡栏末尾的&#x200B;**+**，然后单击&#x200B;**Marketo Sales Insight配置**。

1. 选中&#x200B;**启用Marketo API**&#x200B;复选框。

1. 从Marketo的“Sales Insight管理”页面的“Soap API”面板复制凭据，并将其粘贴到“Salesforce Sales Insight配置”页面的“Soap API”部分。

1. 从Marketo的“Sales Insight管理员”页面的“Rest API”面板复制凭据，并将其粘贴到“Salesforce Sales Insight配置”页面的“Rest API”部分。

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-27.png)

>[!MORELIKETHIS]
>
>* [优先级、紧急性、相对得分和最佳赌注](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [将Marketo Sales Insight选项卡和按钮添加到Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/bulk-actions/add-marketo-sales-insight-tab-and-buttons-to-salesforce.md)
>* [为团队设置销售分析](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/setting-up-sales-insight-for-your-team.md)

