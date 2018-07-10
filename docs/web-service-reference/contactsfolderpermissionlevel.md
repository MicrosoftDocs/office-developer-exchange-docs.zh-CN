---
title: ContactsFolderPermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContactsFolderPermissionLevel
api_type:
- schema
ms.assetid: 805f05e7-b320-436a-9965-ba1ee235ac41
description: ContactsFolderPermissionLevel 元素包含默认联系人文件夹的权限。 Microsoft Exchange Server 2007 Service Pack 1 (SP1) 中引入了此元素。
ms.openlocfilehash: 4b6a109c3a38a20dc5d6f611607b16ada0e4e46b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/25/2018
ms.locfileid: "19753510"
---
# <a name="contactsfolderpermissionlevel"></a><span data-ttu-id="46399-104">ContactsFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="46399-104">ContactsFolderPermissionLevel</span></span>

<span data-ttu-id="46399-105">**ContactsFolderPermissionLevel**元素包含默认联系人文件夹的权限。</span><span class="sxs-lookup"><span data-stu-id="46399-105">The **ContactsFolderPermissionLevel** element contains the permissions for the default Contacts folder.</span></span> <span data-ttu-id="46399-106">Microsoft Exchange Server 2007 Service Pack 1 (SP1) 中引入了此元素。</span><span class="sxs-lookup"><span data-stu-id="46399-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ContactsFolderPermissionLevel>
   None or Editor or Reviewer or Author or Custom
</ContactsFolderPermissionLevel>
```

 <span data-ttu-id="46399-107">**DelegateFolderPermissionLevelType**</span><span class="sxs-lookup"><span data-stu-id="46399-107">**DelegateFolderPermissionLevelType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="46399-108">属性和元素</span><span class="sxs-lookup"><span data-stu-id="46399-108">Attributes and elements</span></span>

<span data-ttu-id="46399-109">如下章节中介绍了属性、子元素和父元素。</span><span class="sxs-lookup"><span data-stu-id="46399-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="46399-110">属性</span><span class="sxs-lookup"><span data-stu-id="46399-110">Attributes</span></span>

<span data-ttu-id="46399-111">无。</span><span class="sxs-lookup"><span data-stu-id="46399-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="46399-112">子元素</span><span class="sxs-lookup"><span data-stu-id="46399-112">Child elements</span></span>

<span data-ttu-id="46399-113">无。</span><span class="sxs-lookup"><span data-stu-id="46399-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="46399-114">父元素</span><span class="sxs-lookup"><span data-stu-id="46399-114">Parent elements</span></span>

|<span data-ttu-id="46399-115">**元素**</span><span class="sxs-lookup"><span data-stu-id="46399-115">**Element**</span></span>|<span data-ttu-id="46399-116">**说明**</span><span class="sxs-lookup"><span data-stu-id="46399-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="46399-117">DelegatePermissions</span><span class="sxs-lookup"><span data-stu-id="46399-117">DelegatePermissions</span></span>](delegatepermissions.md) <br/> |<span data-ttu-id="46399-118">包含用户的委派权限级别设置。</span><span class="sxs-lookup"><span data-stu-id="46399-118">Contains the delegate permission level settings for a user.</span></span> <span data-ttu-id="46399-119">在 Exchange 2007 SP1 引入了此元素。</span><span class="sxs-lookup"><span data-stu-id="46399-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="46399-120">文本值</span><span class="sxs-lookup"><span data-stu-id="46399-120">Text value</span></span>

<span data-ttu-id="46399-121">下表列出了表示的权限级别的文本值。</span><span class="sxs-lookup"><span data-stu-id="46399-121">The following table lists the text values that represent the permission levels.</span></span>
  
<span data-ttu-id="46399-122">**权限级别的文本值**</span><span class="sxs-lookup"><span data-stu-id="46399-122">**Permission level text values**</span></span>

|<span data-ttu-id="46399-123">**权限级别**</span><span class="sxs-lookup"><span data-stu-id="46399-123">**Permission level**</span></span>|<span data-ttu-id="46399-124">**说明**</span><span class="sxs-lookup"><span data-stu-id="46399-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="46399-125">无</span><span class="sxs-lookup"><span data-stu-id="46399-125">None</span></span>  <br/> |<span data-ttu-id="46399-126">代理用户对联系人文件夹具有任何访问权限。</span><span class="sxs-lookup"><span data-stu-id="46399-126">The delegate user has no access permissions to the Contacts folder.</span></span>  <br/> |
|<span data-ttu-id="46399-127">Reviewer</span><span class="sxs-lookup"><span data-stu-id="46399-127">Reviewer</span></span>  <br/> |<span data-ttu-id="46399-128">委派用户可以读取联系人文件夹中的项目。</span><span class="sxs-lookup"><span data-stu-id="46399-128">The delegate user can read items in the Contacts folder.</span></span>  <br/> |
|<span data-ttu-id="46399-129">作者</span><span class="sxs-lookup"><span data-stu-id="46399-129">Author</span></span>  <br/> |<span data-ttu-id="46399-130">委派用户可以读取和在联系人文件夹中创建项目。</span><span class="sxs-lookup"><span data-stu-id="46399-130">The delegate user can read and create items in the Contacts folder.</span></span>  <br/> |
|<span data-ttu-id="46399-131">Editor</span><span class="sxs-lookup"><span data-stu-id="46399-131">Editor</span></span>  <br/> |<span data-ttu-id="46399-132">委派用户可以读取、 创建和修改联系人文件夹中的项目。</span><span class="sxs-lookup"><span data-stu-id="46399-132">The delegate user can read, create, and modify items in the Contacts folder.</span></span>  <br/> |
|<span data-ttu-id="46399-133">自定义</span><span class="sxs-lookup"><span data-stu-id="46399-133">Custom</span></span>  <br/> |<span data-ttu-id="46399-134">代理用户对联系人文件夹具有自定义访问权限。</span><span class="sxs-lookup"><span data-stu-id="46399-134">The delegate user has custom access permissions to the Contacts folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="46399-135">备注</span><span class="sxs-lookup"><span data-stu-id="46399-135">Remarks</span></span>

<span data-ttu-id="46399-136">描述此元素的架构位于正在运行 Microsoft Exchange Server 2007 的计算机（已安装客户端访问服务器角色）的 EWS 虚拟目录中。</span><span class="sxs-lookup"><span data-stu-id="46399-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="46399-137">元素信息</span><span class="sxs-lookup"><span data-stu-id="46399-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="46399-138">命名空间</span><span class="sxs-lookup"><span data-stu-id="46399-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="46399-139">架构名称</span><span class="sxs-lookup"><span data-stu-id="46399-139">Schema Name</span></span>  <br/> |<span data-ttu-id="46399-140">类型架构</span><span class="sxs-lookup"><span data-stu-id="46399-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="46399-141">验证文件</span><span class="sxs-lookup"><span data-stu-id="46399-141">Validation File</span></span>  <br/> |<span data-ttu-id="46399-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="46399-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="46399-143">可以为空</span><span class="sxs-lookup"><span data-stu-id="46399-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="46399-144">False</span><span class="sxs-lookup"><span data-stu-id="46399-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="46399-145">另请参阅</span><span class="sxs-lookup"><span data-stu-id="46399-145">See also</span></span>



[<span data-ttu-id="46399-146">AddDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="46399-146">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="46399-147">UpdateDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="46399-147">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="46399-148">在交换 EWS XML 元素</span><span class="sxs-lookup"><span data-stu-id="46399-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="46399-149">添加代理人</span><span class="sxs-lookup"><span data-stu-id="46399-149">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)
