---
title: PidLidSharingRemoteName 规范属性
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PidLidSharingRemoteName
api_type:
- COM
ms.assetid: be975f74-4b95-45a4-bbee-959fa8e4ad45
description: 上次修改时间：2015 年 3 月 9 日
ms.openlocfilehash: fc3324cb686733f06b9cc0945c93b7df2e5980ae
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19777040"
---
# <a name="pidlidsharingremotename-canonical-property"></a>PidLidSharingRemoteName 规范属性

  
  
**适用于**： Outlook 
  
指定共享远程文件夹的名称。 这是邮件的共享的属性。
  
|||
|:-----|:-----|
|相关属性：  <br/> |dispidSharingRemoteName  <br/> |
|属性进行设置：  <br/> |PSETID_Sharing  <br/> |
|长 ID （盖）：  <br/> |0x00008A05  <br/> |
|数据类型：  <br/> |PT_UNICODE  <br/> |
|区域：  <br/> |共享  <br/> |
   
## <a name="remarks"></a>说明

此属性必须设置为**PR_DISPLAY_NAME** ([PidTagDisplayName](pidtagdisplayname-canonical-property.md)) 属性的值中，在共享文件夹中。
  
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

