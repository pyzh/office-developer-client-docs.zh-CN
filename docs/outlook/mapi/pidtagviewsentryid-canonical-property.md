---
title: PidTagViewsEntryId 规范属性
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MAPI.PidTagViewsEntryId
api_type:
- COM
ms.assetid: 8350a37c-6f42-4bef-82e0-35aa12b09fcf
description: 上次修改时间：2015 年 3 月 9 日
ms.openlocfilehash: 1980e3bd815b370f125f4449dd7b7f340a7dcb9a
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19778526"
---
# <a name="pidtagviewsentryid-canonical-property"></a>PidTagViewsEntryId 规范属性

  
  
**适用于**： Outlook 
  
包含用户定义的视图文件夹的项标识符。
  
|||
|:-----|:-----|
|相关属性：  <br/> |PR_VIEWS_ENTRYID  <br/> |
|标识符：  <br/> |0x35E5  <br/> |
|数据类型：  <br/> |PT_BINARY  <br/> |
|区域：  <br/> |MAPI 邮件存储  <br/> |
   
## <a name="remarks"></a>说明

公共视图文件夹包含一组预定义的标准视图说明符，而视图文件夹包含由消息的用户定义的说明符。 这些文件夹，不可见人际邮件 (IPM) 层次结构中，可以包含多个视图说明符，每个存储为邮件。 客户端应用程序可以选择合并两个说明符集并使其同时可用。
  
## <a name="related-resources"></a>相关资源

### <a name="header-files"></a>头文件

Mapidefs.h
  
> 提供数据类型定义。
    
Mapitags.h
  
> 包含作为替代名称列出的属性的定义。
    
## <a name="see-also"></a>另请参阅



[MAPI 属性](mapi-properties.md)
  
[MAPI 规范属性](mapi-canonical-properties.md)
  
[将规范属性名称映射到 MAPI 名称](mapping-canonical-property-names-to-mapi-names.md)
  
[将 MAPI 名称映射到规范属性名称](mapping-mapi-names-to-canonical-property-names.md)

