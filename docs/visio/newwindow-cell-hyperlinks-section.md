---
title: NewWindow 单元格（“Hyperlinks”内容）
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
f1_keywords:
- Vis_DSS.chm695
localization_priority: Normal
ms.assetid: 44995137-d241-937a-c097-0f9d79203cdf
description: 指定是否在新窗口中打开超链接。
ms.openlocfilehash: b4d927e1970e994047df3cb89afa7799a825511d
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19780788"
---
# <a name="newwindow-cell-hyperlinks-section"></a>NewWindow 单元格（“Hyperlinks”部分）

指定是否在新窗口中打开超链接。
  
|**值**|**说明**|
|:-----|:-----|
| TRUE  <br/> | 在新窗口中打开链接的页、文档或网站。  <br/> |
| FALSE  <br/> | 默认值。不为超链接打开新窗口。  <br/> |
   
## <a name="remarks"></a>注释

要从另一个公式或从使用 **CellsU** 属性的某个程序按名称获取对 NewWindow 单元格的引用，请使用： 
  
|||
|:-----|:-----|
| 单元格名称：  <br/> | 超链接。  *名称*。NewWindow 其中超链接。  *Name*是行名称  <br/> |
   
要从某个程序按索引获取对 NewWindow 单元格的引用，请使用带下列参数的 **CellsSRC** 属性： 
  
|||
|:-----|:-----|
| 内容索引：  <br/> |**visSectionHyperlink** <br/> |
| 行索引：  <br/> |**visRow1stHyperlink** +  *i*其中*i* = 0、 1、 2...  <br/> |
| 单元格索引：  <br/> |**visHLinkNewWin** <br/> |
   

