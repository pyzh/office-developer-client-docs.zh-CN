---
title: 使用 C++ 实现 IUnknown
manager: soliver
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
api_type:
- COM
ms.assetid: 68519f6c-fba8-47f5-9401-316e276f770e
description: 上次修改时间： 2011 年 7 月 23 日
ms.openlocfilehash: c899eb0afd123b26e12081f5157be3bae7917813
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19775813"
---
# <a name="implementing-iunknown-in-c"></a>使用 C++ 实现 IUnknown

**适用于**： Outlook 
  
在 c + + 中实现的[IUnknown](http://msdn.microsoft.com/en-us/library/ms680509%28v=VS.85%29.aspx)接口[IUnknown::QueryInterface](http://msdn.microsoft.com/en-us/library/ms682521%28v=VS.85%29.aspx)、 [IUnknown::AddRef](http://msdn.microsoft.com/en-us/library/ms691379%28v=VS.85%29.aspx)和[IUnknown::Release](http://msdn.microsoft.com/en-us/library/ms682317%28v=VS.85%29.aspx)方法是相当简单。 后的参数中传递的一些标准验证， **QueryInterface**实现检查的受支持接口的列表对请求的接口的标识符。 如果之间所支持的请求的标识符， **AddRef**称为，则返回**此**指针。 如果请求的标识符不在受支持的列表中，将输出指针设置为 NULL，并返回 MAPI_E_INTERFACE_NOT_SUPPORTED 值。 
  
下面的代码示例演示如何实现**QueryInterface** c + + 中对于状态对象，一个对象，它的一个子类[IMAPIStatus: IMAPIProp](imapistatusimapiprop.md)接口。 **IMAPIStatus**继承通过的**IUnknown** [IMAPIProp: IUnknown](imapipropiunknown.md)。 因此，如果呼叫者要求的任何这些接口，**该**指针可以返回，因为通过继承相关的接口。 
  
```cpp
HRESULT CMyMAPIObject::QueryInterface (REFIID   riid,
                                       LPVOID * ppvObj)
{
    // Always set out parameter to NULL, validating it first.
    if (!ppvObj)
        return E_INVALIDARG;
    *ppvObj = NULL;
    if (riid == IID_IUnknown || riid == IID_IMAPIProp ||
        riid == IID_IMAPIStatus)
    {
        // Increment the reference count and return the pointer.
        *ppvObj = (LPVOID)this;
        AddRef();
        return NOERROR;
    }
    return E_NOINTERFACE;
}

```

下面的代码示例演示如何实现**AddRef**和**Release**的方法，用于`CMyMAPIObject`对象。 由于实现**AddRef**和**Release**很简单，许多服务提供商选择实现它们内嵌。 对**InterlockedIncrement**和**InterlockedDecrement** Win32 函数的调用确保线程安全。 通过对析构函数，调用**Release**方法删除该对象时释放对象的内存。 
  
```cpp
ULONG CMyMAPIObject::AddRef()
{
    InterlockedIncrement(m_cRef);
    return m_cRef;
}
ULONG CMyMAPIObject::Release()
{
    // Decrement the object's internal counter.
    ULONG ulRefCount = InterlockedDecrement(m_cRef);
    if (0 == m_cRef)
    {
        delete this;
    }
    return ulRefCount;
}
 
```

## <a name="see-also"></a>另请参阅

- [实现 MAPI 对象](implementing-mapi-objects.md)
- [实施 IUnknown 接口](implementing-the-iunknown-interface.md)

