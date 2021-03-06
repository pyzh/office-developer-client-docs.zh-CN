---
title: IMAPIOfflineMgrUnadvise
manager: soliver
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IMAPIOfflineMgr.Unadvise
api_type:
- COM
ms.assetid: 250b9137-facb-81a2-41b1-96a57366c04e
description: 上次修改时间： 2011 年 7 月 23 日
ms.openlocfilehash: b52dcd87c8714ad59db560a5ae4a8300f9cc83ae
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19775500"
---
# <a name="imapiofflinemgrunadvise"></a>IMAPIOfflineMgr::Unadvise

  
  
**适用于**： Outlook 
  
取消脱机对象的回调。
  
```cpp
HRESULT COfflineObj::Unadvise( 
      ULONG ulFlags, 
      ULONG ulAdviseToken 
);
```

## <a name="parameters"></a>参数

 _ulFlags_
  
> [in]用于取消回调的标志。 支持仅值 MAPIOFFLINE_UNADVISE_DEFAULT。
    
 _ulAdviseToken_
  
> [in]标识要取消此事件的回调注册 advise 令牌。 
    
## <a name="return-value"></a>返回值

S_OK
  
> 呼叫成功。 此调用必须返回 S_OK。
    
## <a name="remarks"></a>说明

删除回调与*ulAdviseToken*从以前调用**[IMAPIOfflineMgr::Advise](imapiofflinemgr-advise.md)** 返回关联的注册。 导致**IMAPIOfflineMgr**对象来释放其上与*ulAdviseToken*关联的**[IMAPIOfflineNotify](imapiofflinenotifyiunknown.md)** 对象的引用。 
  
## <a name="see-also"></a>另请参阅



[IMAPIOfflineMgr::Advise](imapiofflinemgr-advise.md)


[MAPI 常量](mapi-constants.md)

