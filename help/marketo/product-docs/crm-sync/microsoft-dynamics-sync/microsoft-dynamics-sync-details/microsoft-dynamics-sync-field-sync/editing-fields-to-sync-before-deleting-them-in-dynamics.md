---
description: 在Dynamics中编辑要在删除字段之前进行同步的字段 — Marketo文档 — 产品文档
title: 在 Dynamics 中删除字段之前先编辑要同步的字段
exl-id: 6fa9f6c0-c69d-478f-b333-13a5c910f577
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 5%

---

# 在[!DNL Dynamics]中删除字段之前正在编辑要同步的字段 {#editing-fields-to-sync-before-deleting-them-in-dynamics}

有时您可能希望删除[!DNL Dynamics]中的字段。 Marketo保留字段列表作为同步所依据的引用。 如果在同步打开时在[!DNL Dynamics]中删除字段，则同步可能会遇到错误。 在删除任何字段之前，请执行以下步骤。

1. 在Marketo中，单击&#x200B;**[!UICONTROL Admin]**。

   ![](assets/sync-before-deleting-them-in-dynamics-1.png)

1. 在[!UICONTROL Integration]下，单击&#x200B;**[!UICONTROL Microsoft Dynamics]**。

   ![](assets/sync-before-deleting-them-in-dynamics-2.png)

1. 单击 **[!UICONTROL Disable Sync]**。

   ![](assets/sync-before-deleting-them-in-dynamics-3.png)

1. 在浏览器的新选项卡中，登录到[!DNL Dynamics]并删除所需的字段。

1. 返回Marketo中的[!DNL Microsoft Dynamics]下，单击“**[!UICONTROL Edit]**”旁边的[!UICONTROL Step 2: Select Fields to Sync]。

   ![](assets/sync-before-deleting-them-in-dynamics-4.png)

1. 查看字段并单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/sync-before-deleting-them-in-dynamics-5.png)

>[!CAUTION]
>
>需要单击&#x200B;**[!UICONTROL Save]**&#x200B;以保存更新的架构以进行同步，即使未进行任何更改也是如此。

>[!NOTE]
>
>如果在删除[!DNL Dynamics]中的字段之前未停止同步，则同步可能会遇到错误。 如果出现这种情况，同步将停止。 在恢复之前，Marketo管理员需要查看“[!UICONTROL Select Fields to Sync]”（如上所述）并单击&#x200B;**[!UICONTROL Save]**，以便同步接受架构更改。

保存更改后，请记得启用同步！
