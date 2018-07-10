---
title: AttachmentId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttachmentId
api_type:
- schema
ms.assetid: 55a5fd77-60d1-40fa-8144-770600cedc6a
description: AttachmentId 元素标识项目或文件附件。 在 CreateAttachment 响应中使用此元素。
ms.openlocfilehash: 2910503d1661ca3aaeeb4e319deb39f6b57c5c0a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/25/2018
ms.locfileid: "19753277"
---
# <a name="attachmentid"></a><span data-ttu-id="71fa5-104">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="71fa5-104">AttachmentId</span></span>

<span data-ttu-id="71fa5-105">**AttachmentId**元素标识项目或文件附件。</span><span class="sxs-lookup"><span data-stu-id="71fa5-105">The **AttachmentId** element identifies an item or file attachment.</span></span> <span data-ttu-id="71fa5-106">在 CreateAttachment 响应中使用此元素。</span><span class="sxs-lookup"><span data-stu-id="71fa5-106">This element is used in CreateAttachment responses.</span></span> 
  
```xml
<AttachmentId Id="" RootItemId="" RootItemChangeKey="" />
```

 <span data-ttu-id="71fa5-107">**AttachmentIdType**</span><span class="sxs-lookup"><span data-stu-id="71fa5-107">**AttachmentIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="71fa5-108">属性和元素</span><span class="sxs-lookup"><span data-stu-id="71fa5-108">Attributes and elements</span></span>

<span data-ttu-id="71fa5-109">如下章节中介绍了属性、子元素和父元素。</span><span class="sxs-lookup"><span data-stu-id="71fa5-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="71fa5-110">属性</span><span class="sxs-lookup"><span data-stu-id="71fa5-110">Attributes</span></span>

|<span data-ttu-id="71fa5-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="71fa5-111">**Attribute**</span></span>|<span data-ttu-id="71fa5-112">**说明**</span><span class="sxs-lookup"><span data-stu-id="71fa5-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="71fa5-113">
  **Id**</span><span class="sxs-lookup"><span data-stu-id="71fa5-113">**Id**</span></span> <br/> |<span data-ttu-id="71fa5-114">标识附件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="71fa5-114">Identifies the unique identifier of the attachment.</span></span>  <br/> |
|<span data-ttu-id="71fa5-115">**RootItemId**</span><span class="sxs-lookup"><span data-stu-id="71fa5-115">**RootItemId**</span></span> <br/> |<span data-ttu-id="71fa5-116">标识附件附加到根存储项的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="71fa5-116">Identifies the unique identifier of the root store item to which the attachment is attached.</span></span>  <br/> |
|<span data-ttu-id="71fa5-117">**RootItemChangeKey**</span><span class="sxs-lookup"><span data-stu-id="71fa5-117">**RootItemChangeKey**</span></span> <br/> |<span data-ttu-id="71fa5-118">标识附件附加到根存储项的更改键。</span><span class="sxs-lookup"><span data-stu-id="71fa5-118">Identifies the change key of the root store item to which the attachment is attached.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="71fa5-119">子元素</span><span class="sxs-lookup"><span data-stu-id="71fa5-119">Child elements</span></span>

<span data-ttu-id="71fa5-120">无。</span><span class="sxs-lookup"><span data-stu-id="71fa5-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="71fa5-121">父元素</span><span class="sxs-lookup"><span data-stu-id="71fa5-121">Parent elements</span></span>

|<span data-ttu-id="71fa5-122">**元素**</span><span class="sxs-lookup"><span data-stu-id="71fa5-122">**Element**</span></span>|<span data-ttu-id="71fa5-123">**说明**</span><span class="sxs-lookup"><span data-stu-id="71fa5-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71fa5-124">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="71fa5-124">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="71fa5-125">代表附加到另一个 Exchange 项目的 Exchange 项目。</span><span class="sxs-lookup"><span data-stu-id="71fa5-125">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="71fa5-126">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="71fa5-126">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="71fa5-127">代表附加到 Exchange 存储中的项的文件。</span><span class="sxs-lookup"><span data-stu-id="71fa5-127">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="71fa5-128">注解</span><span class="sxs-lookup"><span data-stu-id="71fa5-128">Remarks</span></span>

<span data-ttu-id="71fa5-129">请务必注意创建附件时，已更改的根项目的更改键。</span><span class="sxs-lookup"><span data-stu-id="71fa5-129">It is important to note that when an attachment is created, the change key of the root item is altered.</span></span>
  
<span data-ttu-id="71fa5-130">DeleteAttachment 和 GetAttachment 请求中使用[AttachmentId （GetAttachment 和 DeleteAttachment）](attachmentid-getattachment-and-deleteattachment.md)元素。</span><span class="sxs-lookup"><span data-stu-id="71fa5-130">The [AttachmentId (GetAttachment and DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md) element is used in DeleteAttachment and GetAttachment requests.</span></span> 
  
<span data-ttu-id="71fa5-131">描述此元素的架构位于正在运行 MicrosoftExchange Server 2007 的计算机（已安装客户端访问服务器角色）的 EWS 虚拟目录中。</span><span class="sxs-lookup"><span data-stu-id="71fa5-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="71fa5-132">元素信息</span><span class="sxs-lookup"><span data-stu-id="71fa5-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="71fa5-133">命名空间</span><span class="sxs-lookup"><span data-stu-id="71fa5-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="71fa5-134">架构名称</span><span class="sxs-lookup"><span data-stu-id="71fa5-134">Schema name</span></span>  <br/> |<span data-ttu-id="71fa5-135">类型架构</span><span class="sxs-lookup"><span data-stu-id="71fa5-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="71fa5-136">验证文件</span><span class="sxs-lookup"><span data-stu-id="71fa5-136">Validation file</span></span>  <br/> |<span data-ttu-id="71fa5-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="71fa5-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="71fa5-138">可以为空</span><span class="sxs-lookup"><span data-stu-id="71fa5-138">Can be empty</span></span>  <br/> |<span data-ttu-id="71fa5-139">False</span><span class="sxs-lookup"><span data-stu-id="71fa5-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="71fa5-140">另请参阅</span><span class="sxs-lookup"><span data-stu-id="71fa5-140">See also</span></span>

- [<span data-ttu-id="71fa5-141">在交换 EWS XML 元素</span><span class="sxs-lookup"><span data-stu-id="71fa5-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
