---
title: DeploymentId (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: b879c134-307e-4645-bb53-55d8ba4fad9c
description: DeploymentId 元素唯一地标识 Microsoft Exchange Server 2007 林。
ms.openlocfilehash: 4f2548709753d8407d02218acecd9233f0ba764f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/25/2018
ms.locfileid: "19753837"
---
# <a name="deploymentid-pox"></a><span data-ttu-id="a1309-103">DeploymentId (POX)</span><span class="sxs-lookup"><span data-stu-id="a1309-103">DeploymentId (POX)</span></span>

<span data-ttu-id="a1309-104">**DeploymentId**元素唯一地标识 Microsoft Exchange Server 2007 林。</span><span class="sxs-lookup"><span data-stu-id="a1309-104">The **DeploymentId** element uniquely identifies the Microsoft Exchange Server 2007 forest.</span></span> 
  
- [<span data-ttu-id="a1309-105">自动发现 (POX)</span><span class="sxs-lookup"><span data-stu-id="a1309-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)  
- [<span data-ttu-id="a1309-106">响应 (POX)</span><span class="sxs-lookup"><span data-stu-id="a1309-106">Response (POX)</span></span>](response-pox.md) 
- [<span data-ttu-id="a1309-107">用户 (POX)</span><span class="sxs-lookup"><span data-stu-id="a1309-107">User (POX)</span></span>](user-pox.md)  
- [<span data-ttu-id="a1309-108">DeploymentId (POX)</span><span class="sxs-lookup"><span data-stu-id="a1309-108">DeploymentId (POX)</span></span>](deploymentid-pox.md)
  
```xml
<DeploymentId/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="a1309-109">属性和元素</span><span class="sxs-lookup"><span data-stu-id="a1309-109">Attributes and elements</span></span>

<span data-ttu-id="a1309-110">如下章节中介绍了属性、子元素和父元素。</span><span class="sxs-lookup"><span data-stu-id="a1309-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a1309-111">属性</span><span class="sxs-lookup"><span data-stu-id="a1309-111">Attributes</span></span>

<span data-ttu-id="a1309-112">无。</span><span class="sxs-lookup"><span data-stu-id="a1309-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a1309-113">子元素</span><span class="sxs-lookup"><span data-stu-id="a1309-113">Child elements</span></span>

<span data-ttu-id="a1309-114">无。</span><span class="sxs-lookup"><span data-stu-id="a1309-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a1309-115">父元素</span><span class="sxs-lookup"><span data-stu-id="a1309-115">Parent elements</span></span>

|<span data-ttu-id="a1309-116">**元素**</span><span class="sxs-lookup"><span data-stu-id="a1309-116">**Element**</span></span>|<span data-ttu-id="a1309-117">**说明**</span><span class="sxs-lookup"><span data-stu-id="a1309-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a1309-118">用户 (POX)</span><span class="sxs-lookup"><span data-stu-id="a1309-118">User (POX)</span></span>](user-pox.md) <br/> |<span data-ttu-id="a1309-119">提供特定于用户的信息。</span><span class="sxs-lookup"><span data-stu-id="a1309-119">Provides user-specific information.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a1309-120">文本值</span><span class="sxs-lookup"><span data-stu-id="a1309-120">Text value</span></span>

<span data-ttu-id="a1309-121">文本值唯一地标识 GUID 格式中的为 Exchange 2007 林。</span><span class="sxs-lookup"><span data-stu-id="a1309-121">The text value uniquely identifies the Exchange 2007 forest in GUID format.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a1309-122">注解</span><span class="sxs-lookup"><span data-stu-id="a1309-122">Remarks</span></span>

<span data-ttu-id="a1309-123">如果您卸载并重新安装 Exchange 2007，并使用相同的服务器名称， **DeploymentId**值发生更改。</span><span class="sxs-lookup"><span data-stu-id="a1309-123">If you uninstall and then reinstall Exchange 2007 and you use the same server name, the **DeploymentId** value changes.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="a1309-124">另请参阅</span><span class="sxs-lookup"><span data-stu-id="a1309-124">See also</span></span>

- [<span data-ttu-id="a1309-125">Exchange POX 自动发现 XML 元素</span><span class="sxs-lookup"><span data-stu-id="a1309-125">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)
