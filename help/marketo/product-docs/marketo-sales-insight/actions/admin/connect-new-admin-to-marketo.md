---
description: 将新管理员连接到Marketo - Marketo文档 — 产品文档
title: 将新管理员连接到Marketo
exl-id: ef405bca-a29a-40fc-9efa-eccff5f45956
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# 将新管理员连接到Marketo {#connect-new-admin-to-marketo}

如果其他管理员已连接到Marketo，则他们只需执行步骤1。

如果第二个管理员未作为管理员连接到Marketo...

1. 主要管理员需要从“设置”>“Marketo”>“用户访问”断开第二个管理员与Marketo的连接。

1. 辅助管理员登录到其MSC帐户，转到设置> Marketo，然后单击 **连接**.

1. 现在，辅助用户以管理员身份连接到Marketo。

1. 主要管理员现在可以登录并从Marketo断开自身连接。

>[!NOTE]
>
>在用户A断开连接之前，只要用户B以管理员身份连接，其他用户就会保持连接。

## 更新您的Marketo连接 {#update-your-marketo-connection}

如果您决定要删除设置Marketo集成的管理员，请参阅本文以了解如何操作。

Marketo集成将绑定到Sales Connect/Actions管理员用户。 通常，这是首先单击Marketo连接页面上的“连接”按钮并建立连接的管理员。

要删除建立Marketo连接的管理员，必须首先由其他管理员用户建立新连接。 我们列出了完成此操作需要完成的以下任务。

为了简化说明，我们会将当前连接的管理员称为管理员A，而将您要与Marketo建立新连接的管理员称为管理员B：

1. 管理员A（当前连接的管理员）需要从管理员B（新管理员）中删除对Marketo集成的访问权限。

1. 让管理员B（新管理员）建立与Marketo的新连接。

1. 断开Admin A（最初连接Admin）的连接。

>[!NOTE]
>
>负责Marketo集成的原始管理员将看到“断开连接”选项，在导航到Marketo集成页面时，可单击该选项。 其他管理员（尚未建立连接）则不会。 此外，已被授予Marketo集成访问权限的管理员将无法单击连接，这就是为什么您必须先按照步骤删除对集成的访问权限。

**从管理员B中删除Marketo访问权限**

管理员A（最初负责连接的管理员）应遵循这些步骤。

1. 在Web应用程序中，单击齿轮图标并选择 **设置**.

1. 单击 **Marketo**.

1. 单击 **用户访问**.

1. 搜索要为其建立新Marketo连接的管理员。

1. 删除访问权限。

**为管理员B建立新连接**

管理员B（新管理员）应遵循这些步骤

1. 在Web应用程序中，单击齿轮图标并选择 **设置**.

1. 单击 **Marketo**.

1. 单击 **断开连接**.

**断开与Admin A的Marketo集成**

管理员A（最初连接的管理员）应执行这些步骤。

1. 在Web应用程序中，单击齿轮图标并选择 **设置**.

1. 单击 **Marketo**.

1. 单击 **断开连接**.

现在，新的管理员已建立了与Marketo的连接，并且原始管理员已断开，可以从Sales Connect/Actions实例中安全地删除最初连接的管理员。
