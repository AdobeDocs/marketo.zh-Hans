---
title: 理解——我——令牌
description: 了解我的令牌
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---


# 了解我的令牌

<br> 

我的令牌是自定义变量，您可以在项目或活动文件夹中创建和使用。 它们的外观如下： `{{_my.Name of Token_}}`

## 示例

* `{{my.Event Date}}`
* `{{my.Webinar Speaker}}`

要访问和创建我的令牌，请选择您的项目或活动文件夹，然后转到选 [!UICONTROL My Tokens] 项卡。 将任何令牌拖放到画布 [!UICONTROL Local Tokens] 上。

![图像1](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-1.png)

>[!CAUTION]
>
>保存令牌后，无法更改其名称，请谨慎选择。

>[!NOTE]
>
>在Microsoft Dynamics或Salesforce上从Sales Insight发送电子邮件时，我的令牌将无法解析；只有标准令牌才会填充(潜在客户、公司等)。 但是，令牌的默认值将有效。

>[!NOTE]
>
>链接令牌在纯文本电子邮件中无效。

## 嵌套令牌

当您创建新令牌时，树中的其他对象可以引用该令牌。 可以在树的较低级别覆盖全局变量。 为便于管理创建令牌的位置提供了命名结构。

* **本地令牌：** 标记直接在该项目或文件夹中创建。
* **[被覆盖的令牌：](/help/sky/override-an-inherited-my-token.md)** 该令牌已继承，但在此项目或文件夹中出现异常。
* **继承的令牌：** 标记是在树中某个较高级别的项目或文件夹中创建的。

您可以在项目或活动文件夹 **[!UICONTROL My Tokens]** 的选项卡下找到这三种类型。

![图像2](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-2.png)

移动项目和文件夹也会影响令牌。 始终检查以确保在移动过程中不会损坏引用。

>[!NOTE]
>
>如果从参与项目发送的电子邮件是默认项目的子电子邮件(即，不是您的参与项目的本地电子邮件)，则电子邮件中使用的任何“我的令牌”都将从子电子邮件所在的默认项目解析。

## 令牌使用

选择任意令牌，然后单击右上角的使用图标以查看包含该令牌的资产列表。

![图3](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-3.png)

![图像4](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-4.png)

**深潜**

进一步了解每个“我的令牌”:

* [CRM活动](/help/sky/my-token-crm-campaign.md)
* [日期](/help/sky/my-token-date.md)
* [日历文件](/help/sky/my-token-calendar-file.md)
* [图像](/help/sky/my-token-image.md)
* [链接](/help/sky/my-token-link.md)
* [数字](/help/sky/my-token-number.md)
* [富文本](/help/sky/my-token-rich-text.md)
* [得分](/help/sky/my-token-score.md)
* [电子邮件脚本](/help/sky/my-token-email-script.md)
* [文本](/help/sky/my-token-text.md)
