---
title: PROP_TAG
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MAPI.PROP_TAG
api_type:
- COM
ms.assetid: d8c9d18c-4043-41f3-8501-8be8e3a2c9ac
description: 上次修改时间：2015 年 3 月 9 日
ms.openlocfilehash: 9e53c39b713aa782eb387b85667f5ded6193006f
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19778551"
---
# <a name="proptag"></a>PROP_TAG

**适用于**： Outlook 
  
返回属性标记创建的组合指定的属性类型和标识符。 
  
|||
|:-----|:-----|
|头文件：  <br/> |Mapidefs.h  <br/> |
|相关的结构：  <br/> |[SPropValue](spropvalue.md) <br/> |
   
```cpp
PROP_TAG (ulPropType, ulPropID)
```

## <a name="parameters"></a>参数

_ulPropType_
  
> 新属性标记的属性类型。
    
_ulPropID_
  
> 新属性标记属性标识符。
    
## <a name="remarks"></a>说明

**属性\_标记**宏创建类型_ulPropType_和_ulPropID_中指定的标识符的属性的属性标记。 例如，可以通过，如下所示使用**PROP_TAG**宏创建的项标识符的属性标记： 
  
```cpp
PROP_TAG( PT_BINARY, 0x0FFF)

```

低序位 16 位的返回的属性标记包含属性类型，PT_BINARY，但高阶 16 位包含属性标识符，0xFFFF。
  
有关属性标记的详细信息，请参阅[MAPI 属性标记](mapi-property-tags.md)。
  
## <a name="see-also"></a>另请参阅

- [SPropValue](spropvalue.md)
- [与结构相关的宏](macros-related-to-structures.md)

