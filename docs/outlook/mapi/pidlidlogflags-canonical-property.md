---
title: PidLidLogFlags 规范属性
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PidLidLogFlags
api_type:
- COM
ms.assetid: 3174d931-e045-44db-a203-a27c9c00f4fc
description: 上次修改时间： 2015 年 3 月 9 日
ms.openlocfilehash: 7b2dd30511927f8df8a8bc587a6b1fedd5854810
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19776900"
---
# <a name="pidlidlogflags-canonical-property"></a><span data-ttu-id="0f06f-103">PidLidLogFlags 规范属性</span><span class="sxs-lookup"><span data-stu-id="0f06f-103">PidLidLogFlags Canonical Property</span></span>

  
  
<span data-ttu-id="0f06f-104">**适用于**： Outlook</span><span class="sxs-lookup"><span data-stu-id="0f06f-104">**Applies to**: Outlook</span></span> 
  
<span data-ttu-id="0f06f-105">包含有关日记的元数据。</span><span class="sxs-lookup"><span data-stu-id="0f06f-105">Contains metadata about the journal.</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="0f06f-106">关联的属性：</span><span class="sxs-lookup"><span data-stu-id="0f06f-106">Associated properties:</span></span>  <br/> |<span data-ttu-id="0f06f-107">dispidLogFlags</span><span class="sxs-lookup"><span data-stu-id="0f06f-107">dispidLogFlags</span></span>  <br/> |
|<span data-ttu-id="0f06f-108">属性进行设置：</span><span class="sxs-lookup"><span data-stu-id="0f06f-108">Property set:</span></span>  <br/> |<span data-ttu-id="0f06f-109">PSETID_Log</span><span class="sxs-lookup"><span data-stu-id="0f06f-109">PSETID_Log</span></span>  <br/> |
|<span data-ttu-id="0f06f-110">长 ID （盖）：</span><span class="sxs-lookup"><span data-stu-id="0f06f-110">Long ID (LID):</span></span>  <br/> |<span data-ttu-id="0f06f-111">0x0000870C</span><span class="sxs-lookup"><span data-stu-id="0f06f-111">0x0000870C</span></span>  <br/> |
|<span data-ttu-id="0f06f-112">数据类型：</span><span class="sxs-lookup"><span data-stu-id="0f06f-112">Data type:</span></span>  <br/> |<span data-ttu-id="0f06f-113">PT_LONG</span><span class="sxs-lookup"><span data-stu-id="0f06f-113">PT_LONG</span></span>  <br/> |
|<span data-ttu-id="0f06f-114">区域：</span><span class="sxs-lookup"><span data-stu-id="0f06f-114">Area:</span></span>  <br/> |<span data-ttu-id="0f06f-115">日记</span><span class="sxs-lookup"><span data-stu-id="0f06f-115">Journal</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0f06f-116">备注</span><span class="sxs-lookup"><span data-stu-id="0f06f-116">Remarks</span></span>

<span data-ttu-id="0f06f-117">包含有关日记的元数据的位字段必须零个或"0x40000000"。</span><span class="sxs-lookup"><span data-stu-id="0f06f-117">The bit field that contains metadata about the journal must be either zero or "0x40000000".</span></span>
  
## <a name="related-resources"></a><span data-ttu-id="0f06f-118">相关资源</span><span class="sxs-lookup"><span data-stu-id="0f06f-118">Related resources</span></span>

### <a name="protocol-specifications"></a><span data-ttu-id="0f06f-119">协议规范</span><span class="sxs-lookup"><span data-stu-id="0f06f-119">Protocol specifications</span></span>

<span data-ttu-id="0f06f-120">[[MS OXPROPS]](http://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="0f06f-120">[[MS-OXPROPS]](http://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)</span></span>
  
> <span data-ttu-id="0f06f-121">提供属性集定义和相关的 Exchange Server 协议规范的引用。</span><span class="sxs-lookup"><span data-stu-id="0f06f-121">Provides property set definitions and references to related Exchange Server protocol specifications.</span></span>
    
<span data-ttu-id="0f06f-122">[[MS OXOJRNL]](http://msdn.microsoft.com/library/2aa04fd2-0f36-4ce4-9178-c0fc70aa8d43%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="0f06f-122">[[MS-OXOJRNL]](http://msdn.microsoft.com/library/2aa04fd2-0f36-4ce4-9178-c0fc70aa8d43%28Office.15%29.aspx)</span></span>
  
> <span data-ttu-id="0f06f-123">指定的属性和操作所允许的日志。</span><span class="sxs-lookup"><span data-stu-id="0f06f-123">Specifies the properties and operations that are permissible for journals.</span></span>
    
### <a name="header-files"></a><span data-ttu-id="0f06f-124">头文件</span><span class="sxs-lookup"><span data-stu-id="0f06f-124">Header files</span></span>

<span data-ttu-id="0f06f-125">Mapidefs.h</span><span class="sxs-lookup"><span data-stu-id="0f06f-125">Mapidefs.h</span></span>
  
> <span data-ttu-id="0f06f-126">提供数据类型定义。</span><span class="sxs-lookup"><span data-stu-id="0f06f-126">Provides data type definitions.</span></span>
    
## <a name="see-also"></a><span data-ttu-id="0f06f-127">另请参阅</span><span class="sxs-lookup"><span data-stu-id="0f06f-127">See also</span></span>



[<span data-ttu-id="0f06f-128">MAPI 属性</span><span class="sxs-lookup"><span data-stu-id="0f06f-128">MAPI Properties</span></span>](mapi-properties.md)
  
[<span data-ttu-id="0f06f-129">MAPI 规范属性</span><span class="sxs-lookup"><span data-stu-id="0f06f-129">MAPI Canonical Properties</span></span>](mapi-canonical-properties.md)
  
[<span data-ttu-id="0f06f-130">映射到 MAPI 名称的规范属性名称</span><span class="sxs-lookup"><span data-stu-id="0f06f-130">Mapping Canonical Property Names to MAPI Names</span></span>](mapping-canonical-property-names-to-mapi-names.md)
  
[<span data-ttu-id="0f06f-131">MAPI 名称映射到规范属性名称</span><span class="sxs-lookup"><span data-stu-id="0f06f-131">Mapping MAPI Names to Canonical Property Names</span></span>](mapping-mapi-names-to-canonical-property-names.md)
