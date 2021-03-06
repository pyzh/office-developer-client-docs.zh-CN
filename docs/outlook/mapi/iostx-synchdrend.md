---
title: IOSTXSyncHdrEnd
manager: soliver
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IOSTX.SyncHdrEnd
api_type:
- COM
ms.assetid: a0beb6eb-7978-c64e-dba1-89f0caf2090e
description: 上次修改时间： 2012 年 7 月 3 日
ms.openlocfilehash: ee68052f330bf3239cd12139ffbd77f5a180f6cc
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19775959"
---
# <a name="iostxsynchdrend"></a>IOSTX::SyncHdrEnd

 
  
**适用于**： Outlook 
  
邮件头的两端同步。
  
```cpp
HRESULT SyncHdrEnd( 
    LPMAPIPROGRESS pprog 
);
```

## <a name="parameters"></a>参数

 _pprog_
  
> [in]用于同步的**[IMAPIProgress](imapiprogressiunknown.md)** 界面移动或复制邮件。 请参阅 mapidefs.h **LPMAPIPROGRESS**的类型定义。 
    
## <a name="remarks"></a>说明

时**[IOSTX::SyncBeg](iostx-syncbeg.md)**，本地存储进入[下载邮件头状态](download-message-header-state.md)。 客户端下载完整邮件项目 （作为中**[HDRSYNC](hdrsync.md)** *pmsgFull* )。 如果这是成功，客户端还*ulFlags*中设置**HDRSYNC** **HSF_OK**。 时**IOSTX::SyncHdrEnd**，Outlook 检查**HDRSYNC**结果，并使用在**HDRSYNC** *pprog*和信息，来更新本地邮件头。 
  
本地存储返回到上述**[IOSTX::SyncHdrBeg](iostx-synchdrbeg.md)** 之前的状态。 
  
## <a name="see-also"></a>另请参阅



[IOSTX::GetLastError](iostx-getlasterror.md)
  
[IOSTX::InitSync](iostx-initsync.md)
  
[IOSTX::SetSyncResult](iostx-setsyncresult.md)
  
[IOSTX::SyncBeg](iostx-syncbeg.md)
  
[IOSTX::SyncEnd](iostx-syncend.md)
  
[IOSTX::SyncHdrBeg](iostx-synchdrbeg.md)
  
[IOSTX : IUnknown](iostxiunknown.md)


[MAPI 常量](mapi-constants.md)

