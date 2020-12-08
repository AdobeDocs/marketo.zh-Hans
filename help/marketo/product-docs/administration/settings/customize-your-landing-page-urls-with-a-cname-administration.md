---
unique-page-id: 2360189
description: 使用CNAME（管理）- Marketo Docs —— 产品文档自定义登陆页URL
title: 使用CNAME自定义登陆页URL（管理）
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---


# 使用CNAME自定义登陆页URL（管理） {#customize-your-landing-page-urls-with-a-cname-administration}

即使Marketo托管您的登陆页，也应为您的公司自定义URL。

>[!NOTE]
>
>**示例**
>
>无CNAME:
>
>http://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html
>
>品牌名称：
>
>http://go。**YourCompany**.com/UnsuscribePage.html

>[!NOTE]
>
>**需要管理员权限**

让我们帮你设置！

1. 选择CNAME

   它是URL的前部。 示例：

   * **go**.YourCompany.com/NameOfPage.html
   * **info**.YourCompany.com/NameOfPage.html
   * **页面**.YourCompany.com/NameOfPage.html

   单个词（加上YourCompany.com）称为CNAME。 你以后需要这个，记下来。

1. 查找帐户字符串
1. 转到“管 **理** ”区域并单击 **登陆页**。

   ![](assets/image2014-9-16-13-3a9-3a44.png)

1. 在**登陆页**选项卡下，从“设置”部分复制“帐户字符串”。

   ![](assets/image2014-9-16-13-3a9-3a57.png)

1. 稍后您还需要这个，请记下它。
1. 向IT部门发送请求
1. 请您的IT员工设置以下CNAME(将CNAME [和][ACCOUNT STRING替换为上一步] 中的文本):

   [CNAME].YourCompany.com > [ACCOUNT STRING].mktoweb.com

1. 完成CNAME设置
1. IT人员创建CNAME后，请转至“管 **理员** ”并单击 **登陆页**。

   ![](assets/image2014-9-16-13-3a10-3a14.png)

1. 在“设置 **”部** 分下，单击“ **编辑”**。

   ![](assets/image2014-9-16-13-3a10-3a31.png)

1. 在域名中输 **入登陆页的CNAME**，输 **入回退页面**，输入主 **页**，然后单 ****&#x200B;击保存。

   ![](assets/image2014-9-16-13-3a10-3a45.png)

   如果您的Marketo登陆页不可用，将在您的备用页面重定向人员。
干得好！ 您的登陆页现在与您的公司域一起添加品牌。

