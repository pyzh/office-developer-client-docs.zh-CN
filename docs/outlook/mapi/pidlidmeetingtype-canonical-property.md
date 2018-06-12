---
title: PidLidMeetingType 规范属性
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PidLidMeetingType
api_type:
- COM
ms.assetid: 290b290c-7836-4a7e-bf1a-8d0225a07e56
description: 上次修改时间： 2015 年 3 月 9 日
ms.openlocfilehash: e61ce7798c9e41dbb707d0d5773b116f7cce02d6
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19776908"
---
# <a name="pidlidmeetingtype-canonical-property"></a><span data-ttu-id="7c1a5-103">PidLidMeetingType 规范属性</span><span class="sxs-lookup"><span data-stu-id="7c1a5-103">PidLidMeetingType Canonical Property</span></span>

  
  
<span data-ttu-id="7c1a5-104">**适用于**： Outlook</span><span class="sxs-lookup"><span data-stu-id="7c1a5-104">**Applies to**: Outlook</span></span> 
  
<span data-ttu-id="7c1a5-105">指示会议请求或会议更新的类型。</span><span class="sxs-lookup"><span data-stu-id="7c1a5-105">Indicates the type of meeting request or meeting update.</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="7c1a5-106">关联的属性：</span><span class="sxs-lookup"><span data-stu-id="7c1a5-106">Associated properties:</span></span>  <br/> |<span data-ttu-id="7c1a5-107">dispidMeetingType</span><span class="sxs-lookup"><span data-stu-id="7c1a5-107">dispidMeetingType</span></span>  <br/> |
|<span data-ttu-id="7c1a5-108">属性进行设置：</span><span class="sxs-lookup"><span data-stu-id="7c1a5-108">Property set:</span></span>  <br/> |<span data-ttu-id="7c1a5-109">PSETID_Meeting</span><span class="sxs-lookup"><span data-stu-id="7c1a5-109">PSETID_Meeting</span></span>  <br/> |
|<span data-ttu-id="7c1a5-110">长 ID （盖）：</span><span class="sxs-lookup"><span data-stu-id="7c1a5-110">Long ID (LID):</span></span>  <br/> |<span data-ttu-id="7c1a5-111">0x00000026</span><span class="sxs-lookup"><span data-stu-id="7c1a5-111">0x00000026</span></span>  <br/> |
|<span data-ttu-id="7c1a5-112">数据类型：</span><span class="sxs-lookup"><span data-stu-id="7c1a5-112">Data type:</span></span>  <br/> |<span data-ttu-id="7c1a5-113">PT_LONG</span><span class="sxs-lookup"><span data-stu-id="7c1a5-113">PT_LONG</span></span>  <br/> |
|<span data-ttu-id="7c1a5-114">区域：</span><span class="sxs-lookup"><span data-stu-id="7c1a5-114">Area:</span></span>  <br/> |<span data-ttu-id="7c1a5-115">会议</span><span class="sxs-lookup"><span data-stu-id="7c1a5-115">Meetings</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7c1a5-116">备注</span><span class="sxs-lookup"><span data-stu-id="7c1a5-116">Remarks</span></span>

<span data-ttu-id="7c1a5-117">此属性的值必须设置为下列选项之一：</span><span class="sxs-lookup"><span data-stu-id="7c1a5-117">The value of this property must be set to one of the following:</span></span>
  
|<span data-ttu-id="7c1a5-118">**属性**</span><span class="sxs-lookup"><span data-stu-id="7c1a5-118">**Property**</span></span>|<span data-ttu-id="7c1a5-119">**值**</span><span class="sxs-lookup"><span data-stu-id="7c1a5-119">**Value**</span></span>|<span data-ttu-id="7c1a5-120">**说明**</span><span class="sxs-lookup"><span data-stu-id="7c1a5-120">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7c1a5-121">mtgEmpty</span><span class="sxs-lookup"><span data-stu-id="7c1a5-121">mtgEmpty</span></span>  <br/> |<span data-ttu-id="7c1a5-122">0x00000000</span><span class="sxs-lookup"><span data-stu-id="7c1a5-122">0x00000000</span></span>  <br/> |<span data-ttu-id="7c1a5-123">未指定。</span><span class="sxs-lookup"><span data-stu-id="7c1a5-123">Unspecified.</span></span>  <br/> |
|<span data-ttu-id="7c1a5-124">mtgRequest</span><span class="sxs-lookup"><span data-stu-id="7c1a5-124">mtgRequest</span></span>  <br/> |<span data-ttu-id="7c1a5-125">0x00000001</span><span class="sxs-lookup"><span data-stu-id="7c1a5-125">0x00000001</span></span>  <br/> |<span data-ttu-id="7c1a5-126">初始的会议请求。</span><span class="sxs-lookup"><span data-stu-id="7c1a5-126">Initial meeting request.</span></span>  <br/> |
|<span data-ttu-id="7c1a5-127">mtgFull</span><span class="sxs-lookup"><span data-stu-id="7c1a5-127">mtgFull</span></span>  <br/> |<span data-ttu-id="7c1a5-128">0x00010000</span><span class="sxs-lookup"><span data-stu-id="7c1a5-128">0x00010000</span></span>  <br/> |<span data-ttu-id="7c1a5-129">完全更新。</span><span class="sxs-lookup"><span data-stu-id="7c1a5-129">Full update.</span></span>  <br/> |
|<span data-ttu-id="7c1a5-130">mtgInfo</span><span class="sxs-lookup"><span data-stu-id="7c1a5-130">mtgInfo</span></span>  <br/> |<span data-ttu-id="7c1a5-131">0x00020000</span><span class="sxs-lookup"><span data-stu-id="7c1a5-131">0x00020000</span></span>  <br/> |<span data-ttu-id="7c1a5-132">信息性更新。</span><span class="sxs-lookup"><span data-stu-id="7c1a5-132">Informational update.</span></span>  <br/> |
|<span data-ttu-id="7c1a5-133">mtgOutOfDate</span><span class="sxs-lookup"><span data-stu-id="7c1a5-133">mtgOutOfDate</span></span>  <br/> |<span data-ttu-id="7c1a5-134">0x00080000</span><span class="sxs-lookup"><span data-stu-id="7c1a5-134">0x00080000</span></span>  <br/> |<span data-ttu-id="7c1a5-135">此之后收到较新的会议请求或会议更新。</span><span class="sxs-lookup"><span data-stu-id="7c1a5-135">A newer meeting request or meeting update was received after this one.</span></span>  <br/> |
|<span data-ttu-id="7c1a5-136">mtgDelegatorCopy</span><span class="sxs-lookup"><span data-stu-id="7c1a5-136">mtgDelegatorCopy</span></span>  <br/> |<span data-ttu-id="7c1a5-137">0x00100000</span><span class="sxs-lookup"><span data-stu-id="7c1a5-137">0x00100000</span></span>  <br/> |<span data-ttu-id="7c1a5-138">这是设置 delegator 副本时委托处理与会议相关的对象。</span><span class="sxs-lookup"><span data-stu-id="7c1a5-138">This is set on the delegator's copy when a delegate handles meeting-related objects.</span></span>  <br/> |
   
## <a name="related-resources"></a><span data-ttu-id="7c1a5-139">相关资源</span><span class="sxs-lookup"><span data-stu-id="7c1a5-139">Related resources</span></span>

### <a name="protocol-specifications"></a><span data-ttu-id="7c1a5-140">协议规范</span><span class="sxs-lookup"><span data-stu-id="7c1a5-140">Protocol specifications</span></span>

<span data-ttu-id="7c1a5-141">[[MS OXPROPS]](http://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="7c1a5-141">[[MS-OXPROPS]](http://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)</span></span>
  
> <span data-ttu-id="7c1a5-142">提供属性集定义和相关的 Exchange Server 协议规范的引用。</span><span class="sxs-lookup"><span data-stu-id="7c1a5-142">Provides property set definitions and references to related Exchange Server protocol specifications.</span></span>
    
<span data-ttu-id="7c1a5-143">[[MS OXOCAL]](http://msdn.microsoft.com/library/09861fde-c8e4-4028-9346-e7c214cfdba1%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="7c1a5-143">[[MS-OXOCAL]](http://msdn.microsoft.com/library/09861fde-c8e4-4028-9346-e7c214cfdba1%28Office.15%29.aspx)</span></span>
  
> <span data-ttu-id="7c1a5-144">指定的属性和约会、 会议请求和响应消息的操作。</span><span class="sxs-lookup"><span data-stu-id="7c1a5-144">Specifies the properties and operations for appointment, meeting request, and response messages.</span></span>
    
### <a name="header-files"></a><span data-ttu-id="7c1a5-145">头文件</span><span class="sxs-lookup"><span data-stu-id="7c1a5-145">Header files</span></span>

<span data-ttu-id="7c1a5-146">Mapidefs.h</span><span class="sxs-lookup"><span data-stu-id="7c1a5-146">Mapidefs.h</span></span>
  
> <span data-ttu-id="7c1a5-147">提供数据类型定义。</span><span class="sxs-lookup"><span data-stu-id="7c1a5-147">Provides data type definitions.</span></span>
    
## <a name="see-also"></a><span data-ttu-id="7c1a5-148">另请参阅</span><span class="sxs-lookup"><span data-stu-id="7c1a5-148">See also</span></span>



[<span data-ttu-id="7c1a5-149">MAPI 属性</span><span class="sxs-lookup"><span data-stu-id="7c1a5-149">MAPI Properties</span></span>](mapi-properties.md)
  
[<span data-ttu-id="7c1a5-150">MAPI 规范属性</span><span class="sxs-lookup"><span data-stu-id="7c1a5-150">MAPI Canonical Properties</span></span>](mapi-canonical-properties.md)
  
[<span data-ttu-id="7c1a5-151">映射到 MAPI 名称的规范属性名称</span><span class="sxs-lookup"><span data-stu-id="7c1a5-151">Mapping Canonical Property Names to MAPI Names</span></span>](mapping-canonical-property-names-to-mapi-names.md)
  
[<span data-ttu-id="7c1a5-152">MAPI 名称映射到规范属性名称</span><span class="sxs-lookup"><span data-stu-id="7c1a5-152">Mapping MAPI Names to Canonical Property Names</span></span>](mapping-mapi-names-to-canonical-property-names.md)
