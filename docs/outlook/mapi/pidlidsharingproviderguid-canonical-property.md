---
title: PidLidSharingProviderGuid 规范属性
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PidLidSharingProviderGuid
api_type:
- COM
ms.assetid: 103c9cf2-42fb-4fa5-b9c2-8a92725d3097
description: 上次修改时间：2015 年 3 月 9 日
ms.openlocfilehash: f3138a5994ffc6e32ffebd1a4d5b221db0dd2312
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19777043"
---
# <a name="pidlidsharingproviderguid-canonical-property"></a>PidLidSharingProviderGuid 规范属性

  
  
**适用于**： Outlook 
  
指定共享提供程序全局唯一标识符 (GUID)。 这是邮件的共享的属性。
  
|||
|:-----|:-----|
|相关属性：  <br/> |dispidSharingProviderGuid  <br/> |
|属性进行设置：  <br/> |PSETID_Sharing  <br/> |
|长 ID （盖）：  <br/> |0x00008A01  <br/> |
|数据类型：  <br/> |PT_BINARY  <br/> |
|区域：  <br/> |共享  <br/> |
   
## <a name="remarks"></a>说明

此属性的值必须设置为"%xae.f0.06.00.00.00.00.00.c0.00.00.00.00.00.00.46"。 
  
## <a name="related-resources"></a>相关资源

### <a name="protocol-specifications"></a>协议规范

[[MS OXPROPS]](http://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)
  
> 提供属性集定义和相关的 Exchange Server 协议规范的引用。
    
[[MS OXSHARE]](http://msdn.microsoft.com/library/e4e5bd27-d5e0-43f9-a6ea-550876724f3d%28Office.15%29.aspx)
  
> 共享客户端之间的邮箱文件夹。
    
### <a name="header-files"></a>头文件

Mapidefs.h
  
> 提供数据类型定义。
    
## <a name="see-also"></a>另请参阅



[MAPI 属性](mapi-properties.md)
  
[MAPI 规范属性](mapi-canonical-properties.md)
  
[将规范属性名称映射到 MAPI 名称](mapping-canonical-property-names-to-mapi-names.md)
  
[将 MAPI 名称映射到规范属性名称](mapping-mapi-names-to-canonical-property-names.md)

