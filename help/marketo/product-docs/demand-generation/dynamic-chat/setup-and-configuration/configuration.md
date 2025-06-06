---
description: 配置 — Marketo文档 — 产品文档
title: 配置
feature: Dynamic Chat
exl-id: 01ca6a38-4918-46b0-b0f6-1baffbb0bbaf
source-git-commit: 42e2a23c1c451c61fd62237fd1305924b51437b2
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 0%

---

# 配置 {#configuration}

了解如何自定义聊天机器人对话框窗口的外观。

若要开始，请单击&#x200B;**配置**&#x200B;下的&#x200B;**聊天机器人**。

![](assets/configuration-1.png)

有多种不同的自定义选项。

![](assets/configuration-2.png)

## “样式”选项卡 {#style-tab}

### 样式 {#style}

您将在此处定义显示对话框的聊天机器人的外观，包括：颜色、字体、机器人小部件的放置以及聊天机器人的名称/头像。

每个类别的颜色由[十六进制颜色值](https://color.adobe.com/create/color-wheel){target="_blank"}确定(例如，白色= #ffffff，红色= #bf1932，等等)。

![](assets/configuration-3.png)

锚点允许网站访客打开/关闭聊天盒。 您可以选择该图标显示在右下角还是左下角。 您还可以增加/减少边距（图标和网页底部之间的间距）。

![](assets/configuration-4.png)

### 机器人设置 {#agent-settings}

在“机器人设置”中，您可以向聊天盒添加标签(例如：“Adobe助手”)，该标签将显示在聊天盒顶部。 您还可以确定响应延迟（以秒为单位），并更改您的聊天头像。 要上传您自己的头像图像，请单击&#x200B;**+**&#x200B;按钮。

![](assets/configuration-5.png)

>[!NOTE]
>
>自定义头像应为小于256kb且小于200x200像素的方形图像。 支持的文件类型包括： .jpg、.png、.gif、.webp、.svg。

**新消息通知声音**

单击下拉菜单以在每次在会话中触发聊天机器人时为访客选择提示音。 有多种声音可供选择。

**在移动设备上启用Poke消息**

选择滑块可启用“探查”（该选项在聊天图标旁边显示开头的问题，访客无需单击该图标即可查看），以供访客从移动设备中聊天。

![](assets/configuration-6.png)

>[!NOTE]
>
>Poke仅在对话中的前[张卡片](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md#stream-designer-cards){target="_blank"}上可用。

完成更改后，请记得单击&#x200B;**保存**。

![](assets/configuration-7.png)

## “隐私”选项卡 {#privacy-tab}

单击&#x200B;**隐私**&#x200B;选项卡以添加/编辑网站隐私策略的URL（可选）。

![](assets/configuration-8.png)

## “安装”选项卡 {#installation-tab}

要在您的网站上显示聊天机器人，您首先需要安装Dynamic Chat JavaScript代码片段。 单击此选项卡以查找/复制必要的代码。 如果您不熟悉此操作，请与您的Web团队或IT部门联系以获取帮助。

![](assets/configuration-9.png)

>[!TIP]
>
>在您的网站使用Content-Security-Policy (CSP)时，请查看代码下方以查找要添加的内容。

>[!NOTE]
>
>未设置Marketo支持以帮助对HTML进行故障排除。 如需HTML帮助，请咨询Web开发人员。
