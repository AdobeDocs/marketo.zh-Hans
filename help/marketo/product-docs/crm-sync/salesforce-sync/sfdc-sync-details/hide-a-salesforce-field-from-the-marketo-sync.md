---
unique-page-id: 4719306
description: 从Marketo同步中隐藏Salesforce字段 — Marketo文档 — 产品文档
title: 从Marketo同步中隐藏Salesforce字段
exl-id: 5d7229f0-43b0-4232-93ed-a9ca52ace401
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 1%

---

# 从Marketo同步中隐藏Salesforce字段 {#hide-a-salesforce-field-from-the-marketo-sync}

>[!NOTE]
>
>**需要管理员权限**

Salesforce并非每个字段都对Marketing有用。 您可以通过仅包含所需的字段来优化同步性能。 下面是隐藏字段以防Marketo Engage的方法。

1. 单击名称菜单，然后选择&#x200B;**[!UICONTROL 设置]**。

   ![](assets/image2015-6-30-15-3a11-3a23.png)

1. 在搜索栏中输入“配置文件”，然后单击&#x200B;**[!UICONTROL 管理用户]**&#x200B;下的&#x200B;**[!UICONTROL 配置文件]**。

   ![](assets/image2015-6-30-15-3a12-3a46.png)

1. 单击同步用户的配置文件。

   ![](assets/image2015-6-30-15-3a17-3a38.png)

1. 在&#x200B;**[!UICONTROL 字段级安全性]**&#x200B;部分下，单击包含目标字段的对象旁边的&#x200B;**[!UICONTROL 查看]**。

   ![](assets/image2015-6-30-15-3a24-3a32.png)

1. 单击&#x200B;**[!UICONTROL 编辑]**。

   ![](assets/image2015-6-30-15-3a25-3a42.png)

1. 取消选中要隐藏的字段旁边的&#x200B;**[!UICONTROL 可见]**&#x200B;复选框。 单击&#x200B;**[!UICONTROL 保存]**。

   ![](assets/image2015-6-30-15-3a27-3a16.png)

   >[!NOTE]
   >
   >如果您在Salesforce中隐藏的字段已与Marketo同步，则如果您不想使用它，也需要在Marketo中隐藏该字段。

   就是这样！ 下次同步完成后，您将不会再在Marketo中看到此字段。

   >[!MORELIKETHIS]
   >
   >[隐藏和取消隐藏字段](/help/marketo/product-docs/administration/field-management/hide-and-unhide-a-field.md){target="_blank"}
