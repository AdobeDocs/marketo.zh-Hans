---
unique-page-id: 11378812
description: 发现帐户 — Marketo文档 — 产品文档
title: 发现帐户
exl-id: 90da4ae0-0a12-48bd-8bae-a7431d2cf4f4
feature: Target Account Management
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 1%

---

# 发现帐户 {#discover-accounts}

使用Discover选项确定潜在的目标帐户。

## 发现CRM帐户 {#discover-crm-accounts}

从CRM中确定潜在目标帐户。

>[!NOTE]
>
>将CRM连接到Marketo TAM后， **发现CRM帐户** 将显示所有CRM帐户和相关信息，以帮助您选择正确的指定帐户。 Marketo在从CRM收到的内容的基础上添加了其他信息。

**人员** (在探索CRM帐户和探索Marketo公司中)：包括联系人和潜在客户。 可以使用Marketo发现潜在客户 [商机帐户匹配](/help/marketo/product-docs/target-account-management/target/named-accounts/lead-to-account-matching.md).

**潜在人员** (在发现CRM帐户和发现Marketo公司中)：显示Marketo找到了多少个可能属于CRM帐户的潜在客户。

**自定义CRM字段** （仅在发现CRM帐户中）：这将帮助您调整销售和营销组织，以便选择正确的目标帐户。 一旦您 [映射自定义CRM字段](/help/marketo/product-docs/target-account-management/setup-tam/create-a-custom-field-for-crm-discovery.md) 借助Marketo TAM，我们将向您显示映射的数据以帮助您识别目标帐户。

1. 在指定帐户中，单击 **新** 下拉菜单并选择 **发现CRM帐户**.

   ![](assets/disc-crm-one.png)

1. 将打开一个新窗口/选项卡。 选择要添加到指定帐户的CRM帐户，然后单击 **下一个**.

   ![](assets/disc-crm-two.png)

1. 预览屏幕确认您的选择数量。 单击&#x200B;**创建**。

   ![](assets/disc-three.png)

   就这么多！

   ![](assets/disc-four.png)

## 探索Marketo公司 {#discover-marketo-companies}

确定合适的公司以进行定位。

>[!NOTE]
>
>在发现Marketo公司中，您将看到并非来自您的CRM的Marketo公司。

1. 在指定帐户中，单击 **新** 下拉菜单并选择 **探索Marketo公司**.

   ![](assets/one-1.png)

1. 将打开一个新窗口/选项卡。 选择要添加到指定帐户的公司，然后单击 **下一个**.

   ![](assets/disc-comp-two.png)

   >[!NOTE]
   >
   >在发现Marketo公司和发现CRM中，Marketo会自动执行以下操作：
   >
   >* 从您的Marketo数据库中查找将其公司列在其记录中的人员。 如果您看到某些属性（例如“行业”）有多个值，这是因为Marketo发现为这些单独人员列出的值各不相同。 点击量最多的属性将获得成功
   >
   >In **发现CRM** 仅，Marketo会自动：
   >
   >* 将CRM联系人与指定帐户同步和关联
   >
   >In **探索Marketo公司** 仅，Marketo会自动：
   >
   >* 将大多数Internet服务提供商和公共域(例如yahoo.com、gmail.com)过滤为公司名称
   >
   >* 对CRM帐户进行重复数据删除。 如果某条记录中包含“Acme”和“Acme Inc”（或以下任一后缀：Co， Corp， Corporation， Gmbh， Inc， Incorporated， LLC， LLP， LP， Ltd， PA， PC， PLC， PLLC），我们会将它们作为“Acme”合并到TAM中
   >
   >如果您希望Marketo按CRM ID或帐户所有者而不是按公司名称来删除重复帐户，请联系 [Marketo支持](https://nation.marketo.com/t5/Support/ct-p/Support).

1. 单击“Named Account（指定帐户）”列下的向下箭头以显示下拉列表。

   ![](assets/disc-comp-three.png)

   >[!CAUTION]
   >
   >今后，这些选定公司中的任何新人员都将自动分配到其各自的指定帐户。 请仔细检查这些公司，确保将其分配到正确的指定帐户。

1. 要选择现有帐户，请单击 **指定帐户** 从下拉菜单中选择所需的帐户，然后单击 **下一个**.

   ![](assets/disc-comp-four.png)

   您还可以选择直接在下拉框中键入所需的名称来创建新的指定帐户。 完成后，单击离开该框……

   ![](assets/disc-comp-five.png)

   ...您将会看到新的指定帐户。 此时，只需单击 **下一个** 如步骤4中所示。

   ![](assets/disc-comp-six.png)

1. 单击&#x200B;**创建**。

   ![](assets/disc-comp-seven.png)

   做得不错！

   ![](assets/disc-co-six.png)

>[!NOTE]
>
>如果您选择的CRM帐户与发现CRM网格中的帐户不匹配，可能是由于以下一个或多个原因造成的：
>
>* 拥有名称相似但已删除重复数据的不同CRM帐户
>* 尚未进行下一次计划同步

>[!MORELIKETHIS]
>
>[商机帐户匹配](/help/marketo/product-docs/target-account-management/target/named-accounts/lead-to-account-matching.md)
