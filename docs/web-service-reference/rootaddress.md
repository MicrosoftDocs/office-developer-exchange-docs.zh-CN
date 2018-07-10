---
title: RootAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RootAddress
api_type:
- schema
ms.assetid: 1dbb130a-e4eb-4baf-ae07-2568a8375bff
description: RootAddress 元素均表示启动 RecipientTrackingEvent 事件的事件的第一个地址。
ms.openlocfilehash: afe544d6ee8dea4cb416ad033ed2cd68976ec087
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827250"
---
# <a name="rootaddress"></a><span data-ttu-id="6294c-103">RootAddress</span><span class="sxs-lookup"><span data-stu-id="6294c-103">RootAddress</span></span>

<span data-ttu-id="6294c-104">**RootAddress**元素均表示启动[RecipientTrackingEvent](recipienttrackingevent.md)事件的事件的第一个地址。</span><span class="sxs-lookup"><span data-stu-id="6294c-104">The **RootAddress** element represents the first address that starts the event for a [RecipientTrackingEvent](recipienttrackingevent.md) event.</span></span> 
  
```xml
<RootAddress/>
```

 <span data-ttu-id="6294c-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="6294c-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6294c-106">属性和元素</span><span class="sxs-lookup"><span data-stu-id="6294c-106">Attributes and elements</span></span>

<span data-ttu-id="6294c-107">如下章节中介绍了属性、子元素和父元素。</span><span class="sxs-lookup"><span data-stu-id="6294c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6294c-108">属性</span><span class="sxs-lookup"><span data-stu-id="6294c-108">Attributes</span></span>

<span data-ttu-id="6294c-109">无。</span><span class="sxs-lookup"><span data-stu-id="6294c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6294c-110">子元素</span><span class="sxs-lookup"><span data-stu-id="6294c-110">Child elements</span></span>

<span data-ttu-id="6294c-111">无。</span><span class="sxs-lookup"><span data-stu-id="6294c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6294c-112">父元素</span><span class="sxs-lookup"><span data-stu-id="6294c-112">Parent elements</span></span>

|<span data-ttu-id="6294c-113">**元素**</span><span class="sxs-lookup"><span data-stu-id="6294c-113">**Element**</span></span>|<span data-ttu-id="6294c-114">**说明**</span><span class="sxs-lookup"><span data-stu-id="6294c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6294c-115">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="6294c-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="6294c-116">包含收件人为一个事件的信息。</span><span class="sxs-lookup"><span data-stu-id="6294c-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6294c-117">文本值</span><span class="sxs-lookup"><span data-stu-id="6294c-117">Text value</span></span>

<span data-ttu-id="6294c-118">文本值是启动跟踪事件的地址。</span><span class="sxs-lookup"><span data-stu-id="6294c-118">The text value is the address that starts the tracking event.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6294c-119">备注</span><span class="sxs-lookup"><span data-stu-id="6294c-119">Remarks</span></span>

<span data-ttu-id="6294c-120">描述此元素的架构位于承载 Exchange Web Services 的 IIS 虚拟目录中。Exchange Server 2010 Service Pack 1 (SP1) 中引入了此元素。</span><span class="sxs-lookup"><span data-stu-id="6294c-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6294c-121">元素信息</span><span class="sxs-lookup"><span data-stu-id="6294c-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6294c-122">命名空间</span><span class="sxs-lookup"><span data-stu-id="6294c-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6294c-123">架构名称</span><span class="sxs-lookup"><span data-stu-id="6294c-123">Schema Name</span></span>  <br/> |<span data-ttu-id="6294c-124">类型架构</span><span class="sxs-lookup"><span data-stu-id="6294c-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="6294c-125">验证文件</span><span class="sxs-lookup"><span data-stu-id="6294c-125">Validation File</span></span>  <br/> |<span data-ttu-id="6294c-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6294c-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6294c-127">可以为空</span><span class="sxs-lookup"><span data-stu-id="6294c-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="6294c-128">False</span><span class="sxs-lookup"><span data-stu-id="6294c-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6294c-129">另请参阅</span><span class="sxs-lookup"><span data-stu-id="6294c-129">See also</span></span>



[<span data-ttu-id="6294c-130">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="6294c-130">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="6294c-131">在交换 EWS XML 元素</span><span class="sxs-lookup"><span data-stu-id="6294c-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
