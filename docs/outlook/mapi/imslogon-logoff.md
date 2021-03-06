---
title: IMSLogonLogoff
manager: soliver
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IMSLogon.Logoff
api_type:
- COM
ms.assetid: 1b0d1b52-6651-4de3-9381-86772d9d52a1
description: 上次修改时间： 2011 年 7 月 23 日
ms.openlocfilehash: 5d9a57cee371675493ba71b2df52b83941d34fc2
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19775931"
---
# <a name="imslogonlogoff"></a>IMSLogon::Logoff

  
  
**适用于**： Outlook 
  
注销一条消息存储提供程序。 
  
```cpp
HRESULT Logoff(
  ULONG FAR * lpulFlags
);
```

## <a name="parameters"></a>参数

 _lpulFlags_
  
> [in]保留;必须为零的指针。
    
## <a name="return-value"></a>返回值

S_OK 
  
> 呼叫成功或多个预期值返回。
    
## <a name="remarks"></a>说明

消息存储提供程序实现**IMSLogon::Logoff**方法以强制关闭消息存储提供程序。 在下列情况下调用**IMSLogon::Logoff** : 
  
- 同时给[IMAPISession::Logoff](imapisession-logoff.md)方法调用后 MAPI 正在注销客户端。 
    
- MAPI 注销消息存储提供程序时。 在这种情况下， **IMSLogon::Logoff**称为 MAPI 处理的消息存储提供程序创建处理[IMsgStore::StoreLogoff](imsgstore-storelogoff.md)或**IUnknown 时支持对象的[IUnknown::Release](http://msdn.microsoft.com/en-us/library/ms682317%28v=VS.85%29.aspx)方法的一部分::发行版**消息存储对象上的方法调用。 
    
## <a name="see-also"></a>另请参阅



[IMAPISession::Logoff](imapisession-logoff.md)
  
[IMAPISupport : IUnknown](imapisupportiunknown.md)
  
[IMsgStore::StoreLogoff](imsgstore-storelogoff.md)
  
[IMSProvider::Logon](imsprovider-logon.md)
  
[MAPIFreeBuffer](mapifreebuffer.md)
  
[IMSLogon : IUnknown](imslogoniunknown.md)

