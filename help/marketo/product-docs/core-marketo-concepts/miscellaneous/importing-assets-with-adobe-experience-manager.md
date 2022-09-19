---
unique-page-id: 37355768
description: 使用Adobe Experience Manager导入资产 — Marketo文档 — 产品文档
title: 使用Adobe Experience Manager导入资产
exl-id: 56ccf38f-3c99-4018-9989-719854e37a20
source-git-commit: 2b3a7867811ab2814a668eaa633057b35b7ce68d
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 0%

---

# 使用Adobe Experience Manager导入资产 {#importing-assets-with-adobe-experience-manager}

资产选择器允许Marketo客户访问、选择AEM资产，并将其导入Marketo的Design Studio。 **需要管理员权限**.

>[!AVAILABILITY]
>
>并非所有客户都购买了此功能。 有关详细信息，请联系您的客户成功经理。

>[!PREREQUISITES]
>
>确保已执行 [AEM配置](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/configuring-adobe-experience-manager-integration.md).

>[!IMPORTANT]
>
>目前，仅在Firefox中完全支持此功能。 Safari不支持此功能，并且根据您的SameSite Cookie设置，它可能无法在最新版本的Chrome中使用。

1. 单击 **Design Studio**.

   ![](assets/one-1.png)

1. 单击新建下拉菜单，然后选择 **从Adobe Experience Manager导入**.

   ![](assets/two-1.png)

1. 选择要将图像保存到的文件夹。

   ![](assets/three-1.png)

1. 登录到Adobe Experience Manager（如果尚未登录）。

   ![](assets/four-1.png)

1. 选择您的文件夹。 然后，单击缩略图以选择所需的图像（最多可选择10张）。 单击 **选择** 完成时。

   ![](assets/five.png)

   >[!NOTE]
   >
   >图像大小不能超过100MB。

1. 单击 **导入** 以完成该过程。

   ![](assets/six-1.png)

   就这样！ 单击 **关闭** 返回Design Studio的步骤。

   ![](assets/seven-1.png)

## 注意事项 {#things-to-note}

* Marketo当前支持Adobe Experience Manager版本6.4和6.5。

* 实例中的所有用户都将能够查看/访问您导入的图像。

* 图像不会自动更新。 如果您导入到Marketo Design Studio的图像在AEM中更新，则必须手动将其重新导入Marketo。
