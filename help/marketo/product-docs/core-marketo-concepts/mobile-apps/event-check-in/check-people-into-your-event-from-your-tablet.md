---
unique-page-id: 2949839
description: 通过平板电脑 — Marketo文档 — 产品文档，查看您的事件中的人员
title: 在平板电脑上查看活动中的人员
exl-id: b48f5f95-8e36-441f-a785-1651f42f9f60
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---

# 在平板电脑上查看活动中的人员 {#check-people-into-your-event-from-your-tablet}

当人员出现在您的活动中时，您可以在应用程序中找到他们的信息。 签入后，在您同步到Marketo时，这些用户档案将升级为“已出席”状态。

除了较小的布局和设计差异外，该应用程序在iPad和Android上的工作方式相同。

>[!PREREQUISITES]
>
>* 在Marketo中创建事件，然后向其中填充“已邀请”和“已注册”人员。
>* 下载适用于 [Android](https://play.google.com/store/apps/details?id=com.marketo.eventcheckin&amp;hl=en) 或 [iOS](https://itunes.apple.com/us/app/marketo-events/id522766637?mt=8)


## 登记来宾 {#check-in-registered-guests}

1. 点按iPad或Android平板电脑上的应用程序图标。

1. 点按 **登录** 启动Marketo事件应用程序时，请执行以下操作：

   ![](assets/1.jpg)

1. 输入Marketo用户名和密码，然后单击 **登录**.

   >[!NOTE]
   >
   >您必须具有对数据库的访问权限角色才能查看应用程序中的人员。

1. 选择 **事件**.

   ![](assets/2.jpg)

   >[!TIP]
   >
   >只显示计划在今天日期之前一周和之后一周的事件项目（网络研讨会除外）。

1. 在“Home（主页）”屏幕上，浏览以查找“Registered guesters（注册客人）”。 要在列表中查找人员，您可以：

   * 滚动以查找名称
   * 在搜索字段中输入名称
   * 点按列表右侧的某个姓氏的字母，以跳转到该姓氏的特定首字母

   >[!NOTE]
   >
   >在iPad和Android中，过程相同，但屏幕不同，项目可能位于不同的位置。 本文介绍iPad界面。 比较此部分中的Android屏幕以供参考。

   **iPad**

   ![](assets/image2016-4-15-11-3a55-3a11.png)

   **Android**

   ![](assets/image2016-4-15-14-3a50-3a19.png)

1. 点按选定的名称，然后在人员记录中，点按 **签入**.

   ![](assets/img-0068-35-hands.png)

来宾现在具有“已出席”状态，并收到复选标记。 当您与Marketo同步时，人员记录会更新。 “同步”按钮上的红色计数器将递增，以显示自上次与Marketo同步以来的签入次数。 “同步”按钮看起来不同，并且位于iPad和Android的不同位置：

**iPad**

![](assets/image2016-4-12-14-3a25-3a13.png)

**Android**

![](assets/image2016-4-15-14-3a58-3a6.png)

>[!TIP]
>
>如果某人受邀但未注册，则可通过单击 **在服务器上搜索**，位于“搜索”框下方。 “已邀请”状态将更改为 **已出席** 的值。

## 在平板电脑上创建新人员 {#create-a-new-person-on-the-tablet}

您可以在Marketo数据库中手动添加不是现有人员的来宾。 在您与Marketo同步时，系统会自动将它们签入并添加到数据库中。

1. 单击 **添加**.

   **iPad**

   ![](assets/image2016-4-15-11-3a58-3a51.png)

   **Android**

   ![](assets/image2016-4-15-15-3a2-3a38.png)

1. 填写尽可能多的基本信息字段并点按 **完成**.

   ![](assets/image2016-4-15-11-3a33-3a59.png)

   >[!NOTE]
   >
   >您只能使用现有字段。 无法创建自定义受众。

   >[!CAUTION]
   >
   >仔细检查电子邮件地址。 其他字段稍后可以更正，但电子邮件地址是联系来宾的主要方法。

新人员将注册为已签入到您的事件，并在您同步到Marketo时将添加到状态为“已出席”的Marketo数据库。

## 反向签入 {#reverse-a-check-in}

如果你误报了某人， _在您与Marketo同步之前_，则可以撤销“已出席”状态。

1. 点按列表中的名称，然后在人员记录中，点按 **撤消**.

   ![](assets/image2016-4-15-11-3a38-3a31.png)

   全部修复！

## 在签入时编辑人员记录 {#edit-a-person-record-at-check-in}

您可以在活动中直接添加和修改来宾信息！

1. 点按人员列表中的名称，然后点按 **编辑**.

   ![](assets/image2016-4-15-11-3a43-3a46.png)

1. 编辑信息并将其添加到字段，然后点按 **完成**.

   ![](assets/image2016-4-15-11-3a50-3a18.png)

   >[!NOTE]
   >
   >在Android中， **完成** 按钮。 向下滚动以找到它。

当您将应用程序与Marketo同步时，该信息将会更新。

## 将应用程序与Marketo同步 {#sync-the-app-with-marketo}

在您将活动同步回Marketo数据库之前，Marketo事件应用程序会独立工作。 最好在上次签入后尽快同步。 您的平板电脑必须连接到Internet。

>[!CAUTION]
>
>同步后，无法从应用程序中反向签入。

1. 在平板电脑上，打开应用程序并导航到您的事件。

1. 点按 **同步**.

   您的事件已更新，其中包含Marketo数据库中的新签入。 “同步”按钮上的红色计数器清除，直到您签入其他人为止。

   出于安全原因，您应在完成同步后退出Marketo事件应用程序。

## 使用有限Internet访问 {#working-with-limited-internet-access}

有些场所的互联网连接很差。 您需要良好的连接：

* 下载并安装应用程序
* 登录
* 选择事件
* 将应用程序与Marketo同步

如果您担心会在会场访问Internet，则可能需要先登录到Marketo Events应用程序，然后在具有强Internet访问权限的位置选择您的活动。 这样，您仍然可以脱机使用应用程序。 然后，当您重新获得Internet连接时，立即同步到Marketo数据库。

>[!TIP]
>
>如果您没有Internet连接，则仍然可以为登记的人员创建新人员。 在您同步应用程序时，它将与现有人员协调。

>[!NOTE]
>
>在处于非活动状态八小时后，应用程序会自动将您注销。
