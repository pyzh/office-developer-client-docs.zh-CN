---
title: PidTagSearchFolderEfpFlags 规范属性
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MAPI.PidTagSearchFolderEfpFlags
api_type:
- COM
ms.assetid: ef82a75f-a09f-4880-ba6a-e739b16422a3
description: 上次修改时间：2015 年 3 月 9 日
ms.openlocfilehash: e98416ba7796c66d719adcc27ba8029b7908bb79
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19778381"
---
# <a name="pidtagsearchfolderefpflags-canonical-property"></a>PidTagSearchFolderEfpFlags 规范属性

  
  
**适用于**： Outlook 
  
包含应用于的搜索文件夹的搜索文件夹容器的扩展的文件夹标志。
  
|||
|:-----|:-----|
|相关属性：  <br/> |PR_WB_SF_EFP_FLAGS  <br/> |
|标识符：  <br/> |0x6848  <br/> |
|数据类型：  <br/> |PT_LONG  <br/> |
|区域：  <br/> |搜索  <br/> |
   
## <a name="remarks"></a>说明

具体而言，此属性应包含**PR_EXTENDED_FOLDER_FLAGS** ([PidTagExtendedFolderFlags](pidtagextendedfolderflags-canonical-property.md)) 属性和字段 b 的文件夹中的**ExtendedFlags**子属性中的标志。 有关文件夹标志信息，请参阅[[MS OXOCFG]](http://msdn.microsoft.com/library/7d466dd5-c156-4da9-9a01-75c78e7e1a67%28Office.15%29.aspx)。
  
## <a name="related-resources"></a>相关资源

### <a name="protocol-specifications"></a>协议规范

[[MS OXPROPS]](http://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)
  
> 提供了相关的 Exchange Server 协议规范参考。
    
[[MS OXOSRCH]](http://msdn.microsoft.com/library/c72e49b8-78c7-4483-ad65-e46e9133673b%28Office.15%29.aspx)
  
> 指定的属性和操作的搜索文件夹列表配置的操作。
    
[[MS OXOCFG]](http://msdn.microsoft.com/library/7d466dd5-c156-4da9-9a01-75c78e7e1a67%28Office.15%29.aspx)
  
> 指定的位置和客户端和服务器配置数据，如共享的类别列表和工作时间的属性。
    
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

