---
title: 创建表单配置文件
manager: soliver
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
api_type:
- COM
ms.assetid: aaf3b33d-ad2d-4ef8-847f-1ab1eaf08706
description: 上次修改时间： 2011 年 7 月 23 日
ms.openlocfilehash: 9ceb7ad347e73f69eca3463ed2edc4438a45a21f
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19774729"
---
# <a name="creating-a-form-configuration-file"></a>创建表单配置文件

  
  
**适用于**： Outlook 
  
窗体配置文件正在使用的窗体管理器和客户端应用程序提供有关表单的信息。 窗体配置文件包含大量的窗体，包括用于表单发布的消息客户端、 窗体中，通过实现的动作和按窗体所支持的平台的属性规范。
  
窗体配置文件是一个文件扩展名为.cfg 具有类似于 Windows 的初始化文件的格式。 它是纯文本文件的节的编号。 每一节开始部分名称，用方括号括起来。 每个部分包含定义值和与该节相关的设置的一个或多个行。 值具有以下类型之一：
  
- 字符串
    
- 显示的字符串
    
- 平台字符串
    
- 路径名称
    
- 整数
    
- GUID
    
有关.cfg 文件的部分的详细信息，请参阅[窗体配置文件的文件格式](file-format-of-form-configuration-files.md)。
  
## <a name="see-also"></a>另请参阅



[开发 MAPI 表单服务器](developing-mapi-form-servers.md)

