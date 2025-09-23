---
unique-page-id: 11382535
description: 在我的令牌中使用URL - Marketo文档 — 产品文档
title: 在我的令牌中使用 URL
exl-id: 6830c621-4d94-4f31-a608-2f7b2aced88c
feature: Tokens
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 5%

---

# 在我的令牌中使用 URL {#using-urls-in-my-tokens}

按照以下步骤使用[!UICONTROL My Tokens]将URL插入到您的电子邮件中。

1. 选择您的项目并单击&#x200B;**[!UICONTROL My Tokens]**。

   ![](assets/one-4.png)

1. 选择&#x200B;**[!UICONTROL Text]**&#x200B;我的令牌，并将其拖放到画布上。

   ![](assets/two-4.png)

1. 为令牌提供一个唯一的名称，输入URL(不带https://)并单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/three-4.png)

   >[!CAUTION]
   >
   >**正在使用http/https...**
   >
   >* 若要确保跟踪电子邮件中的点击量，请&#x200B;**不**&#x200B;输入https:// _内部_&#x200B;令牌的值。 在令牌之外使用它，如步骤7中所示。
   >
   >* 我们强烈建议不要忽略http/https。 这样做可能会导致电子邮件的[Web版本](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"}无法正确呈现。

1. 选择项目中的电子邮件。

   ![](assets/four-3.png)

1. 单击 **[!UICONTROL Edit Draft]**。

   ![](assets/five-3.png)

1. 在文本区域中双击以进行编辑。

   ![](assets/six-1.png)

1. 在电子邮件中的任意位置，键入`https://`（后面不留空格）并单击“插入令牌”图标。

   ![](assets/seven.png)

   >[!NOTE]
   >
   >如果您的网站不使用https，您当然也可以选择输入`http://`。

1. 找到您的“我的令牌”，选择它，然后单击&#x200B;**[!UICONTROL Insert]**。

   ![](assets/eight.png)

1. 突出显示https://和令牌，然后按Ctrl/Cmd+X (Ctrl = Windows/Cmd = Mac)以剪切文本。

   ![](assets/nine.png)

1. 突出显示您希望链接显示的文本，然后单击[!UICONTROL Insert/Edit Link]图标。

   ![](assets/ten.png)

1. 按Ctrl/Cmd+V将内容粘贴到&#x200B;**[!UICONTROL URL]**&#x200B;框中，然后单击&#x200B;**[!UICONTROL Insert]**。

   ![](assets/eleven.png)

1. 单击 **[!UICONTROL Save]**。

   ![](assets/twelve.png)

   你完蛋了！ 您的URL将在发送后填充，由于您将https://放在令牌的前面，因此它将生成一个可跟踪链接。
