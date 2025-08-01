---
unique-page-id: 2359828
description: 将SSL添加到登陆页面 — Marketo文档 — 产品文档
title: 将SSL添加到登陆页面
exl-id: 8271d9fe-0575-430c-97c7-407e4b78cf1d
feature: Landing Pages
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 0%

---

# 将SSL添加到登陆页面 {#add-ssl-to-your-landing-pages}

SSL（安全套接字层）加密允许您确保Marketo Engage实例的所有登陆页面安全。

在填写Web表单或访问Marketo Engage托管的登陆页时，默认情况下，信息会通过非安全协议(HTTP)发送。 根据贵公司的策略，您可能希望保护通过(HTTPS)提交到Marketo的信息。 例如，当您访问`http://info.mydomain.com/`时，它现在将为`https://info.mydomain.com/`。

默认情况下，Marketo Engage会通过非安全HTTP协议跟踪“访问的网页”和“单击网页上的链接”。 如果您希望使用自己的证书来保护跟踪链接，则需要让Marketo构建单独的非共享服务器来启用它。 要确保联系人与您交互的各个方面的安全，通常意味着同时保护登陆页面和跟踪链接。

>[!IMPORTANT]
>
>在添加SSL之前，请务必查看您的合同，以了解允许添加的域总数。 否则，您可能需要支付相关费用。 如果找不到相关信息，请联系Adobe客户团队（您的客户经理）以了解详细信息。

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

1. 仍在&#x200B;**管理员**&#x200B;部分中，选择&#x200B;**登陆页面**。 单击&#x200B;**设置**&#x200B;旁边的橙色&#x200B;_编辑_&#x200B;按钮。

   ![](assets/add-ssl-to-your-landing-pages-4.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >如果需要，您还可以在此处修改域名（需要有效的域）。

1. 选中“生成SSL证书”复选框，然后单击保存。

   ![](assets/add-ssl-to-your-landing-pages-5.png)

>[!NOTE]
>
>* 列表中的“SSL证书”列显示在发布此功能后创建的所有域别名的证书状态（2025年4月25日）。 如果您通过Marketo支持为域启用了SSL，则该证书将继续存在，但不会显示在表中。 此表仅反映使用本文中的步骤添加的域的SSL证书。
>
>* SSL可能最多需要3分钟才能处于“就绪”状态。 必须刷新页面才能显示更改。

## 错误消息 {#error-messages}

在下方，您将找到可能收到的错误消息及其定义。

<table><thead>
  <tr>
    <th>错误</th>
    <th>详细信息</th>
  </tr></thead>
<tbody>
  <tr>
    <td><i>创建域时遇到意外错误。 请联系支持人员以获取帮助。</i></td>
    <td>发生意外错误。 请收集日志和错误详细信息，并将问题升级至<a href="https://nation.marketo.com/t5/support/ct-p/Support" target="_blank">Marketo支持</a>。</td>
  </tr>
  <tr>
    <td><i>未找到默认域。 请联系支持人员以获取帮助。</i></td>
    <td>尝试查找默认域时出现问题。 请联系支持部门以便他们进行调查。</td>
  </tr>
  <tr>
    <td><i>已颁发SSL证书。</i></td>
    <td>此自定义域已存在SSL证书。 除非证书已过期或需要重新颁发，否则无需执行进一步操作。</td>
  </tr>
  <tr>
    <td><i>域未映射到默认域。</i></td>
    <td>自定义域未正确映射到默认域。 请验证域映射设置并确保DNS配置指向正确的默认域。</td>
  </tr>
  <tr>
    <td><i>域已存在。</i></td>
    <td>具有相同名称的域已存在。</td>
  </tr>
</tbody></table>

## 注意事项 {#things-to-note}

* 将域的&#x200B;**DNS映射到Marketo Engage**：在UI中添加域之前，必须[将CNAME映射到Marketo提供的域](https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/initial-setup/setup-steps#customize-your-landing-page-urls-with-a-cname){target="_blank"}。

* **自定义SSL**：如果您需要自定义SSL，请提交[支持票证](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}。 请勿使用自助复选框来创建SSL。

* **预先存在的SSL**：在添加域时，系统会检查预先存在的SSL，这些SSL可能在之前已手动创建。 如果您遇到此验证，请在不选择SSL创建的情况下创建您的域，我们将为您连接它们。 [联系支持人员](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}其他详细信息/选项。

* **向现有域添加证书**：目前不支持向现有域添加证书。 对于预先存在的域，或者如果您未选中SSL证书框，则必须联系[Marketo支持](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}以添加证书。

* **删除域**：删除域会自动删除SSL证书。
