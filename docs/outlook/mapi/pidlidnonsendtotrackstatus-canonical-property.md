---
title: PidLidNonSendToTrackStatus 规范属性
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PidLidNonSendToTrackStatus
api_type:
- COM
ms.assetid: 50fec332-e7df-4bc6-8c50-59b9ca545f89
description: 上次修改时间： 2015 年 3 月 9 日
ms.openlocfilehash: 45d8512d48a1908d81e78b87c5975ab2da8c6c80
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19776926"
---
# <a name="pidlidnonsendtotrackstatus-canonical-property"></a><span data-ttu-id="34ac4-103">PidLidNonSendToTrackStatus 规范属性</span><span class="sxs-lookup"><span data-stu-id="34ac4-103">PidLidNonSendToTrackStatus Canonical Property</span></span>

  
  
<span data-ttu-id="34ac4-104">**适用于**： Outlook</span><span class="sxs-lookup"><span data-stu-id="34ac4-104">**Applies to**: Outlook</span></span> 
  
<span data-ttu-id="34ac4-105">包含的每个与会者的**dispidNonSendableTo** ([PidLidNonSendableTo](pidlidnonsendableto-canonical-property.md)) 属性中列出的值。</span><span class="sxs-lookup"><span data-stu-id="34ac4-105">Contains the value for each attendee listed in the **dispidNonSendableTo** ([PidLidNonSendableTo](pidlidnonsendableto-canonical-property.md)) property.</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="34ac4-106">关联的属性：</span><span class="sxs-lookup"><span data-stu-id="34ac4-106">Associated properties:</span></span>  <br/> |<span data-ttu-id="34ac4-107">dispidNonSendToTrackStatus</span><span class="sxs-lookup"><span data-stu-id="34ac4-107">dispidNonSendToTrackStatus</span></span>  <br/> |
|<span data-ttu-id="34ac4-108">属性进行设置：</span><span class="sxs-lookup"><span data-stu-id="34ac4-108">Property set:</span></span>  <br/> |<span data-ttu-id="34ac4-109">PSETID_Common</span><span class="sxs-lookup"><span data-stu-id="34ac4-109">PSETID_Common</span></span>  <br/> |
|<span data-ttu-id="34ac4-110">长 ID （盖）：</span><span class="sxs-lookup"><span data-stu-id="34ac4-110">Long ID (LID):</span></span>  <br/> |<span data-ttu-id="34ac4-111">0x00008543</span><span class="sxs-lookup"><span data-stu-id="34ac4-111">0x00008543</span></span>  <br/> |
|<span data-ttu-id="34ac4-112">数据类型：</span><span class="sxs-lookup"><span data-stu-id="34ac4-112">Data type:</span></span>  <br/> |<span data-ttu-id="34ac4-113">PT_MV_LONG</span><span class="sxs-lookup"><span data-stu-id="34ac4-113">PT_MV_LONG</span></span>  <br/> |
|<span data-ttu-id="34ac4-114">区域：</span><span class="sxs-lookup"><span data-stu-id="34ac4-114">Area:</span></span>  <br/> |<span data-ttu-id="34ac4-115">常规消息</span><span class="sxs-lookup"><span data-stu-id="34ac4-115">General messaging</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="34ac4-116">备注</span><span class="sxs-lookup"><span data-stu-id="34ac4-116">Remarks</span></span>

<span data-ttu-id="34ac4-117">仅当**dispidNonSendableTo**属性设置时，此属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="34ac4-117">This property is required only when the **dispidNonSendableTo** property is set.</span></span> <span data-ttu-id="34ac4-118">此属性中的值的数目必须等于**dispidNonSendableTo**中值的数目。</span><span class="sxs-lookup"><span data-stu-id="34ac4-118">The number of values in this property must equal the number of values in **dispidNonSendableTo**.</span></span> <span data-ttu-id="34ac4-119">此属性中的每个 PT_LONG 值对应于**dispidNonSendableTo**属性在同一索引中的与会者。</span><span class="sxs-lookup"><span data-stu-id="34ac4-119">Each PT_LONG value in this property corresponds to the attendee in the **dispidNonSendableTo** property at the same index.</span></span> 
  
## <a name="related-resources"></a><span data-ttu-id="34ac4-120">相关资源</span><span class="sxs-lookup"><span data-stu-id="34ac4-120">Related resources</span></span>

### <a name="protocol-specifications"></a><span data-ttu-id="34ac4-121">协议规范</span><span class="sxs-lookup"><span data-stu-id="34ac4-121">Protocol specifications</span></span>

<span data-ttu-id="34ac4-122">[[MS OXPROPS]](http://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="34ac4-122">[[MS-OXPROPS]](http://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)</span></span>
  
> <span data-ttu-id="34ac4-123">提供属性集定义和相关的 Exchange Server 协议规范的引用。</span><span class="sxs-lookup"><span data-stu-id="34ac4-123">Provides property set definition and references to related Exchange Server protocol specifications.</span></span>
    
<span data-ttu-id="34ac4-124">[[MS OXOCAL]](http://msdn.microsoft.com/library/09861fde-c8e4-4028-9346-e7c214cfdba1%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="34ac4-124">[[MS-OXOCAL]](http://msdn.microsoft.com/library/09861fde-c8e4-4028-9346-e7c214cfdba1%28Office.15%29.aspx)</span></span>
  
> <span data-ttu-id="34ac4-125">指定的属性和约会、 会议请求和响应消息的操作。</span><span class="sxs-lookup"><span data-stu-id="34ac4-125">Specifies the properties and operations for appointment, meeting request, and response messages.</span></span>
    
### <a name="header-files"></a><span data-ttu-id="34ac4-126">头文件</span><span class="sxs-lookup"><span data-stu-id="34ac4-126">Header files</span></span>

<span data-ttu-id="34ac4-127">Mapidefs.h</span><span class="sxs-lookup"><span data-stu-id="34ac4-127">Mapidefs.h</span></span>
  
> <span data-ttu-id="34ac4-128">提供数据类型定义。</span><span class="sxs-lookup"><span data-stu-id="34ac4-128">Provides data type definitions.</span></span>
    
## <a name="see-also"></a><span data-ttu-id="34ac4-129">另请参阅</span><span class="sxs-lookup"><span data-stu-id="34ac4-129">See also</span></span>



[<span data-ttu-id="34ac4-130">MAPI 属性</span><span class="sxs-lookup"><span data-stu-id="34ac4-130">MAPI Properties</span></span>](mapi-properties.md)
  
[<span data-ttu-id="34ac4-131">MAPI 规范属性</span><span class="sxs-lookup"><span data-stu-id="34ac4-131">MAPI Canonical Properties</span></span>](mapi-canonical-properties.md)
  
[<span data-ttu-id="34ac4-132">映射到 MAPI 名称的规范属性名称</span><span class="sxs-lookup"><span data-stu-id="34ac4-132">Mapping Canonical Property Names to MAPI Names</span></span>](mapping-canonical-property-names-to-mapi-names.md)
  
[<span data-ttu-id="34ac4-133">MAPI 名称映射到规范属性名称</span><span class="sxs-lookup"><span data-stu-id="34ac4-133">Mapping MAPI Names to Canonical Property Names</span></span>](mapping-mapi-names-to-canonical-property-names.md)
