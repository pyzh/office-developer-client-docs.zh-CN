---
title: PidTagSearchRecipientEmailCc 规范属性
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 38fe217d-cf2e-51de-c97a-acb015129fd3
description: 上次修改时间：2015 年 3 月 9 日
ms.openlocfilehash: 6fe59bf837d6123e5655e853531d6ab53393af91
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19778371"
---
# <a name="pidtagsearchrecipientemailcc-canonical-property"></a>PidTagSearchRecipientEmailCc 规范属性

  
  
**适用于**： Outlook 
  
包含所查询的电子邮件地址或显示名称上存储的消息**CC**行中所述的收件人列表中的 Unicode 字符串。 
  
## 

|||
|:-----|:-----|
|相关属性：  <br/> |PR_SEARCH_RECIP_EMAIL_CC_W  <br/> |
|标识符：  <br/> |0x0EA7  <br/> |
|属性类型  <br/> |PT_UNICODE  <br/> |
|区域：  <br/> |搜索  <br/> |
   
## <a name="related-resources"></a>相关资源

> [!NOTE]
> 未可能在您当前拥有的可下载的头文件中定义搜索电子邮件地址或显示的名称为抄送邮件发送到时使用此 MAPI 限制标记。 您可以将其添加到您的代码通过使用以下值： >`#define PR_SEARCH_RECIP_EMAIL_CC_W PROP_TAG(PT_UNICODE, 0x0EA7)`
  
### <a name="protocol-specifications"></a>协议规范

[[MS OXPROPS]](http://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)
  
> 提供了相关的 Microsoft Exchange Server 协议规范参考。
    
[[MS OXOSRCH]](http://msdn.microsoft.com/library/c72e49b8-78c7-4483-ad65-e46e9133673b%28Office.15%29.aspx)
  
> 指定的属性和操作的搜索文件夹列表配置的操作。
    
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

