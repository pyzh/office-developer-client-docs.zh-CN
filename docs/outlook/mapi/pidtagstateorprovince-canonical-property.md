---
title: PidTagStateOrProvince 规范属性
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MAPI.PidTagStateOrProvince
api_type:
- COM
ms.assetid: 5f17874f-fab5-4119-b2eb-845c1f70d882
description: 上次修改时间：2015 年 3 月 9 日
ms.openlocfilehash: da4ed488498d820c7080a87752f58c5b8c524e1d
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19778440"
---
# <a name="pidtagstateorprovince-canonical-property"></a>PidTagStateOrProvince 规范属性

  
  
**适用于**： Outlook 
  
包含的收件人的州或省的名称。
  
|||
|:-----|:-----|
|相关属性：  <br/> |PR_STATE_OR_PROVINCE、 PR_STATE_OR_PROVINCE_A、 PR_STATE_OR_PROVINCE_W、 PR_BUSINESS_ADDRESS_STATE_OR_PROVINCE、 PR_BUSINESS_ADDRESS_STATE_OR_PROVINCE_A、 PR_BUSINESS_ADDRESS_STATE_OR_PROVINCE_W  <br/> |
|标识符：  <br/> |0x3A28  <br/> |
|数据类型：  <br/> |PT_STRING8 PT_UNICODE  <br/> |
|区域：  <br/> |MAPI 邮件用户  <br/> |
   
## <a name="remarks"></a>说明

这些属性提供标识和访问收件人的信息。 它们是按收件人和收件人的组织定义的。 
  
## <a name="related-resources"></a>相关资源

### <a name="protocol-specifications"></a>协议规范

[[MS OXPROPS]](http://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)
  
> 提供了相关的 Exchange Server 协议规范参考。
    
[[MS OXOCNTC]](http://msdn.microsoft.com/library/9b636532-9150-4836-9635-9c9b756c9ccf%28Office.15%29.aspx)
  
> 指定的属性和操作所允许的联系人和个人通讯组列表。
    
[[MS OXOABK]](http://msdn.microsoft.com/library/f4cf9b4c-9232-4506-9e71-2270de217614%28Office.15%29.aspx)
  
> 指定的属性和用户、 联系人、 组和资源的操作列表。
    
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
