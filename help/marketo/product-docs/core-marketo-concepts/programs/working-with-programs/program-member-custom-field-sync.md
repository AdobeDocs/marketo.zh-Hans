---
description: 项目成员自定义字段同步 — Marketo文档 — 产品文档
title: 程序成员自定义字段同步
exl-id: 7facfc79-a411-4ad9-b847-2002763af5bb
source-git-commit: 85e04fb8a52a417982014bc4bb101b6044e53f84
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 4%

---

# 程序成员自定义字段同步 {#program-member-custom-field-sync}

>[!PREREQUISITES]
>
>* 创建 [程序成员自定义字段](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md){target=&quot;_blank&quot;}
>* [将Salesforce营销活动与项目同步](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md){target=&quot;_blank&quot;}


>[!NOTE]
>
>程序成员对象最多可以有20个自定义字段。 这些字段可用于任何程序。

## 将Salesforce字段映射到程序成员自定义字段 {#map-salesforce-fields-to-program-member-custom-fields}

1. 在Marketo中，单击 **管理员**.

   ![](assets/program-member-custom-field-sync-1.png)

1. 单击 **Salesforce**，然后单击 **编辑** 程序成员自定义字段同步旁边。

   ![](assets/program-member-custom-field-sync-2.png)

1. 使用搜索框可找到要映射的Salesforce字段。 在此示例中，我们使用Do Not Call。

   ![](assets/program-member-custom-field-sync-3.png)

1. 单击下拉菜单。

   ![](assets/program-member-custom-field-sync-4.png)

1. 选择要映射的所需Marketo项目成员自定义字段。

   ![](assets/program-member-custom-field-sync-5.png)

   >[!NOTE]
   >
   >下拉列表将仅显示与Salesforce字段的数据类型匹配的程序成员自定义字段。

1. 对于其他字段映射，请清除搜索框并重复步骤3至5。

1. 单击 **保存** 完成时。

   ![](assets/program-member-custom-field-sync-6.png)

   >[!IMPORTANT]
   >
   >今后，对映射字段中程序成员数据的更改将在Marketo和Salesforce之间同步。

   >[!NOTE]
   >
   >如果在Salesforce中重命名或更改字段的数据类型，我们将删除该字段与程序成员自定义字段的任何映射。 但是，您可以在审核后使用新字段重新映射它。

## 从程序成员自定义字段中取消映射Salesforce字段 {#unmap-salesforce-fields-from-program-member-custom-fields}

如果您想要释放字段以替换它，或只是进行一般更改，则必须先执行取消映射。 这是方法。

1. 在Marketo中，单击 **管理员**.

   ![](assets/program-member-custom-field-sync-7.png)

1. 单击 **Salesforce**，然后单击 **编辑** 程序成员自定义字段同步旁边。

   ![](assets/program-member-custom-field-sync-8.png)

1. 使用搜索框可找到要取消映射的字段。 在此示例中，我们使用Do Not Call。

   ![](assets/program-member-custom-field-sync-9.png)

   >[!TIP]
   >
   >您可以选择 **已映射** 复选框以仅查看映射的字段。

1. 通过单击 **X** 字段旁边。

   ![](assets/program-member-custom-field-sync-10.png)

1. 映射现已删除。 单击 **保存**.

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
      <th>程序成员自定义字段数据类型</th>
    </tr>
    <tr>
      <td>文本</td>
      <td>字符串</td>
    </tr>
    <tr>
      <td>挑库</td>
      <td>字符串</td>
    </tr>
    <tr>
      <td>多选选取列表</td>
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
      <td>数(m)</td>
      <td>整数</td>
    </tr>
    <tr>
      <td>数(m，n)</td>
      <td>浮动</td>
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
      <td>Base64</td>
      <td>字符串</td>
    </tr>
  </tbody>
</table>

>[!MORELIKETHIS]
>
>* [更改程序成员数据](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-member-data.md){target=&quot;_blank&quot;}
>* [查看“程序成员”网格上的数据](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/manage-and-view-members.md){target=&quot;_blank&quot;}
>* [SFDC同步 — 促销活动同步](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md){target=&quot;_blank&quot;}

