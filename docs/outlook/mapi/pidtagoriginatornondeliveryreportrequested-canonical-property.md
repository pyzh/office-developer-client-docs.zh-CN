---
title: PidTagOriginatorNonDeliveryReportRequested 规范属性
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MAPI.PidTagOriginatorNonDeliveryReportRequested
api_type:
- COM
ms.assetid: 0a19ba44-abb0-4868-9d7d-75184058d4c0
description: 上次修改时间： 2015 年 3 月 9 日
ms.openlocfilehash: 841d2b14efc781d89727b0c7ed677f527526a4ff
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19777980"
---
# <a name="pidtagoriginatornondeliveryreportrequested-canonical-property"></a><span data-ttu-id="8be5a-103">PidTagOriginatorNonDeliveryReportRequested 规范属性</span><span class="sxs-lookup"><span data-stu-id="8be5a-103">PidTagOriginatorNonDeliveryReportRequested Canonical Property</span></span>

  
  
<span data-ttu-id="8be5a-104">**适用于**： Outlook</span><span class="sxs-lookup"><span data-stu-id="8be5a-104">**Applies to**: Outlook</span></span> 
  
<span data-ttu-id="8be5a-105">如果邮件发件人的特定收件人请求原件报表，包含 TRUE。</span><span class="sxs-lookup"><span data-stu-id="8be5a-105">Contains TRUE if a message sender requests a nondelivery report for a particular recipient.</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="8be5a-106">关联的属性：</span><span class="sxs-lookup"><span data-stu-id="8be5a-106">Associated properties:</span></span>  <br/> |<span data-ttu-id="8be5a-107">PR_ORIGINATOR_NON_DELIVERY_REPORT_REQUESTED</span><span class="sxs-lookup"><span data-stu-id="8be5a-107">PR_ORIGINATOR_NON_DELIVERY_REPORT_REQUESTED</span></span>  <br/> |
|<span data-ttu-id="8be5a-108">标识符:</span><span class="sxs-lookup"><span data-stu-id="8be5a-108">Identifier:</span></span>  <br/> |<span data-ttu-id="8be5a-109">0x0C08</span><span class="sxs-lookup"><span data-stu-id="8be5a-109">0x0C08</span></span>  <br/> |
|<span data-ttu-id="8be5a-110">数据类型：</span><span class="sxs-lookup"><span data-stu-id="8be5a-110">Data type:</span></span>  <br/> |<span data-ttu-id="8be5a-111">PT_BOOLEAN</span><span class="sxs-lookup"><span data-stu-id="8be5a-111">PT_BOOLEAN</span></span>  <br/> |
|<span data-ttu-id="8be5a-112">区域：</span><span class="sxs-lookup"><span data-stu-id="8be5a-112">Area:</span></span>  <br/> |<span data-ttu-id="8be5a-113">MIME</span><span class="sxs-lookup"><span data-stu-id="8be5a-113">MIME</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8be5a-114">备注</span><span class="sxs-lookup"><span data-stu-id="8be5a-114">Remarks</span></span>

<span data-ttu-id="8be5a-115">此属性用于直接在邮件系统中处理未传送的消息。</span><span class="sxs-lookup"><span data-stu-id="8be5a-115">This property is used to direct the messaging system in handling undelivered messages.</span></span> <span data-ttu-id="8be5a-116">在这种情况下，邮件还必须提供该**邮件已被阅读**([PidTagOriginatorDeliveryReportRequested](pidtagoriginatordeliveryreportrequested-canonical-property.md)) 属性设置为 FALSE。</span><span class="sxs-lookup"><span data-stu-id="8be5a-116">In this case, the message must also furnish the **PR_ORIGINATOR_DELIVERY_REPORT_REQUESTED** ([PidTagOriginatorDeliveryReportRequested](pidtagoriginatordeliveryreportrequested-canonical-property.md)) property set to FALSE.</span></span>
  
## <a name="related-resources"></a><span data-ttu-id="8be5a-117">相关资源</span><span class="sxs-lookup"><span data-stu-id="8be5a-117">Related resources</span></span>

### <a name="protocol-specifications"></a><span data-ttu-id="8be5a-118">协议规范</span><span class="sxs-lookup"><span data-stu-id="8be5a-118">Protocol specifications</span></span>

<span data-ttu-id="8be5a-119">[[MS OXOMSG]](http://msdn.microsoft.com/library/daa9120f-f325-4afb-a738-28f91049ab3c%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="8be5a-119">[[MS-OXOMSG]](http://msdn.microsoft.com/library/daa9120f-f325-4afb-a738-28f91049ab3c%28Office.15%29.aspx)</span></span>
  
> <span data-ttu-id="8be5a-120">指定的属性和操作所允许的电子邮件消息对象。</span><span class="sxs-lookup"><span data-stu-id="8be5a-120">Specifies the properties and operations that are permissible for email message objects.</span></span>
    
### <a name="header-files"></a><span data-ttu-id="8be5a-121">头文件</span><span class="sxs-lookup"><span data-stu-id="8be5a-121">Header files</span></span>

<span data-ttu-id="8be5a-122">Mapidefs.h</span><span class="sxs-lookup"><span data-stu-id="8be5a-122">Mapidefs.h</span></span>
  
> <span data-ttu-id="8be5a-123">提供数据类型定义。</span><span class="sxs-lookup"><span data-stu-id="8be5a-123">Provides data type definitions.</span></span>
    
<span data-ttu-id="8be5a-124">Mapitags.h</span><span class="sxs-lookup"><span data-stu-id="8be5a-124">Mapitags.h</span></span>
  
> <span data-ttu-id="8be5a-125">包含作为替代名称列出的属性的定义。</span><span class="sxs-lookup"><span data-stu-id="8be5a-125">Contains definitions of properties listed as alternate names.</span></span>
    
## <a name="see-also"></a><span data-ttu-id="8be5a-126">另请参阅</span><span class="sxs-lookup"><span data-stu-id="8be5a-126">See also</span></span>



[<span data-ttu-id="8be5a-127">MAPI 属性</span><span class="sxs-lookup"><span data-stu-id="8be5a-127">MAPI Properties</span></span>](mapi-properties.md)
  
[<span data-ttu-id="8be5a-128">MAPI 规范属性</span><span class="sxs-lookup"><span data-stu-id="8be5a-128">MAPI Canonical Properties</span></span>](mapi-canonical-properties.md)
  
[<span data-ttu-id="8be5a-129">映射到 MAPI 名称的规范属性名称</span><span class="sxs-lookup"><span data-stu-id="8be5a-129">Mapping Canonical Property Names to MAPI Names</span></span>](mapping-canonical-property-names-to-mapi-names.md)
  
[<span data-ttu-id="8be5a-130">MAPI 名称映射到规范属性名称</span><span class="sxs-lookup"><span data-stu-id="8be5a-130">Mapping MAPI Names to Canonical Property Names</span></span>](mapping-mapi-names-to-canonical-property-names.md)
