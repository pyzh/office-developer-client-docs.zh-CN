---
title: PidLidPercentComplete 规范属性
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MAPI.PidLidPercentComplete
api_type:
- COM
ms.assetid: e63792b1-9580-4702-a6d7-dd3ae5007a4a
description: 上次修改时间： 2015 年 3 月 9 日
ms.openlocfilehash: f4675362de1e9efe4ef16285723cddeface9c403
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19776960"
---
# <a name="pidlidpercentcomplete-canonical-property"></a><span data-ttu-id="3df75-103">PidLidPercentComplete 规范属性</span><span class="sxs-lookup"><span data-stu-id="3df75-103">PidLidPercentComplete Canonical Property</span></span>

  
  
<span data-ttu-id="3df75-104">**适用于**： Outlook</span><span class="sxs-lookup"><span data-stu-id="3df75-104">**Applies to**: Outlook</span></span> 
  
<span data-ttu-id="3df75-105">指示对任务所做的进度用户。</span><span class="sxs-lookup"><span data-stu-id="3df75-105">Indicates the progress the user has made on a task.</span></span> 
  
|||
|:-----|:-----|
|<span data-ttu-id="3df75-106">关联的属性：</span><span class="sxs-lookup"><span data-stu-id="3df75-106">Associated properties:</span></span>  <br/> |<span data-ttu-id="3df75-107">dispidPercentComplete</span><span class="sxs-lookup"><span data-stu-id="3df75-107">dispidPercentComplete</span></span>  <br/> |
|<span data-ttu-id="3df75-108">属性进行设置：</span><span class="sxs-lookup"><span data-stu-id="3df75-108">Property set:</span></span>  <br/> |<span data-ttu-id="3df75-109">PSETID_Task</span><span class="sxs-lookup"><span data-stu-id="3df75-109">PSETID_Task</span></span>  <br/> |
|<span data-ttu-id="3df75-110">长 ID （盖）：</span><span class="sxs-lookup"><span data-stu-id="3df75-110">Long ID (LID):</span></span>  <br/> |<span data-ttu-id="3df75-111">0x00008102</span><span class="sxs-lookup"><span data-stu-id="3df75-111">0x00008102</span></span>  <br/> |
|<span data-ttu-id="3df75-112">数据类型：</span><span class="sxs-lookup"><span data-stu-id="3df75-112">Data type:</span></span>  <br/> |<span data-ttu-id="3df75-113">PT_R8</span><span class="sxs-lookup"><span data-stu-id="3df75-113">PT_R8</span></span>  <br/> |
|<span data-ttu-id="3df75-114">区域：</span><span class="sxs-lookup"><span data-stu-id="3df75-114">Area:</span></span>  <br/> |<span data-ttu-id="3df75-115">任务</span><span class="sxs-lookup"><span data-stu-id="3df75-115">Task</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3df75-116">备注</span><span class="sxs-lookup"><span data-stu-id="3df75-116">Remarks</span></span>

<span data-ttu-id="3df75-117">此属性的值必须大于或等于 0.0 数字和小于或等于 1.0，其中 1.0 表示为完成工作，和 0.0 指示工作尚未开始。</span><span class="sxs-lookup"><span data-stu-id="3df75-117">The value of this property must be a number greater than or equal to 0.0 and less than or equal to 1.0, where 1.0 indicates that work is completed and 0.0 indicates that work has not begun.</span></span>
  
<span data-ttu-id="3df75-118">对于时间已标记的邮件对象，此属性的值必须设置为 1.0 如果标记对象已完成，并且应在否则设置为 0.0。</span><span class="sxs-lookup"><span data-stu-id="3df75-118">For a time-flagged message object, the value of this property must be set to 1.0 if the object is flagged completed, and should be set to 0.0 otherwise.</span></span>
  
## <a name="related-resources"></a><span data-ttu-id="3df75-119">相关资源</span><span class="sxs-lookup"><span data-stu-id="3df75-119">Related resources</span></span>

### <a name="protocol-specifications"></a><span data-ttu-id="3df75-120">协议规范</span><span class="sxs-lookup"><span data-stu-id="3df75-120">Protocol specifications</span></span>

<span data-ttu-id="3df75-121">[[MS OXPROPS]](http://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="3df75-121">[[MS-OXPROPS]](http://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)</span></span>
  
> <span data-ttu-id="3df75-122">提供属性集定义和相关的 Exchange Server 协议规范的引用。</span><span class="sxs-lookup"><span data-stu-id="3df75-122">Provides property set definitions and references to related Exchange Server protocol specifications.</span></span>
    
<span data-ttu-id="3df75-123">[[MS OXOTASK]](http://msdn.microsoft.com/library/55600ec0-6195-4730-8436-59c7931ef27e%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="3df75-123">[[MS-OXOTASK]](http://msdn.microsoft.com/library/55600ec0-6195-4730-8436-59c7931ef27e%28Office.15%29.aspx)</span></span>
  
> <span data-ttu-id="3df75-124">定义模型的任务、 任务分配和任务更新电子等效项的多个对象。</span><span class="sxs-lookup"><span data-stu-id="3df75-124">Defines several objects that model the electronic equivalent of tasks, task assignments, and task updates.</span></span>
    
<span data-ttu-id="3df75-125">[[MS OXOFLAG]](http://msdn.microsoft.com/library/f1e50be4-ed30-4c2a-b5cb-8ff3aaaf9b91%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="3df75-125">[[MS-OXOFLAG]](http://msdn.microsoft.com/library/f1e50be4-ed30-4c2a-b5cb-8ff3aaaf9b91%28Office.15%29.aspx)</span></span>
  
> <span data-ttu-id="3df75-126">指定的属性和与标记的操作。</span><span class="sxs-lookup"><span data-stu-id="3df75-126">Specifies the properties and operations related to flagging.</span></span>
    
<span data-ttu-id="3df75-127">[[MS OXCMAIL]](http://msdn.microsoft.com/library/b60d48db-183f-4bf5-a908-f584e62cb2d4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="3df75-127">[[MS-OXCMAIL]](http://msdn.microsoft.com/library/b60d48db-183f-4bf5-a908-f584e62cb2d4%28Office.15%29.aspx)</span></span>
  
> <span data-ttu-id="3df75-128">从 Internet 标准电子邮件约定转换为消息对象。</span><span class="sxs-lookup"><span data-stu-id="3df75-128">Converts from Internet standard email conventions to message objects.</span></span>
    
<span data-ttu-id="3df75-129">[[MS OXCICAL]](http://msdn.microsoft.com/library/a685a040-5b69-4c84-b084-795113fb4012%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="3df75-129">[[MS-OXCICAL]](http://msdn.microsoft.com/library/a685a040-5b69-4c84-b084-795113fb4012%28Office.15%29.aspx)</span></span>
  
> <span data-ttu-id="3df75-130">IETF RFC2445、 RFC2446，和 RFC2447，和约会和会议对象之间进行转换。</span><span class="sxs-lookup"><span data-stu-id="3df75-130">Converts between IETF RFC2445, RFC2446, and RFC2447, and appointment and meeting objects.</span></span>
    
<span data-ttu-id="3df75-131">[[MS OXCFXICS]](http://msdn.microsoft.com/library/b9752f3d-d50d-44b8-9e6b-608a117c8532%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="3df75-131">[[MS-OXCFXICS]](http://msdn.microsoft.com/library/b9752f3d-d50d-44b8-9e6b-608a117c8532%28Office.15%29.aspx)</span></span>
  
> <span data-ttu-id="3df75-132">处理顺序和客户端和服务器之间的数据传输的流。</span><span class="sxs-lookup"><span data-stu-id="3df75-132">Handles the order and flow for data transfers between a client and server.</span></span>
    
### <a name="header-files"></a><span data-ttu-id="3df75-133">头文件</span><span class="sxs-lookup"><span data-stu-id="3df75-133">Header files</span></span>

<span data-ttu-id="3df75-134">Mapidefs.h</span><span class="sxs-lookup"><span data-stu-id="3df75-134">Mapidefs.h</span></span>
  
> <span data-ttu-id="3df75-135">提供数据类型定义。</span><span class="sxs-lookup"><span data-stu-id="3df75-135">Provides data type definitions.</span></span>
    
## <a name="see-also"></a><span data-ttu-id="3df75-136">另请参阅</span><span class="sxs-lookup"><span data-stu-id="3df75-136">See also</span></span>



[<span data-ttu-id="3df75-137">MAPI 属性</span><span class="sxs-lookup"><span data-stu-id="3df75-137">MAPI Properties</span></span>](mapi-properties.md)
  
[<span data-ttu-id="3df75-138">MAPI 规范属性</span><span class="sxs-lookup"><span data-stu-id="3df75-138">MAPI Canonical Properties</span></span>](mapi-canonical-properties.md)
  
[<span data-ttu-id="3df75-139">映射到 MAPI 名称的规范属性名称</span><span class="sxs-lookup"><span data-stu-id="3df75-139">Mapping Canonical Property Names to MAPI Names</span></span>](mapping-canonical-property-names-to-mapi-names.md)
  
[<span data-ttu-id="3df75-140">MAPI 名称映射到规范属性名称</span><span class="sxs-lookup"><span data-stu-id="3df75-140">Mapping MAPI Names to Canonical Property Names</span></span>](mapping-mapi-names-to-canonical-property-names.md)
