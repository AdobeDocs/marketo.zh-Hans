---
unique-page-id: 37355600
description: 从MS Dynamics实例- Marketo Docs —— 产品文档中卸载MSI
title: 从MS Dynamics实例中卸载MSI
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---


# 从MS Dynamics实例中卸载MSI {#uninstall-msi-from-your-ms-dynamics-instance}

要从MS Dynamics实例卸载MSI，您需要在Marketo和MS Dynamics中执行步骤。

>[!PREREQUISITES]
>
>[禁用全局MS Dynamics同步](http://docs.marketo.com/x/TAA6Ag)

1. 在Marketo中，单击“管 **理员**”。

   ![](assets/one-1.png)

1. 单击 **销售分析**。

   ![](assets/six.png)

1. 单击 **编辑字段同步**。

   ![](assets/seven.png)

1. 选中“禁 **用同步** ”复选框，然 **后单击保存**。

   >[!NOTE]
   >
   >**提醒**
   >
   >
   >请确保在 [禁用字段同步之前禁用](http://docs.marketo.com/x/TAA6Ag) “全局MS Dynamics Sync”。

   ![](assets/eight.png)

## 在MS Dynamics实例中执行以下步骤： {#the-following-steps-take-place-in-your-ms-dynamics-instance}

1. 单击“ **高级设置**”。
1. 单击“ **解决方案**”。
1. 选择 **Marketo Sales Insight** ，然后单击删除图标。
1. 弹出“卸载解决方案”模式时，单击“确 **定”**。

   MS Dynamics解决方案通常需要大约20分钟才能完全卸载。 但是，如果您有一个大型MS Dynamics实例，则可能需要稍长一些。

   >[!NOTE]
   >
   >**提醒**
   >
   >
   >卸载MSI后，请记住打开全局MS Dynamics同步。

