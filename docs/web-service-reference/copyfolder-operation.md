---
title: CopyFolder 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyFolder
api_type:
- schema
ms.assetid: c7ea0d68-9793-4144-b378-d99536776db9
description: CopyFolder 操作将复制邮箱中的文件夹。
ms.openlocfilehash: a83444ff0927a3c8fe075c79d44d02357a737773
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/25/2018
ms.locfileid: "19753603"
---
# <a name="copyfolder-operation"></a><span data-ttu-id="2bae0-103">CopyFolder 操作</span><span class="sxs-lookup"><span data-stu-id="2bae0-103">CopyFolder operation</span></span>

<span data-ttu-id="2bae0-104">CopyFolder 操作将复制邮箱中的文件夹。</span><span class="sxs-lookup"><span data-stu-id="2bae0-104">The CopyFolder operation copies folders in a mailbox.</span></span>
  
## <a name="using-the-copyfolder-operation"></a><span data-ttu-id="2bae0-105">使用 CopyFolder 操作</span><span class="sxs-lookup"><span data-stu-id="2bae0-105">Using the CopyFolder operation</span></span>

<span data-ttu-id="2bae0-106">CopyFolder 操作类似于[MoveFolder 操作](movefolder-operation.md)。</span><span class="sxs-lookup"><span data-stu-id="2bae0-106">The CopyFolder operation is similar to the [MoveFolder operation](movefolder-operation.md).</span></span> <span data-ttu-id="2bae0-107">它将复制标识的文件夹，并返回的**Id**和**更改密钥**的复制的文件夹。</span><span class="sxs-lookup"><span data-stu-id="2bae0-107">It copies identified folders and returns the **Id** and **ChangeKey** of the copied folders.</span></span> 
  
## <a name="copyfolder-request-example"></a><span data-ttu-id="2bae0-108">CopyFolder 请求示例</span><span class="sxs-lookup"><span data-stu-id="2bae0-108">CopyFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="2bae0-109">说明</span><span class="sxs-lookup"><span data-stu-id="2bae0-109">Description</span></span>

<span data-ttu-id="2bae0-110">CopyFolder 请求的下面的示例演示如何将文件夹复制到收件箱文件夹。</span><span class="sxs-lookup"><span data-stu-id="2bae0-110">The following example of a CopyFolder request shows how to copy folders into the Inbox folder.</span></span>
  
> [!NOTE]
> <span data-ttu-id="2bae0-111">为便于阅读缩短了[文件夹 Id](folderid.md)元素的**Id**属性的值。</span><span class="sxs-lookup"><span data-stu-id="2bae0-111">The value of the **Id** attribute of the [FolderId](folderid.md) element has been shortened for readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="2bae0-112">代码</span><span class="sxs-lookup"><span data-stu-id="2bae0-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CopyFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ToFolderId>
        <t:DistinguishedFolderId Id="inbox"/>
      </ToFolderId>
      <FolderIds>
        <t:FolderId Id="AS4A=" ChangeKey="fsVU4=="/>
        <t:FolderId Id="AS4AU=" ChangeKey="fsVU4o=="/>
      </FolderIds>
    </CopyFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="2bae0-113">注释</span><span class="sxs-lookup"><span data-stu-id="2bae0-113">Comments</span></span>

<span data-ttu-id="2bae0-114">可通过[DistinguishedFolderId](distinguishedfolderid.md)元素或在是[ToFolderId](tofolderid.md)中使用的[文件夹 Id](folderid.md)元素或[FolderIds](folderids.md)元素标识文件夹。</span><span class="sxs-lookup"><span data-stu-id="2bae0-114">Folders can be identified by either the [DistinguishedFolderId](distinguishedfolderid.md) element or the [FolderId](folderid.md) element for use in either the [ToFolderId](tofolderid.md) or the [FolderIds](folderids.md) elements.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="2bae0-115">请求元素</span><span class="sxs-lookup"><span data-stu-id="2bae0-115">Request elements</span></span>

<span data-ttu-id="2bae0-116">请求中使用以下元素：</span><span class="sxs-lookup"><span data-stu-id="2bae0-116">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="2bae0-117">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="2bae0-117">CopyFolder</span></span>](copyfolder.md)
    
- [<span data-ttu-id="2bae0-118">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="2bae0-118">ToFolderId</span></span>](tofolderid.md)
    
- [<span data-ttu-id="2bae0-119">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="2bae0-119">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="2bae0-120">FolderIds</span><span class="sxs-lookup"><span data-stu-id="2bae0-120">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="2bae0-121">文件夹 Id</span><span class="sxs-lookup"><span data-stu-id="2bae0-121">FolderId</span></span>](folderid.md)
    
> [!NOTE]
> <span data-ttu-id="2bae0-122">描述此元素的架构位于正在运行 MicrosoftExchange Server 2007 的计算机（已安装客户端访问服务器角色）的 EWS 虚拟目录中。</span><span class="sxs-lookup"><span data-stu-id="2bae0-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="2bae0-123">若要查找的请求邮件 CopyFolder 操作的其他选项，浏览的架构层次结构。</span><span class="sxs-lookup"><span data-stu-id="2bae0-123">To find other options for the request message of the CopyFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="2bae0-124">启动[CopyFolder](copyfolder.md)元素。</span><span class="sxs-lookup"><span data-stu-id="2bae0-124">Start at the [CopyFolder](copyfolder.md) element.</span></span> 
  
## <a name="successful-copyfolder-response"></a><span data-ttu-id="2bae0-125">成功的 CopyFolder 响应</span><span class="sxs-lookup"><span data-stu-id="2bae0-125">Successful CopyFolder response</span></span>

### <a name="description"></a><span data-ttu-id="2bae0-126">说明</span><span class="sxs-lookup"><span data-stu-id="2bae0-126">Description</span></span>

<span data-ttu-id="2bae0-127">下面的示例演示对 CopyFolder 请求成功响应。</span><span class="sxs-lookup"><span data-stu-id="2bae0-127">The following example shows a successful response to the CopyFolder request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="2bae0-128">已缩短文件夹 ID 和更改密钥，以保留可读性。</span><span class="sxs-lookup"><span data-stu-id="2bae0-128">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="2bae0-129">代码</span><span class="sxs-lookup"><span data-stu-id="2bae0-129">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CopyFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AS4AUn=" ChangeKey="fsVU4o==" />
            </t:Folder>
          </m:Folders>
        </m:CopyFolderResponseMessage>
      </m:ResponseMessages>
    </CopyFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comment"></a><span data-ttu-id="2bae0-130">Comment</span><span class="sxs-lookup"><span data-stu-id="2bae0-130">Comment</span></span>

<span data-ttu-id="2bae0-131">响应中返回的[文件夹 Id](folderid.md)元素表示已复制新的文件夹位置的文件夹。</span><span class="sxs-lookup"><span data-stu-id="2bae0-131">The [FolderId](folderid.md) element that is returned in the response represents the folder that was copied in the new folder location.</span></span> 
  
### <a name="response-elements"></a><span data-ttu-id="2bae0-132">响应元素</span><span class="sxs-lookup"><span data-stu-id="2bae0-132">Response elements</span></span>

<span data-ttu-id="2bae0-133">在响应中使用以下元素：</span><span class="sxs-lookup"><span data-stu-id="2bae0-133">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="2bae0-134">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="2bae0-134">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="2bae0-135">CopyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="2bae0-135">CopyFolderResponse</span></span>](copyfolderresponse.md)
    
- [<span data-ttu-id="2bae0-136">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="2bae0-136">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="2bae0-137">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="2bae0-137">CopyFolderResponseMessage</span></span>](copyfolderresponsemessage.md)
    
- [<span data-ttu-id="2bae0-138">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="2bae0-138">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="2bae0-139">Folders</span><span class="sxs-lookup"><span data-stu-id="2bae0-139">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="2bae0-140">Folder</span><span class="sxs-lookup"><span data-stu-id="2bae0-140">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="2bae0-141">文件夹 Id</span><span class="sxs-lookup"><span data-stu-id="2bae0-141">FolderId</span></span>](folderid.md)
    
<span data-ttu-id="2bae0-142">若要查找的响应消息 CopyFolder 操作的其他选项，浏览的架构层次结构。</span><span class="sxs-lookup"><span data-stu-id="2bae0-142">To find other options for the response message of the CopyFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="2bae0-143">启动[CopyFolderResponse](copyfolderresponse.md)元素。</span><span class="sxs-lookup"><span data-stu-id="2bae0-143">Start at the [CopyFolderResponse](copyfolderresponse.md) element.</span></span> 
  
## <a name="copyfolder-error-response"></a><span data-ttu-id="2bae0-144">CopyFolder 错误响应</span><span class="sxs-lookup"><span data-stu-id="2bae0-144">CopyFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="2bae0-145">说明</span><span class="sxs-lookup"><span data-stu-id="2bae0-145">Description</span></span>

<span data-ttu-id="2bae0-146">下面的示例演示对 CopyFolder 请求错误响应。</span><span class="sxs-lookup"><span data-stu-id="2bae0-146">The following example shows an error response to a CopyFolder request.</span></span> <span data-ttu-id="2bae0-147">因为已存在同名的显示文件夹，将发生错误。</span><span class="sxs-lookup"><span data-stu-id="2bae0-147">The error occurred because a folder with the same display name already exists.</span></span>
  
### <a name="code"></a><span data-ttu-id="2bae0-148">代码</span><span class="sxs-lookup"><span data-stu-id="2bae0-148">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CopyFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyFolderResponseMessage ResponseClass="Error">
          <m:MessageText>The move or copy operation failed.</m:MessageText>
          <m:ResponseCode>ErrorMoveCopyFailed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:CopyFolderResponseMessage>
      </m:ResponseMessages>
    </CopyFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="2bae0-149">错误响应元素</span><span class="sxs-lookup"><span data-stu-id="2bae0-149">Error response elements</span></span>

<span data-ttu-id="2bae0-150">错误响应中使用以下元素：</span><span class="sxs-lookup"><span data-stu-id="2bae0-150">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="2bae0-151">CopyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="2bae0-151">CopyFolderResponse</span></span>](copyfolderresponse.md)
    
- [<span data-ttu-id="2bae0-152">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="2bae0-152">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="2bae0-153">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="2bae0-153">CopyFolderResponseMessage</span></span>](copyfolderresponsemessage.md)
    
- [<span data-ttu-id="2bae0-154">MessageText</span><span class="sxs-lookup"><span data-stu-id="2bae0-154">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="2bae0-155">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="2bae0-155">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="2bae0-156">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="2bae0-156">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="2bae0-157">Folders</span><span class="sxs-lookup"><span data-stu-id="2bae0-157">Folders</span></span>](folders-ex15websvcsotherref.md)
    
<span data-ttu-id="2bae0-158">若要查找错误响应消息的 CopyFolder 操作的其他选项，浏览的架构层次结构。</span><span class="sxs-lookup"><span data-stu-id="2bae0-158">To find other options for the error response message of the CopyFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="2bae0-159">启动[CopyFolderResponse](copyfolderresponse.md)元素。</span><span class="sxs-lookup"><span data-stu-id="2bae0-159">Start at the [CopyFolderResponse](copyfolderresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="2bae0-160">另请参阅</span><span class="sxs-lookup"><span data-stu-id="2bae0-160">See also</span></span>

- [<span data-ttu-id="2bae0-161">MoveFolder 操作</span><span class="sxs-lookup"><span data-stu-id="2bae0-161">MoveFolder operation</span></span>](movefolder-operation.md)
- [<span data-ttu-id="2bae0-162">在交换 EWS XML 元素</span><span class="sxs-lookup"><span data-stu-id="2bae0-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
