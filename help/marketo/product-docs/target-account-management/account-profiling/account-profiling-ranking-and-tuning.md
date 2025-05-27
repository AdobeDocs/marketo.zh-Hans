---
unique-page-id: 15695924
description: 帐户分析排名和调整 — Marketo文档 — 产品文档
title: 帐户分析排名和调整
exl-id: 9c5d0a03-0ebe-43cc-95ef-faab19a7f673
feature: Target Account Management
source-git-commit: 2f978d814f4cf2d4d2ca9ead0c1a3e5c15430520
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 1%

---

# 帐户分析排名和调整 {#account-profiling-ranking-and-tuning}

帐户分析标识您的理想客户配置文件(ICP)，根据ICP对数据库中的公司进行排名，并将ICP指示符数据添加到提升为指定帐户的帐户。

>[!IMPORTANT]
>
>从2025年开始，帐户分析不再适用于新用户。 它将继续用于现有用户。

## 模型结果 {#model-results}

结果将显示按级别划分的所有已知帐户。 A是最高等级，D是最低等级。

![](assets/results.png)

虽然可选，但我们仍建议您选中自动提升复选框，因为这将为您节省大量时间。 但是，如果您想查看每个帐户并[手动添加它们](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md#discover-crm-accounts)，只需取消选中该框即可。

<table> 
 <tbody> 
  <tr> 
   <td><strong>排名</strong></td> 
   <td> 
    <div>
      基于理想客户配置文件的客户排名。 A代表最佳匹配，D代表最小匹配。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>倾向</strong></td> 
   <td> 
    <div>
      与非比较方案为基础的账户选择相比，转换率的估计增加。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>帐户(%)</strong></td> 
   <td> 
    <div>
      模型输入中具有此排名的帐户的百分比。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>模型基准百分比</strong></td> 
   <td> 
    <div>
      具有此级别的模型基础中的帐户百分比。 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## 模型调整 {#model-tuning}

在“模型”选项卡中，单击“优化模型”按钮。

![](assets/two.png)

有几个选项卡可供选择，允许进行深入自定义。

![](assets/tuning-page.png)

**指标类别**

<table> 
 <tbody> 
  <tr> 
   <td><strong>合规性</strong></td> 
   <td> 
    <div>
      认证、合规性相关职位/聘用。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>操作</strong></td> 
   <td> 
    <div>
      业务相关职位/聘用。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>小时</strong></td> 
   <td> 
    <div>
      HR或工资单软件、与HR相关的职位/聘用。
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
      针对销售、销售相关职位/招聘的解决方案和软件。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>意图</strong></td> 
   <td> 
    <div>
      意图指示器。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>IT</strong></td> 
   <td> 
    <div>
      硬件和软件解决方案、技术、与IT相关的职位/聘用。
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>财务</strong></td> 
   <td> 
    <div>
      财务软件、财务相关职位/聘用。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>营销</strong></td> 
   <td> 
    <div>
      营销技术和软件、与营销相关的职位/聘用。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>商业</strong></td> 
   <td> 
    <div>
      福布斯或公司上市或商业合作。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>客户体验与关系</strong></td> 
   <td> 
    <div>
      客户成功和客户关系职位/聘用。
    </div></td> 
  </tr> 
 </tbody> 
</table>

将鼠标悬停在工具提示上可查看每列的说明。

![](assets/tool-tip.png)

单击添加ICP指示器下拉列表，将其他指示器插入到模型中。

![](assets/add-icp.png)

通过选中导出框，可在“指定帐户详细信息”页面上查看ICP指示器，并将选定的ICP指示器用作[指定帐户筛选器](/help/marketo/product-docs/target-account-management/engage/account-filters.md)中的约束。

![](assets/export.png)

>[!NOTE]
>
>ICP指示符作为约束包含在指定帐户&#x200B;**筛选器和触发器的**&#x200B;成员中。

指标权重是控制每个指标在模型中接收的重要性级别的内容。

![](assets/weightage.png)

单击“刷新模型”以使这些更改生效。

![](assets/refresh-button.png)

完成模型调整（刷新模型后）后，返回模型结果选项卡，然后单击&#x200B;**保存并应用排名**。

![](assets/ranks.png)
