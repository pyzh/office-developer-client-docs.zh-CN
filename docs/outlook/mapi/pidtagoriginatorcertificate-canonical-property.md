---
title: PidTagOriginatorCertificate 规范属性
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MAPI.PidTagOriginatorCertificate
api_type:
- COM
ms.assetid: 65f890d8-9d25-408e-ab29-89991278b92d
description: 上次修改时间：2015 年 3 月 9 日
ms.openlocfilehash: 871ce5f594a75b9441d0434c3be47b2718540576
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19777982"
---
# <a name="pidtagoriginatorcertificate-canonical-property"></a>PidTagOriginatorCertificate 规范属性

  
  
**适用于**： Outlook 
  
包含消息创建者 ASN.1 证书。
  
|||
|:-----|:-----|
|相关属性：  <br/> |PR_ORIGINATOR_CERTIFICATE  <br/> |
|标识符：  <br/> |0x0022  <br/> |
|数据类型：  <br/> |PT_BINARY  <br/> |
|区域：  <br/> |MIME  <br/> |
   
## <a name="remarks"></a>说明

此属性为原始发件人的**PR_USER_CERTIFICATE** ([PidTagUserCertificate](pidtagusercertificate-canonical-property.md)) 属性的副本。
  
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

