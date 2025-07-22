---
description: 项目群成员自定义字段同步 — Marketo文档 — 产品文档
title: 程序成员自定义字段同步
exl-id: 7facfc79-a411-4ad9-b847-2002763af5bb
feature: Programs
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 6%

---

# 程序成员自定义字段同步 {#program-member-custom-field-sync}

>[!PREREQUISITES]
>
>* 创建[项目群成员自定义字段](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md){target="_blank"}
>* [将 [!DNL Salesforce] 营销活动与项目同步](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md){target="_blank"}

>[!NOTE]
>
>程序成员对象最多可以有20个自定义字段。 这些字段适用于任何项目。

## 将Salesforce字段映射到计划成员自定义字段 {#map-salesforce-fields-to-program-member-custom-fields}

1. 在Marketo中，单击&#x200B;**[!UICONTROL Admin]**。

   ![](assets/program-member-custom-field-sync-1.png)

1. 单击“**[!DNL Salesforce]**”，然后单击“程序成员自定义字段同步”旁边的“**[!UICONTROL Edit]**”。

   ![](assets/program-member-custom-field-sync-2.png)

1. 使用搜索框找到要映射的[!DNL Salesforce]字段。 在此示例中，我们使用“请勿调用”。

   ![](assets/program-member-custom-field-sync-3.png)

1. 单击下拉列表。

   ![](assets/program-member-custom-field-sync-4.png)

1. 选择要映射的Marketo [!UICONTROL Program Member Custom Field]。

   ![](assets/program-member-custom-field-sync-5.png)

   >[!NOTE]
   >
   >下拉列表将仅显示与[!UICONTROL Program Member Custom Fields]字段的数据类型匹配的[!DNL Salesforce]。

1. 对于其他字段映射，请清除搜索框并重复步骤3至5。

1. 完成后单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/program-member-custom-field-sync-6.png)

   >[!IMPORTANT]
   >
   >今后，对映射字段上的项目群成员数据的更改将在Marketo和[!DNL Salesforce]之间同步。

   >[!NOTE]
   >
   >如果您重命名或更改[!DNL Salesforce]中某个字段的数据类型，我们将使用[!UICONTROL Program Member Custom Field]删除该字段的任何映射。 但是，您可以在查看后使用新字段重新映射它。

## 从项目群成员自定义字段中取消映射Salesforce字段 {#unmap-salesforce-fields-from-program-member-custom-fields}

如果您希望释放字段以替换它，或只是进行常规更改，则必须先执行取消映射。 具体方法如下。

1. 在Marketo中，单击&#x200B;**[!UICONTROL Admin]**。

   ![](assets/program-member-custom-field-sync-7.png)

1. 单击“**[!DNL Salesforce]**”，然后单击“程序成员自定义字段同步”旁边的“**[!UICONTROL Edit]**”。

   ![](assets/program-member-custom-field-sync-8.png)

1. 使用搜索框查找要取消映射的字段。 在此示例中，我们使用“请勿调用”。

   ![](assets/program-member-custom-field-sync-9.png)

   >[!TIP]
   >
   >您可以选中&#x200B;**[!UICONTROL Mapped]**&#x200B;复选框以仅查看映射的字段。

1. 通过单击字段旁边的&#x200B;**X**&#x200B;取消映射。

   ![](assets/program-member-custom-field-sync-10.png)

1. 该映射现已删除。 单击 **[!UICONTROL Save]**。

   ![](assets/program-member-custom-field-sync-11.png)

## 数据类型映射 {#data-type-mapping}

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>SFDC数据类型</th>
      <th>项目群成员自定义字段数据类型</th>
    </tr>
    <tr>
      <td>文本</td>
      <td>字符串</td>
    </tr>
    <tr>
      <td>选取列表</td>
      <td>字符串</td>
    </tr>
    <tr>
      <td>多选挑选列表</td>
      <td>字符串</td>
    </tr>
    <tr>
      <td>电话</td>
      <td>字符串</td>
    </tr>
    <tr>
      <td>电子邮件</td>
      <td>字符串</td>
    </tr>
    <tr>
      <td>数字(m)</td>
      <td>整数</td>
    </tr>
    <tr>
      <td>数字(m，n)</td>
      <td>浮点值</td>
    </tr>
    <tr>
      <td>复选框</td>
      <td>布尔值</td>
    </tr>
    <tr>
      <td>URL</td>
      <td>URL</td>
    </tr>
    <tr>
      <td>日期</td>
      <td>日期</td>
    </tr>
    <tr>
      <td>日期时间</td>
      <td>日期时间</td>
    </tr>
    <tr>
      <td>查找（引用）</td>
      <td>字符串</td>
    </tr>
    <tr>
      <td>比值64</td>
      <td>字符串</td>
    </tr>
  </tbody>
</table>

>[!MORELIKETHIS]
>
>* [更改计划成员数据](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-member-data.md){target="_blank"}
>* [查看项目群成员网格上的数据](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/manage-and-view-members.md){target="_blank"}
>* [SFDC同步 — Campaign同步](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md){target="_blank"}
