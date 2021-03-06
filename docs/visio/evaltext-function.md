---
title: EVALTEXT 函数
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
f1_keywords:
- Vis_DSS.chm82251422
localization_priority: Normal
ms.assetid: c9b5b96c-d8c8-6119-e3f1-a2ce9d7c043e
description: 评估 shapename 中文就像它已公式并返回结果。
ms.openlocfilehash: 69e79a23faa9d09aa2ad51f83363064b54742152
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19780196"
---
# <a name="evaltext-function"></a>EVALTEXT 函数

评估_shapename_中文就像它已公式并返回结果。 
  
## <a name="syntax"></a>语法

EVALTEXT (* * *shapename ！ theText* * *) 
  
### <a name="parameters"></a>参数

|**名称**|**必需/可选**|**数据类型**|**说明**|
|:-----|:-----|:-----|:-----|
| _shapename ！ theText_ <br/> |必需  <br/> |**字符串** <br/> |当关联形状的文本构成改变时触发的单元格。  <br/> |
   
### <a name="return-value"></a>返回值

字符串
  
## <a name="remarks"></a>说明

 _shapename_ 可用来指代某形状（不是当前形状）的文本。 
  
如果没有文本，则结果为零。如果无法对文本求值，则该函数将返回错误。
  
## <a name="example"></a>示例

EVALTEXT(Line.2!theText) 
  
对形状 Line.2 中包含的文本求值。例如，如果 Line.2 包含“4 ft + 0.5 ft”，则返回的值为 4.5 ft。 
  

