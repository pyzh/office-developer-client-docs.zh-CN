---
title: PidTagContactAddressBookStoreSupportMasks 规范属性
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PidTagContactAddressBookStoreSupportMasks
api_type:
- HeaderDef
ms.assetid: 68f5aac1-714c-48fc-a0cf-a0c0401a6070
description: 上次修改时间：2015 年 3 月 9 日
ms.openlocfilehash: 29e842584e5145f747aa0ef0c7796e5f7b3a8e0b
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19777436"
---
# <a name="pidtagcontactaddressbookstoresupportmasks-canonical-property"></a>PidTagContactAddressBookStoreSupportMasks 规范属性

  
  
**适用于**： Outlook 
  
包含标志指示的存储支持的功能。
  
|||
|:-----|:-----|
|相关属性：  <br/> |PR_CONTAB_STORE_SUPPORT_MASKS  <br/> |
|标识符：  <br/> |0x6621  <br/> |
|数据类型：  <br/> |PT_MV_LONG  <br/> |
|区域：  <br/> |联系人通讯簿  <br/> |
   
## <a name="remarks"></a>说明

从包含联系人文件夹的存储中获取此属性。 联系人通讯簿提供程序使用它来评估适用性的存储支持的功能。 它是联系人通讯簿配置文件一节的属性。 
  
## <a name="related-resources"></a>相关资源

### <a name="header-files"></a>头文件

Mapidefs.h
  
> 提供数据类型定义。
    
Mapitags.h
  
> 包含列为相关属性的属性的定义。
    
## <a name="see-also"></a>另请参阅



[MAPI 属性](mapi-properties.md)
  
[MAPI 规范属性](mapi-canonical-properties.md)
  
[将规范属性名称映射到 MAPI 名称](mapping-canonical-property-names-to-mapi-names.md)
  
[将 MAPI 名称映射到规范属性名称](mapping-mapi-names-to-canonical-property-names.md)

