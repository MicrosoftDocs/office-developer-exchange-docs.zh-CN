---
title: ContainsSubjectOrBodyStrings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContainsSubjectOrBodyStrings
api_type:
- schema
ms.assetid: 22aebf31-d9f4-4e03-bbff-c675409518d1
description: ContainsSubjectOrBodyStrings 元素表示必须出现在正文或中的条件或例外应用的顺序的传入邮件的主题的字符串。
ms.openlocfilehash: f577e7d26bb7d82ea1017f720e1d3a30892e2ef1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/25/2018
ms.locfileid: "19753543"
---
# <a name="containssubjectorbodystrings"></a><span data-ttu-id="aaaa3-103">ContainsSubjectOrBodyStrings</span><span class="sxs-lookup"><span data-stu-id="aaaa3-103">ContainsSubjectOrBodyStrings</span></span>

<span data-ttu-id="aaaa3-104">**ContainsSubjectOrBodyStrings**元素表示必须出现在正文或中的条件或例外应用的顺序的传入邮件的主题的字符串。</span><span class="sxs-lookup"><span data-stu-id="aaaa3-104">The **ContainsSubjectOrBodyStrings** element indicates the strings that must appear in either the body or the subject of incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ContainsSubjectOrBodyStrings>
    <String/>
</ContainsSubjectOrBodyStrings>
```

 <span data-ttu-id="aaaa3-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="aaaa3-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aaaa3-106">属性和元素</span><span class="sxs-lookup"><span data-stu-id="aaaa3-106">Attributes and elements</span></span>

<span data-ttu-id="aaaa3-107">如下章节中介绍了属性、子元素和父元素。</span><span class="sxs-lookup"><span data-stu-id="aaaa3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aaaa3-108">属性</span><span class="sxs-lookup"><span data-stu-id="aaaa3-108">Attributes</span></span>

<span data-ttu-id="aaaa3-109">无。</span><span class="sxs-lookup"><span data-stu-id="aaaa3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aaaa3-110">子元素</span><span class="sxs-lookup"><span data-stu-id="aaaa3-110">Child elements</span></span>

|<span data-ttu-id="aaaa3-111">**元素**</span><span class="sxs-lookup"><span data-stu-id="aaaa3-111">**Element**</span></span>|<span data-ttu-id="aaaa3-112">**说明**</span><span class="sxs-lookup"><span data-stu-id="aaaa3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aaaa3-113">字符串</span><span class="sxs-lookup"><span data-stu-id="aaaa3-113">String</span></span>](string.md) <br/> |<span data-ttu-id="aaaa3-114">表示一个必须显示在正文或中的条件或例外应用的顺序的传入邮件的主题的字符串。</span><span class="sxs-lookup"><span data-stu-id="aaaa3-114">Represents a string that must appear in either the body or the subject of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aaaa3-115">父元素</span><span class="sxs-lookup"><span data-stu-id="aaaa3-115">Parent elements</span></span>

|<span data-ttu-id="aaaa3-116">**元素**</span><span class="sxs-lookup"><span data-stu-id="aaaa3-116">**Element**</span></span>|<span data-ttu-id="aaaa3-117">**说明**</span><span class="sxs-lookup"><span data-stu-id="aaaa3-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aaaa3-118">条件</span><span class="sxs-lookup"><span data-stu-id="aaaa3-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="aaaa3-119">表示履行时将触发规则的规则操作的条件。</span><span class="sxs-lookup"><span data-stu-id="aaaa3-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="aaaa3-120">异常</span><span class="sxs-lookup"><span data-stu-id="aaaa3-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="aaaa3-121">表示表示收件箱规则的所有可用的规则例外条件的异常。</span><span class="sxs-lookup"><span data-stu-id="aaaa3-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="aaaa3-122">文本值</span><span class="sxs-lookup"><span data-stu-id="aaaa3-122">Text value</span></span>

<span data-ttu-id="aaaa3-123">无。</span><span class="sxs-lookup"><span data-stu-id="aaaa3-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="aaaa3-124">备注</span><span class="sxs-lookup"><span data-stu-id="aaaa3-124">Remarks</span></span>

<span data-ttu-id="aaaa3-125">描述此元素的架构位于承载 Exchange Web Services 的 IIS 虚拟目录中。</span><span class="sxs-lookup"><span data-stu-id="aaaa3-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aaaa3-126">元素信息</span><span class="sxs-lookup"><span data-stu-id="aaaa3-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aaaa3-127">命名空间</span><span class="sxs-lookup"><span data-stu-id="aaaa3-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="aaaa3-128">架构名称</span><span class="sxs-lookup"><span data-stu-id="aaaa3-128">Schema Name</span></span>  <br/> |<span data-ttu-id="aaaa3-129">消息架构</span><span class="sxs-lookup"><span data-stu-id="aaaa3-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="aaaa3-130">验证文件</span><span class="sxs-lookup"><span data-stu-id="aaaa3-130">Validation File</span></span>  <br/> |<span data-ttu-id="aaaa3-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="aaaa3-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="aaaa3-132">可以为空</span><span class="sxs-lookup"><span data-stu-id="aaaa3-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="aaaa3-133">True</span><span class="sxs-lookup"><span data-stu-id="aaaa3-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aaaa3-134">另请参阅</span><span class="sxs-lookup"><span data-stu-id="aaaa3-134">See also</span></span>



- [<span data-ttu-id="aaaa3-135">在交换 EWS XML 元素</span><span class="sxs-lookup"><span data-stu-id="aaaa3-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
