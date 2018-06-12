---
title: 实现 IUnknown 接口
manager: soliver
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
api_type:
- COM
ms.assetid: 01bba63b-a2a1-490e-8b78-5c9ba8d9547b
description: 上次修改时间： 2011 年 7 月 23 日
ms.openlocfilehash: 55bf8831af8f78767b2607c21ab54c32f6e4245f
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19775830"
---
# <a name="implementing-the-iunknown-interface"></a>实现 IUnknown 接口

  
  
**适用于**： Outlook 
  
[IUnknown](http://msdn.microsoft.com/en-us/library/ms680509%28v=VS.85%29.aspx)接口中每个 MAPI 对象，, 实现的方法支持 interobject 通信和对象管理。 
  
 **IUnknown**具有三个方法： [IUnknown::AddRef](http://msdn.microsoft.com/en-us/library/ms691379%28v=VS.85%29.aspx)、 [IUnknown::QueryInterface](http://msdn.microsoft.com/en-us/library/ms682521%28v=VS.85%29.aspx)和[IUnknown::Release](http://msdn.microsoft.com/en-us/library/ms682317%28v=VS.85%29.aspx)。 **QueryInterface**启用一个对象，以确定另一个对象是否支持特定的接口。 与**QueryInterface**，事先不了解彼此的功能与两个对象可以进行交互。 如果实现**QueryInterface**的对象不支持问题的接口，它将返回的实现的接口的指针。 如果对象不支持所请求的接口，则返回的 MAPI_E_INTERFACE_NOT_SUPPORTED 值。 
  
当**QueryInterface**返回请求的接口指针时，它还必须增加新对象的引用计数。 对象的引用计数是用于管理对象的生命周期的数值。 当引用计数大于 1 时，因为正在使用它无法释放对象的内存。 它是仅当引用计数降至 0 对象可以安全地释放。 
  
其他两个**IUnknown**方法， **AddRef**和**Release**，管理引用计数。 **AddRef**增加引用计数，**版本**递减时它。 所有方法或 API 函数的返回接口的指针，如**QueryInterface**，必须都调用**AddRef**以增加引用计数。 接收接口指针的方法的所有实现必须都调用**Release**递减计数，当不再需要将指针。 **版本**检查现有的引用计数，仅当在计数为 0 与接口关联所内存。 
  
> [!NOTE]
> 由于无需**AddRef**和**Release**返回正确的值，这些方法的调用方不必须使用的返回值来确定对象是否仍然有效或已损坏。 
  
## <a name="see-also"></a>另请参阅



[实现 MAPI 对象](implementing-mapi-objects.md)
