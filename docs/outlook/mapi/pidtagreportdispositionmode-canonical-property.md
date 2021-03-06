---
title: PidTagReportDispositionMode 规范属性
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_type:
- COM
ms.assetid: 67b3c76a-f6f7-462b-955c-dc7b53e7e7eb
description: 上次修改时间：2015 年 3 月 9 日
ms.openlocfilehash: bc2d577ad6c6b430c2339dfb0567ca56de0a7f8e
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19778209"
---
# <a name="pidtagreportdispositionmode-canonical-property"></a>PidTagReportDispositionMode 规范属性

  
  
**适用于**： Outlook 
  
指示对回执请求收款的邮件的处置。 
  
|||
|:-----|:-----|
|相关属性：  <br/> |PR_REPORT_DISPOSITION_MODE，PR_REPORT_DISPOSITION_MODE_A，PR_REPORT_DISPOSITION_MODE_W  <br/> |
|标识符：  <br/> |0x0081  <br/> |
|数据类型：  <br/> |PT_STRING8 PT_UNICODE  <br/> |
|区域：  <br/> |MAPI 信封  <br/> |
   
## <a name="remarks"></a>说明

此属性可能的值为"手动-操作/MDN-发送-自动"和"手动-操作/MDN-发送-手动"。
  
## <a name="related-resources"></a>相关资源

### <a name="protocol-specifications"></a>协议规范

[[MS-OXPROPS]] 
  
> 提供了相关的 Exchange Server 协议规范参考。
    
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

