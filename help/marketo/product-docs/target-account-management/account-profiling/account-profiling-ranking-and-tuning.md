---
unique-page-id: 15695924
description: 帐户分析排名和调整 — Marketo文档 — 产品文档
title: 帐户分析排名和调整
exl-id: 9c5d0a03-0ebe-43cc-95ef-faab19a7f673
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 0%

---

# 帐户分析排名和调整 {#account-profiling-ranking-and-tuning}

帐户分析可确定您的理想客户资料(ICP)，根据ICP对数据库中的公司进行排名，并将ICP指标数据添加到作为指定帐户促销的帐户中。

## 模型结果 {#model-results}

结果显示所有已知帐户按级别划分。 A是最高级别，D是最低级别。

![](assets/results.png)

而我们建议您选中自动提升复选框（可选），因为这样可以节省您大量的时间。 但是，如果您希望查看每个帐户和 [手动添加](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md#discover-crm-accounts)，则只需取消选中该框。

<table> 
 <tbody> 
  <tr> 
   <td><strong>排名</strong></td> 
   <td> 
    <div>
      帐户排名基于理想客户资料。 A最合适，D最不适合。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>倾向</strong></td> 
   <td> 
    <div>
      与基于非比较方案的账户选择相比，转换率的估计增加。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>帐户 (%)</strong></td> 
   <td> 
    <div>
      模型输入中具有此排名的帐户百分比。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>模型基础的百分比</strong></td> 
   <td> 
    <div>
      模型基础中具有此排名的帐户百分比。 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## 模型调整 {#model-tuning}

在“模型”(Model)选项卡中，单击“优化模型”(Tune Model)按钮。

![](assets/two.png)

有多个选项卡可供选择，允许进行深入自定义。

![](assets/tuning-page.png)

**指标类别**

<table> 
 <tbody> 
  <tr> 
   <td><strong>合规性</strong></td> 
   <td> 
    <div>
      认证、与法规遵从性相关的职位/招聘。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>操作</strong></td> 
   <td> 
    <div>
      与业务有关的职位/聘用。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>HR</strong></td> 
   <td> 
    <div>
      人力资源或工资单软件，与人力资源相关的职位/聘用。
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>工程</strong></td> 
   <td> 
    <div>
      技术、框架、与工程有关的职位/聘用。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>销售</strong></td> 
   <td> 
    <div>
      用于销售、销售相关职位/招聘的解决方案和软件。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>意图</strong></td> 
   <td> 
    <div>
      意图指标。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>IT</strong></td> 
   <td> 
    <div>
      硬件和软件解决方案、技术、IT相关职位/招聘。
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>金融</strong></td> 
   <td> 
    <div>
      财务软件、财务相关职位/招聘。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>营销</strong></td> 
   <td> 
    <div>
      营销技术和软件，与营销相关的职位/招聘。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>商业</strong></td> 
   <td> 
    <div>
      福布斯或Inc公司的上市或业务合作。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>客户体验和关系</strong></td> 
   <td> 
    <div>
      客户成功和客户关系职位/聘用。
    </div></td> 
  </tr> 
 </tbody> 
</table>

将鼠标悬停在工具提示上可查看每列的描述。

![](assets/tool-tip.png)

单击“添加ICP指示器”下拉列表，将其他指示器插入模型。

![](assets/add-icp.png)

选中“导出”框，可在“指定帐户详细信息”页上查看ICP指示器，并将所选ICP指示器用作 [已命名帐户过滤器](/help/marketo/product-docs/target-account-management/engage/account-filters.md).

![](assets/export.png)

>[!NOTE]
>
>比较方案指标列为 **指定帐户的成员** 过滤器和触发器。

指标权重是控制每个指标在模型中接收的重要性级别的指标。

![](assets/weightage.png)

单击“刷新模型”(Refresh Model)，以使这些更改生效。

![](assets/refresh-button.png)

完成对模型的调整（刷新后）后，返回“模型结果”(Model Results)选项卡并单击 **保存并应用排名**.

![](assets/ranks.png)
