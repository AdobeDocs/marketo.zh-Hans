---
unique-page-id: 4719306
description: 从Marketo同步 — Marketo文档 — 产品文档中隐藏Salesforce字段
title: 从Marketo同步中隐藏Salesforce字段
exl-id: 5d7229f0-43b0-4232-93ed-a9ca52ace401
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 0%

---

# 从Marketo同步{#hide-a-salesforce-field-from-the-marketo-sync}中隐藏Salesforce字段

>[!NOTE]
>
>**需要管理权限**

并非Salesforce中的每个字段都对Marketing有用。 您可以只包含需要的字段，从而优化同步性能。 下面介绍如何隐藏字段以阻止Marketo。

1. 单击您的名称菜单，然后选择&#x200B;**Setup**。

   ![](assets/image2015-6-30-15-3a11-3a23.png)

1. 在搜索栏中输入&#x200B;**用户档案**，然后单击&#x200B;**管理用户**&#x200B;下的&#x200B;**用户档案**。

   ![](assets/image2015-6-30-15-3a12-3a46.png)

1. 单击同步用户的用户档案。

   ![](assets/image2015-6-30-15-3a17-3a38.png)

1. 在&#x200B;**Field-Level Security**&#x200B;部分下，单击包含目标字段的对象旁边的&#x200B;**视图**。

   ![](assets/image2015-6-30-15-3a24-3a32.png)

1. 单击&#x200B;**编辑**。

   ![](assets/image2015-6-30-15-3a25-3a42.png)

1. 取消选中您要隐藏的字段旁边的&#x200B;**可见**&#x200B;复选框。 单击&#x200B;**保存**。

   ![](assets/image2015-6-30-15-3a27-3a16.png)

   >[!NOTE]
   >
   >如果您隐藏在Salesforce中的字段已与Marketo同步，则您还需要在Marketo中隐藏它，如果您不想使用它。

   就这样！ 下次同步完成后，您将不再在Marketo中看到此字段。

   >[!MORELIKETHIS]
   >
   >[隐藏和取消隐藏字段](/help/marketo/product-docs/administration/field-management/hide-and-unhide-a-field.md)
