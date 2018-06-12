---
title: PidLidLogStart 规范属性
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PidLidLogStart
api_type:
- COM
ms.assetid: b8c0c871-51d8-4752-ad4b-607463a9f837
description: 上次修改时间： 2015 年 3 月 9 日
ms.openlocfilehash: 55ba18a1dcbce5e3f7996184dae45a638f9531e5
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19776903"
---
# <a name="pidlidlogstart-canonical-property"></a><span data-ttu-id="ddef1-103">PidLidLogStart 规范属性</span><span class="sxs-lookup"><span data-stu-id="ddef1-103">PidLidLogStart Canonical Property</span></span>

  
  
<span data-ttu-id="ddef1-104">**适用于**： Outlook</span><span class="sxs-lookup"><span data-stu-id="ddef1-104">**Applies to**: Outlook</span></span> 
  
<span data-ttu-id="ddef1-105">表示的开始日期和时间的日记邮件。</span><span class="sxs-lookup"><span data-stu-id="ddef1-105">Represents the start date and time for the journal message.</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="ddef1-106">关联的属性：</span><span class="sxs-lookup"><span data-stu-id="ddef1-106">Associated properties:</span></span>  <br/> |<span data-ttu-id="ddef1-107">dispidLogStart</span><span class="sxs-lookup"><span data-stu-id="ddef1-107">dispidLogStart</span></span>  <br/> |
|<span data-ttu-id="ddef1-108">属性进行设置：</span><span class="sxs-lookup"><span data-stu-id="ddef1-108">Property set:</span></span>  <br/> |<span data-ttu-id="ddef1-109">PSETID_Log</span><span class="sxs-lookup"><span data-stu-id="ddef1-109">PSETID_Log</span></span>  <br/> |
|<span data-ttu-id="ddef1-110">长 ID （盖）：</span><span class="sxs-lookup"><span data-stu-id="ddef1-110">Long ID (LID):</span></span>  <br/> |<span data-ttu-id="ddef1-111">0x00008706</span><span class="sxs-lookup"><span data-stu-id="ddef1-111">0x00008706</span></span>  <br/> |
|<span data-ttu-id="ddef1-112">数据类型：</span><span class="sxs-lookup"><span data-stu-id="ddef1-112">Data type:</span></span>  <br/> |<span data-ttu-id="ddef1-113">PT_SYSTIME</span><span class="sxs-lookup"><span data-stu-id="ddef1-113">PT_SYSTIME</span></span>  <br/> |
|<span data-ttu-id="ddef1-114">区域：</span><span class="sxs-lookup"><span data-stu-id="ddef1-114">Area:</span></span>  <br/> |<span data-ttu-id="ddef1-115">日记</span><span class="sxs-lookup"><span data-stu-id="ddef1-115">Journal</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ddef1-116">备注</span><span class="sxs-lookup"><span data-stu-id="ddef1-116">Remarks</span></span>

<span data-ttu-id="ddef1-117">以协调世界时 (UTC) 活动开始时的时间必须等于**dispidCommonStart** ([PidLidCommonStart](pidlidcommonstart-canonical-property.md)) 属性。</span><span class="sxs-lookup"><span data-stu-id="ddef1-117">The time in Coordinated Universal Time (UTC) when the activity began must be equal to the **dispidCommonStart** ([PidLidCommonStart](pidlidcommonstart-canonical-property.md)) property.</span></span>
  
## <a name="related-resources"></a><span data-ttu-id="ddef1-118">相关资源</span><span class="sxs-lookup"><span data-stu-id="ddef1-118">Related resources</span></span>

### <a name="protocol-specifications"></a><span data-ttu-id="ddef1-119">协议规范</span><span class="sxs-lookup"><span data-stu-id="ddef1-119">Protocol specifications</span></span>

<span data-ttu-id="ddef1-120">[[MS OXPROPS]](http://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="ddef1-120">[[MS-OXPROPS]](http://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)</span></span>
  
> <span data-ttu-id="ddef1-121">提供属性集定义和相关的 Exchange Server 协议规范的引用。</span><span class="sxs-lookup"><span data-stu-id="ddef1-121">Provides property set definition and references to related Exchange Server protocol specifications.</span></span>
    
<span data-ttu-id="ddef1-122">[[MS OXOJRNL]](http://msdn.microsoft.com/library/2aa04fd2-0f36-4ce4-9178-c0fc70aa8d43%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="ddef1-122">[[MS-OXOJRNL]](http://msdn.microsoft.com/library/2aa04fd2-0f36-4ce4-9178-c0fc70aa8d43%28Office.15%29.aspx)</span></span>
  
> <span data-ttu-id="ddef1-123">指定的属性和操作所允许的日志。</span><span class="sxs-lookup"><span data-stu-id="ddef1-123">Specifies the properties and operations that are permissible for journals.</span></span>
    
### <a name="header-files"></a><span data-ttu-id="ddef1-124">头文件</span><span class="sxs-lookup"><span data-stu-id="ddef1-124">Header files</span></span>

<span data-ttu-id="ddef1-125">Mapidefs.h</span><span class="sxs-lookup"><span data-stu-id="ddef1-125">Mapidefs.h</span></span>
  
> <span data-ttu-id="ddef1-126">提供数据类型定义。</span><span class="sxs-lookup"><span data-stu-id="ddef1-126">Provides data type definitions.</span></span>
    
## <a name="see-also"></a><span data-ttu-id="ddef1-127">另请参阅</span><span class="sxs-lookup"><span data-stu-id="ddef1-127">See also</span></span>



[<span data-ttu-id="ddef1-128">MAPI 属性</span><span class="sxs-lookup"><span data-stu-id="ddef1-128">MAPI Properties</span></span>](mapi-properties.md)
  
[<span data-ttu-id="ddef1-129">MAPI 规范属性</span><span class="sxs-lookup"><span data-stu-id="ddef1-129">MAPI Canonical Properties</span></span>](mapi-canonical-properties.md)
  
[<span data-ttu-id="ddef1-130">映射到 MAPI 名称的规范属性名称</span><span class="sxs-lookup"><span data-stu-id="ddef1-130">Mapping Canonical Property Names to MAPI Names</span></span>](mapping-canonical-property-names-to-mapi-names.md)
  
[<span data-ttu-id="ddef1-131">MAPI 名称映射到规范属性名称</span><span class="sxs-lookup"><span data-stu-id="ddef1-131">Mapping MAPI Names to Canonical Property Names</span></span>](mapping-mapi-names-to-canonical-property-names.md)
