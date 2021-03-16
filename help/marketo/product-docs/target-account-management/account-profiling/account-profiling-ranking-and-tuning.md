---
unique-page-id: 15695924
description: 帐户分析排名和调整 — Marketo Docs — 产品文档
title: 帐户分析排名和调整
translation-type: tm+mt
source-git-commit: 9f88e7cebc5e9d0d4491d65d332ccfdd9a31c395
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 0%

---


# 帐户分析排名和调整{#account-profiling-ranking-and-tuning}

“帐户配置”可确定您的理想客户用户档案(ICP)，根据ICP对数据库中的公司进行排名，并将ICP指标数据添加到作为指定帐户提升的帐户。

## 模型结果{#model-results}

结果显示按级别划分的所有已知帐户。 A是最高等级，D是最低。

![](assets/results.png)

虽然可选，但我们建议选中自动提升复选框，因为这将为您节省大量时间。 但是，如果您希望查看每个帐户并手动添加[，只需将该框保留为未选中状态。](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md#discover-crm-accounts)

<table> 
 <tbody> 
  <tr> 
   <td><strong>排名</strong></td> 
   <td> 
    <div>
      基于理想客户用户档案的帐户排名。 A最合适，D最不合适。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>倾向</strong></td> 
   <td> 
    <div>
      与非基于比较方案的账户选择相比，转化率估计增加。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>帐户(%)</strong></td> 
   <td> 
    <div>
      具有此排名的模型输入中帐户的百分比。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>模型基础的%</strong></td> 
   <td> 
    <div>
      模型基础中具有此排名的帐户的百分比。 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## 模型调整{#model-tuning}

在“模型”(Model)选项卡中，单击“调整模型”(Tune Model)按钮。

![](assets/two.png)

有多个选项卡可供选择，可进行深入自定义。

![](assets/tuning-page.png)

**指示类别**

<table> 
 <tbody> 
  <tr> 
   <td><strong>合规性</strong></td> 
   <td> 
    <div>
      认证、合规相关职位/招聘。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>操作</strong></td> 
   <td> 
    <div>
      与运营相关的职位/聘用。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>HR</strong></td> 
   <td> 
    <div>
      HR或工资单软件，与HR相关的职位/聘用。
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>工程</strong></td> 
   <td> 
    <div>
      技术、框架、与工程有关的职位/雇用。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>销售</strong></td> 
   <td> 
    <div>
      用于销售、销售相关职位/雇佣的解决方案和软件。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>用途</strong></td> 
   <td> 
    <div>
      意图指示器。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>IT</strong></td> 
   <td> 
    <div>
      硬件和软件解决方案、技术、IT相关职位/雇佣。
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>金融</strong></td> 
   <td> 
    <div>
      财务软件、财务相关职位/雇佣。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>营销</strong></td> 
   <td> 
    <div>
      营销技术和软件、与营销相关的职位/雇佣。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>商业</strong></td> 
   <td> 
    <div>
      福布斯或Inc上市或与企业建立合作关系。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>客户体验与关系</strong></td> 
   <td> 
    <div>
      客户成功和客户关系职位/雇佣。
    </div></td> 
  </tr> 
 </tbody> 
</table>

将鼠标悬停在工具提示上，可查看每列的说明。

![](assets/tool-tip.png)

单击“添加ICP指示器”下拉框，将其他指示器插入模型。

![](assets/add-icp.png)

选中“导出”框可让您在“指定帐户详细信息”页上查看ICP指示器，并将选定的ICP指示器用作[指定帐户过滤器](/help/marketo/product-docs/target-account-management/engage/account-filters.md)中的约束。

![](assets/export.png)

>[!NOTE]
>
>ICP指示符作为约束包含在&#x200B;**指定帐户成员**&#x200B;过滤器和触发器中。

指标权重是控制模型中每个指标接收的重要性级别的指标。

![](assets/weightage.png)

单击“刷新模型”(Refresh Model)，以使这些更改生效。

![](assets/refresh-button.png)

完成模型调整（刷新模型后）后，返回“模型结果”选项卡，单击&#x200B;**保存并应用排名**。

![](assets/ranks.png)
