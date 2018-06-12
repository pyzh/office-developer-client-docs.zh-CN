---
title: PidTagAlternateRecipient 规范属性
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PidTagAlternateRecipient
api_type:
- HeaderDef
ms.assetid: df787b60-2f53-42ac-89b5-1b52c906f472
description: 上次修改时间： 2015 年 3 月 9 日
ms.openlocfilehash: ea78d9487e4929c2df3d49a9b85ba4aefac90a59
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19777307"
---
# <a name="pidtagalternaterecipient-canonical-property"></a><span data-ttu-id="22f55-103">PidTagAlternateRecipient 规范属性</span><span class="sxs-lookup"><span data-stu-id="22f55-103">PidTagAlternateRecipient Canonical Property</span></span>

  
  
<span data-ttu-id="22f55-104">**适用于**： Outlook</span><span class="sxs-lookup"><span data-stu-id="22f55-104">**Applies to**: Outlook</span></span> 
  
<span data-ttu-id="22f55-105">包含由原始收件人指定的备用收件人的项标识符的列表。</span><span class="sxs-lookup"><span data-stu-id="22f55-105">Contains a list of entry identifiers for alternate recipients designated by the original recipient.</span></span> 
  
|||
|:-----|:-----|
|<span data-ttu-id="22f55-106">关联的属性：</span><span class="sxs-lookup"><span data-stu-id="22f55-106">Associated properties:</span></span>  <br/> |<span data-ttu-id="22f55-107">PR_ALTERNATE_RECIPIENT</span><span class="sxs-lookup"><span data-stu-id="22f55-107">PR_ALTERNATE_RECIPIENT</span></span>  <br/> |
|<span data-ttu-id="22f55-108">标识符:</span><span class="sxs-lookup"><span data-stu-id="22f55-108">Identifier:</span></span>  <br/> |<span data-ttu-id="22f55-109">0x3A01</span><span class="sxs-lookup"><span data-stu-id="22f55-109">0x3A01</span></span>  <br/> |
|<span data-ttu-id="22f55-110">数据类型：</span><span class="sxs-lookup"><span data-stu-id="22f55-110">Data type:</span></span>  <br/> |<span data-ttu-id="22f55-111">PT_BINARY</span><span class="sxs-lookup"><span data-stu-id="22f55-111">PT_BINARY</span></span>  <br/> |
|<span data-ttu-id="22f55-112">区域：</span><span class="sxs-lookup"><span data-stu-id="22f55-112">Area:</span></span>  <br/> |<span data-ttu-id="22f55-113">Address</span><span class="sxs-lookup"><span data-stu-id="22f55-113">Address</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="22f55-114">备注</span><span class="sxs-lookup"><span data-stu-id="22f55-114">Remarks</span></span>

<span data-ttu-id="22f55-115">此属性用于自动转发邮件。</span><span class="sxs-lookup"><span data-stu-id="22f55-115">This property is used for auto forwarded messages.</span></span> <span data-ttu-id="22f55-116">它包含的备用收件人[FLATENTRYLIST](flatentrylist.md)结构。</span><span class="sxs-lookup"><span data-stu-id="22f55-116">It contains a [FLATENTRYLIST](flatentrylist.md) structure of alternate recipients.</span></span> <span data-ttu-id="22f55-117">如果不允许自动转接，或者如果已不指定任何备用收件人，则生成原件报表。</span><span class="sxs-lookup"><span data-stu-id="22f55-117">If autoforwarding is not permitted or if no alternate recipient has been designated, a nondelivery report is generated.</span></span> 
  
## <a name="related-resources"></a><span data-ttu-id="22f55-118">相关资源</span><span class="sxs-lookup"><span data-stu-id="22f55-118">Related resources</span></span>

### <a name="protocol-specifications"></a><span data-ttu-id="22f55-119">协议规范</span><span class="sxs-lookup"><span data-stu-id="22f55-119">Protocol specifications</span></span>

<span data-ttu-id="22f55-120">[[MS OXPROPS]](http://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="22f55-120">[[MS-OXPROPS]](http://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)</span></span>
  
> <span data-ttu-id="22f55-121">提供了相关的 Exchange Server 协议规范参考。</span><span class="sxs-lookup"><span data-stu-id="22f55-121">Provides references to related Exchange Server protocol specifications.</span></span>
    
<span data-ttu-id="22f55-122">[[MS OXCFXICS]](http://msdn.microsoft.com/library/b9752f3d-d50d-44b8-9e6b-608a117c8532%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="22f55-122">[[MS-OXCFXICS]](http://msdn.microsoft.com/library/b9752f3d-d50d-44b8-9e6b-608a117c8532%28Office.15%29.aspx)</span></span>
  
> <span data-ttu-id="22f55-123">处理顺序和客户端和服务器之间的数据传输的流。</span><span class="sxs-lookup"><span data-stu-id="22f55-123">Handles the order and flow for data transfers between a client and server.</span></span>
    
<span data-ttu-id="22f55-124">[[MS OXCICAL]](http://msdn.microsoft.com/library/a685a040-5b69-4c84-b084-795113fb4012%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="22f55-124">[[MS-OXCICAL]](http://msdn.microsoft.com/library/a685a040-5b69-4c84-b084-795113fb4012%28Office.15%29.aspx)</span></span>
  
> <span data-ttu-id="22f55-125">IETF RFC2445、 RFC2446，和 RFC2447，和约会和会议对象之间进行转换。</span><span class="sxs-lookup"><span data-stu-id="22f55-125">Converts between IETF RFC2445, RFC2446, and RFC2447, and appointment and meeting objects.</span></span>
    
<span data-ttu-id="22f55-126">[[MS OXTNEF]](http://msdn.microsoft.com/library/1f0544d7-30b7-4194-b58f-adc82f3763bb%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="22f55-126">[[MS-OXTNEF]](http://msdn.microsoft.com/library/1f0544d7-30b7-4194-b58f-adc82f3763bb%28Office.15%29.aspx)</span></span>
  
> <span data-ttu-id="22f55-127">进行编码和解码为有效的流表示形式的消息和附件对象。</span><span class="sxs-lookup"><span data-stu-id="22f55-127">Encodes and decodes message and attachment objects to an efficient stream representation.</span></span>
    
### <a name="header-files"></a><span data-ttu-id="22f55-128">头文件</span><span class="sxs-lookup"><span data-stu-id="22f55-128">Header files</span></span>

<span data-ttu-id="22f55-129">Mapitags.h</span><span class="sxs-lookup"><span data-stu-id="22f55-129">Mapitags.h</span></span>
  
> <span data-ttu-id="22f55-130">包含列为相关属性的属性的定义。</span><span class="sxs-lookup"><span data-stu-id="22f55-130">Contains definitions of properties listed as associated properties.</span></span>
    
<span data-ttu-id="22f55-131">Mapidefs.h</span><span class="sxs-lookup"><span data-stu-id="22f55-131">Mapidefs.h</span></span>
  
> <span data-ttu-id="22f55-132">提供数据类型定义。</span><span class="sxs-lookup"><span data-stu-id="22f55-132">Provides data type definitions.</span></span>
    
## <a name="see-also"></a><span data-ttu-id="22f55-133">另请参阅</span><span class="sxs-lookup"><span data-stu-id="22f55-133">See also</span></span>



[<span data-ttu-id="22f55-134">FLATENTRYLIST</span><span class="sxs-lookup"><span data-stu-id="22f55-134">FLATENTRYLIST</span></span>](flatentrylist.md)


[<span data-ttu-id="22f55-135">MAPI 属性</span><span class="sxs-lookup"><span data-stu-id="22f55-135">MAPI Properties</span></span>](mapi-properties.md)
  
[<span data-ttu-id="22f55-136">MAPI 规范属性</span><span class="sxs-lookup"><span data-stu-id="22f55-136">MAPI Canonical Properties</span></span>](mapi-canonical-properties.md)
  
[<span data-ttu-id="22f55-137">映射到 MAPI 名称的规范属性名称</span><span class="sxs-lookup"><span data-stu-id="22f55-137">Mapping Canonical Property Names to MAPI Names</span></span>](mapping-canonical-property-names-to-mapi-names.md)
  
[<span data-ttu-id="22f55-138">MAPI 名称映射到规范属性名称</span><span class="sxs-lookup"><span data-stu-id="22f55-138">Mapping MAPI Names to Canonical Property Names</span></span>](mapping-mapi-names-to-canonical-property-names.md)
