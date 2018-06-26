---
title: PidLidReminderSet 规范属性
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PidLidReminderSet
api_type:
- COM
ms.assetid: 06b7792c-1b43-4e20-9a3b-44f2664b2125
description: 上次修改时间： 2015 年 3 月 9 日
ms.openlocfilehash: fd40be7733934002b81482a8bf5cfe8c9ce12313
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19777004"
---
# <a name="pidlidreminderset-canonical-property"></a><span data-ttu-id="73703-103">PidLidReminderSet 规范属性</span><span class="sxs-lookup"><span data-stu-id="73703-103">PidLidReminderSet Canonical Property</span></span>

  
  
<span data-ttu-id="73703-104">**适用于**： Outlook</span><span class="sxs-lookup"><span data-stu-id="73703-104">**Applies to**: Outlook</span></span> 
  
<span data-ttu-id="73703-105">指定是否在对象上设置提醒。</span><span class="sxs-lookup"><span data-stu-id="73703-105">Specifies whether a reminder is set on the object.</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="73703-106">关联的属性：</span><span class="sxs-lookup"><span data-stu-id="73703-106">Associated properties:</span></span>  <br/> |<span data-ttu-id="73703-107">dispidReminderSet</span><span class="sxs-lookup"><span data-stu-id="73703-107">dispidReminderSet</span></span>  <br/> |
|<span data-ttu-id="73703-108">属性进行设置：</span><span class="sxs-lookup"><span data-stu-id="73703-108">Property set:</span></span>  <br/> |<span data-ttu-id="73703-109">PSETID_Common</span><span class="sxs-lookup"><span data-stu-id="73703-109">PSETID_Common</span></span>  <br/> |
|<span data-ttu-id="73703-110">长 ID （盖）：</span><span class="sxs-lookup"><span data-stu-id="73703-110">Long ID (LID):</span></span>  <br/> |<span data-ttu-id="73703-111">0x00008503</span><span class="sxs-lookup"><span data-stu-id="73703-111">0x00008503</span></span>  <br/> |
|<span data-ttu-id="73703-112">数据类型：</span><span class="sxs-lookup"><span data-stu-id="73703-112">Data type:</span></span>  <br/> |<span data-ttu-id="73703-113">PT_BOOLEAN</span><span class="sxs-lookup"><span data-stu-id="73703-113">PT_BOOLEAN</span></span>  <br/> |
|<span data-ttu-id="73703-114">区域：</span><span class="sxs-lookup"><span data-stu-id="73703-114">Area:</span></span>  <br/> |<span data-ttu-id="73703-115">提醒</span><span class="sxs-lookup"><span data-stu-id="73703-115">Reminder</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="73703-116">备注</span><span class="sxs-lookup"><span data-stu-id="73703-116">Remarks</span></span>

<span data-ttu-id="73703-117">如果定期 calendar 对象具有此属性设置为 TRUE，客户端可以替代此值的例外。</span><span class="sxs-lookup"><span data-stu-id="73703-117">If a recurring calendar object has this property set to TRUE, the client can override this value for exceptions.</span></span>
  
<span data-ttu-id="73703-118">如果此属性为 false，则在定期 calendar 对象，禁用整个数据系列，包括例外提醒。</span><span class="sxs-lookup"><span data-stu-id="73703-118">If this property is FALSE on a recurring calendar object, reminders are disabled for the entire series, including exceptions.</span></span> <span data-ttu-id="73703-119">对于定期任务对象，该属性不能重写由异常 （有关详细信息，请参阅[[MS OXOCAL]](http://msdn.microsoft.com/library/09861fde-c8e4-4028-9346-e7c214cfdba1%28Office.15%29.aspx)和[[MS OXOTASK]](http://msdn.microsoft.com/library/55600ec0-6195-4730-8436-59c7931ef27e%28Office.15%29.aspx) ）。</span><span class="sxs-lookup"><span data-stu-id="73703-119">For recurring task objects, this property cannot be overridden by exceptions (see [[MS-OXOCAL]](http://msdn.microsoft.com/library/09861fde-c8e4-4028-9346-e7c214cfdba1%28Office.15%29.aspx) and [[MS-OXOTASK]](http://msdn.microsoft.com/library/55600ec0-6195-4730-8436-59c7931ef27e%28Office.15%29.aspx) for details).</span></span> 
  
## <a name="related-resources"></a><span data-ttu-id="73703-120">相关资源</span><span class="sxs-lookup"><span data-stu-id="73703-120">Related resources</span></span>

### <a name="protocol-specifications"></a><span data-ttu-id="73703-121">协议规范</span><span class="sxs-lookup"><span data-stu-id="73703-121">Protocol specifications</span></span>

<span data-ttu-id="73703-122">[[MS OXPROPS]](http://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="73703-122">[[MS-OXPROPS]](http://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)</span></span>
  
> <span data-ttu-id="73703-123">提供属性集定义和相关的 Exchange Server 协议规范的引用。</span><span class="sxs-lookup"><span data-stu-id="73703-123">Provides property set definitions and references to related Exchange Server protocol specifications.</span></span>
    
<span data-ttu-id="73703-124">[[MS OXORMDR]](http://msdn.microsoft.com/library/5454ebcc-e5d1-4da8-a598-d393b101caab%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="73703-124">[[MS-OXORMDR]](http://msdn.microsoft.com/library/5454ebcc-e5d1-4da8-a598-d393b101caab%28Office.15%29.aspx)</span></span>
  
> <span data-ttu-id="73703-125">指定属性和电子邮件和其他对象提醒的交互模型。</span><span class="sxs-lookup"><span data-stu-id="73703-125">Specifies the properties and the interaction model for email and other object reminders.</span></span>
    
### <a name="header-files"></a><span data-ttu-id="73703-126">头文件</span><span class="sxs-lookup"><span data-stu-id="73703-126">Header files</span></span>

<span data-ttu-id="73703-127">Mapidefs.h</span><span class="sxs-lookup"><span data-stu-id="73703-127">Mapidefs.h</span></span>
  
> <span data-ttu-id="73703-128">提供数据类型定义。</span><span class="sxs-lookup"><span data-stu-id="73703-128">Provides data type definitions.</span></span>
    
## <a name="see-also"></a><span data-ttu-id="73703-129">另请参阅</span><span class="sxs-lookup"><span data-stu-id="73703-129">See also</span></span>



[<span data-ttu-id="73703-130">MAPI 属性</span><span class="sxs-lookup"><span data-stu-id="73703-130">MAPI Properties</span></span>](mapi-properties.md)
  
[<span data-ttu-id="73703-131">MAPI 规范属性</span><span class="sxs-lookup"><span data-stu-id="73703-131">MAPI Canonical Properties</span></span>](mapi-canonical-properties.md)
  
[<span data-ttu-id="73703-132">映射到 MAPI 名称的规范属性名称</span><span class="sxs-lookup"><span data-stu-id="73703-132">Mapping Canonical Property Names to MAPI Names</span></span>](mapping-canonical-property-names-to-mapi-names.md)
  
[<span data-ttu-id="73703-133">MAPI 名称映射到规范属性名称</span><span class="sxs-lookup"><span data-stu-id="73703-133">Mapping MAPI Names to Canonical Property Names</span></span>](mapping-mapi-names-to-canonical-property-names.md)
