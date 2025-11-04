---
solution: Marketo Engage
product: marketo
title: 模板导入
description: 了解如何将现有电子邮件模板从经典编辑器导入新的电子邮件Designer。
level: Beginner, Intermediate
feature: Email Designer
badge: Beta 版
hide: true
hidefromtoc: true
source-git-commit: 3923ddfdffc21b5afd196c413bcf0ea3e2b806f5
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 1%

---

# 模板导入 {#template-import}

轻松地将现有电子邮件模板从经典编辑器导入到新的电子邮件Designer中，保留您的设计，并使用熟悉的可重用结构加快模板创建。 查看[最佳实践](#best-practices)并了解[限制和补救措施](#limitations-and-remedies)。

>[!NOTE]
>
>经典电子邮件模板是使用自由格式的HTML开发的，因此此导入程序可能并不总是完美导入每个组件。 请检查导入的模板，确保所有部分均可编辑并正确映射。 如果某个区域不可选，请重新创建它以获得最佳结果。

## 导入模板 {#import-a-template}

1. 转到&#x200B;**设计工作室**。

   ![](assets/import-template-1.png)

1. 单击&#x200B;**电子邮件模板**&#x200B;并选择&#x200B;**电子邮件模板（新）**。

   ![](assets/import-template-2.png)

1. 单击&#x200B;**创建模板**。

   ![](assets/import-template-3.png)

1. 输入&#x200B;_名称_&#x200B;和（可选）_描述_。

   ![](assets/import-template-4.png)

1. 单击&#x200B;**Marketo模板**&#x200B;选项卡，然后从在经典电子邮件编辑器中创建的现有模板中进行选择。

   ![](assets/import-template-5.png)

   >[!NOTE]
   >
   >只能导入与当前工作区共享的已批准模板和模板。

1. 单击&#x200B;**使用此模板**。

   ![](assets/import-template-6.png)

1. 导入的模板将在Email Designer中打开。

1. 查看组件以了解正确的转换，并使用Designer进行任何所需的调整。 如果您对模板满意，请批准它用于电子邮件。

## 创建片段 {#create-fragments}

最好创建可重复部分的片段以供将来使用。

1. 单击顶部的&#x200B;**...更多**&#x200B;按钮，然后选择&#x200B;**另存为片段**。

   ![](assets/import-template-7.png)

1. 选择组件或结构，然后单击&#x200B;**创建**。

   ![](assets/import-template-8.png)

1. 输入名称（和可选描述）并单击&#x200B;**保存**。

   ![](assets/import-template-9.png)

## 最佳实践 {#best-practices}

* 经典电子邮件模板是使用自由格式的HTML开发的，因此此导入程序可能并不总是完美导入每个组件。 请检查导入的模板，确保所有部分均可编辑并正确映射。 如果某个区域不可选，请重新创建它以获得最佳结果。

* 导入后，您可以将可重用的部分另存为片段，并批准它们以供电子邮件作者使用。 应用品牌主题以保持一致性和合规性。

* 您可以继续使用Velocity脚本，并考虑使用片段和条件内容的组合重新实施较旧的片段，以提高灵活性和控制力。

## 限制和补救措施 {#limitations-and-remedies}

<table><thead>
  <tr>
    <th>限制</th>
    <th>原因</th>
    <th>补救措施</th>
  </tr></thead>
<tbody>
  <tr>
    <td>在经典电子邮件编辑器中定义的变量在电子邮件级别不可用。</td>
    <td>这些变量最初旨在简化编辑器尚未提供WYSIWYG功能时的电子邮件编辑。 在Email Designer中，用户可以通过可用的控件实现类似的灵活性。 导入程序会维护现有模板的结构与组件，帮助您在电子邮件Designer中高效地重新创建模板。</td>
    <td>用户应该能够在Designer中实现此目标。 <p>
    对于模块，您可以将不同的区段另存为片段。 批准的片段将可用于电子邮件级别。</td>
  </tr>
  <tr>
    <td>如果源HTML包含嵌套块，则较深的层在Designer中不可寻址。</td>
    <td>电子邮件Designer不支持嵌套注释。</td>
    <td>即使Designer不允许编辑嵌套结构，它仍应准确呈现。 请务必先测试模板。<p>
    使用网格重新创建结构。</td>
  </tr>
  <tr>
    <td>有时，按钮会导入为包含文本的简单容器。</td>
    <td>在导入期间，可能会对使用HTML的某些实施样式进行错误解释。</td>
    <td>在Designer中重新创建按钮。</td>
  </tr>
  <tr>
    <td>按钮有时可能过大。</td>
    <td>Marketo电子邮件的CSS与其他较低级别元素(<code>&lt;span&gt;</code>)之间发生冲突</td>
    <td>尝试在Designer中调整按钮的边距和边距。</td>
  </tr>
  <tr>
    <td>项目符号本身不受支持。</td>
    <td>电子邮件Designer目前不提供项目符号。</td>
    <td>考虑使用替代技术重新创建项目符号。</td>
  </tr>
  <tr>
    <td>如果容器的内容与值属性值不一致，则垂直对齐会扭曲。</td>
    <td><code>valign</code> 在模板中定义的容器内不起作用。</td>
    <td>尝试在Email Designer中调整按钮的边距和边距。</td>
  </tr>
  <tr>
    <td>模板级别的程序级别Personalization令牌（我的令牌）可能会遇到验证错误。</td>
    <td>电子邮件模板不支持项目级令牌。</td>
    <td>将它们替换为模板中的其他令牌类型，并将它们替换为单个电子邮件中的“我的令牌”。</td>
  </tr>
  <tr>
    <td>分隔线组件可能不可选。</td>
    <td>分隔线组件未包含在发行版中。</td>
    <td>不适用</td>
  </tr>
  <tr>
    <td>如果原来的HTML有任何格式不正确的结构，则它们可能会被转移。</td>
    <td>原始HTML出现问题。</td>
    <td>在导入之前，需要修复这些问题。</td>
  </tr>
  <tr>
    <td>对于导入的内容，内容预览的使用不可靠。</td>
    <td>Designer的预览功能不支持自定义HTML。</td>
    <td>建议使用<b>模拟内容</b>屏幕中的<i>发送校样</i>选项测试电子邮件。</td>
  </tr>
  <tr>
    <td>旧模板中的代码片段在Email Designer中将不起作用。</td>
    <td>电子邮件Designer不支持代码片段。</td>
    <td>将片段重新创建为与条件内容结合的片段。</td>
  </tr>
</tbody></table>
