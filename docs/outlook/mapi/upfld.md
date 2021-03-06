---
title: UPFLD
manager: soliver
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6da9d6b6-a016-ccef-77da-3e037c30450d
description: 上次修改时间： 2011 年 7 月 23 日
ms.openlocfilehash: f25b3fb967f4ed93ac38487f21145f35413764da
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19779045"
---
# <a name="upfld"></a>UPFLD

**适用于**： Outlook 
  
用于[上载文件夹状态](upload-folder-state.md)期间上载文件夹的信息。
  
## <a name="quick-info"></a>快速信息

```cpp
struct UPFLD 
{ 
    ULONG ulFlags; 
    LPMAPIFOLDER pfld; 
    FEID feid; 
}; 

```

## <a name="members"></a>Members

_ulFlags_
  
>  [out] / [输入] 要确定相应操作 uplaod 标志。 
    
  - UPF_NEW
    
    - [输出]新文件夹。
    
  - UPF_MOD_PARENT
    
    - [输出]已移动文件夹。
    
  - UPF_MOD_PROPS
    
    - [输出]文件夹属性已被修改。
    
  - UPF_DEL
    
    - [输出]已删除文件夹。
    
  - UPF_OK
    
    - [in]上载成功。 客户端设置后将文件夹信息上载到服务器。
    
_pfld_
  
> [输出]要上载的打开的文件夹对象。
    
_feid_
  
> [输出]文件夹的条目 ID。
    
## <a name="see-also"></a>另请参阅

- [关于复制 API](about-the-replication-api.md) 
- [关于复制状态计算机](about-the-replication-state-machine.md)
- [MAPI 常量](mapi-constants.md)

