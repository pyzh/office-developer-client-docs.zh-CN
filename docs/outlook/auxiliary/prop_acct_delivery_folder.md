---
title: PROP_ACCT_DELIVERY_FOLDER
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: a409c49b-b390-021e-2ec1-7a5932a0c8de
description: 表示该帐户的默认送达文件夹的条目 ID。
ms.openlocfilehash: 56b648b6a79e7497cab1980a86ca11d1c7a6aa3e
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19774443"
---
# <a name="propacctdeliveryfolder"></a>PROP_ACCT_DELIVERY_FOLDER

表示该帐户的默认送达文件夹的条目 ID。
  
## <a name="quick-info"></a>快速信息

See [IOlkAccount](iolkaccount.md).
  
|||
|:-----|:-----|
|标识符:  <br/> |0x0019  <br/> |
|属性类型  <br/> |PT_BINARY  <br/> |
|属性标记：  <br/> |0x00190102  <br/> |
|访问权限  <br/> |读/写  <br/> |
   
## <a name="remarks"></a>备注

Get or set this property by using [IOlkAccount::GetProp](iolkaccount-getprop.md) or [IOlkAccount::SetProp](iolkaccount-setprop.md), respectively.
  
默认的传递文件夹已 **收件箱**。
  
## <a name="see-also"></a>另请参阅

- [有关帐户管理 API](about-the-account-management-api.md)  
- [常量 （帐户管理 API）](constants-account-management-api.md)

