---
title: 使用 EWS 在 Exchange 公用文件夹访问。
manager: sethgros
ms.date: 7/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d9372057-1deb-45de-8f98-b9149604429a
description: 了解如何使用 EWS 和 EWS 托管 API 访问公用文件夹和 Exchange 路由的公用文件夹请求。
ms.openlocfilehash: cfa089ba617dc760ed12883590e141debb5ecd9b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/25/2018
ms.locfileid: "19753010"
---
# <a name="public-folder-access-with-ews-in-exchange"></a><span data-ttu-id="d4c93-103">使用 EWS 在 Exchange 公用文件夹访问。</span><span class="sxs-lookup"><span data-stu-id="d4c93-103">Public folder access with EWS in Exchange</span></span>

<span data-ttu-id="d4c93-104">了解如何使用 EWS 和 EWS 托管 API 访问公用文件夹和 Exchange 路由的公用文件夹请求。</span><span class="sxs-lookup"><span data-stu-id="d4c93-104">Learn about how to use EWS and the EWS Managed API to access public folders and route public folder requests in Exchange.</span></span>
  
<span data-ttu-id="d4c93-105">公用文件夹提供共享存储库的组织中的用户可以访问的项目。</span><span class="sxs-lookup"><span data-stu-id="d4c93-105">Public folders provide a shared repository of items that users in your organization can access.</span></span> <span data-ttu-id="d4c93-106">Office 365 和 Exchange Online 中，启动与 Exchange 2013 的 Exchange 内部部署版本中引入公用文件夹的新体系的结构。</span><span class="sxs-lookup"><span data-stu-id="d4c93-106">Office 365, Exchange Online, and on-premises versions of Exchange starting with Exchange 2013 introduce a new architecture for public folders.</span></span> <span data-ttu-id="d4c93-107">Exchange 中的公用文件夹使用专用的邮箱设计 （而不是公用文件夹数据库） 来存储公用文件夹层次结构和公用文件夹内容。</span><span class="sxs-lookup"><span data-stu-id="d4c93-107">Public folders in Exchange use a specialized mailbox design (instead of a public folder database) to store the public folder hierarchy and public folder content.</span></span> <span data-ttu-id="d4c93-108">公用文件夹权限管理通过角色基于访问控制 (RBAC)。</span><span class="sxs-lookup"><span data-stu-id="d4c93-108">Public folder permissions are managed through Role Based Access Control (RBAC).</span></span>
  
<span data-ttu-id="d4c93-109">客户端访问技术，如 Exchange Web Services (EWS) 和 EWS 托管 API 提供了公用文件夹层次结构和公用文件夹数据库中的内容项的编程访问。</span><span class="sxs-lookup"><span data-stu-id="d4c93-109">Client access technologies, like Exchange Web Services (EWS) and the EWS Managed API, provide programmatic access to both the public folder hierarchy and content items in a public folder database.</span></span> <span data-ttu-id="d4c93-110">本文提供有关如何使用 EWS 和 EWS 托管 API 访问公用文件夹和公用文件夹和公用文件夹数据的信息。</span><span class="sxs-lookup"><span data-stu-id="d4c93-110">This article provides information about how you can use EWS and the EWS Managed API to access public folders and public folders and public folder data.</span></span> 
  
## <a name="ews-operations-and-ews-managed-api-methods-for-public-folder-access"></a><span data-ttu-id="d4c93-111">EWS 操作和公用文件夹访问 EWS 托管 API 方法</span><span class="sxs-lookup"><span data-stu-id="d4c93-111">EWS operations and EWS Managed API methods for public folder access</span></span>
<span data-ttu-id="d4c93-112"><a name="bk_functionality"> </a></span><span class="sxs-lookup"><span data-stu-id="d4c93-112"></span></span>

<span data-ttu-id="d4c93-113">大多数核心 EWS 操作支持公用文件夹进行访问。</span><span class="sxs-lookup"><span data-stu-id="d4c93-113">Most of the core EWS operations support public folder access.</span></span> <span data-ttu-id="d4c93-114">您可以使用的文件夹和项目操作和下表中列出的 EWS 托管 API 方法处理公用文件夹。</span><span class="sxs-lookup"><span data-stu-id="d4c93-114">You can use the folder and item operations and the EWS Managed API methods listed in the following table to work with public folders.</span></span>
  
<span data-ttu-id="d4c93-115">有关 EWS 托管 API 方法的信息，请参阅[EWS 托管 API 的命名空间](http://msdn.microsoft.com/zh-cn/library/jj220535%28v=exchg.80%29.aspx)。</span><span class="sxs-lookup"><span data-stu-id="d4c93-115">For information about EWS Managed API methods, see [EWS Managed API namespaces](http://msdn.microsoft.com/zh-cn/library/jj220535%28v=exchg.80%29.aspx).</span></span>
  
|<span data-ttu-id="d4c93-116">**EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="d4c93-116">**EWS operation**</span></span>|<span data-ttu-id="d4c93-117">**EWS 托管的 API 方法**</span><span class="sxs-lookup"><span data-stu-id="d4c93-117">**EWS Managed API method**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4c93-118">CreateFolder Operation</span><span class="sxs-lookup"><span data-stu-id="d4c93-118">CreateFolder operation</span></span>](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |<span data-ttu-id="d4c93-119">**Folder.Save()**</span><span class="sxs-lookup"><span data-stu-id="d4c93-119">**Folder.Save()**</span></span> <br/> |
|[<span data-ttu-id="d4c93-120">UpdateFolder Operation</span><span class="sxs-lookup"><span data-stu-id="d4c93-120">UpdateFolder operation</span></span>](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |<span data-ttu-id="d4c93-121">**Folder.Update()**</span><span class="sxs-lookup"><span data-stu-id="d4c93-121">**Folder.Update()**</span></span> <br/> |
|[<span data-ttu-id="d4c93-122">DeleteFolder 操作</span><span class="sxs-lookup"><span data-stu-id="d4c93-122">DeleteFolder operation</span></span>](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |<span data-ttu-id="d4c93-123">**Folder.Delete()**</span><span class="sxs-lookup"><span data-stu-id="d4c93-123">**Folder.Delete()**</span></span> <br/> |
|<span data-ttu-id="d4c93-124">[MoveFolder 操作](http://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx)<sup>1</sup></span><span class="sxs-lookup"><span data-stu-id="d4c93-124">[MoveFolder operation](http://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx)<sup>1</sup></span></span> <br/> |<span data-ttu-id="d4c93-125">**Folder.Move()**</span><span class="sxs-lookup"><span data-stu-id="d4c93-125">**Folder.Move()**</span></span> <br/> |
|<span data-ttu-id="d4c93-126">[CopyFolder 操作](http://msdn.microsoft.com/library/c7ea0d68-9793-4144-b378-d99536776db9%28Office.15%29.aspx)<sup>2</sup></span><span class="sxs-lookup"><span data-stu-id="d4c93-126">[CopyFolder operation](http://msdn.microsoft.com/library/c7ea0d68-9793-4144-b378-d99536776db9%28Office.15%29.aspx)<sup>2</sup></span></span> <br/> |<span data-ttu-id="d4c93-127">**Folder.Copy()**</span><span class="sxs-lookup"><span data-stu-id="d4c93-127">**Folder.Copy()**</span></span> <br/> |
|[<span data-ttu-id="d4c93-128">GetFolder Operation</span><span class="sxs-lookup"><span data-stu-id="d4c93-128">GetFolder operation</span></span>](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |<span data-ttu-id="d4c93-129">**Folder.Bind()**</span><span class="sxs-lookup"><span data-stu-id="d4c93-129">**Folder.Bind()**</span></span> <br/> |
|<span data-ttu-id="d4c93-130">[EmptyFolder 操作](http://msdn.microsoft.com/library/98161486-e2f2-480f-8d5d-708ba81b208a%28Office.15%29.aspx)<sup>3</sup></span><span class="sxs-lookup"><span data-stu-id="d4c93-130">[EmptyFolder operation](http://msdn.microsoft.com/library/98161486-e2f2-480f-8d5d-708ba81b208a%28Office.15%29.aspx)<sup>3</sup></span></span> <br/> |<span data-ttu-id="d4c93-131">**Folder.Empty()**</span><span class="sxs-lookup"><span data-stu-id="d4c93-131">**Folder.Empty()**</span></span> <br/> |
|[<span data-ttu-id="d4c93-132">FindFolder Operation</span><span class="sxs-lookup"><span data-stu-id="d4c93-132">FindFolder operation</span></span>](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |<span data-ttu-id="d4c93-133">**ExchangeService.FindFolders()**</span><span class="sxs-lookup"><span data-stu-id="d4c93-133">**ExchangeService.FindFolders()**</span></span> <br/> <span data-ttu-id="d4c93-134">**Folder.FindFolders()**</span><span class="sxs-lookup"><span data-stu-id="d4c93-134">**Folder.FindFolders()**</span></span> <br/> |
|[<span data-ttu-id="d4c93-135">CreateItem 操作</span><span class="sxs-lookup"><span data-stu-id="d4c93-135">CreateItem operation</span></span>](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> |<span data-ttu-id="d4c93-136">**Item.Save()**</span><span class="sxs-lookup"><span data-stu-id="d4c93-136">**Item.Save()**</span></span> <br/> |
|[<span data-ttu-id="d4c93-137">MoveItem 操作</span><span class="sxs-lookup"><span data-stu-id="d4c93-137">MoveItem operation</span></span>](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> |<span data-ttu-id="d4c93-138">**Item.Move()**</span><span class="sxs-lookup"><span data-stu-id="d4c93-138">**Item.Move()**</span></span> <br/> |
|[<span data-ttu-id="d4c93-139">CopyItem 操作</span><span class="sxs-lookup"><span data-stu-id="d4c93-139">CopyItem operation</span></span>](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |<span data-ttu-id="d4c93-140">**Item.Copy()**</span><span class="sxs-lookup"><span data-stu-id="d4c93-140">**Item.Copy()**</span></span> <br/> |
|[<span data-ttu-id="d4c93-141">UpdateItem 操作</span><span class="sxs-lookup"><span data-stu-id="d4c93-141">UpdateItem operation</span></span>](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |<span data-ttu-id="d4c93-142">**Item.Update()**</span><span class="sxs-lookup"><span data-stu-id="d4c93-142">**Item.Update()**</span></span> <br/> |
|[<span data-ttu-id="d4c93-143">删除项操作</span><span class="sxs-lookup"><span data-stu-id="d4c93-143">DeleteItem operation</span></span>](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |<span data-ttu-id="d4c93-144">**Item.Delete()**</span><span class="sxs-lookup"><span data-stu-id="d4c93-144">**Item.Delete()**</span></span> <br/> |
|<span data-ttu-id="d4c93-145">[FindItem 操作](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)<sup>4</sup></span><span class="sxs-lookup"><span data-stu-id="d4c93-145">[FindItem operation](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)<sup>4</sup></span></span> <br/> |<span data-ttu-id="d4c93-146">**ExchangeService.FindItems()**</span><span class="sxs-lookup"><span data-stu-id="d4c93-146">**ExchangeService.FindItems()**</span></span> <br/> <span data-ttu-id="d4c93-147">**Folder.FindItems()**</span><span class="sxs-lookup"><span data-stu-id="d4c93-147">**Folder.FindItems()**</span></span> <br/> |
|[<span data-ttu-id="d4c93-148">GetItem 操作</span><span class="sxs-lookup"><span data-stu-id="d4c93-148">GetItem operation</span></span>](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |<span data-ttu-id="d4c93-149">**Item.Bind()**</span><span class="sxs-lookup"><span data-stu-id="d4c93-149">**Item.Bind()**</span></span> <br/> |
|<span data-ttu-id="d4c93-150">[ConvertId 操作](http://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx)<sup>5</sup></span><span class="sxs-lookup"><span data-stu-id="d4c93-150">[ConvertId operation](http://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx)<sup>5</sup></span></span> <br/> |<span data-ttu-id="d4c93-151">**ExchangeService.ConvertId()**</span><span class="sxs-lookup"><span data-stu-id="d4c93-151">**ExchangeService.ConvertId()**</span></span> <br/> <span data-ttu-id="d4c93-152">**ExchangeService.ConvertIds()**</span><span class="sxs-lookup"><span data-stu-id="d4c93-152">**ExchangeService.ConvertIds()**</span></span> <br/> |
   
<span data-ttu-id="d4c93-153"><sup>1</sup>公用文件夹和专用文件夹之间移动文件夹不是 Exchange 开头 Exchange 2013 版本中可用。</span><span class="sxs-lookup"><span data-stu-id="d4c93-153"><sup>1</sup> Moving folders between a public folder and private folder is not available in versions of Exchange starting with Exchange 2013.</span></span> 
  
<span data-ttu-id="d4c93-154"><sup>2</sup>此操作仅适用于 Exchange Server 2007 和 Exchange Server 2010 中的公用文件夹。</span><span class="sxs-lookup"><span data-stu-id="d4c93-154"><sup>2</sup> This operation is only applicable to public folders in Exchange Server 2007 and Exchange Server 2010.</span></span> 
  
<span data-ttu-id="d4c93-155"><sup>3</sup>此操作仅适用于公用文件夹在 Exchange 2010。</span><span class="sxs-lookup"><span data-stu-id="d4c93-155"><sup>3</sup> This operation is only applicable to public folders in Exchange 2010.</span></span> 
  
<span data-ttu-id="d4c93-156"><sup>4</sup>开头 Exchange 2013 的 Exchange 版本中受支持的查询字符串搜索选项通过单个公用文件夹内的全文索引的搜索。</span><span class="sxs-lookup"><span data-stu-id="d4c93-156"><sup>4</sup> Full text indexed search within a single public folder by means of the QueryString search option is supported in versions of Exchange starting with Exchange 2013.</span></span> 
  
<span data-ttu-id="d4c93-157"><sup>5</sup> ConvertId 操作不能正确转换公用文件夹标识符从 EWS 标识符与存储标识符。</span><span class="sxs-lookup"><span data-stu-id="d4c93-157"><sup>5</sup> The ConvertId operation does not correctly convert public folder identifiers from the EWS identifier to the store identifier.</span></span> <span data-ttu-id="d4c93-158">您可以手动更新作为[解决方法](http://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx#bk_usingConvertId)返回的标识符。</span><span class="sxs-lookup"><span data-stu-id="d4c93-158">You can manually update the identifier that is returned as a [workaround](http://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx#bk_usingConvertId).</span></span>
  
<span data-ttu-id="d4c93-159">以下操作不受支持，或部分受支持的版本的 Exchange 开头 Exchange 2013 中的公用文件夹：</span><span class="sxs-lookup"><span data-stu-id="d4c93-159">The following operations are not supported, or are partially supported, for public folders in versions of Exchange starting with Exchange 2013:</span></span>
  
- <span data-ttu-id="d4c93-160">**CopyFolder**（不支持）。</span><span class="sxs-lookup"><span data-stu-id="d4c93-160">**CopyFolder** (not supported).</span></span> <span data-ttu-id="d4c93-161">您可以使用与**CopyItems**操作**CreateFolder**实现**CopyFolder**操作功能。</span><span class="sxs-lookup"><span data-stu-id="d4c93-161">You can use **CreateFolder** with the **CopyItems** operation to implement **CopyFolder** operation functionality.</span></span> 
    
- <span data-ttu-id="d4c93-162">**EmptyFolder**（不支持）。</span><span class="sxs-lookup"><span data-stu-id="d4c93-162">**EmptyFolder** (not supported).</span></span> <span data-ttu-id="d4c93-163">您可以使用**FindItem** **删除项**操作来实现**EmptyFolder**操作功能。</span><span class="sxs-lookup"><span data-stu-id="d4c93-163">You can use **FindItem** with the **DeleteItem** operation to implement **EmptyFolder** operation functionality.</span></span> 
    
- <span data-ttu-id="d4c93-164">**MoveFolder**（部分支持）。</span><span class="sxs-lookup"><span data-stu-id="d4c93-164">**MoveFolder** (partially supported).</span></span> <span data-ttu-id="d4c93-165">不能专用和公用文件夹之间移动文件夹。</span><span class="sxs-lookup"><span data-stu-id="d4c93-165">You cannot move folders between private and public folders.</span></span> <span data-ttu-id="d4c93-166">您可以在 Exchange 2007 中的专用和公用文件夹和 Exchange 2010 之间移动文件夹。</span><span class="sxs-lookup"><span data-stu-id="d4c93-166">You can move folders between private and public folders in Exchange 2007 and Exchange 2010.</span></span> <span data-ttu-id="d4c93-167">您可以在所有版本的 Exchange 公用文件夹内移动文件夹。</span><span class="sxs-lookup"><span data-stu-id="d4c93-167">You can move folders within a public folder in all versions of Exchange.</span></span> 
    
<span data-ttu-id="d4c93-168">EWS 和 EWS 托管 API 不支持以下功能的公用文件夹：</span><span class="sxs-lookup"><span data-stu-id="d4c93-168">EWS and the EWS Managed API do not support the following functionality for public folders:</span></span>
  
- <span data-ttu-id="d4c93-169">使用**SyncFolderHierarchy**。</span><span class="sxs-lookup"><span data-stu-id="d4c93-169">Using **SyncFolderHierarchy**.</span></span> <span data-ttu-id="d4c93-170">使用**FindFolder**、 **GetFolder**和**SyncFolderItems**操作同步公用文件夹邮箱中项目和文件夹。</span><span class="sxs-lookup"><span data-stu-id="d4c93-170">Use the **FindFolder**, **GetFolder** and **SyncFolderItems** operations to synchronize items and folders in a public folder mailbox.</span></span> 
    
- <span data-ttu-id="d4c93-171">公用文件夹层次结构的深度遍历搜索。</span><span class="sxs-lookup"><span data-stu-id="d4c93-171">Deep-traversal searches of a public folder hierarchy.</span></span> <span data-ttu-id="d4c93-172">使用递归**FindFolder**操作调用遍历公用文件夹层次结构。</span><span class="sxs-lookup"><span data-stu-id="d4c93-172">Use recursive **FindFolder** operation calls to traverse the public folder hierarchy.</span></span> 
    
- <span data-ttu-id="d4c93-173">使用**CreateFolderPath**操作创建公用文件夹的文件夹层次结构。</span><span class="sxs-lookup"><span data-stu-id="d4c93-173">Using the **CreateFolderPath** operation to create a folder hierarchy for public folders.</span></span> <span data-ttu-id="d4c93-174">您将需要使用不同的文件夹层次结构中的每个文件夹级别的**CreateFolder**操作时目标公用文件夹邮箱。</span><span class="sxs-lookup"><span data-stu-id="d4c93-174">You will need to use the **CreateFolder** operation for each folder level in a distinct folder hierarchy when you target a public folder mailbox.</span></span> 
    
- <span data-ttu-id="d4c93-175">使用**CreateItem** operation 保存发送的电子邮件的副本。</span><span class="sxs-lookup"><span data-stu-id="d4c93-175">Using the **CreateItem** operation to save copies of sent email messages.</span></span> <span data-ttu-id="d4c93-176">而是使用**MoveItem**操作移动到的公用文件夹的邮件的副本。</span><span class="sxs-lookup"><span data-stu-id="d4c93-176">Instead, use the **MoveItem** operation to move a copy of the message into a public folder.</span></span> 
    
## <a name="scenarios-for-using-ews-and-the-ews-managed-api-to-work-with-public-folders"></a><span data-ttu-id="d4c93-177">使用 EWS 和 EWS 托管 API 来使用公用文件夹方案</span><span class="sxs-lookup"><span data-stu-id="d4c93-177">Scenarios for using EWS and the EWS Managed API to work with public folders</span></span>
<span data-ttu-id="d4c93-178"><a name="bk_scenarios"> </a></span><span class="sxs-lookup"><span data-stu-id="d4c93-178"></span></span>

<span data-ttu-id="d4c93-179">公用文件夹启用 Exchange 邮箱用户的许多重要的方案。</span><span class="sxs-lookup"><span data-stu-id="d4c93-179">Public folders enable many important scenarios for Exchange mailbox users.</span></span> <span data-ttu-id="d4c93-180">您可以通过使用 EWS 和 EWS 托管 API 来实现自定义解决方案的访问和使用公用文件夹和及其内容为用户提供强大功能。</span><span class="sxs-lookup"><span data-stu-id="d4c93-180">You can empower users by using EWS and the EWS Managed API to implement custom solutions for accessing and using public folders and their contents.</span></span> 
  
### <a name="programmatically-access-email-messages-that-have-been-sent-to-distribution-lists"></a><span data-ttu-id="d4c93-181">以编程方式访问电子邮件已发送到通讯组列表</span><span class="sxs-lookup"><span data-stu-id="d4c93-181">Programmatically access email messages that have been sent to distribution lists</span></span>

<span data-ttu-id="d4c93-182">Exchange 邮箱用户可以使用公用文件夹来存储电子邮件发送到通讯组列表。</span><span class="sxs-lookup"><span data-stu-id="d4c93-182">Exchange mailbox users can use public folders to store email messages that are sent to distribution lists.</span></span> <span data-ttu-id="d4c93-183">这是一种将通讯组列表历史记录保存简便方法。</span><span class="sxs-lookup"><span data-stu-id="d4c93-183">This is a convenient way to save distribution list history.</span></span> <span data-ttu-id="d4c93-184">您可以使用 ews [FindItem 操作](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)或 EWS 托管 API 中的**ExchangeService.FindItems()** 和**Folder.FindItems()** 方法访问存储通讯组列表的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="d4c93-184">You can use the [FindItem operation](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) in EWS or the **ExchangeService.FindItems()** and **Folder.FindItems()** methods in the EWS Managed API to access stored distribution list email messages.</span></span> 
  
### <a name="share-important-email-messages-and-other-mailbox-items"></a><span data-ttu-id="d4c93-185">共享重要的电子邮件和其他邮箱项目</span><span class="sxs-lookup"><span data-stu-id="d4c93-185">Share important email messages and other mailbox items</span></span>

<span data-ttu-id="d4c93-186">邮箱用户可用作公用文件夹共享存储库的邮箱项目。</span><span class="sxs-lookup"><span data-stu-id="d4c93-186">Mailbox users can use public folders as a shared repository for mailbox items.</span></span> <span data-ttu-id="d4c93-187">组织中的不同用户可以通过使用公用文件夹共享重要的电子邮件或联系人。</span><span class="sxs-lookup"><span data-stu-id="d4c93-187">Different users in an organization can share important email messages or contacts by using public folders.</span></span> <span data-ttu-id="d4c93-188">EWS 可以提供这些共享的邮箱项目的访问权限。</span><span class="sxs-lookup"><span data-stu-id="d4c93-188">EWS can provide the access to these shared mailbox items.</span></span> <span data-ttu-id="d4c93-189">您可以使用 ews [MoveItem 操作](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx)或 EWS 托管 API 中的**Item.Move()** 方法和注销的公用文件夹移动电子邮件、 联系人和其他邮箱项目。</span><span class="sxs-lookup"><span data-stu-id="d4c93-189">You can use the [MoveItem operation](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) in EWS or the **Item.Move()** method in the EWS Managed API to move email messages, contacts, and other mailbox items into and out of a public folder.</span></span> 
  
### <a name="public-discussions-with-post-items"></a><span data-ttu-id="d4c93-190">公共公告项讨论</span><span class="sxs-lookup"><span data-stu-id="d4c93-190">Public discussions with post items</span></span>

<span data-ttu-id="d4c93-191">公用文件夹是公告项的一个方便的容器。</span><span class="sxs-lookup"><span data-stu-id="d4c93-191">Public folders are a convenient container for post items.</span></span> <span data-ttu-id="d4c93-192">公告项提供一种方式使用而无需发送电子邮件用户之间的线程的对话。</span><span class="sxs-lookup"><span data-stu-id="d4c93-192">Post items provide a way to use threaded conversations without having to send email messages between users.</span></span> <span data-ttu-id="d4c93-193">用户可以使用公用文件夹，并发布项目承载和维护组织中的不同的邮箱用户之间的线程的对话。</span><span class="sxs-lookup"><span data-stu-id="d4c93-193">Users can use public folders and post items to host and maintain threaded conversations between different mailbox users in an organization.</span></span> <span data-ttu-id="d4c93-194">这种方式，邮箱用户可以访问共享的使用投递项目，即使它们不是部分对话的对话历史记录。</span><span class="sxs-lookup"><span data-stu-id="d4c93-194">This way, mailbox users can access the shared history of a conversation that uses post items even if they were not part of the conversation.</span></span> <span data-ttu-id="d4c93-195">您可以使用 EWS 中的[CreateItem operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx)或 EWS 托管 API 中的**Item.Save()** 方法，以创建并发布的公用文件夹中存储的项目的响应。</span><span class="sxs-lookup"><span data-stu-id="d4c93-195">You can use the [CreateItem operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) in EWS or the **Item.Save()** method in the EWS Managed API to both create and respond to post items stored in a public folder.</span></span> 
  
## <a name="routing-public-folder-requests"></a><span data-ttu-id="d4c93-196">公用文件夹请求路由</span><span class="sxs-lookup"><span data-stu-id="d4c93-196">Routing public folder requests</span></span>
<span data-ttu-id="d4c93-197"><a name="bk_routing"> </a></span><span class="sxs-lookup"><span data-stu-id="d4c93-197"></span></span>

<span data-ttu-id="d4c93-198">公用文件夹内容可以存储在多个邮箱服务器上。</span><span class="sxs-lookup"><span data-stu-id="d4c93-198">Public folder content can be stored on multiple mailbox servers.</span></span> <span data-ttu-id="d4c93-199">公用文件夹层次结构可以存储上一个邮箱，而公用文件夹的内容存储在另一个。</span><span class="sxs-lookup"><span data-stu-id="d4c93-199">The public folder hierarchy can be stored on one mailbox, while the content for the public folder is stored on another.</span></span> <span data-ttu-id="d4c93-200">每个服务器可以为不同的邮箱服务器的请求信息的用户。</span><span class="sxs-lookup"><span data-stu-id="d4c93-200">And each of these servers can be different than the mailbox server for the user requesting the information.</span></span> <span data-ttu-id="d4c93-201">在这些情况下，务必要包含在您的公用文件夹请求接收有关公用文件夹的正确信息中的其他的 X AnchorMailbox 和 X PublicFolderMailbox 标头。</span><span class="sxs-lookup"><span data-stu-id="d4c93-201">In these situations, it's important to include the additional X-AnchorMailbox and X-PublicFolderMailbox headers in your public folder requests to receive accurate information about public folders.</span></span>
  
<span data-ttu-id="d4c93-202">X AnchorMailbox 和 X PublicFolderMailbox 的值可以有所不同具体取决于是否正在执行请求与文件夹层次结构或文件夹内容。</span><span class="sxs-lookup"><span data-stu-id="d4c93-202">The value for the X-AnchorMailbox and X-PublicFolderMailbox can differ depending on whether you're performing a request related to the folder hierarchy or the folder content.</span></span> <span data-ttu-id="d4c93-203">下表标识了哪些过程需遵循的每个 EWS 托管 API 方法或 EWS 操作。</span><span class="sxs-lookup"><span data-stu-id="d4c93-203">The following table identifies which procedure to follow for each EWS Managed API method or EWS operation.</span></span>
  
<span data-ttu-id="d4c93-204">**EWS 托管 API 方法和路由的公用文件夹请求的 EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="d4c93-204">**EWS Managed API methods and EWS operations for routing public folder requests**</span></span>

|<span data-ttu-id="d4c93-205">**当调用这些方法**</span><span class="sxs-lookup"><span data-stu-id="d4c93-205">**When calling these methods**</span></span>|<span data-ttu-id="d4c93-206">**调用这些操作时**</span><span class="sxs-lookup"><span data-stu-id="d4c93-206">**When calling these operations**</span></span>|<span data-ttu-id="d4c93-207">**使用此过程**</span><span class="sxs-lookup"><span data-stu-id="d4c93-207">**Use this procedure**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="d4c93-208">Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="d4c93-208">Folder.FindFolders</span></span>](http://msdn.microsoft.com/zh-cn/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="d4c93-209">Folder.Delete</span><span class="sxs-lookup"><span data-stu-id="d4c93-209">Folder.Delete</span></span>](http://msdn.microsoft.com/zh-cn/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="d4c93-210">Folder.Update</span><span class="sxs-lookup"><span data-stu-id="d4c93-210">Folder.Update</span></span>](http://msdn.microsoft.com/zh-cn/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="d4c93-211">Folder.Move</span><span class="sxs-lookup"><span data-stu-id="d4c93-211">Folder.Move</span></span>](http://msdn.microsoft.com/zh-cn/library/microsoft.exchange.webservices.data.folder.move%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="d4c93-212">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="d4c93-212">CreateFolder</span></span>](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> [<span data-ttu-id="d4c93-213">FindFolder</span><span class="sxs-lookup"><span data-stu-id="d4c93-213">FindFolder</span></span>](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> [<span data-ttu-id="d4c93-214">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="d4c93-214">DeleteFolder</span></span>](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> [<span data-ttu-id="d4c93-215">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="d4c93-215">UpdateFolder</span></span>](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> [<span data-ttu-id="d4c93-216">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="d4c93-216">MoveFolder</span></span>](http://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <br/> |<span data-ttu-id="d4c93-217">公用文件夹层次结构请求路由</span><span class="sxs-lookup"><span data-stu-id="d4c93-217">Routing public folder hierarchy requests</span></span>  <br/> |
|[<span data-ttu-id="d4c93-218">Item.Bind</span><span class="sxs-lookup"><span data-stu-id="d4c93-218">Item.Bind</span></span>](http://msdn.microsoft.com/zh-cn/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="d4c93-219">Item.Update</span><span class="sxs-lookup"><span data-stu-id="d4c93-219">Item.Update</span></span>](http://msdn.microsoft.com/zh-cn/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="d4c93-220">Item.Copy</span><span class="sxs-lookup"><span data-stu-id="d4c93-220">Item.Copy</span></span>](http://msdn.microsoft.com/zh-cn/library/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="d4c93-221">Item.Move</span><span class="sxs-lookup"><span data-stu-id="d4c93-221">Item.Move</span></span>](http://msdn.microsoft.com/zh-cn/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="d4c93-222">Item.Delete</span><span class="sxs-lookup"><span data-stu-id="d4c93-222">Item.Delete</span></span>](http://msdn.microsoft.com/zh-cn/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="d4c93-223">Folder.Bind</span><span class="sxs-lookup"><span data-stu-id="d4c93-223">Folder.Bind</span></span>](http://msdn.microsoft.com/zh-cn/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="d4c93-224">Folder.FindItems</span><span class="sxs-lookup"><span data-stu-id="d4c93-224">Folder.FindItems</span></span>](http://msdn.microsoft.com/zh-cn/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="d4c93-225">CreateItem</span><span class="sxs-lookup"><span data-stu-id="d4c93-225">CreateItem</span></span>](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> [<span data-ttu-id="d4c93-226">GetItem</span><span class="sxs-lookup"><span data-stu-id="d4c93-226">GetItem</span></span>](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> [<span data-ttu-id="d4c93-227">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="d4c93-227">UpdateItem</span></span>](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> [<span data-ttu-id="d4c93-228">CopyItem</span><span class="sxs-lookup"><span data-stu-id="d4c93-228">CopyItem</span></span>](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> [<span data-ttu-id="d4c93-229">MoveItem</span><span class="sxs-lookup"><span data-stu-id="d4c93-229">MoveItem</span></span>](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> [<span data-ttu-id="d4c93-230">删除项</span><span class="sxs-lookup"><span data-stu-id="d4c93-230">DeleteItem</span></span>](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> [<span data-ttu-id="d4c93-231">GetFolder</span><span class="sxs-lookup"><span data-stu-id="d4c93-231">GetFolder</span></span>](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> [<span data-ttu-id="d4c93-232">FindItem</span><span class="sxs-lookup"><span data-stu-id="d4c93-232">FindItem</span></span>](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |<span data-ttu-id="d4c93-233">公用文件夹内容请求路由</span><span class="sxs-lookup"><span data-stu-id="d4c93-233">Routing public folder content requests</span></span>  <br/> |
   
## <a name="version-differences"></a><span data-ttu-id="d4c93-234">版本差异</span><span class="sxs-lookup"><span data-stu-id="d4c93-234">Version differences</span></span>
<span data-ttu-id="d4c93-235"><a name="VersionDifferences"> </a></span><span class="sxs-lookup"><span data-stu-id="d4c93-235"></span></span>

<span data-ttu-id="d4c93-236">在 Exchange 2007 和 Exchange 2010 中，按预期的 EWS 标识符的公用文件夹标识符转换为存储标识符时，将工作**ConvertId**操作。</span><span class="sxs-lookup"><span data-stu-id="d4c93-236">In Exchange 2007 and Exchange 2010, the **ConvertId** operation works as expected when converting public folder identifiers from the EWS identifier to the store identifier.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="d4c93-237">另请参阅</span><span class="sxs-lookup"><span data-stu-id="d4c93-237">See also</span></span>


- [<span data-ttu-id="d4c93-238">开发 Exchange Web 服务客户端</span><span class="sxs-lookup"><span data-stu-id="d4c93-238">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="d4c93-239">Start using web services in Exchange</span><span class="sxs-lookup"><span data-stu-id="d4c93-239">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
    
- [<span data-ttu-id="d4c93-240">公用文件夹限制</span><span class="sxs-lookup"><span data-stu-id="d4c93-240">Public folder limits</span></span>](http://technet.microsoft.com/zh-cn/library/dn594582%28v=exchg.150%29.aspx)
    
- [<span data-ttu-id="d4c93-241">常见问题： 公用文件夹</span><span class="sxs-lookup"><span data-stu-id="d4c93-241">FAQ: Public Folders</span></span>](http://technet.microsoft.com/zh-cn/library/jj552408.aspx)
    
- [<span data-ttu-id="d4c93-242">公用文件夹过程</span><span class="sxs-lookup"><span data-stu-id="d4c93-242">Public Folder Procedures</span></span>](http://technet.microsoft.com/zh-cn/library/jj657481.aspx)
    
