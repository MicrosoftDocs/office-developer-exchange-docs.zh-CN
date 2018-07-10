---
title: DescriptiveLinkKey
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DescriptiveLinkKey
api_type:
- schema
ms.assetid: f7f36749-00f3-4915-b17c-e3caa0af6e67
description: DescriptiveLinkKey 元素是当前未使用，并且保留以供将来使用。 它包含的值为 0。
ms.openlocfilehash: c917f401c0954a68ddce1226b522d54c87502462
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/25/2018
ms.locfileid: "19753852"
---
# <a name="descriptivelinkkey"></a><span data-ttu-id="76fb0-104">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="76fb0-104">DescriptiveLinkKey</span></span>

<span data-ttu-id="76fb0-105">**DescriptiveLinkKey**元素是当前未使用，并且保留以供将来使用。</span><span class="sxs-lookup"><span data-stu-id="76fb0-105">The **DescriptiveLinkKey** element is currently unused and is reserved for future use.</span></span> <span data-ttu-id="76fb0-106">它包含的值为 0。</span><span class="sxs-lookup"><span data-stu-id="76fb0-106">It contains a value of 0.</span></span> 
  
```XML
<DescriptiveLinkKey/>
```

 <span data-ttu-id="76fb0-107">**int**</span><span class="sxs-lookup"><span data-stu-id="76fb0-107">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="76fb0-108">属性和元素</span><span class="sxs-lookup"><span data-stu-id="76fb0-108">Attributes and elements</span></span>

<span data-ttu-id="76fb0-109">如下章节中介绍了属性、子元素和父元素。</span><span class="sxs-lookup"><span data-stu-id="76fb0-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="76fb0-110">属性</span><span class="sxs-lookup"><span data-stu-id="76fb0-110">Attributes</span></span>

<span data-ttu-id="76fb0-111">无。</span><span class="sxs-lookup"><span data-stu-id="76fb0-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="76fb0-112">子元素</span><span class="sxs-lookup"><span data-stu-id="76fb0-112">Child elements</span></span>

<span data-ttu-id="76fb0-113">无。</span><span class="sxs-lookup"><span data-stu-id="76fb0-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="76fb0-114">父元素</span><span class="sxs-lookup"><span data-stu-id="76fb0-114">Parent elements</span></span>

|<span data-ttu-id="76fb0-115">**元素**</span><span class="sxs-lookup"><span data-stu-id="76fb0-115">**Element**</span></span>|<span data-ttu-id="76fb0-116">**说明**</span><span class="sxs-lookup"><span data-stu-id="76fb0-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="76fb0-117">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-117">ResponseMessage</span></span>](responsemessage.md) <br/> | <span data-ttu-id="76fb0-118">提供有关的响应状态的描述性信息。</span><span class="sxs-lookup"><span data-stu-id="76fb0-118">Provides descriptive information about the response status.</span></span>  <br/><br/><span data-ttu-id="76fb0-119">以下是一些可能的 XPath 表达式到此元素：</span><span class="sxs-lookup"><span data-stu-id="76fb0-119">The following are some possible XPath expressions to this element:</span></span><br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/ResponseMessage` <br/><br/>`/GetUserAvailabilityResponse/SuggestionsResponse/ResponseMessage` <br/><br/>`/SetUserOofSettingsResponse/ResponseMessage` <br/><br/>`/GetUserOofSettingsResponse/ResponseMessage` <br/> |
|[<span data-ttu-id="76fb0-120">DeleteItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-120">DeleteItemResponseMessage</span></span>](deleteitemresponsemessage.md) <br/> |<span data-ttu-id="76fb0-121">包含状态和单个**删除项**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-121">Contains the status and result of a single **DeleteItem** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-122">SendItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-122">SendItemResponseMessage</span></span>](senditemresponsemessage.md) <br/> |<span data-ttu-id="76fb0-123">包含状态和单个**SendItem**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-123">Contains the status and result of a single **SendItem** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-124">DeleteFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-124">DeleteFolderResponseMessage</span></span>](deletefolderresponsemessage.md) <br/> |<span data-ttu-id="76fb0-125">包含状态和单个**DeleteFolder**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-125">Contains the status and result of a single **DeleteFolder** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-126">DeleteAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-126">DeleteAttachmentResponseMessage</span></span>](deleteattachmentresponsemessage.md) <br/> |<span data-ttu-id="76fb0-127">包含状态和单个**DeleteAttachment**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-127">Contains the status and result of a single **DeleteAttachment** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-128">UnsubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-128">UnsubscribeResponseMessage</span></span>](unsubscriberesponsemessage.md) <br/> |<span data-ttu-id="76fb0-129">包含状态和单个**取消订阅**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-129">Contains the status and result of a single **Unsubscribe** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-130">CreateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-130">CreateFolderResponseMessage</span></span>](createfolderresponsemessage.md) <br/> |<span data-ttu-id="76fb0-131">包含状态和单个**CreateFolder**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-131">Contains the status and result of a single **CreateFolder** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-132">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-132">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md) <br/> |<span data-ttu-id="76fb0-133">包含状态和单个**GetFolder**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-133">Contains the status and result of a single **GetFolder** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-134">UpdateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-134">UpdateFolderResponseMessage</span></span>](updatefolderresponsemessage.md) <br/> |<span data-ttu-id="76fb0-135">包含状态和单个**UpdateFolder**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-135">Contains the status and result of a single **UpdateFolder** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-136">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-136">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md) <br/> |<span data-ttu-id="76fb0-137">包含状态和单个**MoveFolder**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-137">Contains the status and result of a single **MoveFolder** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-138">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-138">CopyFolderResponseMessage</span></span>](copyfolderresponsemessage.md) <br/> |<span data-ttu-id="76fb0-139">包含状态和单个**CopyFolder**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-139">Contains the status and result of a single **CopyFolder** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-140">CreateManagedFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-140">CreateManagedFolderResponseMessage</span></span>](createmanagedfolderresponsemessage.md) <br/> |<span data-ttu-id="76fb0-141">包含状态和单个**CreateManagedFolder**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-141">Contains the status and result of a single **CreateManagedFolder** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-142">FindFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-142">FindFolderResponseMessage</span></span>](findfolderresponsemessage.md) <br/> |<span data-ttu-id="76fb0-143">包含状态和单个**FindFolder**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-143">Contains the status and result of a single **FindFolder** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-144">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-144">CreateItemResponseMessage</span></span>](createitemresponsemessage.md) <br/> |<span data-ttu-id="76fb0-145">包含状态和单个**CreateItem**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-145">Contains the status and result of a single **CreateItem** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-146">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-146">GetItemResponseMessage</span></span>](getitemresponsemessage.md) <br/> |<span data-ttu-id="76fb0-147">包含状态和单个**GetItem**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-147">Contains the status and result of a single **GetItem** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-148">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-148">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md) <br/> |<span data-ttu-id="76fb0-149">包含状态和单个**UpdateItem**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-149">Contains the status and result of a single **UpdateItem** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-150">MoveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-150">MoveItemResponseMessage</span></span>](moveitemresponsemessage.md) <br/> |<span data-ttu-id="76fb0-151">包含状态和单个**MoveItem**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-151">Contains the status and result of a single **MoveItem** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-152">CopyItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-152">CopyItemResponseMessage</span></span>](copyitemresponsemessage.md) <br/> |<span data-ttu-id="76fb0-153">包含状态和单个**CopyItem**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-153">Contains the status and result of a single **CopyItem** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-154">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-154">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md) <br/> |<span data-ttu-id="76fb0-155">包含状态和单个**CreateAttachment**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-155">Contains the status and result of a single **CreateAttachment** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-156">GetAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-156">GetAttachmentResponseMessage</span></span>](getattachmentresponsemessage.md) <br/> |<span data-ttu-id="76fb0-157">包含状态和单个**GetAttachment**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-157">Contains the status and result of a single **GetAttachment** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-158">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-158">FindItemResponseMessage</span></span>](finditemresponsemessage.md) <br/> |<span data-ttu-id="76fb0-159">包含状态和单个**FindItem**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-159">Contains the status and result of a single **FindItem** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-160">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-160">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md) <br/> |<span data-ttu-id="76fb0-161">包含状态和**ResolveNames**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-161">Contains the status and result of a **ResolveNames** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-162">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-162">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md) <br/> |<span data-ttu-id="76fb0-163">包含状态和单个**ExpandDL**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-163">Contains the status and result of a single **ExpandDL** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-164">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-164">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md) <br/> |<span data-ttu-id="76fb0-165">包含状态和单个**Subscribe**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-165">Contains the status and result of a single **Subscribe** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-166">GetEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-166">GetEventsResponseMessage</span></span>](geteventsresponsemessage.md) <br/> |<span data-ttu-id="76fb0-167">包含状态和单个**GetEvents**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-167">Contains the status and result of a single **GetEvents** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-168">SendNotificationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-168">SendNotificationResponseMessage</span></span>](sendnotificationresponsemessage.md) <br/> |<span data-ttu-id="76fb0-169">包含状态和单个**SendNotification**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-169">Contains the status and result of a single **SendNotification** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-170">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-170">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md) <br/> |<span data-ttu-id="76fb0-171">包含状态和**SyncFolderHierarchy**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-171">Contains the status and result of a **SyncFolderHierarchy** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-172">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-172">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md) <br/> |<span data-ttu-id="76fb0-173">包含状态和**SyncFolderItems**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-173">Contains the status and result of a **SyncFolderItems** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-174">ConvertIdResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-174">ConvertIdResponseMessage</span></span>](convertidresponsemessage.md) <br/> |<span data-ttu-id="76fb0-175">包含状态和**ConvertId**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-175">Contains the status and result of a **ConvertId** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-176">AddDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="76fb0-176">AddDelegateResponse</span></span>](adddelegateresponse.md) <br/> |<span data-ttu-id="76fb0-177">包含状态和**AddDelegate**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-177">Contains the status and result of an **AddDelegate** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-178">GetServerTimeZonesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-178">GetServerTimeZonesResponseMessage</span></span>](getservertimezonesresponsemessage.md) <br/> |<span data-ttu-id="76fb0-179">包含状态和**GetServerTimeZones**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-179">Contains the status and result of a **GetServerTimeZones** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-180">GetSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-180">GetSharingFolderResponseMessage</span></span>](getsharingfolderresponsemessage.md) <br/> |<span data-ttu-id="76fb0-181">包含状态和**GetSharingFolder**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-181">Contains the status and result of a **GetSharingFolder** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-182">GetSharingFolderResponse</span><span class="sxs-lookup"><span data-stu-id="76fb0-182">GetSharingFolderResponse</span></span>](getsharingfolderresponse.md) <br/> |<span data-ttu-id="76fb0-183">定义**GetSharingFolder**请求的响应。</span><span class="sxs-lookup"><span data-stu-id="76fb0-183">Defines a response to a **GetSharingFolder** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-184">GetSharingMetadataResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-184">GetSharingMetadataResponseMessage</span></span>](getsharingmetadataresponsemessage.md) <br/> |<span data-ttu-id="76fb0-185">包含状态和**GetSharingMetadata**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-185">Contains the status and result of a **GetSharingMetadata** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-186">GetSharingMetadataResponse</span><span class="sxs-lookup"><span data-stu-id="76fb0-186">GetSharingMetadataResponse</span></span>](getsharingmetadataresponse.md) <br/> |<span data-ttu-id="76fb0-187">定义**GetSharingMetadata**请求的响应。</span><span class="sxs-lookup"><span data-stu-id="76fb0-187">Defines a response to a **GetSharingMetadata** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-188">RefreshSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-188">RefreshSharingFolderResponseMessage</span></span>](refreshsharingfolderresponsemessage.md) <br/> |<span data-ttu-id="76fb0-189">包含状态和**RefreshSharingFolder**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-189">Contains the status and result of a **RefreshSharingFolder** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-190">RefreshSharingFolderResponse</span><span class="sxs-lookup"><span data-stu-id="76fb0-190">RefreshSharingFolderResponse</span></span>](refreshsharingfolderresponse.md) <br/> |<span data-ttu-id="76fb0-191">定义**RefreshSharingFolder**请求的响应。</span><span class="sxs-lookup"><span data-stu-id="76fb0-191">Defines a response to a **RefreshSharingFolder** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-192">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="76fb0-192">FindConversationResponse</span></span>](findconversationresponse.md) <br/> |<span data-ttu-id="76fb0-193">包含状态和**FindConversation**响应的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-193">Contains the status and results of a **FindConversation** response.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-194">EmptyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-194">EmptyFolderResponseMessage</span></span>](emptyfolderresponsemessage.md) <br/> |<span data-ttu-id="76fb0-195">包含状态和单个**EmptyFolder**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-195">Contains the status and result of a single **EmptyFolder** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-196">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="76fb0-196">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md) <br/> |<span data-ttu-id="76fb0-197">包含状态和**UpdateInboxRules**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-197">Contains the status and result of an **UpdateInboxRules** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-198">UploadItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76fb0-198">UploadItemsResponseMessage</span></span>](uploaditemsresponsemessage.md) <br/> |<span data-ttu-id="76fb0-199">包含状态和**UploadItemsResponse**请求的结果。</span><span class="sxs-lookup"><span data-stu-id="76fb0-199">Contains a status and result of an **UploadItemsResponse** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-200">GetInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="76fb0-200">GetInboxRulesResponse</span></span>](getinboxrulesresponse.md) <br/> |<span data-ttu-id="76fb0-201">包含**GetInboxRules**请求的响应。</span><span class="sxs-lookup"><span data-stu-id="76fb0-201">Contains a response to a **GetInboxRules** request.</span></span>  <br/> |
|<span data-ttu-id="76fb0-202">GetServiceConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="76fb0-202">GetServiceConfigurationResponse</span></span>  <br/> |<span data-ttu-id="76fb0-203">包含**GetServiceConfiguration**请求的响应。</span><span class="sxs-lookup"><span data-stu-id="76fb0-203">Contains a response to a **GetServiceConfiguration** request.</span></span>  <br/> |
|[<span data-ttu-id="76fb0-204">ServiceConfigurationResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="76fb0-204">ServiceConfigurationResponseMessageType</span></span>](serviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="76fb0-205">包含服务配置设置。</span><span class="sxs-lookup"><span data-stu-id="76fb0-205">Contains service configuration settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="76fb0-206">文本值</span><span class="sxs-lookup"><span data-stu-id="76fb0-206">Text value</span></span>

<span data-ttu-id="76fb0-207">如果使用此元素，则需要的文本值。</span><span class="sxs-lookup"><span data-stu-id="76fb0-207">A text value is required if this element is used.</span></span> <span data-ttu-id="76fb0-208">此元素是只读的。</span><span class="sxs-lookup"><span data-stu-id="76fb0-208">This element is read-only.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="76fb0-209">注解</span><span class="sxs-lookup"><span data-stu-id="76fb0-209">Remarks</span></span>

<span data-ttu-id="76fb0-210">此元素不需要，并且不包含在所有响应。</span><span class="sxs-lookup"><span data-stu-id="76fb0-210">This element is not required and is not included in all responses.</span></span>
  
<span data-ttu-id="76fb0-211">描述此元素的架构位于承载 Exchange Web Services 的 IIS 虚拟目录中。</span><span class="sxs-lookup"><span data-stu-id="76fb0-211">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="76fb0-212">元素信息</span><span class="sxs-lookup"><span data-stu-id="76fb0-212">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="76fb0-213">命名空间</span><span class="sxs-lookup"><span data-stu-id="76fb0-213">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="76fb0-214">架构名称</span><span class="sxs-lookup"><span data-stu-id="76fb0-214">Schema Name</span></span>  <br/> |<span data-ttu-id="76fb0-215">消息架构</span><span class="sxs-lookup"><span data-stu-id="76fb0-215">Messages schema</span></span>  <br/> |
|<span data-ttu-id="76fb0-216">验证文件</span><span class="sxs-lookup"><span data-stu-id="76fb0-216">Validation File</span></span>  <br/> |<span data-ttu-id="76fb0-217">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="76fb0-217">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="76fb0-218">可以为空</span><span class="sxs-lookup"><span data-stu-id="76fb0-218">Can be Empty</span></span>  <br/> |<span data-ttu-id="76fb0-219">False</span><span class="sxs-lookup"><span data-stu-id="76fb0-219">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="76fb0-220">另请参阅</span><span class="sxs-lookup"><span data-stu-id="76fb0-220">See also</span></span>

- [<span data-ttu-id="76fb0-221">Exchange 的 EWS 引用</span><span class="sxs-lookup"><span data-stu-id="76fb0-221">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md) 
- [<span data-ttu-id="76fb0-222">在交换 EWS XML 元素</span><span class="sxs-lookup"><span data-stu-id="76fb0-222">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
