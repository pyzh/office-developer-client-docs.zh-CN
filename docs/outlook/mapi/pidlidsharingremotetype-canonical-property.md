---
title: PidLidSharingRemoteType 规范属性
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PidLidSharingRemoteType
api_type:
- COM
ms.assetid: e9bc7c7c-86df-45d8-922b-76e3b076144a
description: 上次修改时间： 2015 年 3 月 9 日
ms.openlocfilehash: 8a9975090a8b90946482fa77fd2dafdb503c1f68
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19777041"
---
# <a name="pidlidsharingremotetype-canonical-property"></a><span data-ttu-id="3edf8-103">PidLidSharingRemoteType 规范属性</span><span class="sxs-lookup"><span data-stu-id="3edf8-103">PidLidSharingRemoteType Canonical Property</span></span>

  
  
<span data-ttu-id="3edf8-104">**适用于**： Outlook</span><span class="sxs-lookup"><span data-stu-id="3edf8-104">**Applies to**: Outlook</span></span> 
  
<span data-ttu-id="3edf8-105">指定远程共享文件夹的类型。</span><span class="sxs-lookup"><span data-stu-id="3edf8-105">Specifies the type of the remote shared folder.</span></span> <span data-ttu-id="3edf8-106">这是邮件的共享的属性。</span><span class="sxs-lookup"><span data-stu-id="3edf8-106">This is a property of a sharing message.</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="3edf8-107">关联的属性：</span><span class="sxs-lookup"><span data-stu-id="3edf8-107">Associated properties:</span></span>  <br/> |<span data-ttu-id="3edf8-108">dispidSharingRemoteType</span><span class="sxs-lookup"><span data-stu-id="3edf8-108">dispidSharingRemoteType</span></span>  <br/> |
|<span data-ttu-id="3edf8-109">属性进行设置：</span><span class="sxs-lookup"><span data-stu-id="3edf8-109">Property set:</span></span>  <br/> |<span data-ttu-id="3edf8-110">PSETID_Sharing</span><span class="sxs-lookup"><span data-stu-id="3edf8-110">PSETID_Sharing</span></span>  <br/> |
|<span data-ttu-id="3edf8-111">长 ID （盖）：</span><span class="sxs-lookup"><span data-stu-id="3edf8-111">Long ID (LID):</span></span>  <br/> |<span data-ttu-id="3edf8-112">0x00008A1D</span><span class="sxs-lookup"><span data-stu-id="3edf8-112">0x00008A1D</span></span>  <br/> |
|<span data-ttu-id="3edf8-113">数据类型：</span><span class="sxs-lookup"><span data-stu-id="3edf8-113">Data type:</span></span>  <br/> |<span data-ttu-id="3edf8-114">PT_UNICODE</span><span class="sxs-lookup"><span data-stu-id="3edf8-114">PT_UNICODE</span></span>  <br/> |
|<span data-ttu-id="3edf8-115">区域：</span><span class="sxs-lookup"><span data-stu-id="3edf8-115">Area:</span></span>  <br/> |<span data-ttu-id="3edf8-116">共享</span><span class="sxs-lookup"><span data-stu-id="3edf8-116">Sharing</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3edf8-117">备注</span><span class="sxs-lookup"><span data-stu-id="3edf8-117">Remarks</span></span>

<span data-ttu-id="3edf8-118">此属性必须设置为相同的值的**dispidSharingLocalType** ([PidLidSharingLocalType](pidlidsharinglocaltype-canonical-property.md)) 属性，并应忽略。</span><span class="sxs-lookup"><span data-stu-id="3edf8-118">This property must be set to the same value as the **dispidSharingLocalType** ([PidLidSharingLocalType](pidlidsharinglocaltype-canonical-property.md)) property and should be ignored.</span></span>
  
## <a name="related-resources"></a><span data-ttu-id="3edf8-119">相关资源</span><span class="sxs-lookup"><span data-stu-id="3edf8-119">Related resources</span></span>

### <a name="protocol-specifications"></a><span data-ttu-id="3edf8-120">协议规范</span><span class="sxs-lookup"><span data-stu-id="3edf8-120">Protocol specifications</span></span>

<span data-ttu-id="3edf8-121">[[MS OXPROPS]](http://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="3edf8-121">[[MS-OXPROPS]](http://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)</span></span>
  
> <span data-ttu-id="3edf8-122">提供属性集定义和相关的 Exchange Server 协议规范的引用。</span><span class="sxs-lookup"><span data-stu-id="3edf8-122">Provides property set definitions and references to related Exchange Server protocol specifications.</span></span>
    
<span data-ttu-id="3edf8-123">[[MS OXSHARE]](http://msdn.microsoft.com/library/e4e5bd27-d5e0-43f9-a6ea-550876724f3d%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="3edf8-123">[[MS-OXSHARE]](http://msdn.microsoft.com/library/e4e5bd27-d5e0-43f9-a6ea-550876724f3d%28Office.15%29.aspx)</span></span>
  
> <span data-ttu-id="3edf8-124">共享客户端之间的邮箱文件夹。</span><span class="sxs-lookup"><span data-stu-id="3edf8-124">Shares mailbox folders between clients.</span></span>
    
### <a name="header-files"></a><span data-ttu-id="3edf8-125">头文件</span><span class="sxs-lookup"><span data-stu-id="3edf8-125">Header files</span></span>

<span data-ttu-id="3edf8-126">Mapidefs.h</span><span class="sxs-lookup"><span data-stu-id="3edf8-126">Mapidefs.h</span></span>
  
> <span data-ttu-id="3edf8-127">提供数据类型定义。</span><span class="sxs-lookup"><span data-stu-id="3edf8-127">Provides data type definitions.</span></span>
    
## <a name="see-also"></a><span data-ttu-id="3edf8-128">另请参阅</span><span class="sxs-lookup"><span data-stu-id="3edf8-128">See also</span></span>



[<span data-ttu-id="3edf8-129">MAPI 属性</span><span class="sxs-lookup"><span data-stu-id="3edf8-129">MAPI Properties</span></span>](mapi-properties.md)
  
[<span data-ttu-id="3edf8-130">MAPI 规范属性</span><span class="sxs-lookup"><span data-stu-id="3edf8-130">MAPI Canonical Properties</span></span>](mapi-canonical-properties.md)
  
[<span data-ttu-id="3edf8-131">映射到 MAPI 名称的规范属性名称</span><span class="sxs-lookup"><span data-stu-id="3edf8-131">Mapping Canonical Property Names to MAPI Names</span></span>](mapping-canonical-property-names-to-mapi-names.md)
  
[<span data-ttu-id="3edf8-132">MAPI 名称映射到规范属性名称</span><span class="sxs-lookup"><span data-stu-id="3edf8-132">Mapping MAPI Names to Canonical Property Names</span></span>](mapping-mapi-names-to-canonical-property-names.md)
