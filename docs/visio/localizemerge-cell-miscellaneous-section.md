---
title: LocalizeMerge 单元格（“Miscellaneous”内容）
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
f1_keywords:
- Vis_DSS.chm1033773
localization_priority: Normal
ms.assetid: 734d4415-05dd-4c4d-763e-e035fa56dcec
description: 确定在文档间复制时是否本地化形状。
ms.openlocfilehash: 47593802e412c1871685f7218dd2a810bc2bc469
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19780599"
---
# <a name="localizemerge-cell-miscellaneous-section"></a>LocalizeMerge 单元格（“Miscellaneous”部分）

确定在文档间复制时是否本地化形状。
  
|**值**|**说明**|
|:-----|:-----|
| TRUE  <br/> | 使用目标文档的语言本地化形状。  <br/> |
| FALSE  <br/> | 不本地化形状基于目标文档 （默认值） 的语言。  <br/> |
   
## <a name="remarks"></a>说明

要从另一个公式或从使用 **CellsU** 属性的某个程序按名称获取对 LocalizeMerge 单元格的引用，请使用： 
  
|||
|:-----|:-----|
| 单元格名称：  <br/> | LocalizeMerge  <br/> |
   
要从某个程序按索引获取对 LocalizeMerge 单元格的引用，请使用带下列参数的 **CellsSRC** 属性： 
  
|||
|:-----|:-----|
| 内容索引：  <br/> |**visSectionObject** <br/> |
| 行索引：  <br/> |**visRowMisc** <br/> |
| 单元格索引：  <br/> |**visObjLocalizeMerge** <br/> |
   

