---
unique-page-id: 4719306
description: 从Salesforce同步中隐藏Marketo字段 — Marketo文档 — 产品文档
title: 从 Marketo 同步中隐藏 Salesforce 字段
exl-id: 5d7229f0-43b0-4232-93ed-a9ca52ace401
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 7%

---

# 从Marketo同步中隐藏[!DNL Salesforce]字段 {#hide-a-salesforce-field-from-the-marketo-sync}

>[!NOTE]
>
>**需要管理员权限**

Salesforce并非每个字段都对营销有用。 您可以通过仅包含所需的字段来优化同步性能。 下面是如何从Marketo Engage隐藏字段的。

1. 单击名称菜单，然后选择&#x200B;**[!UICONTROL Setup]**。

   ![](assets/image2015-6-30-15-3a11-3a23.png)

1. 在搜索栏中输入“配置文件”，然后单击&#x200B;**[!UICONTROL Profiles]**&#x200B;下的&#x200B;**[!UICONTROL Manage Users]**。

   ![](assets/image2015-6-30-15-3a12-3a46.png)

1. 单击同步用户的配置文件。

   ![](assets/image2015-6-30-15-3a17-3a38.png)

1. 在&#x200B;**[!UICONTROL Field-Level Security]**&#x200B;部分下，单击包含目标字段的对象旁边的&#x200B;**[!UICONTROL View]**。

   ![](assets/image2015-6-30-15-3a24-3a32.png)

1. 单击 **[!UICONTROL Edit]**。

   ![](assets/image2015-6-30-15-3a25-3a42.png)

1. 取消选中要隐藏的字段旁边的&#x200B;**[!UICONTROL Visible]**&#x200B;复选框。 单击 **[!UICONTROL Save]**。

   ![](assets/image2015-6-30-15-3a27-3a16.png)

   >[!NOTE]
   >
   >如果您在[!DNL Salesforce]中隐藏的字段已与Marketo同步，那么如果您不想使用它，您也将需要在Marketo中隐藏该字段。

   操作完成！下次同步完成后，您将不会再在Marketo中看到此字段。

   >[!MORELIKETHIS]
   >
   >[隐藏和取消隐藏字段](/help/marketo/product-docs/administration/field-management/hide-and-unhide-a-field.md){target="_blank"}
