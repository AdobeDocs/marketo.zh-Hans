---
description: 将列表发送到广告网络 — Marketo文档 — 产品文档
title: 将列表发送到广告网络
exl-id: d5c55df7-53c8-491a-9d79-ecf7c25cee08
source-git-commit: 5536b35d71506f11fdf32bf7149bf5c61174ab34
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# 将列表发送到广告网络 {#send-a-list-to-an-ad-network}

了解如何将静态列表发送到LinkedIn、Facebook或Google。

## 如何发送列表 {#how-to-send-a-list}

1. 在Marketo中，选择您的列表，单击 **列出操作** 下拉菜单，然后选择 **发送到广告网络**.

   ![](assets/send-a-list-to-an-ad-network-1.png)

1. 选择LinkedIn、Facebook或Google（其他选项当前不可用）。 在本例中，我们选择 **linkedIn**. 单击 **下一个**.

   ![](assets/send-a-list-to-an-ad-network-2.png)

1. 单击受众下拉列表，然后选择所需的受众。

   ![](assets/send-a-list-to-an-ad-network-3.png)

   >[!TIP]
   >
   >如果您需要检查，可以通过状态选项卡查看列表正在同步到的目标受众。

1. 选择所需的推送类型并单击 **更新**.

   ![](assets/send-a-list-to-an-ad-network-4.png)

   >[!NOTE]
   >
   >如果选择“启用连续受众同步”，则当Marketo实例中的列表发生更改时，Marketo会在选定的广告网络中保持该列表处于最新状态。 我们都加了 **和** 从受众中删除将其添加到静态列表或从静态列表中删除的人员。

1. 就这样！ 单击 **确定** 退出。

   ![](assets/send-a-list-to-an-ad-network-5.png)

## 常见问题解答 {#faq}

**单个静态列表是否可以与多个广告受众同步？**

不能，列表只能同步到单个目标受众。

**如果启用与现有广告受众的连续同步，是否会替换现有受众？**

不会，现有受众将会添加到中，而不是被替换。
