---
unique-page-id: 2949839
description: 从平板电脑- Marketo Docs —— 产品文档将人物检入事件
title: 在平板电脑上将人物检入事件
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---


# 将人员从平板电脑{#check-people-into-your-event-from-your-tablet}检入事件

当人们出现在您的事件时，您可以在应用程序中找到他们的信息。 登记后，当您同步到Marketo时，它们将提升为“已出席”状态。

除了较小的布局和设计差异外，应用程序在iPad和Android上的工作方式相同。

>[!PREREQUISITES]
>
>* 在Marketo中创建事件，并用“已邀请”和“已注册”人员填充它。
>* 下载用于[Android](https://play.google.com/store/apps/details?id=com.marketo.eventcheckin&amp;hl=en)或[iOS](https://itunes.apple.com/us/app/marketo-events/id522766637?mt=8)的平板电脑应用程序

>



## 登记注册客人{#check-in-registered-guests}

1. 点击iPad或Android平板电脑上的应用程序图标。
1. 点按&#x200B;**登录**&#x200B;以启动Marketo事件应用程序。

   ![](assets/1.jpg)

1. 输入您的Marketo用户名和密码，然后单击&#x200B;**登录**。

   >[!NOTE]
   >
   >您必须具有对数据库具有访问权限的角色才能查看应用程序中的人员。

1. 选择&#x200B;**事件**。

   ![](assets/2.jpg)

   >[!TIP]
   >
   >只显示事件项目（网络研讨会除外），它们预定在今天日期的前一周和后一周。

1. 在“主页”屏幕上，浏览以查找注册客人。 要在列表中查找人员，您可以：

   * 滚动以查找名称
   * 在搜索字段中输入名称
   * 点击列表右侧的姓氏的特定初始字母，跳至该字母

   >[!NOTE]
   >
   >在iPad和Android上，过程相同，但屏幕不同，项目可能位于不同的位置。 本文提供iPad界面。 比较本节中的Android屏幕以供参考。

   **iPad** ![](assets/image2016-4-15-11-3a55-3a11.png)

   **Android**

   ![](assets/image2016-4-15-14-3a50-3a19.png)

1. 点按所选名称，然后在人员记录上点按&#x200B;**签入**。

   ![](assets/img-0068-35-hands.png)

客人现在具有“已出席”状态，并收到复选标记。 当您与Marketo同步时，人员记录会更新。 “同步”按钮上的红色计数器会递增，以显示自上次与Marketo同步以来的登记次数。 “同步”按钮的外观有所不同，并且位于iPad和Android的不同位置：

**iPad**

![](assets/image2016-4-12-14-3a25-3a13.png)

**Android**

![](assets/image2016-4-15-14-3a58-3a6.png)

>[!TIP]
>
>如果某人受邀但未注册，则可以单击“搜索”框下的“在服务器上搜索”**来搜索该姓名。**&#x200B;对于事件,“已邀请”状态将更改为&#x200B;**已出席**。

## 在平板电脑上创建新人物{#create-a-new-person-on-the-tablet}

您可以在Marketo数据库中手动添加不是现有人员的客人。 它们将在您与Marketo同步时自动签入并添加到您的数据库。

1. 单击&#x200B;**添加**。

   **iPad**

   ![](assets/image2016-4-15-11-3a58-3a51.png)

   **Android**

   ![](assets/image2016-4-15-15-3a2-3a38.png)

1. 填写尽可能多的基本信息字段，然后点按&#x200B;**完成**。

   ![](assets/image2016-4-15-11-3a33-3a59.png)

   >[!NOTE]
   >
   >您只能使用现有字段。 无法创建自定义。

   >[!CAUTION]
   >
   >多次-检查电子邮件地址。 其他字段稍后可以更正，但电子邮件地址是联系客人的主要方法。

新人员已注册为已签入您的事件，并将在您同步到Marketo时添加到具有“已出席”状态的Marketo数据库。

## 反转签入{#reverse-a-check-in}

如果您在与Marketo *同步之前误登记了某人，则可以颠倒“已出席”状态。*

1. 点按列表中的名称，然后点按人员记录中的&#x200B;**撤消**。

   ![](assets/image2016-4-15-11-3a38-3a31.png)

   全部修复！

## 在签入{#edit-a-person-record-at-check-in}时编辑人员记录

您可以直接在事件添加和修改客人信息！

1. 点按人物列表卡中的名称，然后点按&#x200B;**编辑**。

   ![](assets/image2016-4-15-11-3a43-3a46.png)

1. 编辑信息并添加到字段，然后点按&#x200B;**完成**。

   ![](assets/image2016-4-15-11-3a50-3a18.png)

   >[!NOTE]
   >
   >在Android中，**Done**&#x200B;按钮可能是隐藏的。 向下滚动以找到它。

当您将应用程序与Marketo同步时，信息将会更新。

## 将应用程序与Marketo同步{#sync-the-app-with-marketo}

Marketo事件应用程序独立工作，直到您将活动同步回Marketo数据库。 最好在上次登记后尽快同步。 平板电脑必须连接到Internet。

>[!CAUTION]
>
>同步后，无法从应用程序撤消登记。

1. 在平板电脑上，打开应用程序并导航到事件。
1. 点按&#x200B;**同步**。

   您的事件将使用Marketo数据库中的新签入进行更新。 “同步”按钮上的红色计数器将清除，直到您签入其他人。

   出于安全原因，您应在同步完成后退出Marketo事件应用程序。

## 使用受限Internet访问{#working-with-limited-internet-access}

有些地方的互联网接入很差。 您需要与以下对象建立良好的连接：

* 下载并安装应用程序
* 登录
* 选择事件
* 将应用程序与Marketo同步

如果您担心在场地访问Internet，您可能希望登录Marketo事件应用程序并提前选择您的事件，地点具有强大的Internet访问能力。 这样，您仍可脱机使用应用程序。 然后，当您重新获得Internet连接时，立即同步到Marketo数据库。

>[!TIP]
>
>如果您没有Internet连接，您仍然可以为登记人员创建新人员。 当您同步应用程序时，它将与现有人协调。

>[!NOTE]
>
>应用程序在8小时不活动后自动将您注销。

