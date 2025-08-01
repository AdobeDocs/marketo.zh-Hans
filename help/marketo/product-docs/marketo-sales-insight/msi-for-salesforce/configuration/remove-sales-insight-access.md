---
description: 删除销售Insight访问权限 — Marketo文档 — 产品文档
title: 删除Sales Insight访问权限
exl-id: 3cda112a-524e-469b-a222-c0192b2f5301
feature: Marketo Sales Insights
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 3%

---

# 移除[!DNL Sales Insight]访问权限 {#remove-sales-insight-access}

使用以下步骤移除对[!DNL Sales Insight]中[!DNL Salesforce]功能的访问权限。 适用于[!DNL Salesforce] Classic和Lightning。

## 概述 {#overview}

访问所有[!DNL Sales Insight]功能需要以下提及的对象、Apex类和Visualforce页面的权限。 删除这些项将删除对[!DNL Sales Insight]的访问权限。

**对象设置**

<table>
 <tbody>
 <tr>
   <td>BestBetsCache</td>
   <td>读取、创建、编辑、删除、查看全部、修改全部</td>
  </tr>
  <tr>
   <td>[!DNL Best Bets] 查看详细信息</td>
   <td>读取、创建、编辑、删除、查看全部、修改全部</td>
  </tr>
  <tr>
   <td>[!DNL Best Bets] 视图</td>
   <td>读取、创建、编辑、删除、查看全部、修改全部</td>
  </tr>
  <tr>
   <td>EmailActivityCache</td>
   <td>读取、创建、编辑、删除、查看全部、修改全部</td>
  </tr>
  <tr>
   <td>GetMethodArgus</td>
   <td>读取、创建、编辑、删除、查看全部、修改全部</td>
  </tr>
  <tr>
   <td>GroupedWebActivityCache</td>
   <td>读取、创建、编辑、删除、查看全部、修改全部</td>
  </tr>
  <tr>
   <td>InterestedMentsCache</td>
   <td>读取、创建、编辑、删除、查看全部、修改全部</td>
  </tr>
  <tr>
   <td>[!DNL Marketo Sales Insight] 配置</td>
   <td>读取、创建、编辑、删除、查看全部、修改全部</td>
  </tr>
  <tr>
   <td>评分缓存</td>
   <td>读取、创建、编辑、删除、查看全部、修改全部</td>
  </tr>
  <tr>
   <td>值</td>
   <td>读取、创建、编辑、删除、查看全部、修改全部</td>
  </tr>
  <tr>
   <td>WebActivityCache</td>
   <td>读取、创建、编辑、删除、查看全部、修改全部</td>
  </tr>
 </tbody>
</table>

* Apex类访问：以“mkto_si”开头的159个Apex类
* Visualforce页面访问：64个以“mkto_si”开头的Visualforce页面
* 自定义设置定义：mkto_si.Marketo设置和mkto_si.User首选项

## 正在删除对[!DNL Sales Insight]的访问权限 {#removing-access-to-sales-insight}

1. 登录到您的[!DNL Salesforce]帐户。

1. 单击 **[!UICONTROL Setup]**。

   ![](assets/remove-sales-insight-access-1.png)

1. 在[!UICONTROL Administrator]下，单击&#x200B;**[!UICONTROL Manage Users]**，然后单击&#x200B;**[!UICONTROL Profiles]**。

1. 单击要更新的配置文件，然后单击&#x200B;**[!UICONTROL Edit]**。

1. 向下滚动到[!UICONTROL Custom Tab Settings]下的“[!UICONTROL Tab Settings]”。

1. 从[!UICONTROL Tab Hidden]配置和MSI [!DNL Marketo Sales Insight]发件箱的下拉列表中选择“[!DNL Marketo Sales]”选项。

   ![](assets/remove-sales-insight-access-2.png)

   ![](assets/remove-sales-insight-access-3.png)

1. 向下滚动到“[!UICONTROL Custom Object Permissions]”。

1. 删除以下对象的“读取、创建、编辑、删除”权限：

   * BestBetsCache
   * [!DNL Best Bets]查看详细信息
   * [!DNL Best Bets]次查看
   * EmailActivityCache
   * GetMethodArgus
   * GroupedWebActivityCache
   * InterestedMentsCache
   * [!DNL Marketo Sales Insight]配置
   * 评分缓存
   * 值
   * WebActivityCache

1. 向下滚动到“[!UICONTROL Enabled Apex Class Access]”部分。 单击 **[!UICONTROL Edit]**。

1. 从“[!UICONTROL Enabled Apex Classes]”部分中，选择以“mkto_si”开头的所有类。 这最多可添加159个类。

1. 单击&#x200B;**[!UICONTROL Remove]**，然后单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/remove-sales-insight-access-4.png)

1. 向下滚动到“[!UICONTROL Enabled Visualforce Page Access]”部分。 单击 **[!UICONTROL Edit]**。

1. 从“[!UICONTROL Enabled Visualforce Pages]”部分中，选择以“mkto_si”开头的所有页面。 最多可加64页。

1. 单击&#x200B;**[!UICONTROL Remove]**，然后单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/remove-sales-insight-access-5.png)

1. 向下滚动到“[!UICONTROL Enabled Custom Setting Definitions Access]”部分。 单击 **[!UICONTROL Edit]**。

1. 选择“Marketo Sales Insight.mkto_si.Marketo设置”和“Marketo Sales Insight.mkto_si.User首选项”。

1. 单击&#x200B;**[!UICONTROL Remove]**，然后单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/remove-sales-insight-access-6.png)

操作完成！您已成功移除[!DNL Sales Insight]访问权限。 对要删除其访问权限的任何其他配置文件重复相同的步骤。
