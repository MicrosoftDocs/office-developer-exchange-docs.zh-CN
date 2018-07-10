---
title: CreateContents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateContents
api_type:
- schema
ms.assetid: 8a9cd241-0d73-4be8-a563-a945898d1a0e
description: CreateContents 元素指示客户端是否可以创建内容表。 Microsoft Exchange Server 2007 Service Pack 1 (SP1) 中引入了此元素。
ms.openlocfilehash: f84ffdd2e6b485436d9e4ccd5f03a6e2c57fcfd1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/25/2018
ms.locfileid: "19753631"
---
# <a name="createcontents"></a><span data-ttu-id="3ae05-104">CreateContents</span><span class="sxs-lookup"><span data-stu-id="3ae05-104">CreateContents</span></span>

<span data-ttu-id="3ae05-105">**CreateContents**元素指示客户端是否可以创建内容表。</span><span class="sxs-lookup"><span data-stu-id="3ae05-105">The **CreateContents** element indicates whether a client can create a contents table.</span></span> <span data-ttu-id="3ae05-106">Microsoft Exchange Server 2007 Service Pack 1 (SP1) 中引入了此元素。</span><span class="sxs-lookup"><span data-stu-id="3ae05-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CreateContents>true or false</CreateContents>
```

 <span data-ttu-id="3ae05-107">**boolean**</span><span class="sxs-lookup"><span data-stu-id="3ae05-107">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3ae05-108">属性和元素</span><span class="sxs-lookup"><span data-stu-id="3ae05-108">Attributes and elements</span></span>

<span data-ttu-id="3ae05-109">如下章节中介绍了属性、子元素和父元素。</span><span class="sxs-lookup"><span data-stu-id="3ae05-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3ae05-110">属性</span><span class="sxs-lookup"><span data-stu-id="3ae05-110">Attributes</span></span>

<span data-ttu-id="3ae05-111">无。</span><span class="sxs-lookup"><span data-stu-id="3ae05-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3ae05-112">子元素</span><span class="sxs-lookup"><span data-stu-id="3ae05-112">Child elements</span></span>

<span data-ttu-id="3ae05-113">无。</span><span class="sxs-lookup"><span data-stu-id="3ae05-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3ae05-114">父元素</span><span class="sxs-lookup"><span data-stu-id="3ae05-114">Parent elements</span></span>

|<span data-ttu-id="3ae05-115">**元素**</span><span class="sxs-lookup"><span data-stu-id="3ae05-115">**Element**</span></span>|<span data-ttu-id="3ae05-116">**说明**</span><span class="sxs-lookup"><span data-stu-id="3ae05-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3ae05-117">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="3ae05-117">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="3ae05-118">包含客户端基于的项目或文件夹的权限设置的权限。</span><span class="sxs-lookup"><span data-stu-id="3ae05-118">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="3ae05-119">此元素是引入的 inExchange 2007 SP1。</span><span class="sxs-lookup"><span data-stu-id="3ae05-119">This element was introduced inExchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3ae05-120">文本值</span><span class="sxs-lookup"><span data-stu-id="3ae05-120">Text value</span></span>

<span data-ttu-id="3ae05-121">文本值为**true**指示客户端可以创建内容表。</span><span class="sxs-lookup"><span data-stu-id="3ae05-121">A text value of **true** indicates that a client can create a contents table.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3ae05-122">注解</span><span class="sxs-lookup"><span data-stu-id="3ae05-122">Remarks</span></span>

<span data-ttu-id="3ae05-123">此属性仅可用于文件夹对象。</span><span class="sxs-lookup"><span data-stu-id="3ae05-123">This property is only used on folder objects.</span></span>
  
<span data-ttu-id="3ae05-124">描述此元素的架构位于正在运行 Microsoft Exchange Server 2007 的计算机（已安装客户端访问服务器角色）的 EWS 虚拟目录中。</span><span class="sxs-lookup"><span data-stu-id="3ae05-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3ae05-125">元素信息</span><span class="sxs-lookup"><span data-stu-id="3ae05-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3ae05-126">命名空间</span><span class="sxs-lookup"><span data-stu-id="3ae05-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3ae05-127">架构名称</span><span class="sxs-lookup"><span data-stu-id="3ae05-127">Schema Name</span></span>  <br/> |<span data-ttu-id="3ae05-128">类型架构</span><span class="sxs-lookup"><span data-stu-id="3ae05-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="3ae05-129">验证文件</span><span class="sxs-lookup"><span data-stu-id="3ae05-129">Validation File</span></span>  <br/> |<span data-ttu-id="3ae05-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3ae05-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3ae05-131">可以为空</span><span class="sxs-lookup"><span data-stu-id="3ae05-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="3ae05-132">False</span><span class="sxs-lookup"><span data-stu-id="3ae05-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3ae05-133">另请参阅</span><span class="sxs-lookup"><span data-stu-id="3ae05-133">See also</span></span>



- [<span data-ttu-id="3ae05-134">在交换 EWS XML 元素</span><span class="sxs-lookup"><span data-stu-id="3ae05-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="3ae05-135">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="3ae05-135">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)
