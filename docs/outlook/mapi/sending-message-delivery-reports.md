---
title: 发送邮件送达报告
manager: soliver
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
api_type:
- COM
ms.assetid: abb12ec5-f0b7-488a-a75d-446f4be53e96
description: 上次修改时间： 2011 年 7 月 23 日
ms.openlocfilehash: d94785df9becf46bbfad66465facea35202c6079
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19778737"
---
# <a name="sending-message-delivery-reports"></a>发送邮件送达报告

  
  
**适用于**： Outlook 
  
某些基础的消息系统支持送达报告和有些则未。 传输提供程序如何确定是否可以将邮件传递或原件报告发送给客户端应用程序是特定于单个传输提供程序的实现详细信息。 如果送达报告可被发送到客户端应用程序，传输提供程序使用[IMAPISupport::StatusRecips](imapisupport-statusrecips.md)方法的一个或多个收件人通知的成功或失败传递的 MAPI。 MAPI 然后生成传递或原件对应于这些收件人的报告。 传输提供程序可以通过**StatusRecips**翻译传入邮件系统的 MAPI 传递到本机的交付和原件报告和未送达报告。
  

