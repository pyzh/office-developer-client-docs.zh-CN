---
title: 提供程序表
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
localization_priority: Normal
api_type:
- COM
ms.assetid: 99709a4c-cb52-436e-a322-02ded5d65ce5
description: 上次修改时间： 2015 年 3 月 9 日
ms.openlocfilehash: a613bd744a113b4378c5bef94fb51f6ae3aa4041
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19778576"
---
# <a name="provider-tables"></a><span data-ttu-id="67705-103">提供程序表</span><span class="sxs-lookup"><span data-stu-id="67705-103">Provider Tables</span></span>

  
  
<span data-ttu-id="67705-104">**适用于**： Outlook</span><span class="sxs-lookup"><span data-stu-id="67705-104">**Applies to**: Outlook</span></span> 
  
<span data-ttu-id="67705-105">提供程序表包含有关服务提供商的信息。</span><span class="sxs-lookup"><span data-stu-id="67705-105">A provider table contains information about service providers.</span></span> <span data-ttu-id="67705-106">有两个不同的提供程序表 (由 MAPI 实现和使用的客户端）。</span><span class="sxs-lookup"><span data-stu-id="67705-106">There are two different provider tables, both implemented by MAPI and used by clients.</span></span> <span data-ttu-id="67705-107">第一个表格，通过调用[IMsgServiceAdmin::GetProviderTable](imsgserviceadmin-getprovidertable.md)方法访问包含有关当前配置文件的提供程序的所有信息。</span><span class="sxs-lookup"><span data-stu-id="67705-107">The first table, accessed by calling the [IMsgServiceAdmin::GetProviderTable](imsgserviceadmin-getprovidertable.md) method, holds information about all of the providers for the current profile.</span></span> <span data-ttu-id="67705-108">通过[IProviderAdmin::GetProviderTable](iprovideradmin-getprovidertable.md)，访问第二个表创建表，用于存储有关消息服务的服务提供程序的所有信息。</span><span class="sxs-lookup"><span data-stu-id="67705-108">The second table, accessed through [IProviderAdmin::GetProviderTable](iprovideradmin-getprovidertable.md), creates a table that stores information about all of the service providers for a message service.</span></span>
  
<span data-ttu-id="67705-109">这两个表有另一个差别。</span><span class="sxs-lookup"><span data-stu-id="67705-109">These two tables have another difference.</span></span> <span data-ttu-id="67705-110">可通过**IMsgServiceAdmin::GetProviderTable**提供程序表包含仅表示服务提供商而可通过**IProviderAdmin::GetProviderTable**表可能包括表示行的行与服务提供程序关联的其他信息。</span><span class="sxs-lookup"><span data-stu-id="67705-110">The provider table available through **IMsgServiceAdmin::GetProviderTable** contains only rows that represent service providers while the table available through **IProviderAdmin::GetProviderTable** may include rows that represent additional information associated with a service provider.</span></span> <span data-ttu-id="67705-111">此额外信息添加到与的 MAPISVC.INF"部分"关键字的配置文件。</span><span class="sxs-lookup"><span data-stu-id="67705-111">This extra information is added to the profile with the "Sections" keyword of MAPISVC.INF.</span></span> <span data-ttu-id="67705-112">当提供程序具有额外的配置文件节时，它**PR_SERVICE_EXTRA_UIDS** ([PidTagServiceExtraUids](pidtagserviceextrauids-canonical-property.md)) 属性中存储以下各节的**MAPIUID**值。</span><span class="sxs-lookup"><span data-stu-id="67705-112">When a provider has extra profile sections, it stores the **MAPIUID** values for these sections in the **PR_SERVICE_EXTRA_UIDS** ([PidTagServiceExtraUids](pidtagserviceextrauids-canonical-property.md)) property.</span></span> <span data-ttu-id="67705-113">**PR_SERVICE_EXTRA_UIDS**保存在邮件服务配置文件部分。</span><span class="sxs-lookup"><span data-stu-id="67705-113">**PR_SERVICE_EXTRA_UIDS** is saved in the message service profile section.</span></span> 
  
<span data-ttu-id="67705-114">以下属性构成设置两种类型的提供程序表中所需的列：</span><span class="sxs-lookup"><span data-stu-id="67705-114">The following properties make up the required column set in both types of provider tables:</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="67705-115">**PR_INSTANCE_KEY**([PidTagInstanceKey](pidtaginstancekey-canonical-property.md))</span><span class="sxs-lookup"><span data-stu-id="67705-115">**PR_INSTANCE_KEY** ([PidTagInstanceKey](pidtaginstancekey-canonical-property.md))</span></span>  <br/> |<span data-ttu-id="67705-116">**PR_DISPLAY_NAME**([PidTagDisplayName](pidtagdisplayname-canonical-property.md))</span><span class="sxs-lookup"><span data-stu-id="67705-116">**PR_DISPLAY_NAME** ([PidTagDisplayName](pidtagdisplayname-canonical-property.md))</span></span>  <br/> |
|<span data-ttu-id="67705-117">**PR_PROVIDER_DISPLAY**([PidTagProviderDisplay](pidtagproviderdisplay-canonical-property.md))</span><span class="sxs-lookup"><span data-stu-id="67705-117">**PR_PROVIDER_DISPLAY** ([PidTagProviderDisplay](pidtagproviderdisplay-canonical-property.md))</span></span>  <br/> |<span data-ttu-id="67705-118">**PR_PROVIDER_DLL_NAME**([PidTagProviderDllName](pidtagproviderdllname-canonical-property.md))</span><span class="sxs-lookup"><span data-stu-id="67705-118">**PR_PROVIDER_DLL_NAME** ([PidTagProviderDllName](pidtagproviderdllname-canonical-property.md))</span></span>  <br/> |
|<span data-ttu-id="67705-119">**PR_PROVIDER_ORDINAL**([PidTagProviderOrdinal](pidtagproviderordinal-canonical-property.md))</span><span class="sxs-lookup"><span data-stu-id="67705-119">**PR_PROVIDER_ORDINAL** ([PidTagProviderOrdinal](pidtagproviderordinal-canonical-property.md))</span></span>  <br/> |<span data-ttu-id="67705-120">**PR_PROVIDER_UID**([PidTagProviderUid](pidtagprovideruid-canonical-property.md))</span><span class="sxs-lookup"><span data-stu-id="67705-120">**PR_PROVIDER_UID** ([PidTagProviderUid](pidtagprovideruid-canonical-property.md))</span></span>  <br/> |
|<span data-ttu-id="67705-121">**PR_RESOURCE_FLAGS**([PidTagResourceFlags](pidtagresourceflags-canonical-property.md))</span><span class="sxs-lookup"><span data-stu-id="67705-121">**PR_RESOURCE_FLAGS** ([PidTagResourceFlags](pidtagresourceflags-canonical-property.md))</span></span>  <br/> |<span data-ttu-id="67705-122">**PR_RESOURCE_TYPE**([PidTagResourceType](pidtagresourcetype-canonical-property.md))</span><span class="sxs-lookup"><span data-stu-id="67705-122">**PR_RESOURCE_TYPE** ([PidTagResourceType](pidtagresourcetype-canonical-property.md))</span></span>  <br/> |
|<span data-ttu-id="67705-123">**PR_SERVICE_NAME**([PidTagServiceName](pidtagservicename-canonical-property.md))</span><span class="sxs-lookup"><span data-stu-id="67705-123">**PR_SERVICE_NAME** ([PidTagServiceName](pidtagservicename-canonical-property.md))</span></span>  <br/> |<span data-ttu-id="67705-124">**PR_SERVICE_UID**([PidTagServiceUid](pidtagserviceuid-canonical-property.md))</span><span class="sxs-lookup"><span data-stu-id="67705-124">**PR_SERVICE_UID** ([PidTagServiceUid](pidtagserviceuid-canonical-property.md))</span></span>  <br/> |
   
<span data-ttu-id="67705-125">可使用提供程序表，以显示当前传输订单或更改它。</span><span class="sxs-lookup"><span data-stu-id="67705-125">The provider table can be used to display the current transport order or to change it.</span></span> <span data-ttu-id="67705-126">若要显示当前的顺序，生成**PR_RESOURCE_TYPE**属性设置为 MAPI_TRANSPORT_PROVIDER 检索仅这些行限制。</span><span class="sxs-lookup"><span data-stu-id="67705-126">To display the current order, build a restriction to retrieve only those rows with the **PR_RESOURCE_TYPE** property set to MAPI_TRANSPORT_PROVIDER.</span></span> <span data-ttu-id="67705-127">然后用作**PR_PROVIDER_ORDINAL**排序关键字表格进行排序和检索[IMAPITable::QueryRows](imapitable-queryrows.md)方法或[HrQueryAllRows](hrqueryallrows.md)函数使用的所有行。</span><span class="sxs-lookup"><span data-stu-id="67705-127">Then use **PR_PROVIDER_ORDINAL** as a sort key to sort the table and retrieve all the rows with either the [IMAPITable::QueryRows](imapitable-queryrows.md) method or the [HrQueryAllRows](hrqueryallrows.md) function.</span></span> 
  
<span data-ttu-id="67705-128">若要更改的传输顺序，应用相同的限制和检索的行。</span><span class="sxs-lookup"><span data-stu-id="67705-128">To change the transport order, apply the same restriction and retrieve the rows.</span></span> <span data-ttu-id="67705-129">然后创建从**PR_PROVIDER_UID**属性值，该值代表传输提供程序的唯一标识符的值的数组。</span><span class="sxs-lookup"><span data-stu-id="67705-129">Then create an array of values from the **PR_PROVIDER_UID** property that represents the unique identifiers for the transport providers.</span></span> <span data-ttu-id="67705-130">所需的顺序标识符时，将它们传递给[IMsgServiceAdmin::MsgServiceTransportOrder](imsgserviceadmin-msgservicetransportorder.md)方法。</span><span class="sxs-lookup"><span data-stu-id="67705-130">When the identifiers are in the desired order, pass them to the [IMsgServiceAdmin::MsgServiceTransportOrder](imsgserviceadmin-msgservicetransportorder.md) method.</span></span> 
  
<span data-ttu-id="67705-131">提供程序表中为可用后，将不会反映后续更改，如添加或删除提供程序。</span><span class="sxs-lookup"><span data-stu-id="67705-131">After a provider table has been made available, it will not reflect subsequent changes, such as the addition or deletion of a provider.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="67705-132">另请参阅</span><span class="sxs-lookup"><span data-stu-id="67705-132">See also</span></span>



[<span data-ttu-id="67705-133">MAPI 表</span><span class="sxs-lookup"><span data-stu-id="67705-133">MAPI Tables</span></span>](mapi-tables.md)
