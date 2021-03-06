---
title: IMAPISync IUnknown
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IMAPISync
api_type:
- COM
ms.assetid: c14d1012-f3d4-47eb-8a90-3160331f94e8
description: 上次修改时间：2015 年 3 月 9 日
ms.openlocfilehash: fb7a8ea39d6e7b1d7df1560658ceb67a79d39d92
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19775676"
---
# <a name="imapisync--iunknown"></a>IMAPISync : IUnknown

  
  
**适用于**： Outlook 
  
提供一种机制，同步电子邮件，而不是使用传输 API。 此接口将公开的存储对象。 使用此接口和[IMAPISyncProgressCallback: IUnknown](imapisyncprogresscallbackiunknown.md)、 传输提供程序可以提供更好的进度和比的错误消息的显示在 Microsoft Outlook 中的发送/接收对话框。
  
发件箱仍位于默认存储。 Outlook 将继续使用 Transport Api 来发送邮件，因为传出消息不能在外部存储中。
  
|||
|:-----|:-----|
|由公开：  <br/> |存储和传输提供程序  <br/> |
|通过实现：  <br/> |Outlook  <br/> |
|调用：  <br/> |存储和传输提供程序  <br/> |
|接口标识符：  <br/> |IID_IMAPISync  <br/> |
   
## <a name="vtable-order"></a>Vtable 顺序排列

|||
|:-----|:-----|
|[SynchronizeInBackground](imapisyncsynchronizeinbackground.md) <br/> |由消息存储提供程序实现。 Outlook 2010 和 Outlook 2013 启动同步调用此方法。  <br/> |
   
## <a name="see-also"></a>另请参阅



[IMAPISyncProgressCallback : IUnknown](imapisyncprogresscallbackiunknown.md)


[MAPI 接口](mapi-interfaces.md)

