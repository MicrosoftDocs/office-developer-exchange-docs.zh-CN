---
title: ApprovalDecision
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5e7c5687-cb9e-4f0b-ac8f-b82591914a39
description: ApprovalDecision 元素指定在审批请求消息上所做的决策。
ms.openlocfilehash: 4ca73813440200e5d2fb9f920d81459d8cd5e4ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/25/2018
ms.locfileid: "19753247"
---
# <a name="approvaldecision"></a><span data-ttu-id="940a3-103">ApprovalDecision</span><span class="sxs-lookup"><span data-stu-id="940a3-103">ApprovalDecision</span></span>

<span data-ttu-id="940a3-104">**ApprovalDecision**元素指定在审批请求消息上所做的决策。</span><span class="sxs-lookup"><span data-stu-id="940a3-104">The **ApprovalDecision** element specifies the decision made on an approval request message.</span></span> 
  
```XML
<ApprovalDecision> 1 | 2 </ApprovalDecision>
```

 <span data-ttu-id="940a3-105">**int**</span><span class="sxs-lookup"><span data-stu-id="940a3-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="940a3-106">属性和元素</span><span class="sxs-lookup"><span data-stu-id="940a3-106">Attributes and elements</span></span>

<span data-ttu-id="940a3-107">如下章节中介绍了属性、子元素和父元素。</span><span class="sxs-lookup"><span data-stu-id="940a3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="940a3-108">属性</span><span class="sxs-lookup"><span data-stu-id="940a3-108">Attributes</span></span>

<span data-ttu-id="940a3-109">无。</span><span class="sxs-lookup"><span data-stu-id="940a3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="940a3-110">子元素</span><span class="sxs-lookup"><span data-stu-id="940a3-110">Child elements</span></span>

<span data-ttu-id="940a3-111">无。</span><span class="sxs-lookup"><span data-stu-id="940a3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="940a3-112">父元素</span><span class="sxs-lookup"><span data-stu-id="940a3-112">Parent elements</span></span>

[<span data-ttu-id="940a3-113">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="940a3-113">ApprovalRequestData</span></span>](approvalrequestdata.md)
  
## <a name="text-value"></a><span data-ttu-id="940a3-114">文本值</span><span class="sxs-lookup"><span data-stu-id="940a3-114">Text value</span></span>

<span data-ttu-id="940a3-115">如果已批准的 1 和 2 如果拒绝**ApprovalDecision**元素的文本值。</span><span class="sxs-lookup"><span data-stu-id="940a3-115">The text value of the **ApprovalDecision** element is 1 if approved and 2 if rejected.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="940a3-116">备注</span><span class="sxs-lookup"><span data-stu-id="940a3-116">Remarks</span></span>

<span data-ttu-id="940a3-117">Exchange Server 2013 Service Pack 1 (SP1) 中引入了此元素。</span><span class="sxs-lookup"><span data-stu-id="940a3-117">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="940a3-118">描述此元素的架构位于承载 Exchange Web Services 的 IIS 虚拟目录中。</span><span class="sxs-lookup"><span data-stu-id="940a3-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="940a3-119">元素信息</span><span class="sxs-lookup"><span data-stu-id="940a3-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="940a3-120">命名空间</span><span class="sxs-lookup"><span data-stu-id="940a3-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="940a3-121">架构名称</span><span class="sxs-lookup"><span data-stu-id="940a3-121">Schema Name</span></span>  <br/> |<span data-ttu-id="940a3-122">类型架构</span><span class="sxs-lookup"><span data-stu-id="940a3-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="940a3-123">验证文件</span><span class="sxs-lookup"><span data-stu-id="940a3-123">Validation File</span></span>  <br/> |<span data-ttu-id="940a3-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="940a3-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="940a3-125">可以为空</span><span class="sxs-lookup"><span data-stu-id="940a3-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="940a3-126">True</span><span class="sxs-lookup"><span data-stu-id="940a3-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="940a3-127">另请参阅</span><span class="sxs-lookup"><span data-stu-id="940a3-127">See also</span></span>

- [<span data-ttu-id="940a3-128">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="940a3-128">ApprovalRequestData</span></span>](approvalrequestdata.md)
- [<span data-ttu-id="940a3-129">在交换 EWS XML 元素</span><span class="sxs-lookup"><span data-stu-id="940a3-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
