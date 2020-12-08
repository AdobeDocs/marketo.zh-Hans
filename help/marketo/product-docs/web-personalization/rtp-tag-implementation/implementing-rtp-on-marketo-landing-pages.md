---
unique-page-id: 4720151
description: 在Marketo登陆页上实施RTP - Marketo文档——产品文档
title: 在营销登陆页上实现RTP
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---


# 在营销登陆页上实现RTP {#implementing-rtp-on-marketo-landing-pages}

要实施RTP标签，请按照以下安装说明操作：

1. 转到Design **Studio。** 打开要编辑的项目。 选择“ **模板操作**”，选择“编 **辑草稿”**

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. 在“HTML源”选项卡上 **更改模板** 。

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. 在RTP帐户中，转到**帐户设置。**

1. 如果您已从支持部门收到JavaScript标记，请继续执行步骤5。

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. 在“域”下，找到相关域，然后单击“ **生成标记**”。

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. 复制RTP JavaScript标签并将其粘贴到标签之间的所有登陆页模 **`<head> </head>`** 板中。
1. 单击 **保存****并关** 闭窗口。
1. 返回到Design **Studio中**，从“模板操作” **中批准登陆页**，单 **击批准**。\
   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. 最后，您需要重新批 **准使用该模板** 的任何登陆页，以使模板更改生效。 您可以从主登陆页部分一次重新批准所有批准。

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. 验证它是否出现在所 `pages including` 有登陆页和子域上。

   您可以通过右键单击页面来执行此 `website’s` 操作。 转到 **视图页面源。** 搜索 **RTP** 以找到标记。
