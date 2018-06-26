---
title: PidTagDeliverTime 规范属性
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PidTagDeliverTime
api_type:
- HeaderDef
ms.assetid: da0ad17b-08ac-4c50-ac1d-13062b890dfd
description: 上次修改时间： 2015 年 3 月 9 日
ms.openlocfilehash: 40839e34a61b5e5fdd3d7b69d8c553d7e469cd22
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19777544"
---
# <a name="pidtagdelivertime-canonical-property"></a><span data-ttu-id="49cb6-103">PidTagDeliverTime 规范属性</span><span class="sxs-lookup"><span data-stu-id="49cb6-103">PidTagDeliverTime Canonical Property</span></span>

  
  
<span data-ttu-id="49cb6-104">**适用于**： Outlook</span><span class="sxs-lookup"><span data-stu-id="49cb6-104">**Applies to**: Outlook</span></span> 
  
<span data-ttu-id="49cb6-105">包含的日期和时间时原始邮件已送达。</span><span class="sxs-lookup"><span data-stu-id="49cb6-105">Contains the date and time when the original message was delivered.</span></span> 
  
|||
|:-----|:-----|
|<span data-ttu-id="49cb6-106">关联的属性：</span><span class="sxs-lookup"><span data-stu-id="49cb6-106">Associated properties:</span></span>  <br/> |<span data-ttu-id="49cb6-107">PR_DELIVER_TIME</span><span class="sxs-lookup"><span data-stu-id="49cb6-107">PR_DELIVER_TIME</span></span>  <br/> |
|<span data-ttu-id="49cb6-108">标识符:</span><span class="sxs-lookup"><span data-stu-id="49cb6-108">Identifier:</span></span>  <br/> |<span data-ttu-id="49cb6-109">0x0010</span><span class="sxs-lookup"><span data-stu-id="49cb6-109">0x0010</span></span>  <br/> |
|<span data-ttu-id="49cb6-110">数据类型：</span><span class="sxs-lookup"><span data-stu-id="49cb6-110">Data type:</span></span>  <br/> |<span data-ttu-id="49cb6-111">PT_SYSTIME</span><span class="sxs-lookup"><span data-stu-id="49cb6-111">PT_SYSTIME</span></span>  <br/> |
|<span data-ttu-id="49cb6-112">区域：</span><span class="sxs-lookup"><span data-stu-id="49cb6-112">Area:</span></span>  <br/> |<span data-ttu-id="49cb6-113">MAPI 信封</span><span class="sxs-lookup"><span data-stu-id="49cb6-113">MAPI envelope</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="49cb6-114">备注</span><span class="sxs-lookup"><span data-stu-id="49cb6-114">Remarks</span></span>

<span data-ttu-id="49cb6-115">此属性是指示原始邮件已传递到为其生成送达报告的邮件用户的时间的送达报告的每个收件人属性。</span><span class="sxs-lookup"><span data-stu-id="49cb6-115">This property is a per-recipient property on a delivery report that indicates the time the original message was delivered to the messaging user for which the delivery report is being generated.</span></span>
  
## <a name="related-resources"></a><span data-ttu-id="49cb6-116">相关资源</span><span class="sxs-lookup"><span data-stu-id="49cb6-116">Related resources</span></span>

### <a name="header-files"></a><span data-ttu-id="49cb6-117">头文件</span><span class="sxs-lookup"><span data-stu-id="49cb6-117">Header files</span></span>

<span data-ttu-id="49cb6-118">Mapidefs.h</span><span class="sxs-lookup"><span data-stu-id="49cb6-118">Mapidefs.h</span></span>
  
> <span data-ttu-id="49cb6-119">提供数据类型定义。</span><span class="sxs-lookup"><span data-stu-id="49cb6-119">Provides data type definitions.</span></span>
    
<span data-ttu-id="49cb6-120">Mapitags.h</span><span class="sxs-lookup"><span data-stu-id="49cb6-120">Mapitags.h</span></span>
  
> <span data-ttu-id="49cb6-121">包含作为替代名称列出的属性的定义。</span><span class="sxs-lookup"><span data-stu-id="49cb6-121">Contains definitions of properties listed as alternate names.</span></span>
    
## <a name="see-also"></a><span data-ttu-id="49cb6-122">另请参阅</span><span class="sxs-lookup"><span data-stu-id="49cb6-122">See also</span></span>



[<span data-ttu-id="49cb6-123">IMAPISupport::StatusRecips</span><span class="sxs-lookup"><span data-stu-id="49cb6-123">IMAPISupport::StatusRecips</span></span>](imapisupport-statusrecips.md)


[<span data-ttu-id="49cb6-124">MAPI 属性</span><span class="sxs-lookup"><span data-stu-id="49cb6-124">MAPI Properties</span></span>](mapi-properties.md)
  
[<span data-ttu-id="49cb6-125">MAPI 规范属性</span><span class="sxs-lookup"><span data-stu-id="49cb6-125">MAPI Canonical Properties</span></span>](mapi-canonical-properties.md)
  
[<span data-ttu-id="49cb6-126">映射到 MAPI 名称的规范属性名称</span><span class="sxs-lookup"><span data-stu-id="49cb6-126">Mapping Canonical Property Names to MAPI Names</span></span>](mapping-canonical-property-names-to-mapi-names.md)
  
[<span data-ttu-id="49cb6-127">MAPI 名称映射到规范属性名称</span><span class="sxs-lookup"><span data-stu-id="49cb6-127">Mapping MAPI Names to Canonical Property Names</span></span>](mapping-mapi-names-to-canonical-property-names.md)
