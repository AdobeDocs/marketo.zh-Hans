---
unique-page-id: 4719294
description: 自定义活动同步 — Marketo文档 — 产品文档
title: 自定义活动同步
exl-id: 938d83dc-b9b1-41d8-bf98-04548b074ec4
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# 自定义活动同步 {#customize-activities-sync}

如果您不使用Marketo Sales Insight，Marketo可以为某些事件创建Salesforce活动历史记录。 下面是如何启用它们。

1. 转到 **管理员**.

   ![](assets/admin.png)

1. 单击 **Salesforce**，然后单击 **编辑同步选项**.

   ![](assets/two-1.png)

1. 选中您希望Marketo推送到Salesforce的活动旁边的复选框，然后单击 **保存**.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >启用后，Marketo将推送三个月的活动历史记录。 根据数据量， _这可能需要几天才能完成_. 在初始活动推送期间发生的更新可能会延迟到初始活动同步完成后。

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <thead> 
  <tr> 
   <th>活动类型</th> 
   <th>描述</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>已填写的表单</td> 
   <td>填写任意Marketo表单</td> 
  </tr> 
  <tr> 
   <td>已添加到列表</td> 
   <td><p>流程步骤：已添加到静态列表</p></td> 
  </tr> 
  <tr> 
   <td>电子邮件已发送</td> 
   <td>流程步骤：已发送电子邮件</td> 
  </tr> 
  <tr> 
   <td>电子邮件已投放</td> 
   <td>已收到电子邮件（未退回）</td> 
  </tr> 
  <tr> 
   <td>电子邮件已打开</td> 
   <td>已打开电子邮件（未阻止图像）</td> 
  </tr> 
  <tr> 
   <td>已单击电子邮件中的链接</td> 
   <td>已单击Marketo发送的电子邮件中的链接</td> 
  </tr> 
  <tr> 
   <td>已从列表中删除</td> 
   <td>流程步骤：已从静态列表中删除</td> 
  </tr> 
  <tr> 
   <td>从流中删除</td> 
   <td>流程步骤：从流程中删除</td> 
  </tr> 
  <tr> 
   <td>已发送销售电子邮件</td> 
   <td>通过Marketo Sales Insight发送了一封电子邮件</td> 
  </tr> 
  <tr> 
   <td>已打开销售电子邮件</td> 
   <td>已打开通过Marketo Sales Insight发送的电子邮件</td> 
  </tr> 
  <tr> 
   <td>单击销售电子邮件中的链接</td> 
   <td>单击通过Marketo Sales Insight发送的电子邮件中的链接</td> 
  </tr> 
  <tr> 
   <td>已收到销售电子邮件</td> 
   <td>销售代表在MSI Outlook插件中收到并记录电子邮件</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>“已收到的销售电子邮件”会 **非** 意思是成功了。 对于通过Sales Insight发送的电子邮件，不会捕获已投放状态。

>[!TIP]
>
>如果您有兴趣将更多Marketo信息放入Salesforce，请查看我们的 [Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) 产品。
