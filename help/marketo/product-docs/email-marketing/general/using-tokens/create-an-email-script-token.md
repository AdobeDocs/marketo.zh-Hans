---
unique-page-id: 1900577
description: 创建电子邮件脚本令牌 — Marketo文档 — 产品文档
title: 创建电子邮件脚本令牌
exl-id: c7f8c3e0-6d64-4115-b9b6-261576360ba1
feature: Tokens
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 4%

---

# 创建电子邮件脚本令牌 {#create-an-email-script-token}

对于高级开发人员，您可以在电子邮件中使用[Velocity脚本](https://velocity.apache.org/engine/1.7/user-guide.html)。 下面是操作方法。

1. 转到&#x200B;**[!UICONTROL Marketing Activities]**。

   ![](assets/ma.png)

1. 查找并选择任意项目（事件、默认或参与等）。

   ![](assets/image2014-9-17-22-3a21-3a24.png)

1. 在&#x200B;**[!UICONTROL My Tokens]**&#x200B;选项卡下，拖入&#x200B;**[!UICONTROL Email Script]**&#x200B;令牌。

   ![](assets/image2014-9-17-22-3a21-3a29.png)

1. 命名您的电子邮件脚本令牌并&#x200B;**[!UICONTROL Click to Edit]**&#x200B;其内容。

   ![](assets/image2014-9-17-22-3a21-3a46.png)

1. 使用右侧的树拖入&#x200B;**[!UICONTROL Person]**、**[!UICONTROL Opportunity]**&#x200B;或&#x200B;**[!UICONTROL Custom Object]**&#x200B;令牌。

   ![](assets/five-2.png)

   >[!NOTE]
   >
   >访问数组（商机或自定义对象）时，您将受限于与人员关联的最近10个项目。

1. 请注意，将令牌拖到脚本编辑器后，该令牌会变为选中/活动状态。

   ![](assets/image2014-9-17-22-3a22-3a33.png)

   >[!NOTE]
   >
   >如果您以自由格式键入令牌，请确保检查/激活树中所有相应的令牌，否则这些令牌将被视为纯文本并且不起作用。

1. 在Velocity中编写脚本。 以下是一些有用的资源：

   * [Marketo开发人员电子邮件脚本文档](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/email-scripting)
   * [Velocity用户指南](https://velocity.apache.org/engine/devel/user-guide.html)
   * [Velocity参考指南](https://velocity.apache.org/engine/devel/vtl-reference-guide.html)
   * [Velocity工具Javadoc](https://velocity.apache.org/tools/releases/2.0/javadoc/index.html)

1. 脚本完成后，单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/image2014-9-17-22-3a23-3a1.png)

1. 再次单击&#x200B;**[!UICONTROL Save]**。

   ![](assets/image2014-9-17-22-3a23-3a13.png)

现在，您可以在电子邮件中使用此令牌。 每次发送电子邮件时，它都会运行脚本。

>[!MORELIKETHIS]
>
>[向您的电子邮件添加电子邮件脚本令牌](/help/marketo/product-docs/email-marketing/general/using-tokens/add-an-email-script-token-to-your-email.md)
