---
title: PidTagAnr 规范属性
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PidTagAnr
api_type:
- HeaderDef
ms.assetid: eca3d4ff-2e92-4d20-a498-98e0773c1962
description: 上次修改时间： 2015 年 3 月 9 日
ms.openlocfilehash: 94e83f4a93bac4ee144c5fbf94fd4b3fdb6c2f55
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19777318"
---
# <a name="pidtaganr-canonical-property"></a><span data-ttu-id="24bc0-103">PidTagAnr 规范属性</span><span class="sxs-lookup"><span data-stu-id="24bc0-103">PidTagAnr Canonical Property</span></span>

  
  
<span data-ttu-id="24bc0-104">**适用于**： Outlook</span><span class="sxs-lookup"><span data-stu-id="24bc0-104">**Applies to**: Outlook</span></span> 
  
<span data-ttu-id="24bc0-105">包含在通讯簿容器内容表属性限制中使用的字符串值。</span><span class="sxs-lookup"><span data-stu-id="24bc0-105">Contains a string value for use in a property restriction on an address book container contents table.</span></span> 
  
|||
|:-----|:-----|
|<span data-ttu-id="24bc0-106">关联的属性：</span><span class="sxs-lookup"><span data-stu-id="24bc0-106">Associated properties:</span></span>  <br/> |<span data-ttu-id="24bc0-107">PR_ANR，PR_ANR_A，PR_ANR_W</span><span class="sxs-lookup"><span data-stu-id="24bc0-107">PR_ANR, PR_ANR_A, PR_ANR_W</span></span>  <br/> |
|<span data-ttu-id="24bc0-108">标识符:</span><span class="sxs-lookup"><span data-stu-id="24bc0-108">Identifier:</span></span>  <br/> |<span data-ttu-id="24bc0-109">0x360C</span><span class="sxs-lookup"><span data-stu-id="24bc0-109">0x360C</span></span>  <br/> |
|<span data-ttu-id="24bc0-110">数据类型：</span><span class="sxs-lookup"><span data-stu-id="24bc0-110">Data type:</span></span>  <br/> |<span data-ttu-id="24bc0-111">PT_UNICODE PT_STRING8</span><span class="sxs-lookup"><span data-stu-id="24bc0-111">PT_UNICODE, PT_STRING8</span></span>  <br/> |
|<span data-ttu-id="24bc0-112">区域：</span><span class="sxs-lookup"><span data-stu-id="24bc0-112">Area:</span></span>  <br/> |<span data-ttu-id="24bc0-113">通讯簿</span><span class="sxs-lookup"><span data-stu-id="24bc0-113">Address book</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="24bc0-114">备注</span><span class="sxs-lookup"><span data-stu-id="24bc0-114">Remarks</span></span>

<span data-ttu-id="24bc0-115">这些属性不属于任何对象;它提供通过[SPropertyRestriction](spropertyrestriction.md)结构中的通讯簿提供程序。</span><span class="sxs-lookup"><span data-stu-id="24bc0-115">These properties do not belong to any object; it is furnished by address book providers in [SPropertyRestriction](spropertyrestriction.md) structures.</span></span> <span data-ttu-id="24bc0-116">此属性包含可以对通讯簿容器内容表，以查找相应邮件的收件人，测试模糊名称解析 (ANR) 字符串。</span><span class="sxs-lookup"><span data-stu-id="24bc0-116">This property contains an ambiguous name resolution (ANR) string that can be tested against an address book container's contents table to find corresponding message recipients.</span></span> 
  
<span data-ttu-id="24bc0-117">通讯簿提供程序匹配**PR_ANR**和对在内容表中，每个条目的关联的属性的值使用提供程序定义匹配算法。</span><span class="sxs-lookup"><span data-stu-id="24bc0-117">Address book providers match the value of **PR_ANR** and associated properties against every entry in the contents table, using a provider-defined matching algorithm.</span></span> <span data-ttu-id="24bc0-118">此匹配项中使用的列选择算法的一部分提供程序。</span><span class="sxs-lookup"><span data-stu-id="24bc0-118">The column or columns that are used in this match are chosen by the provider as part of the algorithm.</span></span> <span data-ttu-id="24bc0-119">**PR_DISPLAY_NAME** ([PidTagDisplayName](pidtagdisplayname-canonical-property.md)) 列中最常用;包含用户的电子邮件名称时，则也可以**PR_ACCOUNT** ([PidTagAccount](pidtagaccount-canonical-property.md)) 列。</span><span class="sxs-lookup"><span data-stu-id="24bc0-119">The **PR_DISPLAY_NAME** ([PidTagDisplayName](pidtagdisplayname-canonical-property.md)) column is the most commonly used; the **PR_ACCOUNT** ([PidTagAccount](pidtagaccount-canonical-property.md)) column is also useful when it contains the user's email name.</span></span> 
  
<span data-ttu-id="24bc0-120">模糊名称解析的详细信息，请参阅[地址簿限制](address-book-restrictions.md)。</span><span class="sxs-lookup"><span data-stu-id="24bc0-120">For more information on ambiguous name resolution, see [Address Book Restrictions](address-book-restrictions.md).</span></span> 
  
## <a name="related-resources"></a><span data-ttu-id="24bc0-121">相关资源</span><span class="sxs-lookup"><span data-stu-id="24bc0-121">Related resources</span></span>

### <a name="protocol-specifications"></a><span data-ttu-id="24bc0-122">协议规范</span><span class="sxs-lookup"><span data-stu-id="24bc0-122">Protocol specifications</span></span>

<span data-ttu-id="24bc0-123">[[MS OXPROPS]](http://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="24bc0-123">[[MS-OXPROPS]](http://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)</span></span>
  
> <span data-ttu-id="24bc0-124">提供了相关的 Exchange Server 协议规范参考。</span><span class="sxs-lookup"><span data-stu-id="24bc0-124">Provides references to related Exchange Server protocol specifications.</span></span>
    
<span data-ttu-id="24bc0-125">[[MS OXOABK]](http://msdn.microsoft.com/library/f4cf9b4c-9232-4506-9e71-2270de217614%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="24bc0-125">[[MS-OXOABK]](http://msdn.microsoft.com/library/f4cf9b4c-9232-4506-9e71-2270de217614%28Office.15%29.aspx)</span></span>
  
> <span data-ttu-id="24bc0-126">指定的属性和用户、 联系人、 组和资源的操作列表。</span><span class="sxs-lookup"><span data-stu-id="24bc0-126">Specifies the properties and operations for lists of users, contacts, groups, and resources.</span></span>
    
### <a name="header-files"></a><span data-ttu-id="24bc0-127">头文件</span><span class="sxs-lookup"><span data-stu-id="24bc0-127">Header files</span></span>

<span data-ttu-id="24bc0-128">Mapidefs.h</span><span class="sxs-lookup"><span data-stu-id="24bc0-128">Mapidefs.h</span></span>
  
> <span data-ttu-id="24bc0-129">提供数据类型定义。</span><span class="sxs-lookup"><span data-stu-id="24bc0-129">Provides data type definitions.</span></span>
    
<span data-ttu-id="24bc0-130">Mapitags.h</span><span class="sxs-lookup"><span data-stu-id="24bc0-130">Mapitags.h</span></span>
  
> <span data-ttu-id="24bc0-131">包含列为相关属性的属性的定义。</span><span class="sxs-lookup"><span data-stu-id="24bc0-131">Contains definitions of properties listed as associated properties.</span></span>
    
## <a name="see-also"></a><span data-ttu-id="24bc0-132">另请参阅</span><span class="sxs-lookup"><span data-stu-id="24bc0-132">See also</span></span>



[<span data-ttu-id="24bc0-133">IAddrBook::ResolveName</span><span class="sxs-lookup"><span data-stu-id="24bc0-133">IAddrBook::ResolveName</span></span>](iaddrbook-resolvename.md)
  
[<span data-ttu-id="24bc0-134">IABContainer::ResolveNames</span><span class="sxs-lookup"><span data-stu-id="24bc0-134">IABContainer::ResolveNames</span></span>](iabcontainer-resolvenames.md)


[<span data-ttu-id="24bc0-135">MAPI 属性</span><span class="sxs-lookup"><span data-stu-id="24bc0-135">MAPI Properties</span></span>](mapi-properties.md)
  
[<span data-ttu-id="24bc0-136">MAPI 规范属性</span><span class="sxs-lookup"><span data-stu-id="24bc0-136">MAPI Canonical Properties</span></span>](mapi-canonical-properties.md)
  
[<span data-ttu-id="24bc0-137">映射到 MAPI 名称的规范属性名称</span><span class="sxs-lookup"><span data-stu-id="24bc0-137">Mapping Canonical Property Names to MAPI Names</span></span>](mapping-canonical-property-names-to-mapi-names.md)
  
[<span data-ttu-id="24bc0-138">MAPI 名称映射到规范属性名称</span><span class="sxs-lookup"><span data-stu-id="24bc0-138">Mapping MAPI Names to Canonical Property Names</span></span>](mapping-mapi-names-to-canonical-property-names.md)
