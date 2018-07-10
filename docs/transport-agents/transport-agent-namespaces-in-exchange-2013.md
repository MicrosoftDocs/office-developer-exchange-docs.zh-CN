---
title: 传输代理 Exchange 2013 中的命名空间
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c40788e-c182-4502-9202-206e6aaa53f8
description: 了解有关的.NET Framework 类和成员的可用来创建 Exchange 2013 的自定义传输代理。
ms.openlocfilehash: a8189ca9915312b64fefda3091f8f81e51271ad6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/25/2018
ms.locfileid: "19753088"
---
# <a name="transport-agent-namespaces-in-exchange-2013"></a><span data-ttu-id="96b87-103">传输代理 Exchange 2013 中的命名空间</span><span class="sxs-lookup"><span data-stu-id="96b87-103">Transport agent namespaces in Exchange 2013</span></span>

<span data-ttu-id="96b87-104">了解有关的.NET Framework 类和成员的可用来创建 Exchange 2013 的自定义传输代理。</span><span class="sxs-lookup"><span data-stu-id="96b87-104">Learn about the .NET Framework classes and members that you can use to create custom transport agents for Exchange 2013.</span></span>
  
<span data-ttu-id="96b87-105">**适用于：** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="96b87-105">**Applies to:** Exchange Server 2013</span></span> 
  
<span data-ttu-id="96b87-106">本文提供了有关包含可用于创建传输代理的 Exchange Server 2013 的参考信息的命名空间的信息。</span><span class="sxs-lookup"><span data-stu-id="96b87-106">This article provides information about the namespaces that contain reference information that you can use to create transport agents for Exchange Server 2013.</span></span> <span data-ttu-id="96b87-107">该参数还描述可用于读取和修改通过传输管道传递的电子邮件传输代理的类。</span><span class="sxs-lookup"><span data-stu-id="96b87-107">It also describes the classes that your transport agents can use to read and modify email messages that pass through the transport pipeline.</span></span>
  
## <a name="transport-agent-class-library"></a><span data-ttu-id="96b87-108">传输代理类库</span><span class="sxs-lookup"><span data-stu-id="96b87-108">Transport agent class library</span></span>

<span data-ttu-id="96b87-109">以下命名空间包含可用于创建和扩展传输代理的类型。</span><span class="sxs-lookup"><span data-stu-id="96b87-109">The following namespaces contain types that you can use to create and extend transport agents.</span></span>

<span data-ttu-id="96b87-110">**表 1。.NET framework 命名空间**</span><span class="sxs-lookup"><span data-stu-id="96b87-110">**Table 1. .NET Framework namespaces**</span></span>

|<span data-ttu-id="96b87-111">**命名空间**</span><span class="sxs-lookup"><span data-stu-id="96b87-111">**Namespace**</span></span>|<span data-ttu-id="96b87-112">**说明**</span><span class="sxs-lookup"><span data-stu-id="96b87-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="96b87-113">Microsoft.Exchange.Data</span><span class="sxs-lookup"><span data-stu-id="96b87-113">Microsoft.Exchange.Data</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.aspx) <br/> |<span data-ttu-id="96b87-114">包含指定数据和配置例外的类型。</span><span class="sxs-lookup"><span data-stu-id="96b87-114">Contains types that specify data and configuration exceptions.</span></span>  <br/> |
|[<span data-ttu-id="96b87-115">Microsoft.Exchange.Data.Common</span><span class="sxs-lookup"><span data-stu-id="96b87-115">Microsoft.Exchange.Data.Common</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Common.aspx) <br/> |<span data-ttu-id="96b87-116">包含支持本地化和错误处理的类型。</span><span class="sxs-lookup"><span data-stu-id="96b87-116">Contains types that support localization and error handling.</span></span>  <br/> |
|[<span data-ttu-id="96b87-117">Microsoft.Exchange.Data.ContentTypes.iCalendar</span><span class="sxs-lookup"><span data-stu-id="96b87-117">Microsoft.Exchange.Data.ContentTypes.iCalendar</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.aspx) <br/> |<span data-ttu-id="96b87-118">包含使您能够读取和写入 iCalendar 数据的类型。</span><span class="sxs-lookup"><span data-stu-id="96b87-118">Contains types that enable you to read and write iCalendar data.</span></span>  <br/> |
|[<span data-ttu-id="96b87-119">Microsoft.Exchange.Data.ContentTypes.Tnef</span><span class="sxs-lookup"><span data-stu-id="96b87-119">Microsoft.Exchange.Data.ContentTypes.Tnef</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.aspx) <br/> |<span data-ttu-id="96b87-120">包含使您能够读取和写入 TNEF 数据的类型。</span><span class="sxs-lookup"><span data-stu-id="96b87-120">Contains types that enable you to read and write TNEF data.</span></span>  <br/> |
|[<span data-ttu-id="96b87-121">Microsoft.Exchange.Data.ContentTypes.vCard</span><span class="sxs-lookup"><span data-stu-id="96b87-121">Microsoft.Exchange.Data.ContentTypes.vCard</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.vCard.aspx) <br/> |<span data-ttu-id="96b87-122">包含使您能够读取和写入 vCard 数据的类型。</span><span class="sxs-lookup"><span data-stu-id="96b87-122">Contains types that enable you to read and write vCard data.</span></span>  <br/> |
|[<span data-ttu-id="96b87-123">Microsoft.Exchange.Data.Globalization</span><span class="sxs-lookup"><span data-stu-id="96b87-123">Microsoft.Exchange.Data.Globalization</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Globalization.aspx) <br/> |<span data-ttu-id="96b87-124">包含使您能够使用区域性和字符集以生成本地化的内容的类型。</span><span class="sxs-lookup"><span data-stu-id="96b87-124">Contains types that enable you to work with cultures and character sets to produce localized content.</span></span>  <br/> |
|[<span data-ttu-id="96b87-125">Microsoft.Exchange.Data.Mime</span><span class="sxs-lookup"><span data-stu-id="96b87-125">Microsoft.Exchange.Data.Mime</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.aspx) <br/> |<span data-ttu-id="96b87-126">包含使您能够读取和写入 MIME 数据的类型。</span><span class="sxs-lookup"><span data-stu-id="96b87-126">Contains types that enable you to read and write MIME data.</span></span>  <br/> |
|[<span data-ttu-id="96b87-127">Microsoft.Exchange.Data.Mime.Encoders</span><span class="sxs-lookup"><span data-stu-id="96b87-127">Microsoft.Exchange.Data.Mime.Encoders</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.aspx) <br/> |<span data-ttu-id="96b87-128">包含使您能够进行编码和解码 MIME 数据的类型。</span><span class="sxs-lookup"><span data-stu-id="96b87-128">Contains types that enable you to encode and decode MIME data.</span></span>  <br/> |
|[<span data-ttu-id="96b87-129">Microsoft.Exchange.Data.TextConverters</span><span class="sxs-lookup"><span data-stu-id="96b87-129">Microsoft.Exchange.Data.TextConverters</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.aspx) <br/> |<span data-ttu-id="96b87-130">包含使您能够读取和写入数据使用不同的文本格式，并与这些格式转换数据类型。</span><span class="sxs-lookup"><span data-stu-id="96b87-130">Contains types that enable you to read and write data with different text formats, and convert data to and from those formats.</span></span>  <br/> |
|[<span data-ttu-id="96b87-131">Microsoft.Exchange.Data.Transport</span><span class="sxs-lookup"><span data-stu-id="96b87-131">Microsoft.Exchange.Data.Transport</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.aspx) <br/> |<span data-ttu-id="96b87-132">包含使您能够访问路由、 主机和传输管道的域信息的类型。</span><span class="sxs-lookup"><span data-stu-id="96b87-132">Contains types that enable you to access routing, host, and domain information about the transport pipeline.</span></span>  <br/> |
|[<span data-ttu-id="96b87-133">Microsoft.Exchange.Data.Transport.Delivery</span><span class="sxs-lookup"><span data-stu-id="96b87-133">Microsoft.Exchange.Data.Transport.Delivery</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.aspx) <br/> |<span data-ttu-id="96b87-134">包含支持 Exchange 2013 传递代理的扩展的类型。</span><span class="sxs-lookup"><span data-stu-id="96b87-134">Contains types that support the extension of Exchange 2013 delivery agents.</span></span>  <br/> |
|[<span data-ttu-id="96b87-135">Microsoft.Exchange.Data.Transport.Email</span><span class="sxs-lookup"><span data-stu-id="96b87-135">Microsoft.Exchange.Data.Transport.Email</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Email.aspx) <br/> |<span data-ttu-id="96b87-136">包含支持创建、 读取、 写入，并修改电子邮件的类型。</span><span class="sxs-lookup"><span data-stu-id="96b87-136">Contains types that support creating, reading, writing, and modifying email messages.</span></span>  <br/> |
|[<span data-ttu-id="96b87-137">Microsoft.Exchange.Data.Transport.Routing</span><span class="sxs-lookup"><span data-stu-id="96b87-137">Microsoft.Exchange.Data.Transport.Routing</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.aspx) <br/> |<span data-ttu-id="96b87-138">包含支持的扩展的 Exchange 2013 传输路由行为的类型。</span><span class="sxs-lookup"><span data-stu-id="96b87-138">Contains types that support the extension of the Exchange 2013 transport routing behavior.</span></span>  <br/> |
|[<span data-ttu-id="96b87-139">Microsoft.Exchange.Data.Transport.Smtp</span><span class="sxs-lookup"><span data-stu-id="96b87-139">Microsoft.Exchange.Data.Transport.Smtp</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.aspx) <br/> |<span data-ttu-id="96b87-140">包含支持的扩展的 Exchange 2013 传输 SMTP 行为的类型。</span><span class="sxs-lookup"><span data-stu-id="96b87-140">Contains types that support the extension of the Exchange 2013 transport SMTP behavior.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="96b87-141">另请参阅</span><span class="sxs-lookup"><span data-stu-id="96b87-141">See also</span></span>

- [<span data-ttu-id="96b87-142">在 Exchange 传输代理</span><span class="sxs-lookup"><span data-stu-id="96b87-142">Transport agents in Exchange</span></span>](transport-agents-in-exchange-2013.md)   
- [<span data-ttu-id="96b87-143">传输代理 Exchange 2013 中的概念</span><span class="sxs-lookup"><span data-stu-id="96b87-143">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md) 
- [<span data-ttu-id="96b87-144">Exchange server API 参考</span><span class="sxs-lookup"><span data-stu-id="96b87-144">Server API reference for Exchange</span></span>](http://msdn.microsoft.com/library/6eddd052-f59f-45b4-b846-7e53d4d7eb16%28Office.15%29.aspx)
- [<span data-ttu-id="96b87-145">Exchange 2013 的代理配置文件元素</span><span class="sxs-lookup"><span data-stu-id="96b87-145">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)
    
