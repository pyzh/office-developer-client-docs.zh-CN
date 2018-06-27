---
title: PidTagReportDispositionOptions 规范属性
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_type:
- COM
ms.assetid: bf37786a-b6bd-48a6-a2ec-6a739a8ba0d7
description: 上次修改时间： 2015 年 3 月 9 日
ms.openlocfilehash: b01062a136ff5c6e43ddab1bfbead8ac602acccb
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19778197"
---
# <a name="pidtagreportdispositionoptions-canonical-property"></a><span data-ttu-id="04632-103">PidTagReportDispositionOptions 规范属性</span><span class="sxs-lookup"><span data-stu-id="04632-103">PidTagReportDispositionOptions Canonical Property</span></span>

  
  
<span data-ttu-id="04632-104">**适用于**： Outlook</span><span class="sxs-lookup"><span data-stu-id="04632-104">**Applies to**: Outlook</span></span> 
  
<span data-ttu-id="04632-105">映射到请求收款的消息的 MIME 处置选项标题。</span><span class="sxs-lookup"><span data-stu-id="04632-105">Maps to the MIME Disposition-Options header for messages that request receipts.</span></span> <span data-ttu-id="04632-106">此属性的值应为空字符串。</span><span class="sxs-lookup"><span data-stu-id="04632-106">The value of this property should be an empty string.</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="04632-107">关联的属性：</span><span class="sxs-lookup"><span data-stu-id="04632-107">Associated properties:</span></span>  <br/> |<span data-ttu-id="04632-108">PR_REPORT_DISPOSITION_OPTIONS，PR_REPORT_DISPOSITION_OPTIONS_A，PR_REPORT_DISPOSITION_OPTIONS_W</span><span class="sxs-lookup"><span data-stu-id="04632-108">PR_REPORT_DISPOSITION_OPTIONS, PR_REPORT_DISPOSITION_OPTIONS_A, PR_REPORT_DISPOSITION_OPTIONS_W</span></span>  <br/> |
|<span data-ttu-id="04632-109">标识符:</span><span class="sxs-lookup"><span data-stu-id="04632-109">Identifier:</span></span>  <br/> |<span data-ttu-id="04632-110">0x0085</span><span class="sxs-lookup"><span data-stu-id="04632-110">0x0085</span></span>  <br/> |
|<span data-ttu-id="04632-111">数据类型：</span><span class="sxs-lookup"><span data-stu-id="04632-111">Data type:</span></span>  <br/> |<span data-ttu-id="04632-112">PT_STRING8 PT_UNICODE</span><span class="sxs-lookup"><span data-stu-id="04632-112">PT_STRING8, PT_UNICODE</span></span>  <br/> |
|<span data-ttu-id="04632-113">区域：</span><span class="sxs-lookup"><span data-stu-id="04632-113">Area:</span></span>  <br/> |<span data-ttu-id="04632-114">MAPI 信封</span><span class="sxs-lookup"><span data-stu-id="04632-114">MAPI envelope</span></span>  <br/> |
   
## <a name="related-resources"></a><span data-ttu-id="04632-115">相关资源</span><span class="sxs-lookup"><span data-stu-id="04632-115">Related resources</span></span>

### <a name="protocol-specifications"></a><span data-ttu-id="04632-116">协议规范</span><span class="sxs-lookup"><span data-stu-id="04632-116">Protocol specifications</span></span>

<span data-ttu-id="04632-117">[[MS-OXPROPS]]</span><span class="sxs-lookup"><span data-stu-id="04632-117">[[MS-OXPROPS]]</span></span> 
  
> <span data-ttu-id="04632-118">提供了相关的 Exchange Server 协议规范参考。</span><span class="sxs-lookup"><span data-stu-id="04632-118">Provides references to related Exchange Server protocol specifications.</span></span>
    
### <a name="header-files"></a><span data-ttu-id="04632-119">头文件</span><span class="sxs-lookup"><span data-stu-id="04632-119">Header files</span></span>

<span data-ttu-id="04632-120">Mapidefs.h</span><span class="sxs-lookup"><span data-stu-id="04632-120">Mapidefs.h</span></span>
  
> <span data-ttu-id="04632-121">提供数据类型定义。</span><span class="sxs-lookup"><span data-stu-id="04632-121">Provides data type definitions.</span></span>
    
<span data-ttu-id="04632-122">Mapitags.h</span><span class="sxs-lookup"><span data-stu-id="04632-122">Mapitags.h</span></span>
  
> <span data-ttu-id="04632-123">包含列为相关属性的属性的定义。</span><span class="sxs-lookup"><span data-stu-id="04632-123">Contains definitions of properties listed as associated properties.</span></span>
    
## <a name="see-also"></a><span data-ttu-id="04632-124">另请参阅</span><span class="sxs-lookup"><span data-stu-id="04632-124">See also</span></span>



[<span data-ttu-id="04632-125">MAPI 属性</span><span class="sxs-lookup"><span data-stu-id="04632-125">MAPI Properties</span></span>](mapi-properties.md)
  
[<span data-ttu-id="04632-126">MAPI 规范属性</span><span class="sxs-lookup"><span data-stu-id="04632-126">MAPI Canonical Properties</span></span>](mapi-canonical-properties.md)
  
[<span data-ttu-id="04632-127">映射到 MAPI 名称的规范属性名称</span><span class="sxs-lookup"><span data-stu-id="04632-127">Mapping Canonical Property Names to MAPI Names</span></span>](mapping-canonical-property-names-to-mapi-names.md)
  
[<span data-ttu-id="04632-128">MAPI 名称映射到规范属性名称</span><span class="sxs-lookup"><span data-stu-id="04632-128">Mapping MAPI Names to Canonical Property Names</span></span>](mapping-mapi-names-to-canonical-property-names.md)
