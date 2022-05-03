---
description: 将动态聊天连接到Marketo - Marketo文档 — 产品文档
title: 将动态聊天连接到Marketo
exl-id: bad6c2dc-d4e7-4f98-bf6d-743043f96e4e
source-git-commit: c36b9206494c14a52937fa787a37601eaf6f4bd4
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---

# 将动态聊天连接到Marketo {#connect-dynamic-chat-to-marketo}

完成 [初始设置](/help/marketo/product-docs/demand-generation/dynamic-chat/initial-setup.md)，则该执行一次性同步，将动态聊天连接到Marketo订阅。

1. 在My Marketo中，单击 **动态聊天** 拼贴。

   ![](assets/connect-dynamic-chat-to-marketo-1.png)

   >[!NOTE]
   >
   >如果看不到图块，请联系Marketo管理员。

1. 如果您之前使用Adobe ID访问过应用程序，则会直接转到动态聊天。 如果没有， [设置Adobe ID](https://helpx.adobe.com/manage-account/using/create-update-adobe-id.html).

1. 要连接Marketo实例，请选择 **集成**.

   ![](assets/connect-dynamic-chat-to-marketo-2.png)

1. 在Marketo卡上，单击 **启动同步**.

   ![](assets/connect-dynamic-chat-to-marketo-3.png)

1. 从Marketo实例中选择最多50个标准或自定义字段以同步到动态聊天，以用于受众定位、数据映射和个性化。 单击 **下一个** 完成时。

   ![](assets/connect-dynamic-chat-to-marketo-4.png)

   >[!CAUTION]
   >
   >此时，属性选择 **无法** 在初始同步后进行更改。 完成同步后，您只能返回并添加更多内容（如果选择的同步量小于50个）。

1. 查看您的选择(提醒：您无法在同步后删除属性，因此请单击 **编辑选择** （如果需要在此步骤中更改任意内容）。 单击 **确认** 完成时启动同步。

   ![](assets/connect-dynamic-chat-to-marketo-5.png)

>[!NOTE]
>
>完成同步可能需要2到24小时，具体时间取决于数据库的大小。

## 关联您的Adobe组织和Marketo {#link-your-adobe-org-and-marketo}

接下来，该将Adobe和Marketo关联起来。

>[!IMPORTANT]
>
>建立此映射的Marketo Engage用户的电子邮件地址还必须有权访问正在连接的Adobe组织。

1. 登录到 [experience.adobe.com](https://experience.adobe.com).

1. 单击Experience Cloud中任意位置的屏幕，然后按Ctrl+i。在 **分配的组织** ，突出显示并复制组织ID(_减号_ “@AdobeOrg”)。 按 **关闭** 完成时。

   ![](assets/connect-dynamic-chat-to-marketo-6.png)

1. 在Marketo中，转到 **管理员** 选择 **Adobe组织映射**.

   ![](assets/connect-dynamic-chat-to-marketo-7.png)

1. 单击 **编辑**.

   ![](assets/connect-dynamic-chat-to-marketo-8.png)

1. 粘贴您在步骤2中复制的组织ID，然后单击 **确定**.

   ![](assets/connect-dynamic-chat-to-marketo-9.png)

>[!MORELIKETHIS]
>
>[初始设置](/help/marketo/product-docs/demand-generation/dynamic-chat/initial-setup.md)
