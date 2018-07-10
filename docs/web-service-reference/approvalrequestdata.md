---
title: ApprovalRequestData
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6c971cf7-5c3a-4e5e-9a7d-048f4ac0aadb
description: ApprovalRequestData 元素指定审批请求邮件审批的状态。
ms.openlocfilehash: ed1c1e3db4edd2cf4de032dc61abd73e863d4f1d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/25/2018
ms.locfileid: "19753251"
---
# <a name="approvalrequestdata"></a><span data-ttu-id="c0a14-103">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="c0a14-103">ApprovalRequestData</span></span>

<span data-ttu-id="c0a14-104">**ApprovalRequestData**元素指定审批请求邮件审批的状态。</span><span class="sxs-lookup"><span data-stu-id="c0a14-104">The **ApprovalRequestData** element specifies the approval state of an approval request message.</span></span> 
  
```xml
<ApprovalRequestData>
   <IsUndecidedApprovalRequest/>
   <ApprovalDecision/>
   <ApprovalDecisionMaker/>
   <ApprovalDecisionTime/>
</ApprovalRequestData>
```

 <span data-ttu-id="c0a14-105">**ApprovalRequestDataType**</span><span class="sxs-lookup"><span data-stu-id="c0a14-105">**ApprovalRequestDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c0a14-106">属性和元素</span><span class="sxs-lookup"><span data-stu-id="c0a14-106">Attributes and elements</span></span>

<span data-ttu-id="c0a14-107">如下章节中介绍了属性、子元素和父元素。</span><span class="sxs-lookup"><span data-stu-id="c0a14-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c0a14-108">属性</span><span class="sxs-lookup"><span data-stu-id="c0a14-108">Attributes</span></span>

<span data-ttu-id="c0a14-109">无。</span><span class="sxs-lookup"><span data-stu-id="c0a14-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c0a14-110">子元素</span><span class="sxs-lookup"><span data-stu-id="c0a14-110">Child elements</span></span>

<span data-ttu-id="c0a14-111">[IsUndecidedApprovalRequest](isundecidedapprovalrequest.md) | [ApprovalDecision](approvaldecision.md) | [ApprovalDecisionMaker](approvaldecisionmaker.md) | [ApprovalDecisionTime](approvaldecisiontime.md)</span><span class="sxs-lookup"><span data-stu-id="c0a14-111">[IsUndecidedApprovalRequest](isundecidedapprovalrequest.md) | [ApprovalDecision](approvaldecision.md) | [ApprovalDecisionMaker](approvaldecisionmaker.md) | [ApprovalDecisionTime](approvaldecisiontime.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c0a14-112">父元素</span><span class="sxs-lookup"><span data-stu-id="c0a14-112">Parent elements</span></span>

[<span data-ttu-id="c0a14-113">Message</span><span class="sxs-lookup"><span data-stu-id="c0a14-113">Message</span></span>](message-ex15websvcsotherref.md)
  
## <a name="remarks"></a><span data-ttu-id="c0a14-114">备注</span><span class="sxs-lookup"><span data-stu-id="c0a14-114">Remarks</span></span>

<span data-ttu-id="c0a14-115">Exchange Server 2013 Service Pack 1 (SP1) 中引入了此元素。</span><span class="sxs-lookup"><span data-stu-id="c0a14-115">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="c0a14-116">描述此元素的架构位于承载 Exchange Web Services 的 IIS 虚拟目录中。</span><span class="sxs-lookup"><span data-stu-id="c0a14-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c0a14-117">元素信息</span><span class="sxs-lookup"><span data-stu-id="c0a14-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c0a14-118">命名空间</span><span class="sxs-lookup"><span data-stu-id="c0a14-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c0a14-119">架构名称</span><span class="sxs-lookup"><span data-stu-id="c0a14-119">Schema Name</span></span>  <br/> |<span data-ttu-id="c0a14-120">类型架构</span><span class="sxs-lookup"><span data-stu-id="c0a14-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="c0a14-121">验证文件</span><span class="sxs-lookup"><span data-stu-id="c0a14-121">Validation File</span></span>  <br/> |<span data-ttu-id="c0a14-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c0a14-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c0a14-123">可以为空</span><span class="sxs-lookup"><span data-stu-id="c0a14-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="c0a14-124">True</span><span class="sxs-lookup"><span data-stu-id="c0a14-124">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c0a14-125">另请参阅</span><span class="sxs-lookup"><span data-stu-id="c0a14-125">See also</span></span>

- [<span data-ttu-id="c0a14-126">Message</span><span class="sxs-lookup"><span data-stu-id="c0a14-126">Message</span></span>](message-ex15websvcsotherref.md)
- [<span data-ttu-id="c0a14-127">在交换 EWS XML 元素</span><span class="sxs-lookup"><span data-stu-id="c0a14-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
