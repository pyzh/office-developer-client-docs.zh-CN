---
title: 关于 ShapeSheet 电子表格
manager: soliver
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
f1_keywords:
- Vis_DSS.chm82251822
localization_priority: Normal
ms.assetid: f403890d-4a3a-bacc-53d7-1b9920b23639
description: Microsoft Visio 中的每个元素（每个文档、绘图页、样式、形状、组合、组合中的形状或对象、主控形状、来自其他程序的对象、参考线以及辅助点）都具有用来保存与该对象有关的信息的 ShapeSheet 电子表格。此电子表格包含诸如高度、宽度、角度、颜色以及其他决定形状的外观和行为的属性信息。
ms.openlocfilehash: f443a596174ac4a555d53a271372e73367197da0
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19779605"
---
# <a name="about-the-shapesheet-spreadsheet"></a><span data-ttu-id="cd8d3-104">关于 ShapeSheet 电子表格</span><span class="sxs-lookup"><span data-stu-id="cd8d3-104">About the ShapeSheet Spreadsheet</span></span>

<span data-ttu-id="cd8d3-p102">Microsoft Visio 中的每个元素（每个文档、绘图页、样式、形状、组合、组合中的形状或对象、主控形状、来自其他程序的对象、参考线以及辅助点）都具有用来保存与该对象有关的信息的 ShapeSheet 电子表格。此电子表格包含诸如高度、宽度、角度、颜色以及其他决定形状的外观和行为的属性信息。</span><span class="sxs-lookup"><span data-stu-id="cd8d3-p102">Everything in Microsoft Visio, every document, page, style, shape, group, shape or object within a group, master, object from another program, guide, and guide point, has a ShapeSheet spreadsheet where information about that object is stored. This spreadsheet contains information such as height, width, angle, color, and other attributes that determine the shape's appearance and behavior.</span></span>
  
<span data-ttu-id="cd8d3-p103">作为一名形状开发人员，您需要精确控制所创建的形状的外观和行为。您可以通过在形状的 ShapeSheet 中编辑它来改变其默认行为并增强其功能，可通过 ShapeSheet 窗口或以编程的方式访问该电子表格。</span><span class="sxs-lookup"><span data-stu-id="cd8d3-p103">As a shape developer, you need precise control over the appearance and behavior of the shapes you create. You can change a shape's default behavior and enhance what it can do by editing it in its ShapeSheet, which you can access in a ShapeSheet window or programmatically.</span></span>
  
## <a name="viewing-an-object-in-a-shapesheet-window"></a><span data-ttu-id="cd8d3-109">在 ShapeSheet 窗口中查看对象</span><span class="sxs-lookup"><span data-stu-id="cd8d3-109">Viewing an object in a ShapeSheet window</span></span>

<span data-ttu-id="cd8d3-110">Visio 绘图窗口和 ShapeSheet 窗口只不过是同一形状的不同视图。</span><span class="sxs-lookup"><span data-stu-id="cd8d3-110">The Visio drawing window and ShapeSheet window are simply different views of the same shape.</span></span>
  
- <span data-ttu-id="cd8d3-111">当您在绘图窗口中查看一个形状时，您看到的是根据其 ShapeSheet 中的公式显示的图形外观和行为。</span><span class="sxs-lookup"><span data-stu-id="cd8d3-111">When you view a shape in a drawing window, you see it rendered graphically and behaving according to the formulas in its ShapeSheet.</span></span>
    
- <span data-ttu-id="cd8d3-112">当您在 ShapeSheet 窗口中查看一个形状时，您将看到决定其在绘图页上的外观和行为的基本公式。</span><span class="sxs-lookup"><span data-stu-id="cd8d3-112">When you view a shape in a ShapeSheet window, you see the underlying formulas that determine how it looks and behaves on the drawing page.</span></span>
    
<span data-ttu-id="cd8d3-p104">您可以同时查看 ShapeSheet 窗口和绘图窗口，并且当您在 ShapeSheet 窗口中操作单元格时，可以看到绘图窗口中的形状发生相应变化，反之亦然。例如，当您使用指针移动形状时，“Shape Transform”内容中形状的 PinX 和 PinY 公式会发生改变，以反映形状在绘图页上的新位置。</span><span class="sxs-lookup"><span data-stu-id="cd8d3-p104">You can view a ShapeSheet window and a drawing window simultaneously and see the shape change in the drawing window as you manipulate cells in its ShapeSheet window or vice versa. For example, when you move the shape with the pointer, the shape's PinX and PinY formulas in the Shape Transform section change to reflect its new position on the drawing page.</span></span>
  
## <a name="structure-of-the-shapesheet-window"></a><span data-ttu-id="cd8d3-115">ShapeSheet 窗口的结构</span><span class="sxs-lookup"><span data-stu-id="cd8d3-115">Structure of the ShapeSheet window</span></span>

<span data-ttu-id="cd8d3-116">ShapeSheet 分为*部分*的控制某个特定方面的形状的行为或外观，例如，及其几何图形或格式设置。</span><span class="sxs-lookup"><span data-stu-id="cd8d3-116">A ShapeSheet is divided into  *sections*  that control a particular aspect of a shape's behavior or appearance, for example, its geometry or its formatting.</span></span> <span data-ttu-id="cd8d3-117">每个部分包含*单元格*包含一个或多个*行*。</span><span class="sxs-lookup"><span data-stu-id="cd8d3-117">Each section contains one or more  *rows*  that contain  *cells*  .</span></span> <span data-ttu-id="cd8d3-118">每个单元格包含公式，其 （通常名为单元格的值） 的结果和可选的错误信息。</span><span class="sxs-lookup"><span data-stu-id="cd8d3-118">Each cell can contain a formula, its result (commonly called the cell value), and optional error information.</span></span> <span data-ttu-id="cd8d3-119">公式可能必需或可选的具体取决于特定单元格。</span><span class="sxs-lookup"><span data-stu-id="cd8d3-119">A formula may be required or optional, depending on the particular cell.</span></span> <span data-ttu-id="cd8d3-120">单元格的数据 （例如，其公式或值） 可能是本地定义或者，更频繁地继承自中形状的主控形状或样式的等效单元格。</span><span class="sxs-lookup"><span data-stu-id="cd8d3-120">A cell's data (for example, its formula or value) may be locally defined or, more often, inherited from the equivalent cell in the shape's master or style.</span></span> 
  
<span data-ttu-id="cd8d3-121">以下示例显示了 ShapeSheet 窗口中的公式栏</span><span class="sxs-lookup"><span data-stu-id="cd8d3-121">The following example shows the formula bar</span></span> ![数字 1](media/callout1_ZA01036259.gif)<span data-ttu-id="cd8d3-123">、内容</span><span class="sxs-lookup"><span data-stu-id="cd8d3-123">, a section</span></span> ![数字 2](media/callout2_ZA01036260.gif)<span data-ttu-id="cd8d3-125">、单元格</span><span class="sxs-lookup"><span data-stu-id="cd8d3-125">, a cell</span></span> ![数字 3](media/callout3_ZA01036261.gif)<span data-ttu-id="cd8d3-127">和行</span><span class="sxs-lookup"><span data-stu-id="cd8d3-127">, and a row</span></span> ![数字 4](media/callout4_ZA01036262.gif) <span data-ttu-id="cd8d3-129">。</span><span class="sxs-lookup"><span data-stu-id="cd8d3-129">in the ShapeSheet window.</span></span> 
  
![](media/ShpSheetRef_CA_02a_ZA07645861.gif)
  
<span data-ttu-id="cd8d3-130">时绘制形状，Visio 将记录作为集合的水平和垂直位置与线段连接的形状。</span><span class="sxs-lookup"><span data-stu-id="cd8d3-130">When you draw a shape, Visio records the shape as a collection of horizontal and vertical locations connected with line segments.</span></span> <span data-ttu-id="cd8d3-131">这些位置 （称为顶点） 记录在 X 和 Y 单元格的形状的**geometry**内容中。</span><span class="sxs-lookup"><span data-stu-id="cd8d3-131">These locations (called vertices) are recorded in the X and Y cells of the shape's **Geometry** section.</span></span> <span data-ttu-id="cd8d3-132">下面的示例中所示，当您单击形状的 ShapeSheet 窗口的**geometry**内容中的 X 和 Y 单元格时，您将看到黑色界定框中，突出显示在绘图窗口中的形状的顶点。</span><span class="sxs-lookup"><span data-stu-id="cd8d3-132">As shown in the following example, when you click the X and Y cells in the **Geometry** section of a shape's ShapeSheet window, you will see a black-bordered box highlighting the vertex on the shape in the drawing window.</span></span> 
  
![](media/ShpSheetRef_CA_01_ZA07645860.gif)
  
## <a name="editing-an-object-in-the-shapesheet-window"></a><span data-ttu-id="cd8d3-133">在 ShapeSheet 窗口中编辑对象</span><span class="sxs-lookup"><span data-stu-id="cd8d3-133">Editing an object in the ShapeSheet window</span></span>

<span data-ttu-id="cd8d3-p107">当 ShapeSheet 窗口处于活动状态时，功能区将改为显示在该窗口中工作时特定的选项。选择一个 ShapeSheet 单元格后，将会出现一个公式栏，您可以用它输入和编辑对象的公式。或者，您可以直接在该单元格中工作。</span><span class="sxs-lookup"><span data-stu-id="cd8d3-p107">When a ShapeSheet window is active, the ribbon changes to display options specific to working in this window. When you select a ShapeSheet cell, a formula bar appears, which you can use to enter and edit an object's formulas. Or, you can work directly in the cell.</span></span>
  
<span data-ttu-id="cd8d3-137">在 ShapeSheet 窗口中，您可以添加节到形状的工作表添加到绘图页上的形状的新特征。</span><span class="sxs-lookup"><span data-stu-id="cd8d3-137">In a ShapeSheet window, you can add sections to a shape's sheet to add new characteristics to the shape on the drawing page.</span></span> <span data-ttu-id="cd8d3-138">例如，您可以添加**Connection** points 创建的连接。</span><span class="sxs-lookup"><span data-stu-id="cd8d3-138">For example, you can add a **Connection Points** section to create a connection.</span></span> <span data-ttu-id="cd8d3-139">当不再需要一节时，您可以将其删除。</span><span class="sxs-lookup"><span data-stu-id="cd8d3-139">When you no longer need a section, you can delete it.</span></span> 
  
<span data-ttu-id="cd8d3-140">您还可以添加行于节保存附加公式或更改形状的外观。</span><span class="sxs-lookup"><span data-stu-id="cd8d3-140">You also can add rows to sections to hold additional formulas or to change a shape's appearance.</span></span> <span data-ttu-id="cd8d3-141">例如，您可以将行添加到**geometry**内容添加到形状的一段。</span><span class="sxs-lookup"><span data-stu-id="cd8d3-141">For example, you can add a row to a **Geometry** section to add a segment to a shape.</span></span> <span data-ttu-id="cd8d3-142">同样，您可以删除不再需要的行。</span><span class="sxs-lookup"><span data-stu-id="cd8d3-142">Similarly, you can delete rows you no longer need.</span></span> 
  
<span data-ttu-id="cd8d3-p110">您可以在单元格中显示公式或者值。在输入新公式、编辑现有公式或查看单元格中公式的相互关系时，显示公式。值是 Visio 对单元格的公式求值后得到的结果。您可以显示单元格中的值以便查看求值结果。</span><span class="sxs-lookup"><span data-stu-id="cd8d3-p110">You can display either formulas or values in cells. Display formulas when you are entering new formulas, editing existing formulas, or to see how formulas in cells relate to each other. A value is the result you get when Visio evaluates a cell's formula. You can display values in cells to see the result of an evaluation.</span></span>
  
## <a name="additional-shapesheet-references"></a><span data-ttu-id="cd8d3-147">其他 ShapeSheet 引用</span><span class="sxs-lookup"><span data-stu-id="cd8d3-147">Additional ShapeSheet references</span></span>

<span data-ttu-id="cd8d3-148">有关特定内容、 行或单元格 ShapeSheet 中的详细信息，此[ShapeSheet 参考](reference-visio-shapesheet.md)中查看相应文章。</span><span class="sxs-lookup"><span data-stu-id="cd8d3-148">For details on a particular section, row, or cell in the ShapeSheet, view the corresponding article in this [ShapeSheet Reference](reference-visio-shapesheet.md).</span></span>
  
<span data-ttu-id="cd8d3-149">有关以编程方式访问 ShapeSheet 电子表格的详细信息，请参阅“Microsoft Visio 自动化参考”。</span><span class="sxs-lookup"><span data-stu-id="cd8d3-149">For details on programmatically accessing the ShapeSheet spreadsheet, see the Microsoft Visio Automation Reference.</span></span>
  
