---
title: PidLidTaskMultipleRecipients 规范属性
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PidLidTaskMultipleRecipients
api_type:
- COM
ms.assetid: 28ba9997-72dd-465f-94a7-35a317a361ef
description: 上次修改时间：2015 年 3 月 9 日
ms.openlocfilehash: 1e1cba3d927072cb03dbd34eee518c9b0a9e0383
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19777093"
---
# <a name="pidlidtaskmultiplerecipients-canonical-property"></a>PidLidTaskMultipleRecipients 规范属性

  
  
**适用于**： Outlook 
  
提供有关收件人的任务的优化提示。
  
|||
|:-----|:-----|
|相关属性：  <br/> |dispidTaskMultRecips  <br/> |
|属性进行设置：  <br/> |PSETID_Task  <br/> |
|长 ID （盖）：  <br/> |0x00008120  <br/> |
|数据类型：  <br/> |PT_LONG  <br/> |
|区域：  <br/> |Task  <br/> |
   
## <a name="remarks"></a>说明

如果设置，此属性必须设置为零个或多个下列值的按位**OR**运算。 
  
|**名称**|**值**|**说明**|
|:-----|:-----|:-----|
|发送时间  <br/> |0x00000001  <br/> |该任务具有多个主收件人。  <br/> |
|接收时间  <br/> |0x00000002  <br/> |尽管 Sent 提示不存在，客户端检测到任务具有多个主收件人。  <br/> |
|保留  <br/> |0x00000004  <br/> |保留此值。  <br/> |
   
## <a name="related-resources"></a>相关资源

### <a name="protocol-specifications"></a>协议规范

[[MS OXPROPS]](http://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)
  
> 提供属性集定义和相关的 Exchange Server 协议规范的引用。
    
[[MS OXOTASK]](http://msdn.microsoft.com/library/55600ec0-6195-4730-8436-59c7931ef27e%28Office.15%29.aspx)
  
> 定义模型的任务、 任务分配和任务更新电子等效项的多个对象。
    
### <a name="header-files"></a>头文件

Mapidefs.h
  
> 提供数据类型定义。
    
## <a name="see-also"></a>另请参阅



[MAPI 属性](mapi-properties.md)
  
[MAPI 规范属性](mapi-canonical-properties.md)
  
[将规范属性名称映射到 MAPI 名称](mapping-canonical-property-names-to-mapi-names.md)
  
[将 MAPI 名称映射到规范属性名称](mapping-mapi-names-to-canonical-property-names.md)

