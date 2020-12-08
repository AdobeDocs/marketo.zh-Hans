---
unique-page-id: 1900577
description: 创建电子邮件脚本令牌- Marketo Docs —— 产品文档
title: 创建电子邮件脚本令牌
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 0%

---


# 创建电子邮件脚本令牌 {#create-an-email-script-token}

对于高级开发人员，您可以在电 [子邮件中](http://velocity.apache.org/engine/1.7/user-guide.html) 使用Velocity脚本。 下面介绍如何实现。

1. 转到营 **销活动**。

   ![](assets/ma.png)

1. 查找并选择任何项目(事件、默认或参与等)。

   ![](assets/image2014-9-17-22-3a21-3a24.png)

1. 在“我 **的令牌** ”选项卡下，拖 **入电子邮件脚本令牌** 。

   ![](assets/image2014-9-17-22-3a21-3a29.png)

1. 命名电子邮件脚本令牌并 **单击以编辑** 其内容。

   ![](assets/image2014-9-17-22-3a21-3a46.png)

1. 使用右侧的树拖入Person、 **Opportunity**&#x200B;或 **Custom Object令牌** 。

   ![](assets/five-2.png)

   >[!NOTE]
   >
   >访问数组（机会或自定义对象）时，仅限于与该人关联的最近10个项目。

1. 请注意，将令牌拖入脚本编辑器后，该令牌会变为选中／活动状态。

   ![](assets/image2014-9-17-22-3a22-3a33.png)

   >[!NOTE]
   >
   >**提醒**
   >
   >
   >如果您键入令牌是自由格式，请确保检查／激活树中的所有相应令牌，否则它们将被视为纯文本，无法使用。

1. 以Velocity编写脚本。 以下是一些有用的资源：

   * [营销人员电子邮件脚本文档](http://developers.marketo.com/email-scripting/)
   * [Velocity用户指南](http://velocity.apache.org/engine/devel/user-guide.html)
   * [速度参考指南](http://velocity.apache.org/engine/devel/vtl-reference-guide.html)
   * [Velocity工具Javadoc](http://velocity.apache.org/tools/releases/2.0/javadoc/index.html)

1. 脚本完成后，单击“保 **存**”。

   ![](assets/image2014-9-17-22-3a23-3a1.png)

1. 再 **单击** “保存”。

   ![](assets/image2014-9-17-22-3a23-3a13.png)

现在，您可以在电子邮件中使用此令牌。 每次发送电子邮件时，它都会运行脚本。

>[!NOTE]
>
>**相关文章**
>
>* [向电子邮件中添加电子邮件脚本令牌](add-an-email-script-token-to-your-email.md)

>



