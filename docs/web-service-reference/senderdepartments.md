---
title: SenderDepartments
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SenderDepartments
api_type:
- schema
ms.assetid: b016cdde-d597-40ac-87c4-63ca68bd539d
description: SenderDepartments 元素指定发件人的部门匹配任何子值 (ProtectionRuleValueType) 元素中指定的部门。
ms.openlocfilehash: d40e6299bd46ede559cc2cce3bcc9d1611e96bd7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827331"
---
# <a name="senderdepartments"></a><span data-ttu-id="a2699-103">SenderDepartments</span><span class="sxs-lookup"><span data-stu-id="a2699-103">SenderDepartments</span></span>

<span data-ttu-id="a2699-104">**SenderDepartments**元素指定发件人的部门匹配任何子[值 (ProtectionRuleValueType)](value-protectionrulevaluetype.md)元素中指定的部门。</span><span class="sxs-lookup"><span data-stu-id="a2699-104">The **SenderDepartments** element specifies that the department of the sender matches any of the specified departments in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span> 
  
```XML
<SenderDepartments>
   <Value/>
</SenderDepartments>
```

 <span data-ttu-id="a2699-105">**ProtectionRuleSenderDepartmentsType**</span><span class="sxs-lookup"><span data-stu-id="a2699-105">**ProtectionRuleSenderDepartmentsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a2699-106">属性和元素</span><span class="sxs-lookup"><span data-stu-id="a2699-106">Attributes and elements</span></span>

<span data-ttu-id="a2699-107">如下章节中介绍了属性、子元素和父元素。</span><span class="sxs-lookup"><span data-stu-id="a2699-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a2699-108">属性</span><span class="sxs-lookup"><span data-stu-id="a2699-108">Attributes</span></span>

<span data-ttu-id="a2699-109">无。</span><span class="sxs-lookup"><span data-stu-id="a2699-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a2699-110">子元素</span><span class="sxs-lookup"><span data-stu-id="a2699-110">Child elements</span></span>

|<span data-ttu-id="a2699-111">**元素**</span><span class="sxs-lookup"><span data-stu-id="a2699-111">**Element**</span></span>|<span data-ttu-id="a2699-112">**说明**</span><span class="sxs-lookup"><span data-stu-id="a2699-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2699-113">值 (ProtectionRuleValueType)</span><span class="sxs-lookup"><span data-stu-id="a2699-113">Value (ProtectionRuleValueType)</span></span>](value-protectionrulevaluetype.md) <br/> |<span data-ttu-id="a2699-114">标识单个发件人部门。</span><span class="sxs-lookup"><span data-stu-id="a2699-114">Identifies a single sender department.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a2699-115">父元素</span><span class="sxs-lookup"><span data-stu-id="a2699-115">Parent elements</span></span>

|<span data-ttu-id="a2699-116">**元素**</span><span class="sxs-lookup"><span data-stu-id="a2699-116">**Element**</span></span>|<span data-ttu-id="a2699-117">**说明**</span><span class="sxs-lookup"><span data-stu-id="a2699-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2699-118">条件</span><span class="sxs-lookup"><span data-stu-id="a2699-118">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="a2699-119">确定要执行该规则的操作部分必须满足的条件。</span><span class="sxs-lookup"><span data-stu-id="a2699-119">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|[<span data-ttu-id="a2699-120">和 (ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="a2699-120">And (ProtectionRuleAndType)</span></span>](and-protectionruleandtype.md) <br/> |<span data-ttu-id="a2699-121">指定所有子元素都必须匹配以使值为 **true**。</span><span class="sxs-lookup"><span data-stu-id="a2699-121">Specifies that all child elements must match to evaluate to **true**.</span></span> <span data-ttu-id="a2699-122">指定必须有多个保护规则子条件。</span><span class="sxs-lookup"><span data-stu-id="a2699-122">Specifies that there must be more than one protection rule child condition.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a2699-123">备注</span><span class="sxs-lookup"><span data-stu-id="a2699-123">Remarks</span></span>

<span data-ttu-id="a2699-124">描述此元素的架构位于承载 Exchange Web Services 的 IIS 虚拟目录中。</span><span class="sxs-lookup"><span data-stu-id="a2699-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a2699-125">元素信息</span><span class="sxs-lookup"><span data-stu-id="a2699-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a2699-126">命名空间</span><span class="sxs-lookup"><span data-stu-id="a2699-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a2699-127">架构名称</span><span class="sxs-lookup"><span data-stu-id="a2699-127">Schema Name</span></span>  <br/> |<span data-ttu-id="a2699-128">类型架构</span><span class="sxs-lookup"><span data-stu-id="a2699-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="a2699-129">验证文件</span><span class="sxs-lookup"><span data-stu-id="a2699-129">Validation File</span></span>  <br/> |<span data-ttu-id="a2699-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a2699-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a2699-131">可以为空</span><span class="sxs-lookup"><span data-stu-id="a2699-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="a2699-132">False</span><span class="sxs-lookup"><span data-stu-id="a2699-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a2699-133">另请参阅</span><span class="sxs-lookup"><span data-stu-id="a2699-133">See also</span></span>



- [<span data-ttu-id="a2699-134">在交换 EWS XML 元素</span><span class="sxs-lookup"><span data-stu-id="a2699-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
