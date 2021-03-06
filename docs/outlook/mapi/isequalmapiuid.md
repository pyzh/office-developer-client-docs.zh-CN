---
title: IsEqualMAPIUID
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MAPI.IsEqualMAPIUID
api_type:
- COM
ms.assetid: 85d71b73-0630-4c5d-b0e3-b48d27a300d0
description: 上次修改时间：2015 年 3 月 9 日
ms.openlocfilehash: 635a4a872b83a2996b1a0198975a0ecd2cd906eb
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19776072"
---
# <a name="isequalmapiuid"></a>IsEqualMAPIUID

  
  
**适用于**： Outlook 
  
测试两个[MAPIUID](mapiuid.md)结构，以确定它们是否包含相同的标识符。 
  
|||
|:-----|:-----|
|头文件：  <br/> |Mapidefs.h  <br/> |
|相关的结构：  <br/> |**MAPIUID** <br/> |
   
```cpp
IsEqualMAPIUID(lpuid1, lpuid2)
```

## <a name="parameters"></a>参数

 _lpuid1_
  
> 要测试的第一个**MAPIUID**结构的指针。 
    
 _lpuid2_
  
> 指向要测试的第二个**MAPIUID**结构的指针。 
    
## <a name="remarks"></a>说明

如果两个**MAPIUID**结构包含相同标识符和 FALSE，如果未显示， **IsEqualMAPIUID**宏返回 TRUE。 
  
**IsEqualMAPIUID**宏要求的头文件 Memory.h 包含。 
  
## <a name="see-also"></a>另请参阅



[MAPIUID](mapiuid.md)


[与结构相关的宏](macros-related-to-structures.md)

