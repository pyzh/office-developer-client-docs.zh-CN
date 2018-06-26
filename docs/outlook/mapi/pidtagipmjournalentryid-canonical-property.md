---
title: PidTagIpmJournalEntryId 规范属性
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PidTagIpmJournalEntryId
api_type:
- HeaderDef
ms.assetid: a3765b9d-a108-46d7-a97c-a825ae3980be
description: 上次修改时间： 2015 年 3 月 9 日
ms.openlocfilehash: e48b3af79656279e3c554cd5093385d894525e43
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19777770"
---
# <a name="pidtagipmjournalentryid-canonical-property"></a><span data-ttu-id="feecf-103">PidTagIpmJournalEntryId 规范属性</span><span class="sxs-lookup"><span data-stu-id="feecf-103">PidTagIpmJournalEntryId Canonical Property</span></span>

  
  
<span data-ttu-id="feecf-104">**适用于**： Outlook</span><span class="sxs-lookup"><span data-stu-id="feecf-104">**Applies to**: Outlook</span></span> 
  
<span data-ttu-id="feecf-105">包含 Outlook 日记文件夹的**EntryID** 。</span><span class="sxs-lookup"><span data-stu-id="feecf-105">Contains the **EntryID** of the Outlook Journal folder.</span></span> 
  
|||
|:-----|:-----|
|<span data-ttu-id="feecf-106">关联的属性：</span><span class="sxs-lookup"><span data-stu-id="feecf-106">Associated properties:</span></span>  <br/> |<span data-ttu-id="feecf-107">PR_IPM_JOURNAL_ENTRYID</span><span class="sxs-lookup"><span data-stu-id="feecf-107">PR_IPM_JOURNAL_ENTRYID</span></span>  <br/> |
|<span data-ttu-id="feecf-108">标识符:</span><span class="sxs-lookup"><span data-stu-id="feecf-108">Identifier:</span></span>  <br/> |<span data-ttu-id="feecf-109">0x36D2</span><span class="sxs-lookup"><span data-stu-id="feecf-109">0x36D2</span></span>  <br/> |
|<span data-ttu-id="feecf-110">数据类型：</span><span class="sxs-lookup"><span data-stu-id="feecf-110">Data type:</span></span>  <br/> |<span data-ttu-id="feecf-111">PT_BINARY</span><span class="sxs-lookup"><span data-stu-id="feecf-111">PT_BINARY</span></span>  <br/> |
|<span data-ttu-id="feecf-112">区域：</span><span class="sxs-lookup"><span data-stu-id="feecf-112">Area:</span></span>  <br/> |<span data-ttu-id="feecf-113">Folder</span><span class="sxs-lookup"><span data-stu-id="feecf-113">Folder</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="feecf-114">备注</span><span class="sxs-lookup"><span data-stu-id="feecf-114">Remarks</span></span>

<span data-ttu-id="feecf-115">此属性存储在收件箱文件夹，以及消息存储库的根文件夹中。</span><span class="sxs-lookup"><span data-stu-id="feecf-115">This property is stored in the Inbox folder as well as the root folder of the message store.</span></span> <span data-ttu-id="feecf-116">若要访问特定的邮件存储区上的属性，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="feecf-116">To access the property on a specific message store, do the following:</span></span> 
  
1. <span data-ttu-id="feecf-117">首先，查找收件箱文件夹中的属性。</span><span class="sxs-lookup"><span data-stu-id="feecf-117">First, look for the property in the Inbox folder.</span></span> <span data-ttu-id="feecf-118">使用[IMsgStore::GetReceiveFolder](imsgstore-getreceivefolder.md)获取收件箱文件夹的**EntryID**的引用。</span><span class="sxs-lookup"><span data-stu-id="feecf-118">Use [IMsgStore::GetReceiveFolder](imsgstore-getreceivefolder.md) to obtain a reference to the **EntryID** for the Inbox folder.</span></span> 
    
2. <span data-ttu-id="feecf-119">如果**IMsgStore::GetReceiveFolder**操作成功，则使用**EntryID**的收件箱和[IMsgStore::OpenEntry](imsgstore-openentry.md)引用打开收件箱并获取**IMAPIFolder**对象的引用。</span><span class="sxs-lookup"><span data-stu-id="feecf-119">If **IMsgStore::GetReceiveFolder** is successful, then use the reference to the **EntryID** of the Inbox and [IMsgStore::OpenEntry](imsgstore-openentry.md) to open the Inbox and obtain a reference to an **IMAPIFolder** object.</span></span> 
    
3. <span data-ttu-id="feecf-120">如果**IMsgStore::OpenEntry**成功，然后使用**IMAPIFolder**对象和[IMAPIProp::GetProps](imapiprop-getprops.md)返回的参考获取所需的属性。</span><span class="sxs-lookup"><span data-stu-id="feecf-120">If **IMsgStore::OpenEntry** is successful, then use the returned reference to the **IMAPIFolder** object and [IMAPIProp::GetProps](imapiprop-getprops.md) to obtain the desired property.</span></span> 
    
4. <span data-ttu-id="feecf-121">如果步骤 1、 2 或 3 失败，查找的根文件夹中的属性。</span><span class="sxs-lookup"><span data-stu-id="feecf-121">If Step 1, 2, or 3 fails, look for the property in the root folder.</span></span> <span data-ttu-id="feecf-122">若要执行的操作，使用**IMsgStore::OpenEntry**，指定 NULL 的**lpEntryID**，打开的邮件存储区的根文件夹，并获取**IMAPIFolder**对象的引用。</span><span class="sxs-lookup"><span data-stu-id="feecf-122">To do that, use **IMsgStore::OpenEntry**, specifying NULL for **lpEntryID**, to open the root folder of the message store and obtain a reference to the **IMAPIFolder** object.</span></span> 
    
5. <span data-ttu-id="feecf-123">如果成功打开根文件夹，然后使用**IMAPIFolder**对象和**IMAPIProp::GetProps**返回的参考获取所需的属性。</span><span class="sxs-lookup"><span data-stu-id="feecf-123">If opening the root folder is successful, then use the returned reference to the **IMAPIFolder** object and **IMAPIProp::GetProps** to obtain the desired property.</span></span> 
    
## <a name="related-resources"></a><span data-ttu-id="feecf-124">相关资源</span><span class="sxs-lookup"><span data-stu-id="feecf-124">Related resources</span></span>

### <a name="protocol-specifications"></a><span data-ttu-id="feecf-125">协议规范</span><span class="sxs-lookup"><span data-stu-id="feecf-125">Protocol specifications</span></span>

<span data-ttu-id="feecf-126">[[MS OXPROPS]](http://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="feecf-126">[[MS-OXPROPS]](http://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)</span></span>
  
> <span data-ttu-id="feecf-127">提供了相关的 Exchange Server 协议规范参考。</span><span class="sxs-lookup"><span data-stu-id="feecf-127">Provides references to related Exchange Server protocol specifications.</span></span>
    
<span data-ttu-id="feecf-128">[[MS OXOSFLD]](http://msdn.microsoft.com/library/a60e9c16-2ba8-424b-b60c-385a8a2837cb%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="feecf-128">[[MS-OXOSFLD]](http://msdn.microsoft.com/library/a60e9c16-2ba8-424b-b60c-385a8a2837cb%28Office.15%29.aspx)</span></span>
  
> <span data-ttu-id="feecf-129">指定的属性和用于创建和邮箱中查找的特殊文件夹的操作。</span><span class="sxs-lookup"><span data-stu-id="feecf-129">Specifies the properties and operations for creating and locating the special folders in a mailbox.</span></span>
    
<span data-ttu-id="feecf-130">[[MS OXODLGT]](http://msdn.microsoft.com/library/01a89b11-9c43-4c40-b147-8f6a1ef5a44f%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="feecf-130">[[MS-OXODLGT]](http://msdn.microsoft.com/library/01a89b11-9c43-4c40-b147-8f6a1ef5a44f%28Office.15%29.aspx)</span></span>
  
> <span data-ttu-id="feecf-131">指定用于连接到和它们代表另一个用户操作时，作为代理人，以及与邮件和日历的对象交互配置邮箱的方法。</span><span class="sxs-lookup"><span data-stu-id="feecf-131">Specifies methods for connecting to and configuring mailboxes as delegates, and interactions with message and calendar objects when they act on behalf of another user.</span></span>
    
### <a name="header-files"></a><span data-ttu-id="feecf-132">头文件</span><span class="sxs-lookup"><span data-stu-id="feecf-132">Header files</span></span>

<span data-ttu-id="feecf-133">Mapidefs.h</span><span class="sxs-lookup"><span data-stu-id="feecf-133">Mapidefs.h</span></span>
  
> <span data-ttu-id="feecf-134">提供数据类型定义。</span><span class="sxs-lookup"><span data-stu-id="feecf-134">Provides data type definitions.</span></span>
    
<span data-ttu-id="feecf-135">Mapitags.h</span><span class="sxs-lookup"><span data-stu-id="feecf-135">Mapitags.h</span></span>
  
> <span data-ttu-id="feecf-136">包含作为替代名称列出的属性的定义。</span><span class="sxs-lookup"><span data-stu-id="feecf-136">Contains definitions of properties listed as alternate names.</span></span>
    
## <a name="see-also"></a><span data-ttu-id="feecf-137">另请参阅</span><span class="sxs-lookup"><span data-stu-id="feecf-137">See also</span></span>



[<span data-ttu-id="feecf-138">MAPI 属性</span><span class="sxs-lookup"><span data-stu-id="feecf-138">MAPI Properties</span></span>](mapi-properties.md)
  
[<span data-ttu-id="feecf-139">MAPI 规范属性</span><span class="sxs-lookup"><span data-stu-id="feecf-139">MAPI Canonical Properties</span></span>](mapi-canonical-properties.md)
  
[<span data-ttu-id="feecf-140">映射到 MAPI 名称的规范属性名称</span><span class="sxs-lookup"><span data-stu-id="feecf-140">Mapping Canonical Property Names to MAPI Names</span></span>](mapping-canonical-property-names-to-mapi-names.md)
  
[<span data-ttu-id="feecf-141">MAPI 名称映射到规范属性名称</span><span class="sxs-lookup"><span data-stu-id="feecf-141">Mapping MAPI Names to Canonical Property Names</span></span>](mapping-mapi-names-to-canonical-property-names.md)
