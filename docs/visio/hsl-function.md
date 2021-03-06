---
title: HSL 函数
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
f1_keywords:
- Vis_DSS.chm82251438
localization_priority: Normal
ms.assetid: c9314c39-1d2e-a18f-c01b-8817286099dc
description: 返回一个值，表示在文档的调色板中的索引。 指定由其色调、 饱和度和发光度组件组成的颜色。
ms.openlocfilehash: 50f343d990157d831ac4ac43057d0a2b7fca63f0
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19780412"
---
# <a name="hsl-function"></a>HSL 函数

返回一个值，表示在文档的调色板中的索引。 指定由其色调、 饱和度和发光度组件组成的颜色。
  
## <a name="syntax"></a>语法

HSL (* **色调** *，* **饱和度** *，* **发光度** *) 
  
### <a name="parameters"></a>参数

|**名称**|**必需/可选**|**数据类型**|**说明**|
|:-----|:-----|:-----|:-----|
| _色调_ <br/> |必需  <br/> |**编号** <br/> |颜色的色调，表示为 0 至 239 之间的数字（包括 0 和 239），或可计算出此类数值的表达式。  <br/> |
| _饱和度_ <br/> |必需  <br/> |**编号** <br/> |颜色的饱和度，表示为 0 至 240 之间的数字（包括 0 和 240），或可计算出此类数值的表达式。  <br/> |
| _发光度_ <br/> |必需  <br/> |**编号** <br/> | 颜色的发光度，表示为 0 至 240 之间的数字（包括 0 和 240），或可计算出此类数值的表达式。  <br/> |
   
### <a name="return-value"></a>返回值

Number
  
## <a name="remarks"></a>注解

如果该函数返回的颜色在当前文档的调色板中尚不存在，则它将添加到该文档的可用颜色列表中。 
  
下表列出了一些标准颜色，以及它们的色调、饱和度和发光度的值。 
  
|**颜色**|**色调值**|**饱和度值**|**发光度值**|
|:-----|:-----|:-----|:-----|
|黑色  <br/> |0  <br/> |0  <br/> |24  <br/> |
|蓝色  <br/> |160  <br/> |240  <br/> |120  <br/> |
|绿色  <br/> |80  <br/> |240  <br/> |120  <br/> |
|蓝绿色  <br/> |120  <br/> |240  <br/> |120  <br/> |
|红色  <br/> |0  <br/> |240  <br/> |120  <br/> |
|洋红色  <br/> |200  <br/> |240  <br/> |120  <br/> |
|黄色  <br/> |40  <br/> |240  <br/> |120  <br/> |
|白色  <br/> |0  <br/> |0  <br/> |240  <br/> |
   
## <a name="example-1"></a>示例 1

HSL(160,240,120)
  
返回蓝色的索引值。
  
## <a name="example-2"></a>示例 2

HSL(HUE(FillForegnd),SAT(FillForegnd),MIN(LUM(FillForegnd)+100,240))
  
返回一种颜色的索引值，该颜色比填充前景色的发光度高。
  

