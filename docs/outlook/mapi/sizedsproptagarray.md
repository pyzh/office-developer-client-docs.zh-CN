---
title: SizedSPropTagArray
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MAPI.SizedSPropTagArray
api_type:
- COM
ms.assetid: 1d2dc6e9-735d-4b5b-af6f-adf6a32a666d
description: 上次修改时间：2015 年 3 月 9 日
ms.openlocfilehash: 7505c5dbcfc98a8b868424ae51cbe9c47b1d4338
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19778799"
---
# <a name="sizedsproptagarray"></a>SizedSPropTagArray

**适用于**： Outlook 
  
创建命名的[SPropTagArray](sproptagarray.md)结构，其中包含指定的数目的属性标记。 
  
|||
|:-----|:-----|
|头文件：  <br/> |Mapidefs.h  <br/> |
|相关的结构：  <br/> |**SPropTagArray** <br/> |
   
```cpp
SizedSPropTagArray (_ctag, _name)
```

## <a name="parameters"></a>参数

__ctag_
  
> 要包含在新结构属性标记的计数。
    
__名称_
  
> 新结构的的名称。
    
## <a name="remarks"></a>说明

使用**SizedSPropTagArray**宏来使用显式边界创建属性标记数组。 
  
若要使用新结构的结果从**SizedSPropTagArray**宏作为指针指向**SPropTagArray**结构，执行下列转换： 
  
```cpp
lpPropTagArray = (LPPropTagArray) &SizedSPropTagArray;

```

## <a name="see-also"></a>另请参阅

- [SPropTagArray](sproptagarray.md)
- [与结构相关的宏](macros-related-to-structures.md)

