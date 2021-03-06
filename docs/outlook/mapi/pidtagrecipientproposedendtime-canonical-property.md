---
title: PidTagRecipientProposedEndTime 规范属性
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MAPI.PidTagRecipientProposedEndTime
api_type:
- COM
ms.assetid: 08dc1f81-964b-4059-9167-e517391b26e9
description: 上次修改时间：2015 年 3 月 9 日
ms.openlocfilehash: f0310d8dcde9acc1e14f0be124543897e9867951
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19778159"
---
# <a name="pidtagrecipientproposedendtime-canonical-property"></a>PidTagRecipientProposedEndTime 规范属性

  
  
**适用于**： Outlook 
  
表示会议建议的结束时间。
  
|||
|:-----|:-----|
|相关属性：  <br/> |PR_RECIPIENT_PROPOSEDENDTIME  <br/> |
|标识符：  <br/> |0x5FE4  <br/> |
|数据类型：  <br/> |PT_SYSTIME  <br/> |
|区域：  <br/> |传输收件人  <br/> |
   
## <a name="remarks"></a>说明

此属性的值时**PR_RECIPIENT_PROPOSED** ([PidTagRecipientProposed](pidtagrecipientproposed-canonical-property.md)) 属性的值设置为 TRUE，指示请求参与者设置为**dispidApptEndWhole** ([的值的值PidLidAppointmentEndWhole](pidlidappointmentendwhole-canonical-property.md)) 的单个实例会议对象或 exception 对象的属性。
  
## <a name="related-resources"></a>相关资源

### <a name="protocol-specifications"></a>协议规范

[[MS OXPROPS]](http://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)
  
> 提供了相关的 Exchange Server 协议规范参考。
    
[[MS OXOCAL]](http://msdn.microsoft.com/library/09861fde-c8e4-4028-9346-e7c214cfdba1%28Office.15%29.aspx)
  
> 指定的属性和约会、 会议请求和响应消息的操作。
    
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

