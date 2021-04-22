---
unique-page-id: 4719294
description: 自定义活动同步 — Marketo Docs — 产品文档
title: 自定义活动同步
exl-id: 938d83dc-b9b1-41d8-bf98-04548b074ec4
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# 自定义活动同步{#customize-activities-sync}

如果您不使用Marketo Sales Insight，Marketo可以为某些事件创建Salesforce活动历史记录。 下面介绍如何启用它们。

1. 转至&#x200B;**Admin**。

   ![](assets/admin.png)

1. 单击&#x200B;**Salesforce**，然后单击&#x200B;**编辑同步选项**。

   ![](assets/two-1.png)

1. 选中要Marketo推送到Salesforce的活动旁的复选框，然后单击&#x200B;**保存**。

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >启用后，Marketo将推动价值三个月的活动历史。 根据数据量，_完成此操作可能需要几天时间。_ 在初始活动推送期间发生的更新可能会延迟到初始活动同步完成之后。

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <thead> 
  <tr> 
   <th>活动类型</th> 
   <th>说明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>已填写表单</td> 
   <td>填写任何Marketo表单</td> 
  </tr> 
  <tr> 
   <td>添加到列表</td> 
   <td><p>流步骤：已添加到静态列表</p></td> 
  </tr> 
  <tr> 
   <td>电子邮件已发送</td> 
   <td>流步骤：已发送电子邮件</td> 
  </tr> 
  <tr> 
   <td>电子邮件</td> 
   <td>已收到电子邮件（未退回）</td> 
  </tr> 
  <tr> 
   <td>电子邮件已打开</td> 
   <td>打开电子邮件（不阻止图像）</td> 
  </tr> 
  <tr> 
   <td>已单击电子邮件中的链接</td> 
   <td>单击了Marketo发送的电子邮件中的链接</td> 
  </tr> 
  <tr> 
   <td>已从列表中删除</td> 
   <td>流步骤：已从静态列表中删除</td> 
  </tr> 
  <tr> 
   <td>从流中删除</td> 
   <td>流步骤：从流中删除</td> 
  </tr> 
  <tr> 
   <td>已发送销售电子邮件</td> 
   <td>通过Marketo Sales Insight发送了电子邮件</td> 
  </tr> 
  <tr> 
   <td>已打开销售电子邮件</td> 
   <td>已打开通过Marketo Sales Insight发送的电子邮件</td> 
  </tr> 
  <tr> 
   <td>单击销售电子邮件中的链接</td> 
   <td>已点击通过Marketo Sales Insight发送的电子邮件中的链接</td> 
  </tr> 
  <tr> 
   <td>收到销售电子邮件</td> 
   <td>销售代表在MSI Outlook插件中收到并记录了电子邮件</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>“收到销售电子邮件”**不**&#x200B;表示已送达。 未为通过Sales Insight发送的电子邮件捕获已交付状态。

>[!TIP]
>
>如果您有兴趣将更多Marketo信息导入Salesforce，请查看我们的[Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)产品。
