---
title: PidLidFlagString 规范属性
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PidLidFlagString
api_type:
- COM
ms.assetid: 4cf1e08b-c869-4965-a1e4-512a0684700f
description: 上次修改时间： 2015 年 3 月 9 日
ms.openlocfilehash: 53fe309fb15807ad698fef5a06781e5c3e0bae0c
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19776853"
---
# <a name="pidlidflagstring-canonical-property"></a><span data-ttu-id="7a7ff-103">PidLidFlagString 规范属性</span><span class="sxs-lookup"><span data-stu-id="7a7ff-103">PidLidFlagString Canonical Property</span></span>

  
  
<span data-ttu-id="7a7ff-104">**适用于**： Outlook</span><span class="sxs-lookup"><span data-stu-id="7a7ff-104">**Applies to**: Outlook</span></span> 
  
<span data-ttu-id="7a7ff-105">包含标识之一的一组预定义的文本字符串标志相关联的索引。</span><span class="sxs-lookup"><span data-stu-id="7a7ff-105">Contains an index that identifies one of a set of pre-defined text strings associated with the flag.</span></span>
  
|||
|:-----|:-----|
|<span data-ttu-id="7a7ff-106">关联的属性：</span><span class="sxs-lookup"><span data-stu-id="7a7ff-106">Associated properties:</span></span>  <br/> |<span data-ttu-id="7a7ff-107">dispidFlagStringEnum</span><span class="sxs-lookup"><span data-stu-id="7a7ff-107">dispidFlagStringEnum</span></span>  <br/> |
|<span data-ttu-id="7a7ff-108">属性进行设置：</span><span class="sxs-lookup"><span data-stu-id="7a7ff-108">Property set:</span></span>  <br/> |<span data-ttu-id="7a7ff-109">PSETID_Common</span><span class="sxs-lookup"><span data-stu-id="7a7ff-109">PSETID_Common</span></span>  <br/> |
|<span data-ttu-id="7a7ff-110">长 ID （盖）：</span><span class="sxs-lookup"><span data-stu-id="7a7ff-110">Long ID (LID):</span></span>  <br/> |<span data-ttu-id="7a7ff-111">0x000085C0</span><span class="sxs-lookup"><span data-stu-id="7a7ff-111">0x000085C0</span></span>  <br/> |
|<span data-ttu-id="7a7ff-112">数据类型：</span><span class="sxs-lookup"><span data-stu-id="7a7ff-112">Data type:</span></span>  <br/> |<span data-ttu-id="7a7ff-113">PT_LONG</span><span class="sxs-lookup"><span data-stu-id="7a7ff-113">PT_LONG</span></span>  <br/> |
|<span data-ttu-id="7a7ff-114">区域：</span><span class="sxs-lookup"><span data-stu-id="7a7ff-114">Area:</span></span>  <br/> |<span data-ttu-id="7a7ff-115">任务</span><span class="sxs-lookup"><span data-stu-id="7a7ff-115">Task</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7a7ff-116">备注</span><span class="sxs-lookup"><span data-stu-id="7a7ff-116">Remarks</span></span>

<span data-ttu-id="7a7ff-117">如果设置此属性，客户端应下表中 （例如，若要替换的字符串转换为当前用户的语言），使用相应的字符串值，并应忽略**dispidFlagRequest** ([中设置的值PidLidFlagRequest](pidlidflagrequest-canonical-property.md)) 和**dispidValidFlagStringProof** ([PidLidValidFlagStringProof](pidlidvalidflagstringproof-canonical-property.md))。</span><span class="sxs-lookup"><span data-stu-id="7a7ff-117">If this property is set, clients should use the corresponding string value in the tables below (for example, to substitute a string that is translated into the current user's language), and should ignore the value set in **dispidFlagRequest** ([PidLidFlagRequest](pidlidflagrequest-canonical-property.md)) and **dispidValidFlagStringProof** ([PidLidValidFlagStringProof](pidlidvalidflagstringproof-canonical-property.md)).</span></span> 
  
<span data-ttu-id="7a7ff-118">建议为用户联系人对象的默认值如下所示：</span><span class="sxs-lookup"><span data-stu-id="7a7ff-118">Defaults suggested to the user for contact objects are as follows:</span></span>
  
|<span data-ttu-id="7a7ff-119">**值**</span><span class="sxs-lookup"><span data-stu-id="7a7ff-119">**Value**</span></span>|<span data-ttu-id="7a7ff-120">**英语字符串**</span><span class="sxs-lookup"><span data-stu-id="7a7ff-120">**English string**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7a7ff-121">0x00000000 或不存在</span><span class="sxs-lookup"><span data-stu-id="7a7ff-121">0x00000000 or not present</span></span>  <br/> | <span data-ttu-id="7a7ff-122">按照与显示**dispidFlagRequest**相关的指南。</span><span class="sxs-lookup"><span data-stu-id="7a7ff-122">Follow the guidance related to displaying **dispidFlagRequest**.</span></span>  <br/> |
|<span data-ttu-id="7a7ff-123">0x0000006E</span><span class="sxs-lookup"><span data-stu-id="7a7ff-123">0x0000006E</span></span>  <br/> |<span data-ttu-id="7a7ff-124">"跟踪"</span><span class="sxs-lookup"><span data-stu-id="7a7ff-124">"Follow up"</span></span>  <br/> |
|<span data-ttu-id="7a7ff-125">0x0000006F</span><span class="sxs-lookup"><span data-stu-id="7a7ff-125">0x0000006F</span></span>  <br/> |<span data-ttu-id="7a7ff-126">"呼叫"</span><span class="sxs-lookup"><span data-stu-id="7a7ff-126">"Call"</span></span>  <br/> |
|<span data-ttu-id="7a7ff-127">0x00000070</span><span class="sxs-lookup"><span data-stu-id="7a7ff-127">0x00000070</span></span>  <br/> |<span data-ttu-id="7a7ff-128">"安排会议"</span><span class="sxs-lookup"><span data-stu-id="7a7ff-128">"Arrange Meeting"</span></span>  <br/> |
|<span data-ttu-id="7a7ff-129">0x00000071</span><span class="sxs-lookup"><span data-stu-id="7a7ff-129">0x00000071</span></span>  <br/> |<span data-ttu-id="7a7ff-130">"发送电子邮件"</span><span class="sxs-lookup"><span data-stu-id="7a7ff-130">"Send Email"</span></span>  <br/> |
|<span data-ttu-id="7a7ff-131">0x00000072</span><span class="sxs-lookup"><span data-stu-id="7a7ff-131">0x00000072</span></span>  <br/> |<span data-ttu-id="7a7ff-132">"发送字母"</span><span class="sxs-lookup"><span data-stu-id="7a7ff-132">"Send Letter"</span></span>  <br/> |
   
<span data-ttu-id="7a7ff-133">建议对所有其他消息对象的用户的默认值如下所示：</span><span class="sxs-lookup"><span data-stu-id="7a7ff-133">Defaults suggested to the user for all other message objects are as follows:</span></span>
  
|<span data-ttu-id="7a7ff-134">**值**</span><span class="sxs-lookup"><span data-stu-id="7a7ff-134">**Value**</span></span>|<span data-ttu-id="7a7ff-135">**英语字符串**</span><span class="sxs-lookup"><span data-stu-id="7a7ff-135">**English string**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7a7ff-136">0x00000000 或不存在</span><span class="sxs-lookup"><span data-stu-id="7a7ff-136">0x00000000 or not present</span></span>  <br/> | <span data-ttu-id="7a7ff-137">按照与显示**dispidFlagRequest**相关的指南。</span><span class="sxs-lookup"><span data-stu-id="7a7ff-137">Follow the guidance related to displaying **dispidFlagRequest**.</span></span>  <br/> |
|<span data-ttu-id="7a7ff-138">0x00000001</span><span class="sxs-lookup"><span data-stu-id="7a7ff-138">0x00000001</span></span>  <br/> |<span data-ttu-id="7a7ff-139">"呼叫"</span><span class="sxs-lookup"><span data-stu-id="7a7ff-139">"Call"</span></span>  <br/> |
|<span data-ttu-id="7a7ff-140">0x00000002</span><span class="sxs-lookup"><span data-stu-id="7a7ff-140">0x00000002</span></span>  <br/> |<span data-ttu-id="7a7ff-141">"不要转发"</span><span class="sxs-lookup"><span data-stu-id="7a7ff-141">"Do not Forward"</span></span>  <br/> |
|<span data-ttu-id="7a7ff-142">0x00000003</span><span class="sxs-lookup"><span data-stu-id="7a7ff-142">0x00000003</span></span>  <br/> |<span data-ttu-id="7a7ff-143">"跟踪"</span><span class="sxs-lookup"><span data-stu-id="7a7ff-143">"Follow up"</span></span>  <br/> |
|<span data-ttu-id="7a7ff-144">0x00000004</span><span class="sxs-lookup"><span data-stu-id="7a7ff-144">0x00000004</span></span>  <br/> |<span data-ttu-id="7a7ff-145">"为您的信息"</span><span class="sxs-lookup"><span data-stu-id="7a7ff-145">"For Your Information"</span></span>  <br/> |
|<span data-ttu-id="7a7ff-146">0x00000005</span><span class="sxs-lookup"><span data-stu-id="7a7ff-146">0x00000005</span></span>  <br/> |<span data-ttu-id="7a7ff-147">"转接"</span><span class="sxs-lookup"><span data-stu-id="7a7ff-147">"Forward"</span></span>  <br/> |
|<span data-ttu-id="7a7ff-148">0x00000006</span><span class="sxs-lookup"><span data-stu-id="7a7ff-148">0x00000006</span></span>  <br/> |<span data-ttu-id="7a7ff-149">"不需要响应"</span><span class="sxs-lookup"><span data-stu-id="7a7ff-149">"No Response Necessary"</span></span>  <br/> |
|<span data-ttu-id="7a7ff-150">0x00000007</span><span class="sxs-lookup"><span data-stu-id="7a7ff-150">0x00000007</span></span>  <br/> |<span data-ttu-id="7a7ff-151">"Read"</span><span class="sxs-lookup"><span data-stu-id="7a7ff-151">"Read"</span></span>  <br/> |
|<span data-ttu-id="7a7ff-152">0x00000008</span><span class="sxs-lookup"><span data-stu-id="7a7ff-152">0x00000008</span></span>  <br/> |<span data-ttu-id="7a7ff-153">"答复"</span><span class="sxs-lookup"><span data-stu-id="7a7ff-153">"Reply"</span></span>  <br/> |
|<span data-ttu-id="7a7ff-154">0x00000009</span><span class="sxs-lookup"><span data-stu-id="7a7ff-154">0x00000009</span></span>  <br/> |<span data-ttu-id="7a7ff-155">"全部答复"</span><span class="sxs-lookup"><span data-stu-id="7a7ff-155">"Reply to All"</span></span>  <br/> |
|<span data-ttu-id="7a7ff-156">0x0000000A</span><span class="sxs-lookup"><span data-stu-id="7a7ff-156">0x0000000A</span></span>  <br/> |<span data-ttu-id="7a7ff-157">"审阅"</span><span class="sxs-lookup"><span data-stu-id="7a7ff-157">"Review"</span></span>  <br/> |
   
<span data-ttu-id="7a7ff-158">上面指定的所有字符串可以都转换到用户的语言，如果适用。</span><span class="sxs-lookup"><span data-stu-id="7a7ff-158">All strings specified above can be translated to the user's language, if appropriate.</span></span>
  
## <a name="related-resources"></a><span data-ttu-id="7a7ff-159">相关资源</span><span class="sxs-lookup"><span data-stu-id="7a7ff-159">Related resources</span></span>

### <a name="protocol-specifications"></a><span data-ttu-id="7a7ff-160">协议规范</span><span class="sxs-lookup"><span data-stu-id="7a7ff-160">Protocol specifications</span></span>

<span data-ttu-id="7a7ff-161">[[MS OXPROPS]](http://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="7a7ff-161">[[MS-OXPROPS]](http://msdn.microsoft.com/library/f6ab1613-aefe-447d-a49c-18217230b148%28Office.15%29.aspx)</span></span>
  
> <span data-ttu-id="7a7ff-162">提供属性集定义和相关的 Exchange Server 协议规范的引用。</span><span class="sxs-lookup"><span data-stu-id="7a7ff-162">Provides property set definitions and references to related Exchange Server protocol specifications.</span></span>
    
<span data-ttu-id="7a7ff-163">[[MS OXOFLAG]](http://msdn.microsoft.com/library/f1e50be4-ed30-4c2a-b5cb-8ff3aaaf9b91%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="7a7ff-163">[[MS-OXOFLAG]](http://msdn.microsoft.com/library/f1e50be4-ed30-4c2a-b5cb-8ff3aaaf9b91%28Office.15%29.aspx)</span></span>
  
> <span data-ttu-id="7a7ff-164">指定的属性和与标记的操作。</span><span class="sxs-lookup"><span data-stu-id="7a7ff-164">Specifies the properties and operations related to flagging.</span></span>
    
### <a name="header-files"></a><span data-ttu-id="7a7ff-165">头文件</span><span class="sxs-lookup"><span data-stu-id="7a7ff-165">Header files</span></span>

<span data-ttu-id="7a7ff-166">Mapidefs.h</span><span class="sxs-lookup"><span data-stu-id="7a7ff-166">Mapidefs.h</span></span>
  
> <span data-ttu-id="7a7ff-167">提供数据类型定义。</span><span class="sxs-lookup"><span data-stu-id="7a7ff-167">Provides data type definitions.</span></span>
    
## <a name="see-also"></a><span data-ttu-id="7a7ff-168">另请参阅</span><span class="sxs-lookup"><span data-stu-id="7a7ff-168">See also</span></span>



[<span data-ttu-id="7a7ff-169">MAPI 属性</span><span class="sxs-lookup"><span data-stu-id="7a7ff-169">MAPI Properties</span></span>](mapi-properties.md)
  
[<span data-ttu-id="7a7ff-170">MAPI 规范属性</span><span class="sxs-lookup"><span data-stu-id="7a7ff-170">MAPI Canonical Properties</span></span>](mapi-canonical-properties.md)
  
[<span data-ttu-id="7a7ff-171">映射到 MAPI 名称的规范属性名称</span><span class="sxs-lookup"><span data-stu-id="7a7ff-171">Mapping Canonical Property Names to MAPI Names</span></span>](mapping-canonical-property-names-to-mapi-names.md)
  
[<span data-ttu-id="7a7ff-172">MAPI 名称映射到规范属性名称</span><span class="sxs-lookup"><span data-stu-id="7a7ff-172">Mapping MAPI Names to Canonical Property Names</span></span>](mapping-mapi-names-to-canonical-property-names.md)
