---
title: Tip 单元格（“Controls”内容）
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
f1_keywords:
- vis_sdr.chm1010
localization_priority: Normal
ms.assetid: 7fd11650-fffa-1316-d302-3122ac5feb14
description: 表示说明性文本字符串，当用户将指针停留在形状的控制手柄之上时，说明性的文本字符串就作为工具提示显示出来。应用程序在单元格中自动用引号引起提示字符串，但引号不会在工具提示中显示出来。
ms.openlocfilehash: ff593ee95dc27ba7192ee31d35791127b666eac0
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19781533"
---
# <a name="tip-cell-controls-section"></a>Tip 单元格（“Controls”部分）

表示说明性文本字符串，当用户将指针停留在形状的控制手柄之上时，说明性的文本字符串就作为工具提示显示出来。应用程序在单元格中自动用引号引起提示字符串，但引号不会在工具提示中显示出来。
  
## <a name="remarks"></a>注释

要从另一个公式或从使用 **CellsU** 属性的某个程序按名称获取对 Tip 单元格的引用，请使用： 
  
|||
|:-----|:-----|
| 单元格名称：  <br/> | 控件。  *名称*。Tipwhere 控件。  *name*是控制行的名称。  <br/> |
   
要从某个程序按索引获取对 Tip 单元格的引用，请使用带下列参数的 **CellsSRC** 属性： 
  
|||
|:-----|:-----|
| 内容索引：  <br/> |**visSectionControls** <br/> |
| 行索引：  <br/> |**visRowControl** +  *i*其中*i* = 0、 1、 2...  <br/> |
| 单元格索引：  <br/> |**visCtlTip** <br/> |
   

