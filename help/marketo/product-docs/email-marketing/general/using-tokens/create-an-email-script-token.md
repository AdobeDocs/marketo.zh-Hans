---
unique-page-id: 1900577
description: 创建电子邮件脚本令牌 — Marketo文档 — 产品文档
title: 创建电子邮件脚本令牌
exl-id: c7f8c3e0-6d64-4115-b9b6-261576360ba1
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---

# 创建电子邮件脚本令牌 {#create-an-email-script-token}

对于高级开发人员，您可以使用 [Velocity脚本](https://velocity.apache.org/engine/1.7/user-guide.html) 邮件中。 这是如何做到的。

1. 转到 **营销活动**.

   ![](assets/ma.png)

1. 查找并选择任意项目（“事件”、“默认”或“参与度”等）。

   ![](assets/image2014-9-17-22-3a21-3a24.png)

1. 在 **我的令牌** 选项卡，在 **电子邮件脚本** 令牌。

   ![](assets/image2014-9-17-22-3a21-3a29.png)

1. 命名您的电子邮件脚本令牌和 **单击以编辑** 内容。

   ![](assets/image2014-9-17-22-3a21-3a46.png)

1. 使用右侧的树拖入 **人员、机会**&#x200B;或 **自定义对象** 令牌。

   ![](assets/five-2.png)

   >[!NOTE]
   >
   >访问数组（机会或自定义对象）时，您只能访问与该人员关联的最近10个项目。

1. 请注意，将令牌拖动到脚本编辑器后，该令牌会变为选中/活动状态。

   ![](assets/image2014-9-17-22-3a22-3a33.png)

   >[!NOTE]
   >
   >如果您在令牌中键入自由格式，请确保检查/激活树中的所有对应令牌，否则这些令牌将被视为纯文本，并且无法正常使用。

1. 用Velocity编写脚本。 以下是一些有用的资源：

   * [Marketo开发人员电子邮件脚本文档](https://developers.marketo.com/email-scripting/)
   * [Velocity用户指南](https://velocity.apache.org/engine/devel/user-guide.html)
   * [Velocity参考指南](https://velocity.apache.org/engine/devel/vtl-reference-guide.html)
   * [Velocity工具Javadoc](https://velocity.apache.org/tools/releases/2.0/javadoc/index.html)

1. 脚本完成后，单击 **保存**.

   ![](assets/image2014-9-17-22-3a23-3a1.png)

1. 单击 **保存** 再来一次。

   ![](assets/image2014-9-17-22-3a23-3a13.png)

现在，您可以在电子邮件中使用此令牌。 每次发送电子邮件时，它都会运行脚本。

>[!MORELIKETHIS]
>
>[向电子邮件中添加电子邮件脚本令牌](/help/marketo/product-docs/email-marketing/general/using-tokens/add-an-email-script-token-to-your-email.md)
