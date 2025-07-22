---
unique-page-id: 15695924
description: 帐户分析排名和调整 — Marketo文档 — 产品文档
title: 帐户分析排名和调整
exl-id: 9c5d0a03-0ebe-43cc-95ef-faab19a7f673
feature: Target Account Management
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 1%

---

# 帐户分析排名和调整 {#account-profiling-ranking-and-tuning}

帐户分析标识您的理想客户配置文件(ICP)，根据ICP对数据库中的公司进行排名，并将ICP指示符数据添加到提升为[!UICONTROL Named Accounts]的帐户。

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
   <td><strong><span class="uicontrol">排名</span></strong></td> 
   <td> 
    <div>
      基于理想客户配置文件的客户排名。 A代表最佳匹配，D代表最小匹配。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong><span class="uicontrol">倾向</span></strong></td> 
   <td> 
    <div>
      与非比较方案为基础的账户选择相比，转换率的估计增加。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong><span class="uicontrol">帐户(%)</span></strong></td> 
   <td> 
    <div>
      模型输入中具有此排名的帐户的百分比。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong><span class="uicontrol">模型基准百分比</span></strong></td> 
   <td> 
    <div>
      具有此级别的模型基础中的帐户百分比。 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## 模型调整 {#model-tuning}

在“模型”选项卡中，单击&#x200B;**[!UICONTROL Tune Model]**&#x200B;按钮。

![](assets/two.png)

有几个选项卡可供选择，允许进行深入自定义。

![](assets/tuning-page.png)

**指标类别**

<table> 
 <tbody> 
  <tr> 
   <td><strong><span class="uicontrol">合规性</span></strong></td> 
   <td> 
    <div>
      认证、合规性相关职位/聘用。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong><span class="uicontrol">操作</span></strong></td> 
   <td> 
    <div>
      业务相关职位/聘用。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong><span class="uicontrol">小时</span></strong></td> 
   <td> 
    <div>
      HR或工资单软件、与HR相关的职位/聘用。
    </div></td> 
  </tr> 
  <tr> 
   <td><strong><span class="uicontrol">工程</span></strong></td> 
   <td> 
    <div>
      技术、框架、与工程有关的职位/聘用。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong><span class="uicontrol">销售</span></strong></td> 
   <td> 
    <div>
      针对销售、销售相关职位/招聘的解决方案和软件。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong><span class="uicontrol">意图</span></strong></td> 
   <td> 
    <div>
      意图指示器。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong><span class="uicontrol">IT</span></strong></td> 
   <td> 
    <div>
      硬件和软件解决方案、技术、与IT相关的职位/聘用。
    </div></td> 
  </tr> 
  <tr> 
   <td><strong><span class="uicontrol">财务</span></strong></td> 
   <td> 
    <div>
      财务软件、财务相关职位/聘用。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong><span class="uicontrol">营销</span></strong></td> 
   <td> 
    <div>
      营销技术和软件、与营销相关的职位/聘用。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong><span class="uicontrol">商业</span></strong></td> 
   <td> 
    <div>
      福布斯或公司上市或商业合作。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong><span class="uicontrol">客户体验与关系</span></strong></td> 
   <td> 
    <div>
      客户成功和客户关系职位/聘用。
    </div></td> 
  </tr> 
 </tbody> 
</table>

将鼠标悬停在工具提示上可查看每列的说明。

![](assets/tool-tip.png)

单击[!UICONTROL Add ICP Indicator]下拉菜单将其他指示器插入到模型中。

![](assets/add-icp.png)

选中[!UICONTROL Export]框允许您在[!UICONTROL Named Account]详细信息页面上查看ICP指示器，并将选定的ICP指示器用作[命名帐户筛选器](/help/marketo/product-docs/target-account-management/engage/account-filters.md)中的约束。

![](assets/export.png)

>[!NOTE]
>
>ICP指示器作为约束包含在&#x200B;**[!UICONTROL Member of Named Account]**&#x200B;筛选器和触发器中。

[!UICONTROL Indicator Weightage]控制每个指标在您的模型中接收的重要性级别。

![](assets/weightage.png)

单击&#x200B;**[!UICONTROL Refresh Model]**&#x200B;以使这些更改生效。

![](assets/refresh-button.png)

完成模型调整（刷新模型后）后，返回模型结果选项卡并单击&#x200B;**[!UICONTROL Save & Apply Ranks]**。

![](assets/ranks.png)
