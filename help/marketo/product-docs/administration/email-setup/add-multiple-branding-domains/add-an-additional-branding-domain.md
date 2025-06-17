---
unique-page-id: 11377395
description: 添加其他品牌推广域 — Marketo文档 — 产品文档
title: 添加附加品牌策略域
exl-id: df6e5afe-dbb0-4fbe-bf06-79d92a91b986
feature: Email Setup
source-git-commit: dafac137a6c626794f3b9b2bfaa2fc2de9f2cb75
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 0%

---

# 添加附加品牌策略域 {#add-an-additional-branding-domain}

当您在单个Marketo实例中运行多个品牌并希望每个品牌都有自己的品牌跟踪链接时，可以添加额外的品牌推广域。

>[!PREREQUISITES]
>
>在添加其他品牌域之前，您必须[将通用跟踪链接](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md){target="_blank"}替换为品牌域。

1. 转到&#x200B;**[!UICONTROL Admin]**&#x200B;区域。

   ![](assets/add-an-additional-branding-domain-1.png)

1. 单击 **[!UICONTROL Email]**。

   ![](assets/add-an-additional-branding-domain-2.png)

1. 单击&#x200B;**[!UICONTROL Add]**&#x200B;可添加其他品牌策略域。

   ![](assets/add-an-additional-branding-domain-3.png)

1. 输入新品牌化域的名称，选择&#x200B;_生成主域_&#x200B;和/或&#x200B;_生成SSL证书_（均为可选），然后单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/add-an-additional-branding-domain-4.png)

>[!NOTE]
>
>* _设为主要域_：设为主要域，所有现有未发送电子邮件设为“默认”，所有新创建的电子邮件将默认设为主要域。 您可以[根据每封电子邮件](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/overwrite-primary-domain-for-emails.md){target="_blank"}覆盖此内容。
>
>* _生成SSL证书_：您可以通过创建域来创建安全套接字层(SSL)。 第一个跟踪域将启动可能需要几个小时的一次性基础设施设置。 完成后，您将收到通知，然后您可以设置第一个域。 要将SSL添加到现有域，请联系[Marketo支持](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}。

## 错误消息 {#error-messages}

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
    <td><i>已颁发SSL证书。</i></td>
    <td>此自定义域已存在SSL证书。 除非证书已过期或需要重新颁发，否则无需执行进一步操作。</td>
  </tr>
  <tr>
    <td><i>域未映射到默认域。</i></td>
    <td>自定义域未正确映射到默认域。 请验证域映射设置并确保DNS配置指向正确的默认域。</td>
  </tr>
  <tr>
    <td><i>Cloudflare设置已启动。 请稍后重试。</i></td>
    <td>为实例创建第一个跟踪域时，会在Cloudfare中进行一次性基础架构设置。 此消息表示设置已启动，最长可能需要三个小时。</td>
  </tr>
  <tr>
    <td><i>Cloudflare设置仍在进行中。 请稍后重试。</i></td>
    <td>请参阅上文</td>
  </tr>
  <tr>
    <td><i>由于意外错误，Cloudflare安装程序失败。 请联系客户支持。</i></td>
    <td>初始Cloudfare基础架构设置失败。 请联系<a href="https://nation.marketo.com/t5/support/ct-p/Support" target="_blank">Marketo支持</a>寻求帮助。</td>
  </tr>
</tbody></table>

## 注意事项 {#things-to-note}

* 将域的&#x200B;**DNS映射到Marketo Engage**：在UI中添加域之前，必须[将CNAME映射到Marketo提供的域](https://experienceleague.adobe.com/zh-hans/docs/marketo/using/getting-started/initial-setup/setup-steps#customize-your-landing-page-urls-with-a-cname){target="_blank"}。

* **自定义SSL**：如果您需要自定义SSL，请提交[支持票证](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}。 请勿使用自助复选框来创建SSL。

* **预先存在的SSL**：在添加域时，系统会检查预先存在的SSL，这些SSL可能在之前已手动创建。 如果您遇到此验证，请在不选择SSL创建的情况下创建您的域，我们将为您连接它们。 [联系支持人员](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}其他详细信息/选项。

* **首次跟踪域**：首次创建电子邮件跟踪链接域将需要[Marketo支持](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}的手动干预。 UI中允许在同一域下后续创建子域。

* **向现有域添加证书**：目前不支持向现有域添加证书。 对于预先存在的域，或者如果您未选中SSL证书框，则必须联系[Marketo支持](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}以添加证书。

* **编辑或删除现有域上的证书**：如果您需要更新或删除现有SSL，请联系[Marketo支持](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}。

* **删除域**：删除域此时不会自动删除SSL证书。 将在未来版本中解决此问题。

>[!MORELIKETHIS]
>
>[编辑您的默认品牌策略域](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md){target="_blank"}
