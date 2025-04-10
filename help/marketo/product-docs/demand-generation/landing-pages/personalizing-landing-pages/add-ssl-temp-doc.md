---
description: 将SSL添加到登陆页面 — Marketo文档 — 产品文档
title: 将SSL添加到登陆页面
hide: true
hidefromtoc: true
feature: Landing Pages
exl-id: 00ec2d91-3d4f-4671-af9d-9750c1642d40
source-git-commit: d20a560d3ef0a76081787c962e2e9c7276caf5cf
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# 将SSL添加到登陆页面 {#add-ssl-to-your-landing-pages}

SSL（安全套接字层）加密允许您确保Marketo Engage实例的所有登陆页面安全。

在填写Web表单或访问Marketo Engage托管的登陆页时，默认情况下，信息会通过非安全协议(HTTP)发送。 根据贵公司的策略，您可能希望保护通过(HTTPS)提交到Marketo的信息。 例如，当您访问`http://info.mydomain.com/`时，它现在将为`https://info.mydomain.com/`。

默认情况下，Marketo Engage会通过非安全HTTP协议跟踪“访问的网页”和“单击网页上的链接”。 如果您希望使用自己的证书来保护跟踪链接，则需要让Marketo构建单独的非共享服务器来启用它。 要确保联系人与您交互的各个方面的安全，通常意味着同时保护登陆页面和跟踪链接。

## 启用SSL认证 {#enable-ssl-certification}

自动为您在登陆页面规则中创建的所有域别名添加SSL。

1. 转到&#x200B;**管理员**&#x200B;区域。

   ![](assets/add-ssl-to-your-landing-pages-1.png)

1. 从树中选择&#x200B;**登陆页面**。 在&#x200B;**规则**&#x200B;选项卡中，单击&#x200B;**新建**&#x200B;下拉列表，然后选择&#x200B;**新建域别名**。

   ![](assets/add-ssl-to-your-landing-pages-2.png)

1. 输入您的&#x200B;_域别名_&#x200B;和&#x200B;_默认页面_。 选中&#x200B;**生成SSL证书**&#x200B;复选框。 完成后单击&#x200B;**创建**。

   ![](assets/add-ssl-to-your-landing-pages-3.png)

这会自动为此域添加SSL证书。

## 为默认域启用SSL {#enable-ssl-default-domain}

请按照以下步骤为默认域启用SSL。

1. 仍在&#x200B;**管理员**&#x200B;部分中，选择&#x200B;**登陆页面**。 单击&#x200B;_设置_&#x200B;旁边的橙色&#x200B;**编辑**&#x200B;按钮。

   ![](assets/add-ssl-to-your-landing-pages-4.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >如果需要，您还可以在此处修改域名（需要有效的域）。

1. 选中“生成SSL证书”复选框，然后单击保存。

   ![](assets/add-ssl-to-your-landing-pages-5.png)

>[!NOTE]
>
>* 列表中的“SSL证书”列显示在此功能发布后创建的所有域别名的证书状态(DATE)。 如果您通过Marketo支持为域启用了SSL，则该证书将继续存在，但不会显示在表中。 此表仅反映使用本文中的步骤添加的域的SSL证书。
>
>* SSL可能最多需要3分钟才能处于“就绪”状态。 必须刷新页面才能显示更改。
