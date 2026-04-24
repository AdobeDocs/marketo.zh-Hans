---
unique-page-id: 11377395
description: 在一个实例中为多个品牌添加额外的品牌域，以便每个品牌都有自己的品牌跟踪链接。
title: 添加附加品牌域名
exl-id: df6e5afe-dbb0-4fbe-bf06-79d92a91b986
feature: Email Setup
source-git-commit: 6638f4a24aac6cf828f443d17b896a9dec9bca16
workflow-type: tm+mt
source-wordcount: '713'
ht-degree: 19%

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
    <td>CAA记录不是最新的。 对于使用Marketo Engage托管的SSL证书的使用者，CAA记录需要更新为我们的供应商推荐的证书。 Please contact your IT department to update the CAA records. See <a href="https://nation.marketo.com/t5/product-blogs/changes-to-marketo-engage-secured-domains-platform/ba-p/329305#M2246">this page</a> for additional details.</td>
  </tr>
  <tr>
    <td><i>SSL certificate has already been issued.</i></td>
    <td>此自定义域已存在SSL证书。 No further action is needed unless the certificate has expired or needs to be reissued.</td>
  </tr>
  <tr>
    <td><i>The default domain was not found. Please contact Support for assistance.</i></td>
    <td>尝试查找默认域时出现问题。 Please reach out to Support so they can investigate.</td>
  </tr>
  <tr>
    <td><i>Unexpected error encountered while creating a domain. Please contact Support for assistance.</i></td>
    <td>An unexpected error has occurred. Please gather logs and error details, and escalate the issue to <a href="https://nation.marketo.com/t5/support/ct-p/Support" target="_blank">Marketo Support</a>.</td>
  </tr>
</tbody></table>

## Things to Note {#things-to-note}

* **DNS mapping for domain to Marketo Engage**: Before adding adding domains in the UI, you must [map CNAMEs to a Marketo-provided domain](https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/initial-setup/setup-steps#customize-your-landing-page-urls-with-a-cname){target="_blank"}.

* **Custom SSLs**: If you need a custom SSL, please submit a [Support ticket](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. Do not use the self-service checkbox for SSL creation.

* **Pre-existing SSLs**: While adding a domain, the system checks for pre-existing SSLs, which may have been manually created prior. If you encounter this validation, create your domain without selecting SSL creation, and we will connect them for you. [Contact Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} more additional details/options.

* **Deletion of domains**: Automatically deleting a domain **does not** delete the SSL certificate. 此护栏可防止导致网站没有SSL证书的用户错误。 If you do want to remove the SSL certificates, [contact Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

* If the domain you add is listed as anything other than a CNAME, the ability to add further branded tracking domains will be locked out. You will need to edit any existing domain and ensure it is a CNAME record and not, say, an A record. The Add button dynamically checks for CNAMES and CNAMES only.

>[!MORELIKETHIS]
>
>[Edit Your Default Branding Domain](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md){target="_blank"}
