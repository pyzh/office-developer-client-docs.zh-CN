---
title: PidTagFormMessageBehavior 规范属性
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PidTagFormMessageBehavior
api_type:
- HeaderDef
ms.assetid: 8fd82432-9fd9-49ed-aa52-72109db04dc9
description: 上次修改时间：2015 年 3 月 9 日
ms.openlocfilehash: 127770c04e6d77932a49d4f447b0bf109afcc194
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19777676"
---
# <a name="pidtagformmessagebehavior-canonical-property"></a>PidTagFormMessageBehavior 规范属性

  
  
**适用于**： Outlook 
  
包含 TRUE 如果应在当前文件夹中包含一条消息。 
  
|||
|:-----|:-----|
|相关属性：  <br/> |PR_FORM_MESSAGE_BEHAVIOR  <br/> |
|标识符：  <br/> |0x330A  <br/> |
|数据类型：  <br/> |PT_LONG  <br/> |
|区域：  <br/> |常见的 MAPI  <br/> |
   
## <a name="remarks"></a>说明

值为 FALSE 指示的邮件应由为任何其他人际邮件时，即发件箱文件夹中。 
  
## <a name="related-resources"></a>相关资源

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

