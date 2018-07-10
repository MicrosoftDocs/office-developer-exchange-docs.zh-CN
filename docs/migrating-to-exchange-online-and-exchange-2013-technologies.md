---
title: 迁移到 Exchange 技术
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 946a722f-0892-4a59-9e58-a291bfb6834a
description: 如果您正在从早期版本的 Exchange 迁移的使用本文中的信息以找出哪些开发技术支持在当前的产品版本和要迁移到的技术。
ms.openlocfilehash: 82362b7bcdb79d6ca43603335d51a8bd8c1df239
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/25/2018
ms.locfileid: "19753052"
---
# <a name="migrating-to-exchange-technologies"></a><span data-ttu-id="49da4-103">迁移到 Exchange 技术</span><span class="sxs-lookup"><span data-stu-id="49da4-103">Migrating to Exchange technologies</span></span>

<span data-ttu-id="49da4-104">如果您正在从早期版本的 Exchange 迁移的使用本文中的信息以找出哪些开发技术支持在当前的产品版本和要迁移到的技术。</span><span class="sxs-lookup"><span data-stu-id="49da4-104">If you're migrating from an earlier version of Exchange, use the information in this article to find out which development technologies are supported in current product versions, and which technology to migrate to.</span></span>
  
## <a name="determine-if-your-technology-is-available-in-current-versions"></a><span data-ttu-id="49da4-105">确定您的技术是否在当前版本中可用</span><span class="sxs-lookup"><span data-stu-id="49da4-105">Determine if your technology is available in current versions</span></span>

<span data-ttu-id="49da4-106">下表用于确定是否开发技术支持在 Exchange Online 或 Exchange 2013。</span><span class="sxs-lookup"><span data-stu-id="49da4-106">Use the following table to determine whether a development technology is supported in Exchange Online or Exchange 2013.</span></span> <span data-ttu-id="49da4-107">如果不支持这种技术，请参阅[Choose 迁移到开发技术](#bk_choose)。</span><span class="sxs-lookup"><span data-stu-id="49da4-107">If the technology is not supported, see [Choose a development technology to migrate to](#bk_choose).</span></span>

<br/> 

<span data-ttu-id="49da4-108">**Exchange 开发技术和产品版本**</span><span class="sxs-lookup"><span data-stu-id="49da4-108">**Exchange development technologies and product versions**</span></span>

|<span data-ttu-id="49da4-109">技术</span><span class="sxs-lookup"><span data-stu-id="49da4-109">Technology</span></span>|<span data-ttu-id="49da4-110">Office 365 和 Exchange Online</span><span class="sxs-lookup"><span data-stu-id="49da4-110">Office 365 and Exchange Online</span></span>|<span data-ttu-id="49da4-111">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="49da4-111">Exchange 2013</span></span>|<span data-ttu-id="49da4-112">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="49da4-112">Exchange 2010</span></span>|<span data-ttu-id="49da4-113">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="49da4-113">Exchange 2007</span></span>|
|:-----|:-----:|:-----:|:-----:|:-----:|
|[<span data-ttu-id="49da4-114">Office 365 Api 平台概述</span><span class="sxs-lookup"><span data-stu-id="49da4-114">Office 365 APIs platform overview</span></span>](http://msdn.microsoft.com/library/16fbf0c0-5470-466b-aab8-a0c9074c94e2%28Office.15%29.aspx) <br/> |<span data-ttu-id="49da4-115">X</span><span class="sxs-lookup"><span data-stu-id="49da4-115">X</span></span>  <br/> ||||
|[<span data-ttu-id="49da4-116">EWS Managed API</span><span class="sxs-lookup"><span data-stu-id="49da4-116">EWS Managed API</span></span>](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |<span data-ttu-id="49da4-117">X</span><span class="sxs-lookup"><span data-stu-id="49da4-117">X</span></span>  <br/> |<span data-ttu-id="49da4-118">X</span><span class="sxs-lookup"><span data-stu-id="49da4-118">X</span></span>  <br/> |<span data-ttu-id="49da4-119">X</span><span class="sxs-lookup"><span data-stu-id="49da4-119">X</span></span>  <br/> |<span data-ttu-id="49da4-120">X</span><span class="sxs-lookup"><span data-stu-id="49da4-120">X</span></span>  <br/> |
|[<span data-ttu-id="49da4-121">Exchange Web 服务 (EWS)</span><span class="sxs-lookup"><span data-stu-id="49da4-121">Exchange Web Services (EWS)</span></span>](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |<span data-ttu-id="49da4-122">X</span><span class="sxs-lookup"><span data-stu-id="49da4-122">X</span></span>  <br/> |<span data-ttu-id="49da4-123">X</span><span class="sxs-lookup"><span data-stu-id="49da4-123">X</span></span>  <br/> |<span data-ttu-id="49da4-124">X</span><span class="sxs-lookup"><span data-stu-id="49da4-124">X</span></span>  <br/> |<span data-ttu-id="49da4-125">X</span><span class="sxs-lookup"><span data-stu-id="49da4-125">X</span></span>  <br/> |
|[<span data-ttu-id="49da4-126">Outlook 邮件应用程序</span><span class="sxs-lookup"><span data-stu-id="49da4-126">Mail apps for Outlook</span></span>](exchange-web-services/mail-apps-for-outlook-and-ews-in-exchange.md) <br/> |<span data-ttu-id="49da4-127">X</span><span class="sxs-lookup"><span data-stu-id="49da4-127">X</span></span>  <br/> |<span data-ttu-id="49da4-128">X</span><span class="sxs-lookup"><span data-stu-id="49da4-128">X</span></span>  <br/> |||
|[<span data-ttu-id="49da4-129">Outlook 对象模型 (OOM)</span><span class="sxs-lookup"><span data-stu-id="49da4-129">Outlook Object Model (OOM)</span></span>](http://msdn.microsoft.com/library/75e4ad96-62a2-49d2-bc51-48ceab50634c%28Office.15%29.aspx) <br/> |<span data-ttu-id="49da4-130">X</span><span class="sxs-lookup"><span data-stu-id="49da4-130">X</span></span>  <br/> |<span data-ttu-id="49da4-131">X</span><span class="sxs-lookup"><span data-stu-id="49da4-131">X</span></span>  <br/> |<span data-ttu-id="49da4-132">X</span><span class="sxs-lookup"><span data-stu-id="49da4-132">X</span></span>  <br/> |<span data-ttu-id="49da4-133">X</span><span class="sxs-lookup"><span data-stu-id="49da4-133">X</span></span>  <br/> |
|[<span data-ttu-id="49da4-134">Exchange 命令行管理程序</span><span class="sxs-lookup"><span data-stu-id="49da4-134">Exchange Management Shell</span></span>](management/exchange-management-shell.md) <br/> |<span data-ttu-id="49da4-135">X</span><span class="sxs-lookup"><span data-stu-id="49da4-135">X</span></span>  <br/> |<span data-ttu-id="49da4-136">X</span><span class="sxs-lookup"><span data-stu-id="49da4-136">X</span></span>  <br/> |<span data-ttu-id="49da4-137">X</span><span class="sxs-lookup"><span data-stu-id="49da4-137">X</span></span>  <br/> |<span data-ttu-id="49da4-138">X</span><span class="sxs-lookup"><span data-stu-id="49da4-138">X</span></span>  <br/> |
|[<span data-ttu-id="49da4-139">备份和还原</span><span class="sxs-lookup"><span data-stu-id="49da4-139">Backup and restore</span></span>](backup-restore/backup-and-restore-for-exchange-2013.md) <br/> ||<span data-ttu-id="49da4-140">X</span><span class="sxs-lookup"><span data-stu-id="49da4-140">X</span></span>  <br/> |<span data-ttu-id="49da4-141">X</span><span class="sxs-lookup"><span data-stu-id="49da4-141">X</span></span>  <br/> |<span data-ttu-id="49da4-142">X</span><span class="sxs-lookup"><span data-stu-id="49da4-142">X</span></span>  <br/> |
|[<span data-ttu-id="49da4-143">传输代理</span><span class="sxs-lookup"><span data-stu-id="49da4-143">Transport agents</span></span>](transport-agents/transport-agents-in-exchange-2013.md) <br/> ||<span data-ttu-id="49da4-144">X</span><span class="sxs-lookup"><span data-stu-id="49da4-144">X</span></span>  <br/> |<span data-ttu-id="49da4-145">X</span><span class="sxs-lookup"><span data-stu-id="49da4-145">X</span></span>  <br/> |<span data-ttu-id="49da4-146">X</span><span class="sxs-lookup"><span data-stu-id="49da4-146">X</span></span>  <br/> |
|<span data-ttu-id="49da4-147">Active Directory 服务接口 (ADSI)</span><span class="sxs-lookup"><span data-stu-id="49da4-147">Active Directory Services Interface (ADSI)</span></span>  <br/> ||||<span data-ttu-id="49da4-148">X</span><span class="sxs-lookup"><span data-stu-id="49da4-148">X</span></span>  <br/> |
|<span data-ttu-id="49da4-149">协作数据对象 (CDOEX) Exchange</span><span class="sxs-lookup"><span data-stu-id="49da4-149">Collaborative Data Objects for Exchange (CDOEX)</span></span>  <br/> ||||<span data-ttu-id="49da4-150">X</span><span class="sxs-lookup"><span data-stu-id="49da4-150">X</span></span>  <br/> |
|<span data-ttu-id="49da4-151">对于 Windows 2000 (CDOSYS) 的协作数据对象</span><span class="sxs-lookup"><span data-stu-id="49da4-151">Collaborative Data Objects for Windows 2000 (CDOSYS)</span></span>  <br/> ||||<span data-ttu-id="49da4-152">X</span><span class="sxs-lookup"><span data-stu-id="49da4-152">X</span></span>  <br/> |
|<span data-ttu-id="49da4-153">Exchange OLE DB 提供程序 (EXOLEDB)</span><span class="sxs-lookup"><span data-stu-id="49da4-153">Exchange OLE DB Provider (EXOLEDB)</span></span>  <br/> ||||<span data-ttu-id="49da4-154">X</span><span class="sxs-lookup"><span data-stu-id="49da4-154">X</span></span>  <br/> |
|<span data-ttu-id="49da4-155">Exchange 存储事件接收器</span><span class="sxs-lookup"><span data-stu-id="49da4-155">Exchange Store Event Sinks</span></span>  <br/> ||||<span data-ttu-id="49da4-156">X</span><span class="sxs-lookup"><span data-stu-id="49da4-156">X</span></span>  <br/> |
|<span data-ttu-id="49da4-157">增量更改同步 (ICS)</span><span class="sxs-lookup"><span data-stu-id="49da4-157">Incremental Change Synchronization (ICS)</span></span>  <br/> ||||<span data-ttu-id="49da4-158">X</span><span class="sxs-lookup"><span data-stu-id="49da4-158">X</span></span>  <br/> |
|<span data-ttu-id="49da4-159">轻型目录访问协议 (LDAP)</span><span class="sxs-lookup"><span data-stu-id="49da4-159">Lightweight Directory Access Protocol (LDAP)</span></span>  <br/> ||||<span data-ttu-id="49da4-160">X</span><span class="sxs-lookup"><span data-stu-id="49da4-160">X</span></span>  <br/> |
|[<span data-ttu-id="49da4-161">消息处理 API (MAPI)</span><span class="sxs-lookup"><span data-stu-id="49da4-161">Messaging API (MAPI)</span></span>](http://msdn.microsoft.com/library/3d980b86-7001-4869-9780-121c6bfc7275%28Office.15%29.aspx) <br/> |<span data-ttu-id="49da4-162">X</span><span class="sxs-lookup"><span data-stu-id="49da4-162">X</span></span>  <br/> |<span data-ttu-id="49da4-163">X</span><span class="sxs-lookup"><span data-stu-id="49da4-163">X</span></span>  <br/> |<span data-ttu-id="49da4-164">X</span><span class="sxs-lookup"><span data-stu-id="49da4-164">X</span></span>  <br/> |<span data-ttu-id="49da4-165">X</span><span class="sxs-lookup"><span data-stu-id="49da4-165">X</span></span>  <br/> |
|<span data-ttu-id="49da4-166">Outlook Web App 自定义</span><span class="sxs-lookup"><span data-stu-id="49da4-166">Outlook Web App customization</span></span>  <br/> |||<span data-ttu-id="49da4-167">X</span><span class="sxs-lookup"><span data-stu-id="49da4-167">X</span></span>  <br/> ||
|<span data-ttu-id="49da4-168">Web 分布式创作和版本管理 (WebDAV)</span><span class="sxs-lookup"><span data-stu-id="49da4-168">Web Distributed Authoring and Versioning (WebDAV)</span></span>  <br/> ||||<span data-ttu-id="49da4-169">X</span><span class="sxs-lookup"><span data-stu-id="49da4-169">X</span></span>  <br/> |

<span data-ttu-id="49da4-170"><a name="bk_choose"> </a></span><span class="sxs-lookup"><span data-stu-id="49da4-170"></span></span>

## <a name="choose-a-development-technology-to-migrate-to"></a><span data-ttu-id="49da4-171">选择身份验证迁移到开发技术</span><span class="sxs-lookup"><span data-stu-id="49da4-171">Choose a development technology to migrate to</span></span>

<span data-ttu-id="49da4-172">如果您的应用程序使用的技术不受支持或 deemphasized 在 Exchange Online 或 Exchange 2013，请使用下表确定哪种技术迁移到。</span><span class="sxs-lookup"><span data-stu-id="49da4-172">If the technology your application uses is not supported or deemphasized in Exchange Online or Exchange 2013, use the following table to decide which technology to migrate to.</span></span>
  
<span data-ttu-id="49da4-173">**建议使用的技术的迁移路径**</span><span class="sxs-lookup"><span data-stu-id="49da4-173">**Recommended technology migration paths**</span></span>

|<span data-ttu-id="49da4-174">**技术**</span><span class="sxs-lookup"><span data-stu-id="49da4-174">**Technology**</span></span>|<span data-ttu-id="49da4-175">**Office 365，Online，Exchange 和 Exchange 2013 中受支持？**</span><span class="sxs-lookup"><span data-stu-id="49da4-175">**Supported in Office 365, Exchange Online, and Exchange 2013?**</span></span>|<span data-ttu-id="49da4-176">**迁移到**</span><span class="sxs-lookup"><span data-stu-id="49da4-176">**Migrate to**</span></span>|<span data-ttu-id="49da4-177">**更多信息**</span><span class="sxs-lookup"><span data-stu-id="49da4-177">**More info**</span></span>|
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="49da4-178">ADSI</span><span class="sxs-lookup"><span data-stu-id="49da4-178">ADSI</span></span>  <br/> |<span data-ttu-id="49da4-179">是，但 deemphasized</span><span class="sxs-lookup"><span data-stu-id="49da4-179">Yes, but deemphasized</span></span> <br/>|[<span data-ttu-id="49da4-180">Exchange 命令行管理程序</span><span class="sxs-lookup"><span data-stu-id="49da4-180">Exchange Management Shell</span></span>](management/exchange-management-shell.md)<br/> |<span data-ttu-id="49da4-181">无。</span><span class="sxs-lookup"><span data-stu-id="49da4-181">None.</span></span>  <br/> |
|<span data-ttu-id="49da4-182">CDOEX</span><span class="sxs-lookup"><span data-stu-id="49da4-182">CDOEX</span></span>  <br/> |<span data-ttu-id="49da4-183">否</span><span class="sxs-lookup"><span data-stu-id="49da4-183">No</span></span>  <br/> |[<span data-ttu-id="49da4-184">EWS 托管 API 或 EWS</span><span class="sxs-lookup"><span data-stu-id="49da4-184">EWS Managed API or EWS</span></span>](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |<span data-ttu-id="49da4-185">EWS 托管 API 和 EWS 可以访问同一 Exchange 存储 CDOEX 提供。</span><span class="sxs-lookup"><span data-stu-id="49da4-185">The EWS Managed API and EWS can access the same Exchange store that CDOEX provides.</span></span> <span data-ttu-id="49da4-186">与使用 CDOEX 构建的客户端应用程序，您可以在本地或远程计算机上运行 EWS 应用程序。</span><span class="sxs-lookup"><span data-stu-id="49da4-186">Unlike client applications built by using CDOEX, you can run EWS applications on a local or remote computer.</span></span>  <br/> |
|<span data-ttu-id="49da4-187">CDOEXM</span><span class="sxs-lookup"><span data-stu-id="49da4-187">CDOEXM</span></span>  <br/> |<span data-ttu-id="49da4-188">否</span><span class="sxs-lookup"><span data-stu-id="49da4-188">No</span></span> <br/> |[<span data-ttu-id="49da4-189">Exchange 命令行管理程序</span><span class="sxs-lookup"><span data-stu-id="49da4-189">Exchange Management Shell</span></span>](management/exchange-management-shell.md) <br/> |<span data-ttu-id="49da4-190">Exchange 命令行管理程序命令地控制 Exchange 服务器、 存储组、 数据库和用户比相应 CDOEXM Api。</span><span class="sxs-lookup"><span data-stu-id="49da4-190">Exchange Management Shell commands control Exchange servers, storage groups, databases, and users more simply than the corresponding CDOEXM APIs.</span></span> <span data-ttu-id="49da4-191">此外，您可以轻松地迁移到 Exchange 命令行管理程序命令 CDOEXM 应用程序。</span><span class="sxs-lookup"><span data-stu-id="49da4-191">Plus, you can easily migrate your CDOEXM applications to Exchange Management Shell commands.</span></span>  <br/> |
|<span data-ttu-id="49da4-192">CDOSYS</span><span class="sxs-lookup"><span data-stu-id="49da4-192">CDOSYS</span></span><br/> |<span data-ttu-id="49da4-193">否</span><span class="sxs-lookup"><span data-stu-id="49da4-193">No</span></span><br/> |[<span data-ttu-id="49da4-194">传输代理</span><span class="sxs-lookup"><span data-stu-id="49da4-194">Transport agents</span></span>](transport-agents/transport-agents-in-exchange-2013.md)   <br/> |<span data-ttu-id="49da4-195">使用基于通知的应用程序与 Exchange 2010 开头的 Exchange 版本一起使用的传输代理。</span><span class="sxs-lookup"><span data-stu-id="49da4-195">Use transport agents for notification-based applications that work with versions of Exchange starting with Exchange 2010.</span></span><br/><br/> <span data-ttu-id="49da4-196">CDOSYS 包含在当前版本的 Windows 中。</span><span class="sxs-lookup"><span data-stu-id="49da4-196">CDOSYS is included in current versions of Windows.</span></span> <span data-ttu-id="49da4-197">CDOSYS 中的功能是.NET Framework 中可用。</span><span class="sxs-lookup"><span data-stu-id="49da4-197">The functionality in CDOSYS is available in the .NET Framework.</span></span>  <br/> |
|<span data-ttu-id="49da4-198">CDOWF</span><span class="sxs-lookup"><span data-stu-id="49da4-198">CDOWF</span></span>  <br/> |<span data-ttu-id="49da4-199">否</span><span class="sxs-lookup"><span data-stu-id="49da4-199">No</span></span>  <br/> |[<span data-ttu-id="49da4-200">Windows Workflow Foundation (WWF)</span><span class="sxs-lookup"><span data-stu-id="49da4-200">Windows Workflow Foundation (WWF)</span></span>](http://msdn.microsoft.com/zh-cn/library/vstudio/ms735967%28v=vs.90%29.aspx) <br/> |<span data-ttu-id="49da4-201">您可以使用 WWF 创建使用 Exchange 2007 的高级工作流应用程序。</span><span class="sxs-lookup"><span data-stu-id="49da4-201">You can use WWF to create advanced workflow applications that work with Exchange 2007.</span></span>   <br/> |
|<span data-ttu-id="49da4-202">ExOLEDB</span><span class="sxs-lookup"><span data-stu-id="49da4-202">ExOLEDB</span></span>  <br/> |<span data-ttu-id="49da4-203">否</span><span class="sxs-lookup"><span data-stu-id="49da4-203">No</span></span>  <br/> |[<span data-ttu-id="49da4-204">EWS 托管 API 或 EWS</span><span class="sxs-lookup"><span data-stu-id="49da4-204">EWS Managed API or EWS</span></span>](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |<span data-ttu-id="49da4-205">EWS 托管 API 和 EWS 提供 ExOLEDB 提供的 Exchange 存储到相同的访问。</span><span class="sxs-lookup"><span data-stu-id="49da4-205">The EWS Managed API and EWS provide the same access to the Exchange store that ExOLEDB provides.</span></span> <span data-ttu-id="49da4-206">与使用 ExOLEDB 构建的客户端应用程序，您可以在本地或远程计算机上运行 EWS 应用程序。</span><span class="sxs-lookup"><span data-stu-id="49da4-206">Unlike client applications built by using ExOLEDB, You can run EWS applications on a local or remote computer.</span></span>  <br/> |
|<span data-ttu-id="49da4-207">ICS</span><span class="sxs-lookup"><span data-stu-id="49da4-207">ICS</span></span>  <br/> |<span data-ttu-id="49da4-208">是，但 deemphasized</span><span class="sxs-lookup"><span data-stu-id="49da4-208">Yes, but deemphasized</span></span>  <br/> |<span data-ttu-id="49da4-209">EWS 托管 API 或 EWS</span><span class="sxs-lookup"><span data-stu-id="49da4-209">EWS Managed API or EWS</span></span><br/> |<span data-ttu-id="49da4-210">您可以使用 EWS 托管 API 或 EWS[订阅通知](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md)并[同步邮箱数据](exchange-web-services/mailbox-synchronization-and-ews-in-exchange.md)。</span><span class="sxs-lookup"><span data-stu-id="49da4-210">You can use the EWS Managed API or EWS to [subscribe to notifications](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md) and [synchronize mailbox data](exchange-web-services/mailbox-synchronization-and-ews-in-exchange.md).</span></span>  <br/> |
|<span data-ttu-id="49da4-211">LDAP</span><span class="sxs-lookup"><span data-stu-id="49da4-211">LDAP</span></span>  <br/> |<span data-ttu-id="49da4-212">是，但 deemphasized</span><span class="sxs-lookup"><span data-stu-id="49da4-212">Yes, but deemphasized</span></span>  <br/> |[<span data-ttu-id="49da4-213">Exchange 命令行管理程序</span><span class="sxs-lookup"><span data-stu-id="49da4-213">Exchange Management Shell</span></span>](management/exchange-management-shell.md) <br/> |<span data-ttu-id="49da4-214">无。</span><span class="sxs-lookup"><span data-stu-id="49da4-214">None.</span></span>  <br/> |
|<span data-ttu-id="49da4-215">MAPI</span><span class="sxs-lookup"><span data-stu-id="49da4-215">MAPI</span></span>  <br/> |<span data-ttu-id="49da4-216">是，但 deemphasized</span><span class="sxs-lookup"><span data-stu-id="49da4-216">Yes, but deemphasized</span></span>  <br/> |<span data-ttu-id="49da4-217">Office 365 Api 平台概述，EWS 托管 API EWS</span><span class="sxs-lookup"><span data-stu-id="49da4-217">Office 365 APIs platform overview, EWS Managed API, EWS</span></span> <br/> |<span data-ttu-id="49da4-218">尽管 MAPI 当前是受支持的开发技术，您将最终需要重新设计您的 MAPI 应用程序能够使用较新的技术。</span><span class="sxs-lookup"><span data-stu-id="49da4-218">Although MAPI is currently a supported development technology, you will eventually have to redesign your MAPI applications to use a newer technology.</span></span><br/><br/><span data-ttu-id="49da4-219">如果您的 MAPI 应用程序执行简单的读取、 写入和更新操作对邮件、 日历或联系对象和目标 Office 365，您可以使用[Office 365 REST Api 的邮件、 日历和联系人](exchange-web-services/office-365-rest-apis-for-mail-calendars-and-contacts.md)。</span><span class="sxs-lookup"><span data-stu-id="49da4-219">If your MAPI application is performing simple read, write, and update operations on mail, calendar, or contact objects, and targets Office 365, you can use the [Office 365 REST APIs for mail, calendars, and contacts](exchange-web-services/office-365-rest-apis-for-mail-calendars-and-contacts.md).</span></span><br/><br/><span data-ttu-id="49da4-220">如果您面向的 Exchange 内部部署，您需要访问 MAPI 可以访问的所有属性，您可以使用 EWS 托管 API 或 EWS 和[架构化属性或扩展属性](http://msdn.microsoft.com/library/68623048-060e-4602-b3fa-62617a94cf72%28Office.15%29.aspx)。</span><span class="sxs-lookup"><span data-stu-id="49da4-220">If you are targeting Exchange on-premises and you need to access all the properties that MAPI can access, you can use the EWS Managed API or EWS and either [schematized properties or extended properties](http://msdn.microsoft.com/library/68623048-060e-4602-b3fa-62617a94cf72%28Office.15%29.aspx).</span></span><br/><br/><span data-ttu-id="49da4-221">**注意**： [ExtendedPropertyDefinition](http://msdn.microsoft.com/zh-cn/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx)类提供对 MAPI 从 EWS 托管 API 的访问并[ExtendedFieldURI](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx)元素提供对 MAPI 属性从 EWS 的访问。</span><span class="sxs-lookup"><span data-stu-id="49da4-221">**NOTE**: The [ExtendedPropertyDefinition](http://msdn.microsoft.com/zh-cn/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx) class provides access to MAPI from the EWS Managed API, and the [ExtendedFieldURI](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) element provides access to MAPI properties from EWS.</span></span>           |
|<span data-ttu-id="49da4-222">Outlook Web App 自定义</span><span class="sxs-lookup"><span data-stu-id="49da4-222">Outlook Web App customization</span></span>  <br/> |<span data-ttu-id="49da4-223">否</span><span class="sxs-lookup"><span data-stu-id="49da4-223">No</span></span>  <br/> |[<span data-ttu-id="49da4-224">邮件应用程序</span><span class="sxs-lookup"><span data-stu-id="49da4-224">Mail apps</span></span>](exchange-web-services/mail-apps-for-outlook-and-ews-in-exchange.md) <br/> |<span data-ttu-id="49da4-225">无。</span><span class="sxs-lookup"><span data-stu-id="49da4-225">None.</span></span>  <br/> |
|<span data-ttu-id="49da4-226">存储事件接收器</span><span class="sxs-lookup"><span data-stu-id="49da4-226">Store event sinks</span></span>  <br/> |<span data-ttu-id="49da4-227">否</span><span class="sxs-lookup"><span data-stu-id="49da4-227">No</span></span>  <br/> |<span data-ttu-id="49da4-228">EWS 托管 API 或 EWS</span><span class="sxs-lookup"><span data-stu-id="49da4-228">EWS Managed API or EWS</span></span> <br/> |<span data-ttu-id="49da4-229">您可以使用 EWS 托管 API 或 EWS[订阅通知](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md)并[同步邮箱数据](exchange-web-services/mailbox-synchronization-and-ews-in-exchange.md)。</span><span class="sxs-lookup"><span data-stu-id="49da4-229">You can use the EWS Managed API or EWS to [subscribe to notifications](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md) and [synchronize mailbox data](exchange-web-services/mailbox-synchronization-and-ews-in-exchange.md).</span></span><br/><br/><span data-ttu-id="49da4-230">通知中的 ews 提供对 Exchange 存储的同一访问存储事件接收器提供。</span><span class="sxs-lookup"><span data-stu-id="49da4-230">The notifications in EWS provide the same access to the Exchange store that store event sinks provide.</span></span> <span data-ttu-id="49da4-231">Visual Studio 工具可用于简化开发使用 EWS 的存储事件感知客户端应用程序。</span><span class="sxs-lookup"><span data-stu-id="49da4-231">You can use Visual Studio tools to streamline the development of store event-aware client applications that use EWS.</span></span>  <br/> |
|<span data-ttu-id="49da4-232">流式备份和还原</span><span class="sxs-lookup"><span data-stu-id="49da4-232">Streaming backup and restore</span></span>  <br/> |<span data-ttu-id="49da4-233">否</span><span class="sxs-lookup"><span data-stu-id="49da4-233">No</span></span>  <br/> |[<span data-ttu-id="49da4-234">卷影复制服务 (VSS) 编写器</span><span class="sxs-lookup"><span data-stu-id="49da4-234">Volume Shadow Copy Service (VSS) writer</span></span>](backup-restore/backup-and-restore-for-exchange-2013.md) <br/> |<span data-ttu-id="49da4-235">无。</span><span class="sxs-lookup"><span data-stu-id="49da4-235">None.</span></span>  <br/> |
|<span data-ttu-id="49da4-236">WebDAV</span><span class="sxs-lookup"><span data-stu-id="49da4-236">WebDAV</span></span>  <br/> |<span data-ttu-id="49da4-237">否</span><span class="sxs-lookup"><span data-stu-id="49da4-237">No</span></span>  <br/> |<span data-ttu-id="49da4-238">Office 365 Api 平台概述，EWS 托管 API 或 EWS</span><span class="sxs-lookup"><span data-stu-id="49da4-238">Office 365 APIs platform overview, EWS Managed API or EWS</span></span> <br/> |<span data-ttu-id="49da4-239">如果您 WebDAV 应用程序的执行简单的读取、 写入和更新操作对邮件、 日历或联系对象，您将面向 Office 365 使用的[Office 365 REST Api 的邮件、 日历和联系人](exchange-web-services/office-365-rest-apis-for-mail-calendars-and-contacts.md)。</span><span class="sxs-lookup"><span data-stu-id="49da4-239">If your WebDAV application is performing simple read, write, and update operations on mail, calendar, or contact objects, and you will be targeting Office 365, use the [Office 365 REST APIs for mail, calendars, and contacts](exchange-web-services/office-365-rest-apis-for-mail-calendars-and-contacts.md).</span></span><br/><br/><span data-ttu-id="49da4-240">否则，如果您面向的 Exchange 内部部署并且您需要在 Exchange 存储中的相同属性访问该 WebDAV 提供，使用 EWS 托管 API 或 EWS。</span><span class="sxs-lookup"><span data-stu-id="49da4-240">Otherwise, if you are targeting Exchange on-premises and you need access to the same properties in the Exchange store that WebDAV provides, use the EWS Managed API or EWS.</span></span>  <br/> |
|<span data-ttu-id="49da4-241">WebDAV 通知</span><span class="sxs-lookup"><span data-stu-id="49da4-241">WebDAV notifications</span></span>  <br/> |<span data-ttu-id="49da4-242">否</span><span class="sxs-lookup"><span data-stu-id="49da4-242">No</span></span>  <br/> |<span data-ttu-id="49da4-243">EWS 托管 API 或 EWS</span><span class="sxs-lookup"><span data-stu-id="49da4-243">EWS Managed API or EWS</span></span><br/> |<span data-ttu-id="49da4-244">您可以使用 EWS 托管 API 或 EWS 来[订阅通知](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md)。</span><span class="sxs-lookup"><span data-stu-id="49da4-244">You can use the EWS Managed API or EWS to [subscribe to notifications](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md).</span></span>  <br/> |
|<span data-ttu-id="49da4-245">Web 窗体</span><span class="sxs-lookup"><span data-stu-id="49da4-245">Web forms</span></span>  <br/> |<span data-ttu-id="49da4-246">否</span><span class="sxs-lookup"><span data-stu-id="49da4-246">No</span></span>  <br/> |[<span data-ttu-id="49da4-247">ASP.NET</span><span class="sxs-lookup"><span data-stu-id="49da4-247">ASP.NET</span></span>](http://www.asp.net/web-forms) <br/> |<span data-ttu-id="49da4-248">切换到 ASP.NET 并更新应用程序使用 EWS 访问邮箱和服务器的信息。</span><span class="sxs-lookup"><span data-stu-id="49da4-248">Switch to ASP.NET and update applications to access mailbox and server information by using EWS.</span></span>  <br/> |
|<span data-ttu-id="49da4-249">WMI 提供程序</span><span class="sxs-lookup"><span data-stu-id="49da4-249">WMI providers</span></span>  <br/> |<span data-ttu-id="49da4-250">否</span><span class="sxs-lookup"><span data-stu-id="49da4-250">No</span></span>  <br/> |[<span data-ttu-id="49da4-251">Exchange 命令行管理程序</span><span class="sxs-lookup"><span data-stu-id="49da4-251">Exchange Management Shell</span></span>](management/exchange-management-shell.md) <br/> |<span data-ttu-id="49da4-252">无。</span><span class="sxs-lookup"><span data-stu-id="49da4-252">None.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="49da4-253">另请参阅</span><span class="sxs-lookup"><span data-stu-id="49da4-253">See also</span></span>

- [<span data-ttu-id="49da4-254">选择的 API 或技术来开发 Outlook 解决方案</span><span class="sxs-lookup"><span data-stu-id="49da4-254">Selecting an API or technology for developing solutions for Outlook</span></span>](http://msdn.microsoft.com/library/01a46083-03d0-4333-920c-01a9f17f68cb%28Office.15%29.aspx)
    
