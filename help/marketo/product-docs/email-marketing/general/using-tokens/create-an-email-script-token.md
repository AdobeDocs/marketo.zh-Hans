---
unique-page-id: 1900577
description: 创建电子邮件脚本令牌- Marketo Docs —— 产品文档
title: 创建电子邮件脚本令牌
translation-type: tm+mt
source-git-commit: 0f0217a88929661798015b51a26259a973f9f6ea
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---


# 创建电子邮件脚本令牌{#create-an-email-script-token}

对于高级开发人员，您可以在电子邮件中使用[Velocity脚本](https://velocity.apache.org/engine/1.7/user-guide.html)。 下面介绍如何实现。

1. 转到&#x200B;**营销活动**。

   ![](assets/ma.png)

1. 查找并选择任何项目(事件、默认或参与等)。

   ![](assets/image2014-9-17-22-3a21-3a24.png)

1. 在&#x200B;**我的令牌**&#x200B;选项卡下，拖入&#x200B;**电子邮件脚本**&#x200B;令牌。

   ![](assets/image2014-9-17-22-3a21-3a29.png)

1. 命名您的电子邮件脚本令牌并单击&#x200B;**以编辑**&#x200B;其内容。

   ![](assets/image2014-9-17-22-3a21-3a46.png)

1. 使用右侧的树拖入&#x200B;**Person、Opportunity**&#x200B;或&#x200B;**Custom Object**&#x200B;令牌。

   ![](assets/five-2.png)

   >[!NOTE]
   >
   >访问数组（机会或自定义对象）时，仅限于与该人关联的最近10个项目。

1. 请注意，将令牌拖入脚本编辑器后，该令牌会变为选中／活动状态。

   ![](assets/image2014-9-17-22-3a22-3a33.png)

   >[!NOTE]
   >
   >如果您键入令牌是自由格式，请确保检查／激活树中的所有相应令牌，否则它们将被视为纯文本，无法使用。

1. 以Velocity编写脚本。 以下是一些有用的资源：

   * [营销人员电子邮件脚本文档](https://developers.marketo.com/email-scripting/)
   * [Velocity用户指南](https://velocity.apache.org/engine/devel/user-guide.html)
   * [速度参考指南](https://velocity.apache.org/engine/devel/vtl-reference-guide.html)
   * [Velocity工具Javadoc](https://velocity.apache.org/tools/releases/2.0/javadoc/index.html)

1. 完成脚本后，单击&#x200B;**保存**。

   ![](assets/image2014-9-17-22-3a23-3a1.png)

1. 再单击一次&#x200B;**保存**。

   ![](assets/image2014-9-17-22-3a23-3a13.png)

现在，您可以在电子邮件中使用此令牌。 每次发送电子邮件时，它都会运行脚本。

>[!MORELIKETHIS]
>
>[向电子邮件中添加电子邮件脚本令牌](/help/marketo/product-docs/email-marketing/general/using-tokens/add-an-email-script-token-to-your-email.md)
