---
unique-page-id: 11377395
description: 添加其他品牌推广域 — Marketo文档 — 产品文档
title: 添加附加品牌域名
exl-id: df6e5afe-dbb0-4fbe-bf06-79d92a91b986
feature: Email Setup
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 3%

---

# 添加附加品牌域名 {#add-an-additional-branding-domain}

当您在单个Marketo实例中运行多个品牌并希望每个品牌都有自己的品牌跟踪链接时，可以添加额外的品牌推广域。

>[!PREREQUISITES]
>
>在添加其他品牌域之前，您必须[将通用跟踪链接](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md){target="_blank"}替换为品牌域。

1. 进入 **[!UICONTROL Admin]** 区域。

   ![](assets/add-an-additional-branding-domain-1.png)

1. 单击 **[!UICONTROL Email]**。

   ![](assets/add-an-additional-branding-domain-2.png)

1. 单击&#x200B;**[!UICONTROL Add]**&#x200B;可添加其他品牌策略域。

   ![](assets/add-an-additional-branding-domain-3.png){width="600"}

1. 输入新品牌化域的名称，选择&#x200B;_生成主域_&#x200B;和/或&#x200B;_生成SSL证书_（均为可选），然后单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/add-an-additional-branding-domain-4.png)

>[!NOTE]
>
>* _设为主要域_：设为主要域，所有现有未发送电子邮件设为“默认”，所有新创建的电子邮件将默认设为主要域。 您可以[根据每封电子邮件](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/overwrite-primary-domain-for-emails.md){target="_blank"}覆盖此内容。
>
>* _生成SSL证书_：您可以通过创建域来创建安全套接字层(SSL)。 第一个跟踪域将启动可能需要几个小时的一次性基础设施设置。 完成后，您将收到通知，然后您可以设置第一个域。 要将SSL添加到现有域，请联系[Marketo支持](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}。

## 编辑现有域的SSL

按照以下步骤为现有域启用SSL。

1. 从&#x200B;_[!UICONTROL Admin]_&#x200B;区域，选择&#x200B;**[!UICONTROL Email]**。

1. 在&#x200B;_[!UICONTROL Domain]_&#x200B;选项卡上，选择域行并单击&#x200B;**[!UICONTROL Add SSL]**。

   ![管理员 — 电子邮件 — 域 — 添加SSL](./assets/admin-email-branding-domain-add-ssl.png){width="600"}

1. 在对话框中，单击&#x200B;**[!UICONTROL Confirm]**。

   ![添加SSL — 确认](./assets/generate-ssl-cert-confirm.png){width="400"}

## 错误消息 {#error-messages}

<table><thead>
  <tr>
    <th>错误</th>
    <th>详细信息</th>
  </tr></thead>
<tbody>
<tr>
    <td><i>域已存在。</i></td>
    <td>具有相同名称的域已存在。</td>
  </tr>
  <tr>
    <td><i>域未映射到默认域。</i></td>
    <td>自定义域未正确映射到默认域。 请验证域映射设置并确保DNS配置指向正确的默认域。</td>
  </tr>
  <tr>
    <td><i>由于不支持的CAA记录，无法颁发SSL证书。 请求您的IT更新CAA记录。</i></td>
    <td>CAA记录不是最新的。 对于使用Marketo Engage托管的SSL证书的使用者，CAA记录需要更新为我们的供应商推荐的证书。 请联系您的IT部门以更新CAA记录。 有关其他详细信息，请参阅<a href="https://nation.marketo.com/t5/product-blogs/changes-to-marketo-engage-secured-domains-platform/ba-p/329305#M2246">此页面</a>。</td>
  </tr>
  <tr>
    <td><i>已颁发SSL证书。</i></td>
    <td>此自定义域已存在SSL证书。 除非证书已过期或需要重新颁发，否则无需执行进一步操作。</td>
  </tr>
  <tr>
    <td><i>未找到默认域。 请联系支持人员以获取帮助。</i></td>
    <td>尝试查找默认域时出现问题。 请联系支持部门以便他们进行调查。</td>
  </tr>
  <tr>
    <td><i>创建域时遇到意外错误。 请联系支持人员以获取帮助。</i></td>
    <td>发生意外错误。 请收集日志和错误详细信息，并将问题升级至<a href="https://nation.marketo.com/t5/support/ct-p/Support" target="_blank">Marketo支持</a>。</td>
  </tr>
</tbody></table>

## 注意事项 {#things-to-note}

* 将域的&#x200B;**DNS映射到Marketo Engage**：在UI中添加域之前，必须[将CNAME映射到Marketo提供的域](https://experienceleague.adobe.com/zh-hans/docs/marketo/using/getting-started/initial-setup/setup-steps#customize-your-landing-page-urls-with-a-cname){target="_blank"}。

* **自定义SSL**：如果您需要自定义SSL，请提交[支持票证](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}。 请勿使用自助复选框来创建SSL。

* **预先存在的SSL**：在添加域时，系统会检查预先存在的SSL，这些SSL可能在之前已手动创建。 如果您遇到此验证，请在不选择SSL创建的情况下创建您的域，我们将为您连接它们。 [联系支持人员](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}其他详细信息/选项。

* **删除域**：自动删除域&#x200B;**不会**&#x200B;删除SSL证书。 此护栏可防止导致网站没有SSL证书的用户错误。 如果您确实要删除SSL证书，请[联系支持人员](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}。

>[!MORELIKETHIS]
>
>[编辑您的默认品牌策略域](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md){target="_blank"}
