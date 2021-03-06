---
title: PidTagAttachMimeSequence 规范属性
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PidTagAttachMimeSequence
api_type:
- HeaderDef
ms.assetid: d2a84f24-b4a5-4e16-9219-7a579a31a8f8
description: 上次修改时间：2015 年 3 月 9 日
ms.openlocfilehash: e46a6556b88452fb453b031fc1a90762fd748f7d
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19777377"
---
# <a name="pidtagattachmimesequence-canonical-property"></a>PidTagAttachMimeSequence 规范属性

  
  
**适用于**： Outlook 
  
包含的 MIME 邮件附件的 MIME 序列号。
  
|||
|:-----|:-----|
|相关属性：  <br/> |PR_ATTACH_MIME_SEQUENCE  <br/> |
|标识符：  <br/> |0x3710  <br/> |
|数据类型：  <br/> |PT_LONG  <br/> |
|区域：  <br/> |附件的邮件属性  <br/> |
   
## <a name="remarks"></a>说明

此属性用于 MHTML 支持。 它表示在父 MIME 多部分正文部分的 MIME 邮件的附件的序列号。
  
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

