---
title: PidTagBodyContentLocation 规范属性
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PidTagBodyContentLocation
api_type:
- HeaderDef
ms.assetid: a66d1c64-5c5a-4980-9acd-72448108fd2c
description: 上次修改时间： 2015 年 3 月 9 日
ms.openlocfilehash: a05743f2fa10326a358dd92a72cf530740274f2d
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19777413"
---
# <a name="pidtagbodycontentlocation-canonical-property"></a>PidTagBodyContentLocation 规范属性

  
  
**适用于**： Outlook 
  
包含 MIME 内容位置标头字段的值。
  
|||
|:-----|:-----|
|关联的属性：  <br/> |PR_BODY_CONTENT_LOCATION，PR_BODY_CONTENT_LOCATION_A，PR_BODY_CONTENT_LOCATION_W  <br/> |
|标识符:  <br/> |0x1014  <br/> |
|数据类型：  <br/> |PT_STRING8 PT_UNICODE  <br/> |
|区域：  <br/> |MIME  <br/> |
   
## <a name="remarks"></a>备注

若要设置这些属性的值，MIME 客户端应所需的值都写入到内容位置标头字段映射到邮件正文 MIME 实体。
  
MIME 读者应将此类的 MIME 实体的内容位置标头字段的值复制到这些属性的值。
  
## <a name="related-resources"></a>相关资源

### <a name="protocol-specifications"></a>协议规范

[[MS OXPROPS]](http://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)
  
> 提供了相关的 Exchange Server 协议规范参考。
    
[[MS OXCMAIL]](http://msdn.microsoft.com/library/b60d48db-183f-4bf5-a908-f584e62cb2d4%28Office.15%29.aspx)
  
> 从 Internet 标准电子邮件约定转换为消息对象。
    
### <a name="header-files"></a>头文件

Mapidefs.h
  
> 提供数据类型定义。
    
Mapitags.h
  
> 包含作为替代名称列出的属性的定义。
    
## <a name="see-also"></a>另请参阅



[MAPI 属性](mapi-properties.md)
  
[MAPI 规范属性](mapi-canonical-properties.md)
  
[映射到 MAPI 名称的规范属性名称](mapping-canonical-property-names-to-mapi-names.md)
  
[MAPI 名称映射到规范属性名称](mapping-mapi-names-to-canonical-property-names.md)
