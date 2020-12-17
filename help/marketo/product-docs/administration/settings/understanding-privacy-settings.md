---
unique-page-id: 10617187
description: 了解隐私设置- Marketo Docs —— 产品文档
title: 了解隐私设置
translation-type: tm+mt
source-git-commit: efadb7eb3845012c273e1a60f9cd98ac884eb543
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 0%

---


# 了解隐私设置{#understanding-privacy-settings}

## 概述{#overview}

Marketo为营销人员提供了一种获得Web访客同意跟踪他们的方法。 有两种方选择退出法，或者您可以选择由匿名IP跟踪。

* Web访客在其浏览器中选择“不跟踪(DNT)”功能(营销人员接受Web访客的“不跟踪”请求)
* 网络访客使选择退出用网站上的营销人员提供的Cookie

或者，营销人员可以跟踪用户，但使用匿名IP。

这些方法可能会影响Marketo在特定领域的价值和功能。 但是，如果营销人员&#x200B;*没有*&#x200B;更改Marketo配置中的任何内容，Marketo功能将保持不变。

## 不跟踪{#browser-settings-for-do-not-track}的浏览器设置

Web访客可以通过选择“不跟踪”(DNT)来设置其浏览器以防止任何网站进行跟踪。 这会阻止对此特定浏览器和设备的跟踪。 有关完整的详细信息，请参阅浏览器的隐私设置。

在Munchkin中，营销人员可以[决定是支持还是忽略浏览器的DNT设置](edit-do-not-track-browser-support-settings.md)。

在Web个性化中，营销人员可以决定是支持还是忽略浏览器的DNT设置[。](/help/marketo/product-docs/web-personalization/getting-started/setting-web-personalization-to-do-not-track.md)

## 从选择退出特定网站{#opt-out-from-a-specific-website}

您还可以允许站点访客选择退出从您的网站跟踪网站，而不管是否配置了&#x200B;**浏览器不跟踪**&#x200B;设置。 这允许网站访客直接从您的网站指定其跟踪首选项。

为此，必须向启用了Munchkin跟踪的网选择退出页上的链接添加参数。 这可以是任何网页，但网页链接必须包含以下参数：

?marketo_opt_out=true

以下是带有退出链接的网页和单击链接后的登陆页的示例。 您的会有所不同。

这是一个网页，其中有一个按钮，该按钮在退出链接中带有“?marketo_opt_out=true”参数。

![](assets/opt-out-1.png)

您可以创建并发布登陆页，作为单击带“?marketo_opt_out=true”参数的链接的后续页面。

![](assets/opt-out-2.png)

单击链接时，Marketo会向访客的浏览器中添加一个名为&#x200B;**mkto_opt_out**&#x200B;的cookie，以禁用Munchkin跟踪点击上述参数链接的站点访客。

要验证是否可以植入Cookie，请验证您是Cookie潜在客户，然后单击链接。 然后检查您的浏览器cookies以验证是否已添加&#x200B;**mkto_opt_out** cookie。

![](assets/opt-out-3.png)

>[!NOTE]
>
>目前，仅Munchkin版本152及更高版本可使用。

## 选择加入 {#opt-in}

营销人员可以通选择加入过在电子邮件、表单、登陆页和其他方法中使用Marketo的功能，使用户能够使用Marketo的功能。

## 使用匿名IP {#tracking-using-an-anonymized-ip}进行跟踪

营销人员可以通过使用匿名IP地址跟踪用户来保护隐私。 为此，请将此代码添加到嵌入在网站中的RTP或Munchkin Javascript。

* 对于Munchkin，只需向init函数添加{&quot;anonyizeIP&quot;,true}。

   >[!NOTE]
   >
   >使用此参数需要启用Munchkin V2。 要为您的订阅启用它，请联系[Marketo Support](http://nation.marketo.com/community/support_solutions)。

* 对于Web个性化(RTP)，请将其添加到javascript:

匿名IP:在调用rtp(&#39;send&#39;,&#39;视图&#39;)之前；添加rtp(&#39;set&#39;, &#39;settings&#39;, {&#39;anonymizeIP&#39;:true});

