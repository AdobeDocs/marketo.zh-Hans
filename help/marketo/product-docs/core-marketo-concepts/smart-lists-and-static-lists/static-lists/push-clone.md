---
description: 推送克隆 — Marketo文档 — 产品文档
title: 推送克隆
hide: true
hidefromtoc: true
source-git-commit: 8920bc525075923b32e7330da20debb7b8f47b06
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 推送克隆 {#push-clone}

此功能允许您以静态列表的形式将位于Adobe Experience Platform中的区段推送到Marketo。

>[!PREREQUISITES]
>
>* [创建API用户](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md) 在Marketo。
>* 然后，转到 **管理员** > **Launchpoint**. 查找您刚刚创建的角色的名称，然后单击 **查看详细信息**. 复制信息并将其保存在 **客户端ID** 和 **客户端密钥**，因为您将需要它才能使用此功能。


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

1. 选择目标帐户并单击 **选择**.

   ![](assets/push-an-adobe-experience-platform-segment-8.png)

接下来，您将必须选择是仅匹配现有Marketo人员，还是匹配现有Marketo人员并在Marketo中创建缺失的人员。 下面是概述如何执行每项操作的部分。

## 在Marketo中匹配现有Marketo人员并创建缺失人员 {#match-existing-marketo-people-create-missing-people}

执行上面的步骤1-8后……

1. 输入目标 **名称** 和可选描述。 单击“人员创建”下拉列表，然后选择 **在Marketo中匹配现有Marketo人员并创建缺失人员**.

   ![](assets/push-an-adobe-experience-platform-segment-9.png)

1. 此部分是可选的。 单击 **创建** 跳过。

   ![](assets/push-an-adobe-experience-platform-segment-10.png)

1. 选择您创建的目标并单击 **下一个**.

   ![](assets/push-an-adobe-experience-platform-segment-11.png)

1. 选择要发送到Marketo的区段，然后单击 **下一个**.

   ![](assets/push-an-adobe-experience-platform-segment-12.png)

1. 单击 **添加新映射**.

   ![](assets/push-an-adobe-experience-platform-segment-13.png)

1. 单击映射图标。

   ![](assets/push-an-adobe-experience-platform-segment-14.png)

1. 通过选择映射名字 **firstName** 单击 **选择**.

   ![](assets/push-an-adobe-experience-platform-segment-15.png)

1. 通过单击 **添加新映射** 再次重复步骤7，选择lastName，然后选择companyName。

   ![](assets/push-an-adobe-experience-platform-segment-16.png)

1. 现在该映射电子邮件地址了。 单击 **添加新映射** 再次。

   ![](assets/push-an-adobe-experience-platform-segment-17.png)

1. 单击映射图标。

   ![](assets/push-an-adobe-experience-platform-segment-18.png)

1. 单击“选择身份命名空间”单选按钮，然后选择  **电子邮件**，然后单击 **选择**.

   ![](assets/push-an-adobe-experience-platform-segment-19.png)

1. 现在该选择源字段了。 对于电子邮件，单击光标图标。

   ![](assets/push-an-adobe-experience-platform-segment-20.png)

1. 单击“选择身份命名空间”单选按钮，找到并选择 **电子邮件**，然后单击 **选择**.

   ![](assets/push-an-adobe-experience-platform-segment-21.png)

莫里埃

## 仅匹配现有Marketo人员 {#match-existing-marketo-people-only}

>[!NOTE]
>
>标识用于在Marketo中查找匹配项。 如果找到匹配项，则会将人员添加到静态列表。 如果未找到匹配项，则会删除这些人员(即，未在Marketo中创建)。

1. _在Marketo_、创建静态列表，或查找并选择已创建的列表。 复制URL末尾的映射ID。

PICC

>[!NOTE]
>
>为获得最佳结果，请确保您在Marketo中引用的列表为空。

1. 返回Adobe Experience Platform，输入您刚才复制的ID。 选择开始日期。 在选定的结束日期之前，用户将持续同步。 对于无限同步，请将结束日期留空。 单击 **下一个** 完成时。

PICC

1. 确认更改并单击 **完成**.

PICC
