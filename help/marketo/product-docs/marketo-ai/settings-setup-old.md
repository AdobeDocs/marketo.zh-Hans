---
description: 了解如何启用Marketo AI权限、配置组织规则以及管理集成和通知等设置。
title: 设置和设置
hide: true
hidefromtoc: true
exl-id: d6f37214-65b9-48c1-bf9f-d64b4eda87b9
source-git-commit: f26e46d4e6cb4855e5eb7f4d34a90f801e9654a7
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# 设置和设置 {#settings-setup}

了解如何启用权限并使用“设置”区域查看连接详细信息、定义组织规则以及设置集成和通知。

## 权限 {#permissions}

>[!IMPORTANT]
>
>在Marketo AI的Alpha阶段，默认情况下为以下角色启用&#x200B;_访问权限：管理员、Adobe产品管理员、营销用户、标准用户。_&#x200B;因此，对于想要访问的角色，您必须将其关闭，而不是为想要访问的角色打开它。

### 所有用户的访问权限 {#access-for-all}

如果您希望为上面列出的所有角色启用Marketo AI，则无需执行任何操作。

### 部分用户的访问权限 {#access-for-some}

如果要删除任何角色的访问权限，请执行以下步骤。

1. 在“我的Marketo”中，单击&#x200B;**管理员**，然后单击&#x200B;**用户和角色**。

   ![](assets/settings-setup-1.png)

1. 在&#x200B;_角色_&#x200B;选项卡中，选择所需的角色，然后单击&#x200B;**编辑角色**。

   ![](assets/settings-setup-2.png)

1. 向下滚动并&#x200B;_取消选中_**使用AI访问生成**&#x200B;复选框，然后单击&#x200B;**保存**。

   ![](assets/settings-setup-3.png)

对任何其他所需角色重复这些步骤。

### 自定义角色 {#custom-role}

您还可以选择[创建新角色](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role#create-a-role){target="_blank"}并自定义其权限，添加&#x200B;_使用AI访问Build_&#x200B;以及您需要的任何其他内容，并[将该角色](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user){target="_blank"}分配给特定用户。

<!-- ## Permissions {#permissions}

In order to access Marketo AI, Admins must first enable role permissions. 

1. In your My Marketo, click **Admin**, then **Users & Roles**.

   ![](assets/settings-setup-1.png)

1. In the _Roles_ tab, select the desired role and click **Edit Role**.

   ![](assets/settings-setup-2.png)

1. Scroll down and select the **Access Build with AI** checkbox and click **Save**.

   ![](assets/settings-setup-3.png)

-->

## 设置 {#settings}

1. 在“我的Marketo”中，单击&#x200B;**使用AI构建**&#x200B;图块。

   ![](assets/settings-setup-4.png)

1. 单击齿轮图标。

   ![](assets/settings-setup-5.png)

### 连接 {#connection}

此选项卡不包含可编辑的字段。 它会显示您的Munchkin ID和IMS组织等帐户信息。

![](assets/settings-setup-6.png)

### 组织规则 {#organizational-rules}

定义创建或修改Marketo资源时Marketo Engage AI遵循的组织准则和限制。

![](assets/settings-setup-7.png){width="800" zoomable="yes"}

>[!NOTE]
>
>规则对YAML frontmatter使用Markdown格式。 全局规则适用于所有工作区。 Workspace规则会覆盖全局设置。

### 集成（即将推出） {#integrations}

配置与外部服务和API的连接。

_此选项卡可能会显示在UI中，但尚未可用。 请返回查看更新_。

### 通知（即将推出） {#notifications}

管理警报首选项和通知渠道。

_此选项卡可能会显示在UI中，但尚未可用。 请返回查看更新_。
