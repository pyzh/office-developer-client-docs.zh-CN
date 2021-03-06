---
title: PreviewScope 单元格（“Document Properties”内容）
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
f1_keywords:
- Vis_DSS.chm820
localization_priority: Normal
ms.assetid: d03ae1b3-da6c-56d3-4f96-6e131c04e93e
description: 确定您的绘图是否包含预览。如果绘图中确实包含预览，则确定该预览是只显示绘图中的第一页还是显示所有页。
ms.openlocfilehash: 865da052f710481c146d3c2692ddf506018be789
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19780967"
---
# <a name="previewscope-cell-document-properties-section"></a>PreviewScope 单元格（“Document Properties”部分）

确定您的绘图是否包含预览。如果绘图中确实包含预览，则确定该预览是只显示绘图中的第一页还是显示所有页。
  
|**值**|**预览范围**|**自动常量**|
|:-----|:-----|:-----|
| 0  <br/> | 第一页  <br/> |**visDocPreviewScope1stPage** <br/> |
| 1  <br/> | 无  <br/> |**visDocPreviewScopeNone** <br/> |
| 2  <br/> | 所有页  <br/> |**visDocPreviewScopeAllPages** <br/> |
   
## <a name="remarks"></a>说明

您还可以在**属性**对话框中的**摘要**选项卡上设置此值 （单击**Office**按钮，单击**信息**选项卡，单击**文档属性**，然后单击**高级属性**）。
  
若要从另一个公式或使用 **CellsU** 属性从某个程序按名称获取对 PreviewScope 单元格的引用，请使用： 
  
|||
|:-----|:-----|
| 单元格名称：  <br/> | PreviewScope  <br/> |
   
若要从某个程序按索引获取对 PreviewScope 单元格的引用，请使用带下列参数的 **CellsSRC** 属性： 
  
|||
|:-----|:-----|
| 内容索引：  <br/> |**visSectionObject** <br/> |
| 行索引：  <br/> |**visRowDoc** <br/> |
| 单元格索引：  <br/> |**visDocPreviewScope** <br/> |
   

