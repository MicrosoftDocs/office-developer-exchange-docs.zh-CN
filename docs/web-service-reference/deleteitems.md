---
title: DeleteItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItems
api_type:
- schema
ms.assetid: a5898bfc-f5ae-451d-9713-3e55864c690c
description: DeleteItems 元素指示文件夹中的哪些项目用户有权删除。 Microsoft Exchange Server 2007 Service Pack 1 (SP1) 中引入了此元素。
ms.openlocfilehash: 0be2154d1ceb6a995df8b27033fdc59bca81f9ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/25/2018
ms.locfileid: "19753820"
---
# <a name="deleteitems"></a><span data-ttu-id="78cc6-104">DeleteItems</span><span class="sxs-lookup"><span data-stu-id="78cc6-104">DeleteItems</span></span>

<span data-ttu-id="78cc6-105">**DeleteItems**元素指示文件夹中的哪些项目用户有权删除。</span><span class="sxs-lookup"><span data-stu-id="78cc6-105">The **DeleteItems** element indicates which items in a folder a user has permission to delete.</span></span> <span data-ttu-id="78cc6-106">Microsoft Exchange Server 2007 Service Pack 1 (SP1) 中引入了此元素。</span><span class="sxs-lookup"><span data-stu-id="78cc6-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<DeleteItems>None or Owned or All</DeleteItems>
```

 <span data-ttu-id="78cc6-107">**PermissionActionType**</span><span class="sxs-lookup"><span data-stu-id="78cc6-107">**PermissionActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="78cc6-108">属性和元素</span><span class="sxs-lookup"><span data-stu-id="78cc6-108">Attributes and elements</span></span>

<span data-ttu-id="78cc6-109">如下章节中介绍了属性、子元素和父元素。</span><span class="sxs-lookup"><span data-stu-id="78cc6-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="78cc6-110">属性</span><span class="sxs-lookup"><span data-stu-id="78cc6-110">Attributes</span></span>

<span data-ttu-id="78cc6-111">无。</span><span class="sxs-lookup"><span data-stu-id="78cc6-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="78cc6-112">子元素</span><span class="sxs-lookup"><span data-stu-id="78cc6-112">Child elements</span></span>

<span data-ttu-id="78cc6-113">无。</span><span class="sxs-lookup"><span data-stu-id="78cc6-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="78cc6-114">父元素</span><span class="sxs-lookup"><span data-stu-id="78cc6-114">Parent elements</span></span>

|<span data-ttu-id="78cc6-115">**元素**</span><span class="sxs-lookup"><span data-stu-id="78cc6-115">**Element**</span></span>|<span data-ttu-id="78cc6-116">**说明**</span><span class="sxs-lookup"><span data-stu-id="78cc6-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="78cc6-117">权限</span><span class="sxs-lookup"><span data-stu-id="78cc6-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="78cc6-p103">到文件夹定义用户拥有的访问权限。在 Exchange 2007 SP1 引入了此元素。</span><span class="sxs-lookup"><span data-stu-id="78cc6-p103">Defines the access that a user has to a folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="78cc6-120">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="78cc6-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="78cc6-p104">定义日历文件夹的用户具有的访问权限。在 Exchange 2007 SP1 引入了此元素。</span><span class="sxs-lookup"><span data-stu-id="78cc6-p104">Defines the access that a user has to a Calendar folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="78cc6-123">文本值</span><span class="sxs-lookup"><span data-stu-id="78cc6-123">Text value</span></span>

<span data-ttu-id="78cc6-124">下表列出了**DeleteItems**元素的可能值。</span><span class="sxs-lookup"><span data-stu-id="78cc6-124">The following table lists the possible values for the **DeleteItems** element.</span></span> 
  
<span data-ttu-id="78cc6-125">**DeleteItems 元素的文本值**</span><span class="sxs-lookup"><span data-stu-id="78cc6-125">**DeleteItems element text values**</span></span>

|<span data-ttu-id="78cc6-126">**值**</span><span class="sxs-lookup"><span data-stu-id="78cc6-126">**Value**</span></span>|<span data-ttu-id="78cc6-127">**说明**</span><span class="sxs-lookup"><span data-stu-id="78cc6-127">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="78cc6-128">无</span><span class="sxs-lookup"><span data-stu-id="78cc6-128">None</span></span>  <br/> |<span data-ttu-id="78cc6-129">指示用户没有删除文件夹中的项目的权限。</span><span class="sxs-lookup"><span data-stu-id="78cc6-129">Indicates that the user does not have permission to delete items in the folder.</span></span>  <br/> |
|<span data-ttu-id="78cc6-130">拥有</span><span class="sxs-lookup"><span data-stu-id="78cc6-130">Owned</span></span>  <br/> |<span data-ttu-id="78cc6-131">指示用户有权删除文件夹中的用户所拥有的项目。</span><span class="sxs-lookup"><span data-stu-id="78cc6-131">Indicates that the user has permission to delete the items that the user owns in the folder.</span></span>  <br/> |
|<span data-ttu-id="78cc6-132">所有</span><span class="sxs-lookup"><span data-stu-id="78cc6-132">All</span></span>  <br/> |<span data-ttu-id="78cc6-133">指示用户有权删除文件夹中的所有项目。</span><span class="sxs-lookup"><span data-stu-id="78cc6-133">Indicates that the user has permission to delete all items in the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="78cc6-134">备注</span><span class="sxs-lookup"><span data-stu-id="78cc6-134">Remarks</span></span>

<span data-ttu-id="78cc6-135">描述此元素的架构位于正在运行 Microsoft Exchange Server 2007 的计算机（已安装客户端访问服务器角色）的 EWS 虚拟目录中。</span><span class="sxs-lookup"><span data-stu-id="78cc6-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="78cc6-136">元素信息</span><span class="sxs-lookup"><span data-stu-id="78cc6-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="78cc6-137">命名空间</span><span class="sxs-lookup"><span data-stu-id="78cc6-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="78cc6-138">架构名称</span><span class="sxs-lookup"><span data-stu-id="78cc6-138">Schema Name</span></span>  <br/> |<span data-ttu-id="78cc6-139">类型架构</span><span class="sxs-lookup"><span data-stu-id="78cc6-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="78cc6-140">验证文件</span><span class="sxs-lookup"><span data-stu-id="78cc6-140">Validation File</span></span>  <br/> |<span data-ttu-id="78cc6-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="78cc6-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="78cc6-142">可以为空</span><span class="sxs-lookup"><span data-stu-id="78cc6-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="78cc6-143">False</span><span class="sxs-lookup"><span data-stu-id="78cc6-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="78cc6-144">另请参阅</span><span class="sxs-lookup"><span data-stu-id="78cc6-144">See also</span></span>

- [<span data-ttu-id="78cc6-145">在交换 EWS XML 元素</span><span class="sxs-lookup"><span data-stu-id="78cc6-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="78cc6-146">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="78cc6-146">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)
