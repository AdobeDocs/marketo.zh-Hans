---
description: 推送克隆 — Marketo文档 — 产品文档
title: 推送克隆
hide: true
hidefromtoc: true
source-git-commit: 58b9589e5364584c3b2f41dc1a32496a18574429
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 0%

---

# 推送克隆 {#push-clone}

此功能允许您以静态列表的形式将位于Adobe Experience Platform中的区段推送到Marketo。

>[!PREREQUISITES]
>
>* [创建API用户](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md) 在Marketo。
>* 然后，转到 **管理员** > **Launchpoint**. 查找您刚刚创建的角色的名称，然后单击 **查看详细信息**. 复制信息并将其保存在 **客户端ID** 和 **客户端密钥**，因为您将需要它才能使用此功能。
>* 在Marketo中，创建静态列表，或查找并选择一个已创建的列表。 你需要它的身份证。


1. 登录到 [Adobe Experience Platform](https://experience.adobe.com/).

   ![](assets/push-an-adobe-experience-platform-segment-1.png)

1. 单击网格图标，然后选择 **Experience Platform**.

   ![](assets/push-an-adobe-experience-platform-segment-2.png)

1. 在左侧导航栏中，单击 **目标**.

   ![](assets/push-an-adobe-experience-platform-segment-3.png)

1. 单击 **目录**.

   ![](assets/push-an-adobe-experience-platform-segment-4.png)

1. 查找Marketo Engage拼贴并单击 **激活区段**.

   ![](assets/push-an-adobe-experience-platform-segment-5.png)

1. 单击 **配置新目标**.

   ![](assets/push-an-adobe-experience-platform-segment-6.png)


1. 在“帐户类型”下，选择“现有帐户”或“新建帐户”单选按钮(在本例中，我们选择 **现有帐户**)。 单击选择帐户图标。

   ![](assets/push-an-adobe-experience-platform-segment-7.png)

   >[!NOTE]
   >
   >如果您选择“新帐户”，则可以通过以下路径找到您的Munchkin ID: **管理员** > **蒙奇金** (登录后，它也会成为Marketo URL的一部分)。 客户端ID/密钥您应当具有，以便遵循本文顶部的先决条件。

1. 选择目标帐户并单击 **选择**.

   ![](assets/push-an-adobe-experience-platform-segment-8.png)

1. 输入目标 **名称** 和可选描述。 单击“人员创建”下拉列表，然后选择“在Marketo中匹配现有的Marketo人员并创建缺失的人员” _或_ “仅匹配现有Marketo人员。” 在本例中，我们选择前者。

   ![](assets/push-an-adobe-experience-platform-segment-9.png)

   >[!NOTE]
   >
   >如果您选择“仅匹配现有Marketo人员”，则只需映射电子邮件和/或ECID，即可跳过步骤13-16。

1. 此部分是可选的。 单击 **创建** 跳过。

   ![](assets/push-an-adobe-experience-platform-segment-10.png)

1. 选择您创建的目标并单击 **下一个**.

   ![](assets/push-an-adobe-experience-platform-segment-11.png)

1. 选择要发送到Marketo的区段，然后单击 **下一个**.

   ![](assets/push-an-adobe-experience-platform-segment-12.png)

   >[!NOTE]
   >
   >如果在此处选择多个区段，则必须在区段计划选项卡中将每个区段映射到指定的静态列表。

1. 单击 **添加新映射**.

   ![](assets/push-an-adobe-experience-platform-segment-13.png)

1. 单击映射图标。

   ![](assets/push-an-adobe-experience-platform-segment-14.png)

1. 通过选择映射名字 **firstName** 单击 **选择**.

   ![](assets/push-an-adobe-experience-platform-segment-15.png)

1. 通过单击 **添加新映射** 重复步骤15，选择 **lastName** 然后 **companyName**.

   ![](assets/push-an-adobe-experience-platform-segment-16.png)

1. 现在该映射电子邮件地址了。 单击 **添加新映射** 再次。

   ![](assets/push-an-adobe-experience-platform-segment-17.png)

1. 单击映射图标。

   ![](assets/push-an-adobe-experience-platform-segment-18.png)

1. 单击“选择身份命名空间”单选按钮，然后选择  **电子邮件**，然后单击 **选择**.

   ![](assets/push-an-adobe-experience-platform-segment-19.png)

   >[!IMPORTANT]
   >
   >从映射电子邮件和/或ECID **身份命名空间** 选项卡是确保人员在Marketo中进行匹配时最重要的操作。 映射电子邮件将确保最高匹配率。

1. 现在该选择源字段了。 对于电子邮件，单击光标图标。

   ![](assets/push-an-adobe-experience-platform-segment-20.png)

1. 单击“选择身份命名空间”单选按钮，找到并选择 **电子邮件**，然后单击 **选择**.

   ![](assets/push-an-adobe-experience-platform-segment-21.png)

1. 要选择公司名称源字段，请单击其行中的光标图标。

   ![](assets/push-an-adobe-experience-platform-segment-22.png)

1. 保持选中“选择属性”(Select Attribute)单选按钮。 搜索“company”并选择 **companyName**，然后单击 **选择**.

   ![](assets/push-an-adobe-experience-platform-segment-23.png)

1. 通过单击每个的光标图标并重复步骤23两次来映射姓氏和名字的源字段，选择 **lastName** 然后 **firstName**.

   ![](assets/push-an-adobe-experience-platform-segment-24.png)

1. 单击 **下一个**.

   ![](assets/push-an-adobe-experience-platform-segment-25.png)

1. 您现在需要列表的ID。 单击浏览器中已打开Marketo静态列表的选项卡（或打开一个新选项卡并选择所需的静态列表）。

   ![](assets/push-an-adobe-experience-platform-segment-26.png)

   >[!NOTE]
   >
   >为获得最佳结果，请使用空的Marketo Engage列表。

1. 突出显示并复制URL末尾的列表ID。

   ![](assets/push-an-adobe-experience-platform-segment-27.png)

1. 在映射ID下粘贴您刚才复制的ID，然后单击 **下一个**.

   ![](assets/push-an-adobe-experience-platform-segment-28.png)

1. 单击 **完成**.

   ![](assets/push-an-adobe-experience-platform-segment-29.png)
