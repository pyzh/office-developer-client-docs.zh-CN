---
title: PidTagContentUnreadCount 规范属性
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PidTagContentUnreadCount
api_type:
- HeaderDef
ms.assetid: 4fe207e9-a77f-46b9-b51d-d989847a9d02
description: 上次修改时间：2015 年 3 月 9 日
ms.openlocfilehash: ce7092840037345ae99b31c39cfbd4ac96b99ff5
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19777493"
---
# <a name="pidtagcontentunreadcount-canonical-property"></a>PidTagContentUnreadCount 规范属性

  
  
**适用于**： Outlook 
  
计算出的消息存储库包含文件夹中的未读邮件数。 
  
|||
|:-----|:-----|
|相关属性：  <br/> |PR_CONTENT_UNREAD  <br/> |
|标识符：  <br/> |0x3603  <br/> |
|数据类型：  <br/> |PT_LONG  <br/> |
|区域：  <br/> |Folder  <br/> |
   
## <a name="remarks"></a>说明

消息存储通过计算此属性用于两个不同的但相关，目的。 MAPI folder 对象，它包含文件夹中的消息的数。 在分类 MAPI 表中的标题行中，它包含该标题行所对应的类别中的未读非关联消息的数目。
  
此属性包含**PR_MESSAGE_FLAGS** ([PidTagMessageFlags](pidtagmessageflags-canonical-property.md)) 属性中未设置 MSGFLAG_READ 标志是文件夹内容表中的消息数。 **PR_CONTENT_COUNT** ([PidTagContentCount](pidtagcontentcount-canonical-property.md)) 属性包含的文件夹的邮件总数计数。 **PR_CONTENT_COUNT**和此属性是只读的客户端。 
  
某些客户端应用程序显示根据该属性的值不同类别的标题行。 例如，客户端可以显示包含未读的邮件以粗体显示的类别。 此属性不能用作类别并尝试使用，以便从[IMAPITable::SortTable](imapitable-sorttable.md)方法返回 MAPI_E_INVALID_PARAMETER 值中的结果，正在进行。 
  
## <a name="related-resources"></a>相关资源

### <a name="protocol-specifications"></a>协议规范

[[MS OXPROPS]](http://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)
  
> 提供了相关的 Microsoft Exchange Server 协议规范参考。
    
[[MS OXCFOLD]](http://msdn.microsoft.com/library/c0f31b95-c07f-486c-98d9-535ed9705fbf%28Office.15%29.aspx)
  
> 处理文件夹的操作。
    
[[MS OXCTABL]](http://msdn.microsoft.com/library/d33612dc-36a8-4623-8a26-c156cf8aae4b%28Office.15%29.aspx)
  
> 包含允许的操作的核心 table 对象。
    
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

