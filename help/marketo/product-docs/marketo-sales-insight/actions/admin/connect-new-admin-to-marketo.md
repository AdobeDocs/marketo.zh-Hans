---
description: 将新管理员连接到Marketo - Marketo文档 — 产品文档
title: 将新管理员连接到Marketo
hide: true
hidefromtoc: true
exl-id: ef405bca-a29a-40fc-9efa-eccff5f45956
source-git-commit: 4055b121b416f3fa56abcfa21d370d148d3ab3c4
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 将新管理员连接到Marketo {#connect-new-admin-to-marketo}

如果其他管理员已连接到Marketo，则他们只需执行步骤1。

如果第二个管理员未以管理员身份连接到Marketo...

1. 主管理员需要从“设置”>“Marketo”>“用户访问”中，从Marketo中断开第二个管理员的连接。

1. 次管理员登录到其MSC帐户，转到“设置”>“Marketo”，然后单击 **连接**.

1. 现在，辅助用户以管理员身份连接到Marketo。

1. 主管理员现在可以登录并断开与Marketo的连接。

>[!NOTE]
>
>在用户A断开连接之前，只要用户B以管理员身份连接，其他用户就会保持连接。

## 更新Marketo连接 {#update-your-marketo-connection}

如果您决定删除设置Marketo集成的管理员，请查看本文以了解操作方法。

Marketo集成将绑定到Sales Connect/Actions管理员用户。 通常，是管理员，该管理员首先单击了Marketo连接页面上的“连接”按钮并建立了连接。

要删除建立Marketo连接的管理员，必须先由其他管理员用户建立新连接。 下面列出了为完成此操作需要完成的任务。

为简化说明，我们将以管理员A的身份，将当前连接的管理员称为Marketo，以及以管理员B的身份要与Admin建立新连接的管理员：

1. 管理员A（当前连接的管理员）将需要从管理员B（新管理员）中删除对与Marketo集成的访问权限。

1. 让管理员B（新管理员）建立与Marketo的新连接。

1. 断开管理员A（最初连接的管理员）的连接。

>[!NOTE]
>
>负责Marketo集成的原始管理员将看到一个“断开连接”选项，该选项在导航到Marketo集成页面时可单击。 其他管理员（尚未建立连接）将不会。 此外，已获得Marketo集成访问权限的管理员将无法单击连接，因此您必须先执行步骤以删除对集成的访问权限。

**从管理员B中删除Marketo访问权限**

管理员A（最初负责连接的管理员）应执行以下步骤。

1. 在Web应用程序中，单击齿轮图标，然后选择 **设置**.

1. 单击 **Marketo**.

1. 单击 **用户访问**.

1. 搜索要为其建立新Marketo连接的管理员。

1. 删除访问权限。

**为管理员B建立新连接**

这些步骤应由管理员B（新管理员）执行

1. 在Web应用程序中，单击齿轮图标，然后选择 **设置**.

1. 单击 **Marketo**.

1. 单击 **断开连接**.

**断开Marketo A集成**

这些步骤应由管理员A（最初连接的管理员）执行。

1. 在Web应用程序中，单击齿轮图标，然后选择 **设置**.

1. 单击 **Marketo**.

1. 单击 **断开连接**.

现在，新管理员已建立与Marketo的连接，并且原始管理员已断开连接，因此可以安全地从Sales Connect/Actions实例中删除最初连接的管理员。
