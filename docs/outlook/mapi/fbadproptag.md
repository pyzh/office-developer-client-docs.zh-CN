---
title: FBadPropTag
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FBadPropTag
api_type:
- HeaderDef
ms.assetid: 143bd3c6-5a55-4122-8522-9c48473aa781
description: 上次修改时间：2015 年 3 月 9 日
ms.openlocfilehash: d1503aaa5bddd23a90035219901e1dc232dbd026
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19774908"
---
# <a name="fbadproptag"></a>FBadPropTag

  
  
**适用于**： Outlook 
  
验证指定的属性标记。 
  
|||
|:-----|:-----|
|头文件：  <br/> |Mapival.h  <br/> |
|通过实现：  <br/> |MAPI  <br/> |
|调用：  <br/> |服务提供商  <br/> |
   
```cpp
ULONG FBadPropTag(
  ULONG ulPropTag
);
```

## <a name="parameters"></a>参数

 _ulPropTag_
  
> [in]要验证属性标记。
    
## <a name="return-value"></a>返回值

TRUE 
  
> 指定的属性标记不是有效的 MAPI 属性标记。 
    
FALSE 
  
> 指定的属性标记是一个有效的 MAPI 属性标记。
    
## <a name="remarks"></a>说明

**FBadPropTag**函数验证基于 MAPI 定义的指定的属性标记。 它使的 sures 属性类型之一的 MAPI 所定义的类型和属性标识符定义的类型。 
  
## <a name="see-also"></a>另请参阅



[FBadProp](fbadprop.md)

