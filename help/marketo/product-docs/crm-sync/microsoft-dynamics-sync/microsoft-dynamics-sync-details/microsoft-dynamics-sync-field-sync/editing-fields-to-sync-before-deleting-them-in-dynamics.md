---
description: 在Dynamics中编辑要在删除字段之前进行同步的字段 — Marketo文档 — 产品文档
title: 在Dynamics中删除字段之前编辑要同步的字段
exl-id: 6fa9f6c0-c69d-478f-b333-13a5c910f577
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '208'
ht-degree: 0%

---

# 在Dynamics中删除字段之前编辑要同步的字段 {#editing-fields-to-sync-before-deleting-them-in-dynamics}

有时，您可能希望删除Dynamics中的字段。 Marketo Engage保留字段列表作为同步所依据的引用。 如果在同步打开时在Dynamics中删除某个字段，则同步可能会遇到错误。 在删除任何字段之前，请执行以下步骤。

1. 在Marketo中，单击 **[!UICONTROL 管理员]**.

   ![](assets/sync-before-deleting-them-in-dynamics-1.png)

1. 在集成下，单击 **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/sync-before-deleting-them-in-dynamics-2.png)

1. 单击 **[!UICONTROL 禁用同步]**.

   ![](assets/sync-before-deleting-them-in-dynamics-3.png)

1. 在浏览器的新选项卡中，登录到Dynamics并删除所需的字段。

1. 返回到Marketo中的Microsoft Dynamics下，单击 **[!UICONTROL 编辑]** “Step 2： Select Fields to Sync（步骤2：选择要同步的字段）”旁边。

   ![](assets/sync-before-deleting-them-in-dynamics-4.png)

1. 查看字段并单击 **[!UICONTROL 保存]**.

   ![](assets/sync-before-deleting-them-in-dynamics-5.png)

>[!CAUTION]
>
>点击 **[!UICONTROL 保存]** 需要保存更新的架构以进行同步，即使未进行任何更改也是如此。

>[!NOTE]
>
>如果在删除Dynamics中的字段之前未停止同步，则同步可能会遇到错误。 如果出现这种情况，同步将停止。 在恢复之前，Marketo管理员需要查看“选择要同步的字段”（如上所述），然后单击 **[!UICONTROL 保存]** 以便同步接受架构更改。

保存更改后，请记得启用同步！
