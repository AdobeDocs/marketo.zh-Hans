---
unique-page-id: 2359906
description: 管理Marketo用户 — Marketo文档 — 产品文档
title: 管理Marketo用户
exl-id: 40506d3c-a7cb-45fb-bc10-021bd0c70806
feature: Users and Roles
source-git-commit: ab4358ac1d3e1aa1d3733fa5191c5d59022bdf9f
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# 管理Marketo用户 {#managing-marketo-users}

>[!IMPORTANT]
>
>本文仅适用于拥有这些权限的用户 _非_ 使用 [具有Adobe身份的Marketo](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md){target="_blank"}. 如果您这样做，请按照中的步骤操作 [本文](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md){target="_blank"}.

## 创建用户 {#create-users}

1. 转到 **[!UICONTROL 管理员]** 区域。

   ![](assets/managing-marketo-users-1.png)

1. 单击 **[!UICONTROL 用户和角色]**.

   ![](assets/managing-marketo-users-2.png)

1. 单击 **[!UICONTROL 邀请新用户]**.

   ![](assets/managing-marketo-users-3.png)

1. 输入 **[!UICONTROL 电子邮件]**， **[!UICONTROL 名字]**、和 **[!UICONTROL 姓氏]**.

   ![](assets/managing-marketo-users-4.png)

1. （可选）输入邀请原因，然后在以下选项中选择到期日期： **[!UICONTROL 访问过期]** 使用日期选取器的字段。

   ![](assets/managing-marketo-users-5.png)

1. 单击 **[!UICONTROL 下一个]**.

   ![](assets/managing-marketo-users-6.png)

   >[!TIP]
   >
   >对于短期外部利益相关者或仅需要在短时间内访问Marketo的顾问而言，过期日期非常有用。

   >[!NOTE]
   >
   >到达到期日期时，用户会收到到期通知，并且其帐户将被锁定。

1. 选择 **[!UICONTROL 角色]** ，然后单击 **[!UICONTROL 下一个]**.

   ![](assets/managing-marketo-users-7.png)

1. 根据需要编辑邀请邮件。 单击 **send**.

   ![](assets/managing-marketo-users-8.png)

   >[!NOTE]
   >
   >电子邮件/登录名必须是唯一的；如果您已在沙盒实例中使用过它，则需要在生产中使用不同的电子邮件/登录名，反之亦然。

   ![](assets/managing-marketo-users-9.png)

   >[!NOTE]
   >
   >邀请会在添加新用户后三天过期。

新用户现在列在用户选项卡中，并将收到一封电子邮件，其中包含有关如何激活其帐户的说明。

## 删除用户 {#delete-users}

>[!NOTE]
>
>如果要删除的用户也是Dynamic Chat用户，则必须 [从Dynamic Chat中删除它们](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#remove-a-chat-user){target="_blank"} 在Marketo Engage中删除它们之前，请先在Admin Console中将其删除。

1. 转到 **[!UICONTROL 管理员]** 区域。

   ![](assets/managing-marketo-users-10.png)

1. 单击 **[!UICONTROL 用户和角色]**.

   ![](assets/managing-marketo-users-11.png)

1. 选择要删除的用户并单击 **[!UICONTROL 删除用户]**.

   ![](assets/managing-marketo-users-12.png)

1. 单击确认 **[!UICONTROL 确定]**.

   ![](assets/managing-marketo-users-13.png)

## 重置用户密码 {#reset-user-passwords}

1. 转到 **[!UICONTROL 管理员]** 区域。

   ![](assets/managing-marketo-users-14.png)

1. 单击 **[!UICONTROL 用户和角色]**.

   ![](assets/managing-marketo-users-15.png)

1. 选择用户并单击 **[!UICONTROL 重置密码]**.

   ![](assets/managing-marketo-users-16.png)

1. 单击 **[!UICONTROL 关闭]** 关闭提示。

   ![](assets/managing-marketo-users-17.png)

用户将收到一封包含密码重置说明的电子邮件。

>[!TIP]
>
>如果用户在其收件箱中看不到电子邮件，请要求他们检查其垃圾邮件文件夹。

## 更改权限和编辑用户信息 {#change-permissions-and-edit-user-information}

1. 转到 **[!UICONTROL 管理员]** 区域。

   ![](assets/managing-marketo-users-18.png)

1. 单击 **[!UICONTROL 用户和角色]**.

   ![](assets/managing-marketo-users-19.png)

1. 选择用户并单击 **[!UICONTROL 编辑用户]**.

   ![](assets/managing-marketo-users-20.png)

1. 您可以编辑用户信息并更改关联的角色。 单击&#x200B;**[!UICONTROL 保存]**。

   ![](assets/managing-marketo-users-21.png)

>[!CAUTION]
>
>如果您是Marketo中的唯一管理员，请确保不要删除自己的管理员权限。

>[!NOTE]
>
>如果邀请新用户担任管理员，或者删除管理员，则所有当前管理员都将收到电子邮件通知。

做得很棒！ 您现在知道如何创建用户、删除用户、重置用户密码以及编辑用户。
