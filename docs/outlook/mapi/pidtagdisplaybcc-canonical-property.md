---
title: PidTagDisplayBcc 规范属性
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PidTagDisplayBcc
api_type:
- HeaderDef
ms.assetid: ab5bcd67-d54e-46e9-b94e-a652aac3e81c
description: 上次修改时间：2015 年 3 月 9 日
ms.openlocfilehash: 55ee55fefd82f29c8b780a350ecdfe0285b3d649
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19777564"
---
# <a name="pidtagdisplaybcc-canonical-property"></a>PidTagDisplayBcc 规范属性

  
  
**适用于**： Outlook 
  
包含任何密件抄送 (BCC) 邮件的收件人，用分号 （;） 分隔的显示名称 ASCII 的列表。
  
|||
|:-----|:-----|
|相关属性：  <br/> |PR_DISPLAY_BCC，PR_DISPLAY_BCC_A，PR_DISPLAY_BCC_W  <br/> |
|标识符：  <br/> |0x0E02  <br/> |
|数据类型：  <br/> |PT_STRING8 PT_UNICODE  <br/> |
|区域：  <br/> |Message  <br/> |
   
## <a name="remarks"></a>说明

消息存储库使用[IMessage::ModifyRecipients](imessage-modifyrecipients.md)方法计算这些消息对象的属性。 消息存储还维护这些属性，以便它始终反映消息的上次保存的状态。 在每次调用[IMAPIProp::SaveChanges](imapiprop-savechanges.md)方法时同步值。 
  
如果邮件没有密件抄送收件人，消息存储应响应**PR_DISPLAY_BCC** [IMAPIProp::GetProps](imapiprop-getprops.md)呼叫的返回值为 S_OK 和为空字符串。 
  
由于可能需要本地化，MAPI 为所有收件人姓名提供以下准则：
  
- 所有名称应该都能够都进行本地化。 
    
- 分号应为用于分隔名称**PR_DISPLAY_BCC**、 **PR_DISPLAY_CC** ([PidTagDisplayCc](pidtagdisplaycc-canonical-property.md)) 和**仅包含显示名称**([PidTagDisplayTo](pidtagdisplayto-canonical-property.md)) 属性中的字符。 MAPI 中的收件人姓名内不允许使用分号分隔。 
    
- 客户端应翻译使属性信息的用户界面中可见之前遇到本地化的分隔符对此属性中的每个分号。 
    
- 将邮件转发，当客户端不需要翻译密件抄送副本收件人行上的分隔符。 
    
## <a name="related-resources"></a>相关资源

### <a name="protocol-specifications"></a>协议规范

[[MS OXOMSG]](http://msdn.microsoft.com/library/daa9120f-f325-4afb-a738-28f91049ab3c%28Office.15%29.aspx)
  
> 介绍用于发送到客户端上共享文件夹相关的信息的消息的格式。
    
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

