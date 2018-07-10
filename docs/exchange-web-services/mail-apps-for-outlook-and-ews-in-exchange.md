---
title: Outlook 和 Exchange 中的 EWS 的邮件应用程序
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 821c8eb9-bb58-42e8-9a3a-61ca635cba59
description: 查找有关邮件应用程序的 Outlook 和如何使用 EWS 在 Exchange 中的信息。
ms.openlocfilehash: 2f44045d80a74ed6a835604d516949ca3bc27379
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752914"
---
# <a name="mail-apps-for-outlook-and-ews-in-exchange"></a><span data-ttu-id="81a64-103">Outlook 和 Exchange 中的 EWS 的邮件应用程序</span><span class="sxs-lookup"><span data-stu-id="81a64-103">Mail apps for Outlook and EWS in Exchange</span></span>

<span data-ttu-id="81a64-104">查找有关邮件应用程序的 Outlook 和如何使用 EWS 在 Exchange 中的信息。</span><span class="sxs-lookup"><span data-stu-id="81a64-104">Find information about mail apps for Outlook and how they work with EWS in Exchange.</span></span>
  
<span data-ttu-id="81a64-105">Outlook 邮件应用程序提供了单一界面和使用 web 标准来使您能够创建自定义电子邮件用户体验的编程模型。</span><span class="sxs-lookup"><span data-stu-id="81a64-105">Mail apps for Outlook provide a single interface and programming model that uses web standards to enable you to create a custom experience for your email users.</span></span> <span data-ttu-id="81a64-106">您可以创建在 Outlook 中; 承载 HTML5 框架中显示上下文或有用信息的邮件应用程序例如，邮件应用程序可以使用突出显示时的电子邮件包含地址的地址显示必应 Bing 地图。</span><span class="sxs-lookup"><span data-stu-id="81a64-106">You can create mail apps that display contextual or helpful information in an HTML5 frame hosted in Outlook; for example, a mail app can show a Bing map with an address highlighted when an email message contains an address.</span></span> <span data-ttu-id="81a64-107">或者，当用户撰写邮件时，邮件应用程序可以显示收件人，有关其他信息，然后在按钮的触摸电子邮件中插入的标准的问候语。</span><span class="sxs-lookup"><span data-stu-id="81a64-107">Or when a user is composing a message, a mail app can show additional information about the recipient, and insert a standard greeting into the email at the touch of a button.</span></span>
  
> [!NOTE]
> <span data-ttu-id="81a64-108">除非另有说明，否则本文中提及“Outlook”的地方也适用于 Outlook 富客户端、Outlook Web App 和适用于设备的 OWA。</span><span class="sxs-lookup"><span data-stu-id="81a64-108">"Outlook" in this article refers to the Outlook rich client, Outlook RT, Outlook Web App, and OWA for Devices.</span></span> 
  
<span data-ttu-id="81a64-109">邮件应用程序界面属于 JavaScript API for Office。</span><span class="sxs-lookup"><span data-stu-id="81a64-109">The mail apps interface is part of the JavaScript API for Office.</span></span> <span data-ttu-id="81a64-110">您可以使用 API 访问 Exchange 中启用对邮件应用程序的信息：</span><span class="sxs-lookup"><span data-stu-id="81a64-110">You can use the API to access information in Exchange to enable your mail app to:</span></span>
  
- <span data-ttu-id="81a64-111">[识别实体](http://msdn.microsoft.com/library/a6b0904b-afe9-4882-9136-3d8cfd57fcf8%28Office.15%29.aspx)，如地址、 电话号码、 任务建议或电子邮件中的会议建议。</span><span class="sxs-lookup"><span data-stu-id="81a64-111">[Recognize entities](http://msdn.microsoft.com/library/a6b0904b-afe9-4882-9136-3d8cfd57fcf8%28Office.15%29.aspx), like addresses, phone numbers, task suggestions, or meeting suggestions in an email.</span></span> 
    
- <span data-ttu-id="81a64-112">在打开并显示现有[邮件](http://msdn.microsoft.com/library/d0bca550-70c3-457c-85f8-e19b39e3b892%28Office.15%29.aspx)和[约会](http://msdn.microsoft.com/library/6cfbc29d-8581-474e-9a8b-510471e4bf8b%28Office.15%29.aspx)单独的视图，以便用户可以交叉引用中一个或多个邮件的信息。</span><span class="sxs-lookup"><span data-stu-id="81a64-112">Open and display existing [messages](http://msdn.microsoft.com/library/d0bca550-70c3-457c-85f8-e19b39e3b892%28Office.15%29.aspx) and [appointments](http://msdn.microsoft.com/library/6cfbc29d-8581-474e-9a8b-510471e4bf8b%28Office.15%29.aspx) in a separate view so that users can cross-reference information in one or more messages.</span></span> 
    
- <span data-ttu-id="81a64-113">向承载用户邮箱的 Exchange 服务器[发出 EWS 请求](http://msdn.microsoft.com/library/2ec380e0-4a67-4146-92a6-6a39f65dc6f2%28Office.15%29.aspx)。</span><span class="sxs-lookup"><span data-stu-id="81a64-113">[Make EWS requests](http://msdn.microsoft.com/library/2ec380e0-4a67-4146-92a6-6a39f65dc6f2%28Office.15%29.aspx) to the Exchange server that hosts the user's mailbox.</span></span> <span data-ttu-id="81a64-114">例如，邮件应用程序可以文件夹的列表，以便用户可以选择一个要存储该邮件，或在对话中，显示所有项或标记为垃圾邮件的电子邮件中。</span><span class="sxs-lookup"><span data-stu-id="81a64-114">A mail app can, for example, get a list of folders so that the user can choose one to store the message, or show all the items in a conversation, or mark an email message as junk.</span></span> 
    
- <span data-ttu-id="81a64-115">[获取令牌](http://msdn.microsoft.com/library/c658518b-6867-41a0-99cf-810303e4c539%28Office.15%29.aspx)来唯一标识的电子邮件帐户，若要启用单一登录第三方服务。</span><span class="sxs-lookup"><span data-stu-id="81a64-115">[Get a token](http://msdn.microsoft.com/library/c658518b-6867-41a0-99cf-810303e4c539%28Office.15%29.aspx) to uniquely identify an email account to enable single sign on on a third-party service.</span></span> 
    
- <span data-ttu-id="81a64-116">[获取令牌](http://msdn.microsoft.com/library/c658518b-6867-41a0-99cf-810303e4c539%28Office.15%29.aspx)，例如发出 EWS 请求代表用户，以提取附件从项目，或进一步处理从 Exchange 服务器获取项目的第三方服务。</span><span class="sxs-lookup"><span data-stu-id="81a64-116">[Get a token](http://msdn.microsoft.com/library/c658518b-6867-41a0-99cf-810303e4c539%28Office.15%29.aspx) that enables a third-party service to make EWS requests on behalf of the user, for example, to extract the attachments from an item, or to get an item from the Exchange server for further processing.</span></span> 
    
<span data-ttu-id="81a64-117">您可以使用邮件应用程序用户; 自定义的 Outlook Web App 体验如果，但是，您想要自定义"外观"Outlook Web app，请参阅 TechNet 上的以下文章：</span><span class="sxs-lookup"><span data-stu-id="81a64-117">You can use mail apps to customize the Outlook Web App experience for your users; if, however, you want to customize the "look and feel" of Outlook Web App, see these articles on TechNet:</span></span>
  
- [<span data-ttu-id="81a64-118">为 Outlook Web App 中创建主题</span><span class="sxs-lookup"><span data-stu-id="81a64-118">Create a theme for Outlook Web App</span></span>](http://technet.microsoft.com/zh-cn/library/bb201700%28v=exchg.150%29.aspx)
    
- [<span data-ttu-id="81a64-119">自定义 Outlook Web App 登录、 语言选择和错误页</span><span class="sxs-lookup"><span data-stu-id="81a64-119">Customize the Outlook Web App sign-in, language selection, and error pages</span></span>](http://technet.microsoft.com/zh-cn/library/ee633483%28v=exchg.150%29.aspx)
    
<span data-ttu-id="81a64-120">您的组织可以在要限制对授权用户访问的内部服务器上安装邮件应用程序或您和其他邮件应用程序开发人员可以将邮件应用程序置于[Office 商店](http://office.microsoft.com/store/)出售向公众。</span><span class="sxs-lookup"><span data-stu-id="81a64-120">Your organization can install mail apps on an internal server to limit access to authorized users, or you and other mail app developers can put mail apps on the [Office Store](http://office.microsoft.com/store/) for sale to the general public.</span></span> <span data-ttu-id="81a64-121">运行 Outlook 的任何人都可以下载、 安装和使用市场中的邮件应用程序。</span><span class="sxs-lookup"><span data-stu-id="81a64-121">Anyone who is running Outlook can download, install, and use mail apps from the marketplace.</span></span> 
  
<span data-ttu-id="81a64-122">如果您想要了解有关创建邮件应用程序详细信息，签出[的 Outlook 文档的邮件应用程序](http://msdn.microsoft.com/library/71e64bc9-e347-4f5d-8948-0a47b5dd93e6%28Office.15%29.aspx)或[发出 EWS 请求](http://code.msdn.microsoft.com/exchange/Mail-apps-for-Outlook-Make-770b2528)示例。</span><span class="sxs-lookup"><span data-stu-id="81a64-122">If you want to learn more about creating mail apps, check out the [mail apps for Outlook documentation](http://msdn.microsoft.com/library/71e64bc9-e347-4f5d-8948-0a47b5dd93e6%28Office.15%29.aspx) or the [Make an EWS request](http://code.msdn.microsoft.com/exchange/Mail-apps-for-Outlook-Make-770b2528) sample.</span></span> 
  
## <a name="ews-and-mail-apps-for-outlook"></a><span data-ttu-id="81a64-123">用于 Outlook 的 EWS 和邮件应用程序</span><span class="sxs-lookup"><span data-stu-id="81a64-123">EWS and mail apps for Outlook</span></span>

<span data-ttu-id="81a64-124">您可以使用承载运行邮件应用程序的帐户的 Exchange 服务器上的 EWS 操作的一个子集。</span><span class="sxs-lookup"><span data-stu-id="81a64-124">You can use a subset of EWS operations on the Exchange server that hosts the account that runs a mail app.</span></span>
  
<span data-ttu-id="81a64-125">[Mailbox.makeEwsRequestAsync](http://msdn.microsoft.com/library/2ec380e0-4a67-4146-92a6-6a39f65dc6f2%28Office.15%29.aspx)函数使您能够从邮件应用程序回服务器承载用户邮箱的 EWS 请求。</span><span class="sxs-lookup"><span data-stu-id="81a64-125">The [mailbox.makeEwsRequestAsync](http://msdn.microsoft.com/library/2ec380e0-4a67-4146-92a6-6a39f65dc6f2%28Office.15%29.aspx) function enables you to make EWS requests from your mail app back to the server that hosts the user's mailbox.</span></span> <span data-ttu-id="81a64-126">创建用于标识邮箱身份验证令牌 SOAP 信封 XML 请求和**makeEwsRequestAsync**函数调用 EWS 和邮件应用程序发出请求。</span><span class="sxs-lookup"><span data-stu-id="81a64-126">You create the SOAP envelope and XML request, and the **makeEwsRequestAsync** function calls EWS with an authentication token that identifies the mailbox and mail app that is making the request.</span></span> <span data-ttu-id="81a64-127">若要帮助保护用户的邮箱，Exchange 服务器将拒绝并非从邮件应用程序或未承载邮箱服务器的任何请求。</span><span class="sxs-lookup"><span data-stu-id="81a64-127">To help secure the user's mailbox, the Exchange server will reject any requests that do not come from the mail app or from a mailbox that is not hosted on the server.</span></span> 
  
<span data-ttu-id="81a64-128">任何其他应用程序，如邮件应用程序需要使用权限。</span><span class="sxs-lookup"><span data-stu-id="81a64-128">Like any other application, a mail app needs permissions to work.</span></span> <span data-ttu-id="81a64-129">管理员需要为：</span><span class="sxs-lookup"><span data-stu-id="81a64-129">Your administrator needs to:</span></span>
  
- <span data-ttu-id="81a64-130">邮件应用程序用户[授予 EWS 访问](controlling-client-application-access-to-ews-in-exchange.md)。</span><span class="sxs-lookup"><span data-stu-id="81a64-130">[Grant EWS access](controlling-client-application-access-to-ews-in-exchange.md) to the mail apps user.</span></span> 
    
- <span data-ttu-id="81a64-131">在客户端访问服务器 EWS 目录上[设置为 true 的"OAuthAuthentication"](http://technet.microsoft.com/zh-cn/library/aa997233%28v=exchg.150%29.aspx) 。</span><span class="sxs-lookup"><span data-stu-id="81a64-131">[Set "OAuthAuthentication" to true](http://technet.microsoft.com/zh-cn/library/aa997233%28v=exchg.150%29.aspx) on the Client Access Server EWS directory.</span></span> 
    
<span data-ttu-id="81a64-132">您还需要以确保您的应用程序请求读/写邮箱权限 for Office[权限模型](http://msdn.microsoft.com/library/5bca69f2-b287-4e19-8f0f-78d896b2a3d3%28Office.15%29.aspx)应用程序中。</span><span class="sxs-lookup"><span data-stu-id="81a64-132">You also need to make sure that your app requests the read/write mailbox permission in the apps for Office [permission model](http://msdn.microsoft.com/library/5bca69f2-b287-4e19-8f0f-78d896b2a3d3%28Office.15%29.aspx).</span></span>
  
<span data-ttu-id="81a64-133">完成这些步骤后，为邮件应用程序使用提供了文件夹和项目 EWS 操作的子集。</span><span class="sxs-lookup"><span data-stu-id="81a64-133">When these steps are complete, a subset of folder and item EWS operations are available for the mail app to use.</span></span> 
  
<span data-ttu-id="81a64-134">**表 1。可以使用邮件应用程序的 EWS 文件夹和项目操作**</span><span class="sxs-lookup"><span data-stu-id="81a64-134">**Table 1. EWS folder and item operations that mail apps can use**</span></span>

|<span data-ttu-id="81a64-135">**文件夹操作**</span><span class="sxs-lookup"><span data-stu-id="81a64-135">**Folder operations**</span></span>|<span data-ttu-id="81a64-136">**项目操作**</span><span class="sxs-lookup"><span data-stu-id="81a64-136">**Item operations**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="81a64-137">CreateFolder Operation</span><span class="sxs-lookup"><span data-stu-id="81a64-137">CreateFolder operation</span></span>](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> [<span data-ttu-id="81a64-138">FindFolder Operation</span><span class="sxs-lookup"><span data-stu-id="81a64-138">FindFolder operation</span></span>](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> [<span data-ttu-id="81a64-139">GetFolder Operation</span><span class="sxs-lookup"><span data-stu-id="81a64-139">GetFolder operation</span></span>](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> [<span data-ttu-id="81a64-140">UpdateFolder Operation</span><span class="sxs-lookup"><span data-stu-id="81a64-140">UpdateFolder operation</span></span>](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |[<span data-ttu-id="81a64-141">CopyItem 操作</span><span class="sxs-lookup"><span data-stu-id="81a64-141">CopyItem operation</span></span>](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> [<span data-ttu-id="81a64-142">CreateItem 操作</span><span class="sxs-lookup"><span data-stu-id="81a64-142">CreateItem operation</span></span>](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> [<span data-ttu-id="81a64-143">FindItem 操作</span><span class="sxs-lookup"><span data-stu-id="81a64-143">FindItem operation</span></span>](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> [<span data-ttu-id="81a64-144">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="81a64-144">FindConversation operation</span></span>](http://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) <br/> [<span data-ttu-id="81a64-145">GetConversationItems 操作</span><span class="sxs-lookup"><span data-stu-id="81a64-145">GetConversationItems operation</span></span>](http://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) <br/> [<span data-ttu-id="81a64-146">GetItem 操作</span><span class="sxs-lookup"><span data-stu-id="81a64-146">GetItem operation</span></span>](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> [<span data-ttu-id="81a64-147">MarkAsJunk 操作</span><span class="sxs-lookup"><span data-stu-id="81a64-147">MarkAsJunk operation</span></span>](http://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx) <br/> [<span data-ttu-id="81a64-148">MoveItem 操作</span><span class="sxs-lookup"><span data-stu-id="81a64-148">MoveItem operation</span></span>](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> [<span data-ttu-id="81a64-149">SendItem 操作</span><span class="sxs-lookup"><span data-stu-id="81a64-149">SendItem operation</span></span>](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) <br/> [<span data-ttu-id="81a64-150">UpdateItem 操作</span><span class="sxs-lookup"><span data-stu-id="81a64-150">UpdateItem operation</span></span>](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
   
### <a name="service-callback-tokens"></a><span data-ttu-id="81a64-151">服务回调令牌</span><span class="sxs-lookup"><span data-stu-id="81a64-151">Service callback tokens</span></span>

<span data-ttu-id="81a64-152">服务回调令牌启用邮件应用程序将传递给第三方服务的访问令牌，以便服务可以到承载邮箱的 Exchange 服务器发出 EWS 请求。</span><span class="sxs-lookup"><span data-stu-id="81a64-152">Service callback tokens enable mail apps to pass an access token to a third-party service so that the service can make EWS requests to the Exchange server that hosts the mailbox.</span></span> <span data-ttu-id="81a64-153">例如，邮件应用程序可以将服务回调令牌传递给第三方服务以及附加到电子邮件的图片的附件 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="81a64-153">For example, a mail app can pass a service callback token to a third-party service along with a list of attachment IDs for pictures attached to an email.</span></span> <span data-ttu-id="81a64-154">该服务然后可以使用附件 Id 和回调令牌以向用户的 Exchange 服务器获取附加的图片发出 EWS 请求。</span><span class="sxs-lookup"><span data-stu-id="81a64-154">The service can then use the attachment IDs and the callback token to make an EWS request to the user's Exchange server to get the attached pictures.</span></span> <span data-ttu-id="81a64-155">邮件应用程序也可以用于服务回调令牌一组项目 Id 从 Exchange 服务器获取电子邮件和约会项。</span><span class="sxs-lookup"><span data-stu-id="81a64-155">Mail apps can also use the service callback token with a list of item IDs to get email and appointment items from the Exchange server.</span></span>
  
<span data-ttu-id="81a64-156">服务回调令牌是不透明令牌的第三方服务将附加到持有者 authentication 标头中的 EWS 请求。</span><span class="sxs-lookup"><span data-stu-id="81a64-156">The service callback token is an opaque token that the third-party service attaches to the EWS request in a bearer authentication header.</span></span> <span data-ttu-id="81a64-157">标记标识邮件应用程序和要帮助保护 EWS 请求的邮箱。</span><span class="sxs-lookup"><span data-stu-id="81a64-157">The token identifies the mail app and the mailbox to help secure the EWS request.</span></span> <span data-ttu-id="81a64-158">若要了解如何使用服务回调令牌，请参阅[Outlook 邮件应用程序： 从 Exchange 服务器获取附件](http://code.msdn.microsoft.com/exchange/Mail-apps-for-Office-Get-38babdc9)示例。</span><span class="sxs-lookup"><span data-stu-id="81a64-158">To learn how to use service callback tokens, see the [Mail apps for Outlook: Get attachments from an Exchange server](http://code.msdn.microsoft.com/exchange/Mail-apps-for-Office-Get-38babdc9) sample.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="81a64-159">另请参阅</span><span class="sxs-lookup"><span data-stu-id="81a64-159">See also</span></span>


- [<span data-ttu-id="81a64-160">在 Exchange 控制客户端应用程序访问 EWS</span><span class="sxs-lookup"><span data-stu-id="81a64-160">Controlling client application access to EWS in Exchange</span></span>](controlling-client-application-access-to-ews-in-exchange.md)
    
- [<span data-ttu-id="81a64-161">Mailbox.makeEwsRequestAsync 方法 (Office 的 JavaScript API)</span><span class="sxs-lookup"><span data-stu-id="81a64-161">Mailbox.makeEwsRequestAsync method (JavaScript API for Office)</span></span>](http://msdn.microsoft.com/library/2ec380e0-4a67-4146-92a6-6a39f65dc6f2%28Office.15%29.aspx)
    
- [<span data-ttu-id="81a64-162">Outlook 外接程序</span><span class="sxs-lookup"><span data-stu-id="81a64-162">Outlook add-ins</span></span>](http://msdn.microsoft.com/library/71e64bc9-e347-4f5d-8948-0a47b5dd93e6%28Office.15%29.aspx)
    
- [<span data-ttu-id="81a64-163">Mailbox.getUserIdentityTokenAsync 方法 (Office 的 JavaScript API)</span><span class="sxs-lookup"><span data-stu-id="81a64-163">Mailbox.getUserIdentityTokenAsync method (JavaScript API for Office)</span></span>](http://msdn.microsoft.com/library/c658518b-6867-41a0-99cf-810303e4c539%28Office.15%29.aspx)
    
- [<span data-ttu-id="81a64-164">使用 Exchange 标识令牌对 Outlook 外接程序进行身份验证</span><span class="sxs-lookup"><span data-stu-id="81a64-164">Authenticate an Outlook add-in by using Exchange identity tokens</span></span>](http://msdn.microsoft.com/library/c0520a1e-d9ba-495a-a99f-6816d7d2a23e%28Office.15%29.aspx)
    
- [<span data-ttu-id="81a64-165">指定 Outlook 外接程序对用户邮箱的访问权限</span><span class="sxs-lookup"><span data-stu-id="81a64-165">Understanding Outlook add-in permissions</span></span>](http://msdn.microsoft.com/library/5bca69f2-b287-4e19-8f0f-78d896b2a3d3%28Office.15%29.aspx)
    
- [<span data-ttu-id="81a64-166">Set-webservicesvirtualdirectory</span><span class="sxs-lookup"><span data-stu-id="81a64-166">Set-WebServicesVirtualDirectory</span></span>](http://technet.microsoft.com/zh-cn/library/aa997233%28v=exchg.150%29.aspx)
    
- [<span data-ttu-id="81a64-167">Outlook 邮件应用程序： 发出 EWS 请求</span><span class="sxs-lookup"><span data-stu-id="81a64-167">Mail apps for Outlook: Make an EWS request</span></span>](http://code.msdn.microsoft.com/office/Mail-apps-for-Outlook-Make-770b2528)
    
- [<span data-ttu-id="81a64-168">Outlook 邮件应用程序： 使用客户端身份令牌</span><span class="sxs-lookup"><span data-stu-id="81a64-168">Mail apps for Outlook: Use a client identity token</span></span>](http://code.msdn.microsoft.com/Mail-apps-for-Outlook-Use-b20a66b6)
    
- [<span data-ttu-id="81a64-169">Outlook 邮件应用程序： 从 Exchange 服务器获取附件</span><span class="sxs-lookup"><span data-stu-id="81a64-169">Mail apps for Outlook: Get attachments from an Exchange server</span></span>](http://code.msdn.microsoft.com/office/Mail-apps-for-Office-Get-38babdc9)
    
