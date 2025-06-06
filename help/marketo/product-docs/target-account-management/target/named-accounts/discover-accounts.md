---
unique-page-id: 11378812
description: 发现帐户 — Marketo文档 — 产品文档
title: 发现帐户
exl-id: 90da4ae0-0a12-48bd-8bae-a7431d2cf4f4
feature: Target Account Management
source-git-commit: dd4c8472ec3f453462bd8046daf70c89c587724a
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# 发现帐户 {#discover-accounts}

使用Discover选项确定潜在的目标帐户。

## 发现CRM帐户 {#discover-crm-accounts}

从CRM中确定潜在的目标帐户。

>[!NOTE]
>
>将CRM连接到Marketo TAM后，**发现CRM帐户**&#x200B;将显示所有CRM帐户和相关信息，以帮助您选择正确的命名帐户。 Marketo在从CRM收到的内容的基础上添加了其他信息。

**人员** (在发现CRM帐户和发现Marketo公司中)：包括联系人和潜在客户。 可以使用Marketo的[潜在客户与帐户匹配](/help/marketo/product-docs/target-account-management/target/named-accounts/lead-to-account-matching.md)来发现潜在客户。

**潜在人员** (在发现CRM帐户和发现Marketo公司中)：显示Marketo找到的可能属于CRM帐户的潜在客户数量。

**自定义CRM字段** （仅在发现CRM帐户中）：这将帮助您调整销售和营销组织，以便选择正确的目标帐户。 使用Marketo TAM [映射自定义CRM字段](/help/marketo/product-docs/target-account-management/setup-tam/create-a-custom-field-for-crm-discovery.md)后，我们将向您显示映射的数据以帮助您识别目标帐户。

1. 在指定帐户中，单击&#x200B;**新建**&#x200B;下拉列表，然后选择&#x200B;**发现CRM帐户**。

   ![](assets/disc-crm-one.png)

1. 此时将打开一个新窗口/选项卡。 选择要添加到指定帐户的CRM帐户，然后单击&#x200B;**下一步**。

   ![](assets/disc-crm-two.png)

1. 预览屏幕将确认您的选择数量。 单击&#x200B;**创建**。

   ![](assets/disc-three.png)

   就这么多！

   ![](assets/disc-four.png)

## 探索Marketo公司 {#discover-marketo-companies}

确定合适的公司以进行定位。

>[!NOTE]
>
>在发现Marketo公司中，您将看到并非来自您的CRM的Marketo公司。

1. 在指定帐户中，单击&#x200B;**新建**&#x200B;下拉列表，然后选择&#x200B;**发现Marketo公司**。

   ![](assets/one-1.png)

1. 此时将打开一个新窗口/选项卡。 选择要添加到指定帐户的公司，然后单击&#x200B;**下一步**。

   ![](assets/disc-comp-two.png)

   >[!NOTE]
   >
   >在发现Marketo公司和发现CRM中，Marketo会自动执行以下操作：
   >
   >* 从您的Marketo数据库中查找将其公司列入其记录的人员。 如果您看到某些属性（例如“行业”）的多个值，这是因为Marketo发现为这些单独人员列出的值不同。 命中次数最多的属性将获胜
   >
   >在&#x200B;**仅发现CRM**&#x200B;中，Marketo自动：
   >
   >* 将CRM联系人与指定帐户同步和关联
   >
   >在&#x200B;**仅发现Marketo公司**&#x200B;中，Marketo会自动：
   >
   >* 将大多数Internet服务提供商和公共域(例如yahoo.com、gmail.com)过滤为公司名称
   >
   >* 对CRM帐户进行重复数据删除。 如果您有一条记录中包含“Acme”和“Acme Inc”（或以下任一后缀： Co， Corp， Corporation， Gmbh， Inc， Incorporated， LLC， LLP， LP， Ltd， PA， PC， PLC， PLLC），我们将在TAM中将它们合并为“Acme”

1. 单击“Named Account（指定帐户）”列下的向下箭头以显示下拉列表。

   ![](assets/disc-comp-three.png)

   >[!CAUTION]
   >
   >今后，这些选定公司中的任何新员工都将自动分配到其各自的指定帐户。 请仔细检查这些公司，确保它们被分配到正确的指定帐户。

1. 要选择现有帐户，请单击&#x200B;**命名帐户**&#x200B;下拉列表，选择所需的帐户，然后单击&#x200B;**下一步**。

   ![](assets/disc-comp-four.png)

   您还可以选择直接在下拉框中键入所需的名称来创建新的指定帐户。 完成后，单击离开该框……

   ![](assets/disc-comp-five.png)

   ...您将会看到新的指定帐户。 此时，只需单击步骤4中的&#x200B;**下一步**。

   ![](assets/disc-comp-six.png)

1. 单击&#x200B;**创建**。

   ![](assets/disc-comp-seven.png)

   做得好！

   ![](assets/disc-co-six.png)

>[!NOTE]
>
>如果您看到所选的CRM帐户与发现CRM网格中的帐户不匹配，可能是由于以下一个或多个原因造成的：
>
>* 拥有名称相似但已删除重复数据的不同CRM帐户
>* 尚未进行下一次计划同步

>[!MORELIKETHIS]
>
>[潜在客户帐户匹配](/help/marketo/product-docs/target-account-management/target/named-accounts/lead-to-account-matching.md)
