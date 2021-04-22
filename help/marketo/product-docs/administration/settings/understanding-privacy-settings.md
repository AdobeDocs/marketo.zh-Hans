---
unique-page-id: 10617187
description: 了解隐私设置 — Marketo Docs — 产品文档
title: 了解隐私设置
exl-id: 1fde9011-02a9-4ec9-bfa4-c56a52ce1eed
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 0%

---

# 了解隐私设置{#understanding-privacy-settings}

## 概述{#overview}

Marketo为营销人员提供了获得网络访客同意跟踪他们的方式。 有两种方法选择退出，或者您可以选择由匿名IP跟踪。

* Web访客在其浏览器中选择“不跟踪(DNT)”功能(营销人员接受Web访客的“不跟踪”请求)
* 网络访客使选择退出用网站上的营销人员提供的Cookie

或者，营销人员可以跟踪用户，但使用匿名IP。

这些方法可能影响Marketo在特定领域的价值和功能。 但是，如果营销人员&#x200B;*未*&#x200B;更改Marketo配置中的任何内容，则Marketo功能将保持不变。

## 不跟踪{#browser-settings-for-do-not-track}的浏览器设置

Web访客可以通过选择“不跟踪”(DNT)来设置其浏览器以防止任何网站进行跟踪。 这会阻止对此特定浏览器和设备的跟踪。 有关完整的详细信息，请参阅浏览器的隐私设置。

在Munchkin中，营销人员可以[决定是支持还是忽略浏览器的DNT设置](/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md)。

在Web个性化中，营销人员可以决定是支持还是忽略浏览器的DNT设置](/help/marketo/product-docs/web-personalization/getting-started/setting-web-personalization-to-do-not-track.md)。[

## 从选择退出特定网站{#opt-out-from-a-specific-website}

您还可以允许站点访客从选择退出您的网站跟踪，而不管是否配置了&#x200B;**浏览器不跟踪**&#x200B;设置。 这允许网站访客直接从您的网站指定其跟踪首选项。

为此，您必须向启用了Munchkin跟踪的网选择退出页上的链接添加参数。 这可以是任何网页，但网页链接必须包含以下参数：

?marketo_opt_out=true

以下是带有退出链接的网页的示例，该网页在单击链接后具有登陆页。 你的会有所不同。

这是一个网页，其中有一个按钮，在选择退出链接中带有“？marketo_opt_out=true”参数。

![](assets/opt-out-1.png)

您可以创建并发布登陆页，作为单击带有“？marketo_opt_out=true”参数的链接的后续页面。

![](assets/opt-out-2.png)

单击链接时，Marketo会向访客的浏览器添加一个名为&#x200B;**mkto_opt_out**&#x200B;的Cookie，以禁用Munchkin跟踪功能，以跟踪单击带有上述参数的链接的站点访客。

要验证是否可以植入Cookie，请验证您是否为Cookie潜在客户，然后单击链接。 然后检查您的浏览器cookies以验证是否添加了&#x200B;**mkto_opt_out** cookie。

![](assets/opt-out-3.png)

>[!NOTE]
>
>目前，仅适用于Munchkin版本152及更高版本。

## 选择加入 {#opt-in}

营销人员可以通选择加入过使用Marketo在电子邮件、表单、登陆页和其他方法中的功能，使用户能够使用。

## 使用匿名IP {#tracking-using-an-anonymized-ip}进行跟踪

营销人员可以通过使用匿名IP地址跟踪用户来保护隐私。 为此，请将此代码添加到嵌入到网站中的RTP或Munchkin Javascript。

* 对于Munchkin，只需将{&quot;anonyizeIP&quot;,true}添加到init函数。

   >[!NOTE]
   >
   >使用此参数要求启用Munchkin V2。 要启用订阅，请联系[Marketo支持](https://nation.marketo.com/community/support_solutions)。

* 对于Web个性化(RTP)，请将其添加到javascript中：

`anonymize IP : before calling rtp('send','view'); add rtp('set', 'settings', {'anonymizeIP' : true});`
