---
title: 在 Exchange 中的 EWS 中的电子数据展示
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3128419f-dd5f-46d2-bb0d-0940738d0bb6
description: 在 Exchange 中了解有关电子数据展示中的 ews。
ms.openlocfilehash: 6491fdd9f2246870a89bfa89bf7d97b972d67c92
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752707"
---
# <a name="ediscovery-in-ews-in-exchange"></a><span data-ttu-id="38fb2-103">在 Exchange 中的 EWS 中的电子数据展示</span><span class="sxs-lookup"><span data-stu-id="38fb2-103">eDiscovery in EWS in Exchange</span></span>

<span data-ttu-id="38fb2-104">在 Exchange 中了解有关电子数据展示中的 ews。</span><span class="sxs-lookup"><span data-stu-id="38fb2-104">Learn about eDiscovery in EWS in Exchange.</span></span>
  
<span data-ttu-id="38fb2-105">电子数据展示是允许外部应用程序以执行 Exchange 数据的查询联合的查询 web 服务。</span><span class="sxs-lookup"><span data-stu-id="38fb2-105">eDiscovery is a federated query web service that enables external applications to perform queries of Exchange data.</span></span>
  
<span data-ttu-id="38fb2-106">发现包含几个阶段，包括标识和保留项数据、 下挑选和查看数据，以及生成庭院中的数据。</span><span class="sxs-lookup"><span data-stu-id="38fb2-106">Discovery consists of several phases, including identifying and preserving key data, culling down and reviewing the data, and producing data in court.</span></span> <span data-ttu-id="38fb2-107">电子数据展示查询加快发现过程，通过提供跨 Exchange 和 SharePoint 的单个发现工作流。</span><span class="sxs-lookup"><span data-stu-id="38fb2-107">eDiscovery queries facilitate the discovery process by providing a single discovery workflow across Exchange and SharePoint.</span></span>
  
## <a name="ediscovery-operations"></a><span data-ttu-id="38fb2-108">电子数据展示操作</span><span class="sxs-lookup"><span data-stu-id="38fb2-108">eDiscovery operations</span></span>

<span data-ttu-id="38fb2-109">由 EWS 公开该电子数据展示功能，通过在 Exchange Online 中，Exchange Online 作为 Office 365 的一部分和版本的 Exchange 开头 Exchange 2013 中引入的操作。</span><span class="sxs-lookup"><span data-stu-id="38fb2-109">The eDiscovery functionality that is exposed by EWS is available via operations introduced in Exchange Online, Exchange Online as part of Office 365, and versions of Exchange starting with Exchange 2013.</span></span> 
  
<span data-ttu-id="38fb2-110">**表 1。电子数据展示的新操作**</span><span class="sxs-lookup"><span data-stu-id="38fb2-110">**Table 1. New operations for eDiscovery**</span></span>

|<span data-ttu-id="38fb2-111">**操作名称**</span><span class="sxs-lookup"><span data-stu-id="38fb2-111">**Operation name**</span></span>|<span data-ttu-id="38fb2-112">**说明**</span><span class="sxs-lookup"><span data-stu-id="38fb2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="38fb2-113">GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="38fb2-113">GetDiscoverySearchConfiguration</span></span>](http://msdn.microsoft.com/library/8a54a6dc-110c-4972-a8bc-5ddb43c4b857%28Office.15%29.aspx) <br/> |<span data-ttu-id="38fb2-114">获取就地保留，保存查询搜索和启用了发现搜索邮箱的配置信息。</span><span class="sxs-lookup"><span data-stu-id="38fb2-114">Gets configuration information for in-place holds, saved discovery searches, and the mailboxes that are enabled for discovery search.</span></span>  <br/> |
|[<span data-ttu-id="38fb2-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="38fb2-115">GetHoldOnMailboxes</span></span>](http://msdn.microsoft.com/library/9157f329-80b4-4cd0-a158-378064966ae6%28Office.15%29.aspx) <br/> |<span data-ttu-id="38fb2-116">获取使用[SetHoldOnMailboxes 操作](http://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx)设置了基于查询的保留状态。</span><span class="sxs-lookup"><span data-stu-id="38fb2-116">Gets the status of a query-based hold, which is set by using the [SetHoldOnMailboxes operation](http://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx).</span></span>  <br/> |
|[<span data-ttu-id="38fb2-117">GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="38fb2-117">GetNonIndexableItemDetails</span></span>](http://msdn.microsoft.com/library/9279c3ad-f7c8-4bbc-b0a7-2c78416cb39a%28Office.15%29.aspx) <br/> |<span data-ttu-id="38fb2-118">检索有关无法编制索引的项目的详细信息。</span><span class="sxs-lookup"><span data-stu-id="38fb2-118">Retrieves details about items that cannot be indexed.</span></span> <span data-ttu-id="38fb2-119">这包括但不限于的项标识符的错误代码、 错误说明，当尝试索引项，以及有关文件的其他信息。</span><span class="sxs-lookup"><span data-stu-id="38fb2-119">This includes, but is not limited to, the item identifier, an error code, an error description, when an attempt was made to index the item, and additional information about the file.</span></span>  <br/> |
|[<span data-ttu-id="38fb2-120">GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="38fb2-120">GetNonIndexableItemStatistics</span></span>](http://msdn.microsoft.com/library/ed077877-9d98-4434-b8b6-a4a905e7f7a6%28Office.15%29.aspx) <br/> |<span data-ttu-id="38fb2-121">检索邮箱中无法编制索引的项的计数。</span><span class="sxs-lookup"><span data-stu-id="38fb2-121">Retrieves the count of items that cannot be indexed in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="38fb2-122">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="38fb2-122">GetSearchableMailboxes</span></span>](http://msdn.microsoft.com/library/47f8ff57-4835-4d2d-9136-44afb31a4cbe%28Office.15%29.aspx) <br/> |<span data-ttu-id="38fb2-123">获取邮箱的列表的客户端有搜索或上执行电子数据展示的权限。</span><span class="sxs-lookup"><span data-stu-id="38fb2-123">Gets a list of mailboxes that the client has permission to search or perform eDiscovery on.</span></span>  <br/> |
|[<span data-ttu-id="38fb2-124">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="38fb2-124">SearchMailboxes</span></span>](http://msdn.microsoft.com/library/8a67c1d8-d021-4e68-aa62-35f7d9c2edc7%28Office.15%29.aspx) <br/> |<span data-ttu-id="38fb2-125">搜索查询关键字匹配的特定邮箱中的项目。</span><span class="sxs-lookup"><span data-stu-id="38fb2-125">Searches for items in specific mailboxes that match query keywords.</span></span>  <br/> |
|[<span data-ttu-id="38fb2-126">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="38fb2-126">SetHoldOnMailboxes</span></span>](http://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx) <br/> |<span data-ttu-id="38fb2-127">设置基于查询的保留项。</span><span class="sxs-lookup"><span data-stu-id="38fb2-127">Sets a query-based hold on items.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="38fb2-128">另请参阅</span><span class="sxs-lookup"><span data-stu-id="38fb2-128">See also</span></span>

- [<span data-ttu-id="38fb2-129">开发 Exchange Web 服务客户端</span><span class="sxs-lookup"><span data-stu-id="38fb2-129">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="38fb2-130">Start using web services in Exchange</span><span class="sxs-lookup"><span data-stu-id="38fb2-130">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
    
- [<span data-ttu-id="38fb2-131">Exchange 的 EWS 客户端设计概述</span><span class="sxs-lookup"><span data-stu-id="38fb2-131">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)
    
