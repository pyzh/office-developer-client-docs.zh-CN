---
title: PidTagContactAddressBookFolderName 规范属性
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PidTagContactAddressBookFolderName
api_type:
- HeaderDef
ms.assetid: 6149da2f-6e42-429c-bcdb-d517d21df720
description: 上次修改时间：2015 年 3 月 9 日
ms.openlocfilehash: a4a72e6d5136d7e78648cb62849f7162b7b35f6c
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19777426"
---
# <a name="pidtagcontactaddressbookfoldername-canonical-property"></a>PidTagContactAddressBookFolderName 规范属性

  
  
**适用于**： Outlook 
  
包含用于通讯簿条目的文件夹名称。
  
|||
|:-----|:-----|
|相关属性：  <br/> |PR_CONTAB_FOLDER_NAME PR_CONTAB_FOLDER_NAME_W  <br/> |
|标识符：  <br/> |0x6613  <br/> |
|数据类型：  <br/> |PT_UNICODE PT_STRING8  <br/> |
|区域：  <br/> |联系人通讯簿  <br/> |
   
## <a name="remarks"></a>说明

文件夹名称中不能使用以下字符：
  
[ ] / \ &amp; ~ ? \* | \<\> " ; : +
  
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

