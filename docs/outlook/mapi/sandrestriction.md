---
title: SAndRestriction
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MAPI.SAndRestriction
api_type:
- COM
ms.assetid: 1b7dfe87-f87f-43e3-8332-a0d9c3f70d16
description: 上次修改时间：2015 年 3 月 9 日
ms.openlocfilehash: 1437130caecd57344fc171d234c5391ea92e1d4b
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19778681"
---
# <a name="sandrestriction"></a>SAndRestriction

  
  
**适用于**： Outlook 
  
描述**和**限制，用来加入一组使用的逻辑**和**操作的限制。 
  
|||
|:-----|:-----|
|头文件：  <br/> |Mapidefs.h  <br/> |
   
```cpp
typedef struct _SAndRestriction
{
  ULONG cRes;
  LPSRestriction lpRes;
} SAndRestriction;

```

## <a name="members"></a>Members

 **cRes**
  
> 由**lpRes**成员指向搜索限制数组中的计数。 
    
 **lpRes**
  
> 指向将合并在一起的逻辑**和**操作的[SRestriction](srestriction.md)结构的数组。 
    
## <a name="remarks"></a>说明

如果及其所有子限制的计算都结果为 TRUE，则**SAndRestriction**的结果为 TRUE。 如果任何子限制的计算结果为 FALSE，则为 FALSE。 
  
有关的类型的限制，说明如何构建其和示例代码，请参阅[有关限制](about-restrictions.md)。
  
## <a name="see-also"></a>另请参阅



[SRestriction](srestriction.md)


[MAPI 结构](mapi-structures.md)

