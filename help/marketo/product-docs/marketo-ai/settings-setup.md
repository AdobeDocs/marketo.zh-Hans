---
description: 了解如何启用Marketo AI权限、配置组织规则以及管理集成和通知等设置。
title: 设置和设置
exl-id: faf642a1-25f0-4566-b35d-074b003835ed
source-git-commit: 7e869a7a66badbb274355a676d9950068bb8b68e
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 1%

---

# 设置和设置 {#settings-setup}

了解如何启用权限并使用“设置”区域查看连接详细信息、定义组织规则以及设置集成和通知。

>[!AVAILABILITY]
>
>此功能仅在有限范围内可用。 若要请求访问权限，请填写[此表单](https://forms.cloud.microsoft/Pages/ResponsePage.aspx?id=Wht7-jR7h0OUrtLBeN7O4Y-uSf63sAxCmWyqMJg8eMFUMVZSVExSNDA3T0I4SEcwRDFSVTBGWU01Uy4u&origin=QRCode){target="_blank"}。 确保准备好您的订阅Munchkin ID。

>[!PREREQUISITES]
>
>若要使用此功能，您必须首先同意[Core Gen-AI条款和补充条款](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"}。 有关详细信息，请与您的客户经理联系。

## 权限和角色 {#permission-and-role}

具有&#x200B;_访问Marketo人工智能_&#x200B;权限和&#x200B;_Marketo人工智能用户_&#x200B;角色，可让管理员更好地控制哪些用户可以访问&#x200B;**Marketo人工智能**&#x200B;功能。 权限在角色级别分配。 _Marketo AI用户_&#x200B;角色附带默认启用的&#x200B;_访问Marketo AI_&#x200B;权限。

>[!IMPORTANT]
>
>默认情况下，并非所有角色都启用&#x200B;_访问Marketo AI_&#x200B;权限。 有关详细信息，请参阅下表。

| 角色 | 默认状态 |
| --- | --- |
| 管理员 | 已启用 |
| Adobe产品管理员 | 已启用 |
| 营销用户 | 已禁用 |
| 标准用户 | 不可用 |
| Marketo AI用户 | 已启用 |
| 自定义角色 | 已禁用 |

### 访问Marketo AI权限 {#access-marketo-ai-permission}

按照以下步骤启用&#x200B;_访问Marketo AI_，以授予尚未启用它的角色资格。

1. 在“我的Marketo”中，单击&#x200B;**管理员**，然后单击&#x200B;**用户和角色**。

   ![](assets/settings-setup-1.png)

1. 在&#x200B;_角色_&#x200B;选项卡中，选择所需的角色，然后单击&#x200B;**编辑角色**。

   ![](assets/settings-setup-2.png)

1. 向下滚动并选中&#x200B;_访问Marketo AI_&#x200B;复选框，然后单击&#x200B;**保存**。

   ![](assets/settings-setup-3.png)

   >[!NOTE]
   >
   >您可以使用这些相同步骤通过&#x200B;**取消**&#x200B;选中&#x200B;_访问Marketo AI_&#x200B;复选框来删除权限。

### Marketo人工智能用户角色 {#marketo-ai-user-role}

按照以下步骤将特定用户分配给&#x200B;_Marketo AI用户_&#x200B;角色。

>[!NOTE]
>
>此角色&#x200B;**only**&#x200B;包含&#x200B;_访问Marketo AI_&#x200B;权限。

1. 在“我的Marketo”中，单击&#x200B;**管理员**，然后单击&#x200B;**用户和角色**。

   ![](assets/settings-setup-4.png)

1. 选择所需的用户并单击&#x200B;**编辑用户**。

   ![](assets/settings-setup-5.png)

1. 在&#x200B;_角色和工作区_&#x200B;中，选中&#x200B;_Marketo AI用户_&#x200B;复选框。 如果您有多个工作区，则可以在&#x200B;**+**&#x200B;签名下拉列表中指定哪些工作区具有访问权限。 完成后单击&#x200B;**保存**。

   ![](assets/settings-setup-6.png)

### 自定义角色 {#custom-role}

您还可以选择[创建新角色](https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role#create-a-role){target="_blank"}并自定义其权限，添加&#x200B;_访问Marketo AI_&#x200B;以及您需要的任何其他内容，并[将该角色](https://experienceleague.adobe.com/zh-hans/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user){target="_blank"}分配给特定用户。

## 设置 {#settings}

1. 在“我的Marketo”中，单击&#x200B;**Marketo AI**&#x200B;图块。

   ![](assets/settings-setup-7.png)

1. 单击齿轮图标。

   ![](assets/settings-setup-8.png)

### 连接 {#connection}

此选项卡不包含可编辑的字段。 它会显示您的Munchkin ID和IMS组织等帐户信息。

![](assets/settings-setup-9.png)

### 组织规则 {#organizational-rules}

定义创建或修改Marketo资源时Marketo Engage AI遵循的组织准则和限制。

![](assets/settings-setup-10.png){width="800" zoomable="yes"}

>[!NOTE]
>
>规则对YAML frontmatter使用Markdown格式。 全局规则适用于所有工作区。 Workspace规则会覆盖全局设置。

### 集成（即将推出） {#integrations}

配置与外部服务和API的连接。

_此选项卡可能会显示在UI中，但尚未可用。 请返回查看更新_。

### 通知（即将推出） {#notifications}

管理警报首选项和通知渠道。

_此选项卡可能会显示在UI中，但尚未可用。 请返回查看更新_。
