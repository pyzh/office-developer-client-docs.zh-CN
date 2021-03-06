---
title: IMAPISyncProgressCallback IUnknown
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IMAPISyncProgressCallback
api_type:
- COM
ms.assetid: 146b5e36-8d73-4949-9fed-1074f707423d
description: 上次修改时间：2015 年 3 月 9 日
ms.openlocfilehash: bce70d891bc33dcddb94fc05992c09991c6cdc63
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19775687"
---
# <a name="imapisyncprogresscallback--iunknown"></a>IMAPISyncProgressCallback : IUnknown

  
  
**适用于**： Outlook 
  
传入的存储提供程序作为字段的 MAPISIB 结构到在呼叫过程中[IMAPISync: SynchronizeInBackground](imapisyncsynchronizeinbackground.md)。 存储提供程序使用此接口提供反馈到 Microsoft Outlook 同步的状态。
  
|||
|:-----|:-----|
|头文件：  <br/> ||
|由公开：  <br/> |Outlook  <br/> |
|通过实现：  <br/> |Outlook  <br/> |
|调用：  <br/> |存储提供程序  <br/> |
|接口标识符：  <br/> |IID_IMAPISyncProgressCallback  <br/> |
   
## <a name="vtable-order"></a>Vtable 顺序排列

|||
|:-----|:-----|
|[Progress](imapisyncprogresscallback-progress.md) <br/> |存储提供程序定期调用此函数可更新发送/接收对话框中的状态。  <br/> |
|[Error](imapisyncprogresscallback-error.md) <br/> |如果同步过程中遇到错误，存储提供程序调用此函数可提供发送/接收对话框中显示的详细信息。  <br/> |
|[完成](imapisyncprogresscallback-done.md) <br/> |存储提供程序调用此函数来通知 Outlook 同步已完成。  <br/> |
   
## <a name="see-also"></a>另请参阅



[IMAPISync : IUnknown](imapisynciunknown.md)


[MAPI 接口](mapi-interfaces.md)

