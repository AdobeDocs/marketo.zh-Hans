---
unique-page-id: 4719291
description: 设置默认人员姓氏和公司名- Marketo Docs —— 产品文档
title: 设置默认人员姓氏和公司名
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 0%

---


# 设置默认人员姓氏和公司名 {#set-default-person-last-name-and-company-name}

Salesforce需要（最小）Lead和Contacts的姓氏和公司名。 未完成的记录将不会同步到Salesforce。 如果要同步部分记录，则必须设置Market才能与Salesforce一起使用的默认值。

1. 转到“管 **理员** ”，单 **击“Salesforce**”。

   ![](assets/image2014-12-9-13-3a41-3a58.png)

1. 单击“ **编辑同步选项**”。

   ![](assets/image2014-12-9-13-3a42-3a6.png)

1. 输入默 **认人员姓** 、**默认**人员&#x200B;**公司，然后** 单击 **保存**。

   ![](assets/sync-options-hands.png)

   >[!NOTE]
   >
   >Marketo仅在记录最初同步到Salesforce时（并且其中一个必填字段为空）才分配默认值。

就这样！ 每次缺少姓和／或公司时，Marketo都会添加默认值，因为它会同步记录。
