---
title: IsTextEditTarget 单元格（“Group Properties”内容）
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
f1_keywords:
- Vis_DSS.chm82251627
localization_priority: Normal
ms.assetid: 355cef8b-9213-479a-af95-b591f4bc51ad
description: 确定组合的文本分配。
ms.openlocfilehash: 65baf90254f6b213efea04739d8e4a66952b2856
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19780508"
---
# <a name="istextedittarget-cell-group-properties-section"></a>IsTextEditTarget 单元格（“Group Properties”部分）

确定组合的文本分配。
  
|**值**|**说明**|
|:-----|:-----|
|TRUE  <br/> |文本被添加到组合形状中。  <br/> |
|FALSE  <br/> |文本被添加到位于堆放顺序顶端的组合的形状中。  <br/> |
   
## <a name="remarks"></a>注解

您还可以采用以下方法设置此值：选择该组合，在[“开发工具”](run-in-developer-mode-display-the-developer-tab.md)选项卡上单击 **“行为”**，然后选中 **“编辑组合文本”** 复选框。 
  
在低于 Visio 2000 的版本中创建的组合的默认值为 FALSE。从 Visio 2000 版起，默认值为 TRUE。 
  
若要从另一个公式或使用 **CellsU** 属性从某个程序按名称获取对 IsTextEditTarget 单元格的引用，请使用： 
  
|||
|:-----|:-----|
|单元格名称：  <br/> |Istextedittarget 的值  <br/> |
   
若要从某个程序按索引获取对 IsTextEditTarget 单元格的引用，请使用带下列参数的 **CellsSRC** 属性： 
  
|||
|:-----|:-----|
|内容索引：  <br/> |**visSectionObject** <br/> |
|行索引：  <br/> |**visRowGroup** <br/> |
|单元格索引：  <br/> |**visGroupIsTextEditTarget** <br/> |
   

