---
title: LineJumpFactorX 单元格（“Page Layout”内容）
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
f1_keywords:
- vis_sdr.chm545
localization_priority: Normal
ms.assetid: 0649672f-f496-ce80-6dc3-3affc9b6f913
description: 确定页中水平动态连接线上跨线的大小（相对于 LineToLineX 单元格的值）。该单元格的值范围可介于 0 到 10 之间，但建议使用 0 到 1 之间的小数值。
ms.openlocfilehash: fb6205407070485a0e234ee594e84979bca40891
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19780566"
---
# <a name="linejumpfactorx-cell-page-layout-section"></a>LineJumpFactorX 单元格（“Page Layout”部分）

确定页中水平动态连接线上跨线的大小（相对于 LineToLineX 单元格的值）。该单元格的值范围可介于 0 到 10 之间，但建议使用 0 到 1 之间的小数值。
  
## <a name="remarks"></a>注解

还可以在 **“页面设置”** 对话框中的 **“布局与排列”** 选项卡（在 **“设计”** 选项卡上，单击 **“页面设置”** 箭头，然后单击 **“布局与排列”**）上设置此单元格的值。
  
若要从另一个公式或使用 **CellsU** 属性从某个程序按名称获取对 LineJumpFactorX 单元格的引用，请使用： 
  
|||
|:-----|:-----|
|单元格名称：  <br/> |LineJumpFactorX  <br/> |
   
若要从某个程序按索引获取对 LineJumpFactorX 单元格的引用，请使用带下列参数的 **CellsSRC** 属性： 
  
|||
|:-----|:-----|
|内容索引：  <br/> |**visSectionObject** <br/> |
|行索引：  <br/> |**visRowPageLayout** <br/> |
|单元格索引：  <br/> |**visPLOJumpFactorX** <br/> |
   

