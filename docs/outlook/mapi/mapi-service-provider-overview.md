---
title: MAPI 服务提供程序概述
manager: soliver
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
api_type:
- COM
ms.assetid: e7cbc79f-3d60-4f21-a378-7b0088ee8ad3
description: 上次修改时间： 2012 年 6 月 25 日
ms.openlocfilehash: 15a53a0bb16db3683e4c1320ac2e54648c8c697b
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19776327"
---
# <a name="mapi-service-provider-overview"></a>MAPI 服务提供程序概述

  
  
**适用于**： Outlook 
  
MAPI 子系统和消息的系统之间的各种服务提供商。 服务提供商就像连接到基础消息系统的 MAPI 客户端应用程序的驱动程序。 有三种类型的提供程序： 消息存储提供程序、 通讯簿或目录提供商和邮件传输提供程序。 MAPI 支持每种服务独立，使供应商，以提供一个或多个自定义服务提供商。 例如，供应商可能希望在创建使用员工的公司电话簿目录通讯簿提供程序或创建一个使用现有数据库的消息存储提供程序。
  
服务提供商的软件开发人员有专门的知识或体验的通常编写特定的邮件系统的特定的系统。 例如，Microsoft Outlook 2013 和 Microsoft Outlook 2010 Mobile 服务使用通讯簿提供程序公开在 Outlook 中的手机通讯簿。 
  
MAPI 提供统一的地址簿和传输提供程序信息的视图的客户端应用程序。 此集成的方法防止客户端应用程序无需将数据映射到相应的提供程序。 它还可以阻止用户无需协商之间多个通讯簿和传输提供程序寻址方案。 消息存储提供程序的信息，但是，不统一的并且负责处理它们分别使用多个消息存储提供程序的客户端。
  
服务提供商使用 MAPI 创建和发送消息，采用以下方式： 通过使用适用于特定类型的类，邮件的窗体创建消息。 许多消息进行与标准注释表单附带的 MAPI 子系统，可由用户的客户端应用程序或以编程方式无需用户交互。 已完成的消息将发送到一个或多个收件人 — 用户组的指定其接收邮件。 收件人可能或可能不具有的目录中安装的通讯簿提供程序之一拥有一个条目。 未与安装的通讯簿提供程序关联的收件人被称为自定义收件人或一次性地址。 一次性地址可以是临时，持续仅之前该邮件提交。 
  
当客户端应用程序发送邮件时，消息存储提供程序将检查每个收件人具有唯一的并且有效地址以及邮件是否具有所有传输所需的信息。 如果没有疑问 （例如，具有相同名称的多个收件人时） 的收件人，通讯簿提供程序负责解决歧义。 邮件然后放在出站队列。 
  
## <a name="see-also"></a>另请参阅



[MAPI 功能和体系结构](mapi-features-and-architecture.md)

