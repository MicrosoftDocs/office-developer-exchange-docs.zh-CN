---
title: CurrentMeetingTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CurrentMeetingTime
api_type:
- schema
ms.assetid: 1ff68154-24b5-465a-a31c-3d3bab0d491e
description: CurrentMeetingTime 元素均表示您要更新与建议的会议与会者的会议时间的会议的开始时间。
ms.openlocfilehash: 88adbe566270d759986e9b55afd4827c0513ca43
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/25/2018
ms.locfileid: "19753708"
---
# <a name="currentmeetingtime"></a><span data-ttu-id="6085b-103">CurrentMeetingTime</span><span class="sxs-lookup"><span data-stu-id="6085b-103">CurrentMeetingTime</span></span>

<span data-ttu-id="6085b-104">**CurrentMeetingTime**元素均表示您要更新与建议的会议与会者的会议时间的会议的开始时间。</span><span class="sxs-lookup"><span data-stu-id="6085b-104">The **CurrentMeetingTime** element represents the start time of a meeting that you want to update with a meeting time proposed by a meeting attendee.</span></span> 
  
[<span data-ttu-id="6085b-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="6085b-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="6085b-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="6085b-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="6085b-107">CurrentMeetingTime</span><span class="sxs-lookup"><span data-stu-id="6085b-107">CurrentMeetingTime</span></span>](currentmeetingtime.md)
  
```xml
<CurrentMeetingTime>...</CurrentMeetingTime>
```

 <span data-ttu-id="6085b-108">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="6085b-108">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6085b-109">属性和元素</span><span class="sxs-lookup"><span data-stu-id="6085b-109">Attributes and elements</span></span>

<span data-ttu-id="6085b-110">如下章节中介绍了属性、子元素和父元素。</span><span class="sxs-lookup"><span data-stu-id="6085b-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6085b-111">属性</span><span class="sxs-lookup"><span data-stu-id="6085b-111">Attributes</span></span>

<span data-ttu-id="6085b-112">无。</span><span class="sxs-lookup"><span data-stu-id="6085b-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6085b-113">子元素</span><span class="sxs-lookup"><span data-stu-id="6085b-113">Child elements</span></span>

<span data-ttu-id="6085b-114">无。</span><span class="sxs-lookup"><span data-stu-id="6085b-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6085b-115">父元素</span><span class="sxs-lookup"><span data-stu-id="6085b-115">Parent elements</span></span>

|<span data-ttu-id="6085b-116">**元素**</span><span class="sxs-lookup"><span data-stu-id="6085b-116">**Element**</span></span>|<span data-ttu-id="6085b-117">**说明**</span><span class="sxs-lookup"><span data-stu-id="6085b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6085b-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="6085b-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="6085b-119">包含选项的获取会议建议信息。</span><span class="sxs-lookup"><span data-stu-id="6085b-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="6085b-120">以下是此元素的 XPath:</span><span class="sxs-lookup"><span data-stu-id="6085b-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6085b-121">注解</span><span class="sxs-lookup"><span data-stu-id="6085b-121">Remarks</span></span>

<span data-ttu-id="6085b-122">此元素不是必需的。</span><span class="sxs-lookup"><span data-stu-id="6085b-122">This element is not required.</span></span>
  
> [!NOTE]
> <span data-ttu-id="6085b-123">描述此元素的架构位于运行 MicrosoftExchange Server 2007 的安装了客户端访问服务器角色的计算机的 /EWS/ 目录中。</span><span class="sxs-lookup"><span data-stu-id="6085b-123">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="6085b-124">元素信息</span><span class="sxs-lookup"><span data-stu-id="6085b-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6085b-125">命名空间</span><span class="sxs-lookup"><span data-stu-id="6085b-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6085b-126">架构名称</span><span class="sxs-lookup"><span data-stu-id="6085b-126">Schema Name</span></span>  <br/> |<span data-ttu-id="6085b-127">类型架构</span><span class="sxs-lookup"><span data-stu-id="6085b-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="6085b-128">验证文件</span><span class="sxs-lookup"><span data-stu-id="6085b-128">Validation File</span></span>  <br/> |<span data-ttu-id="6085b-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6085b-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6085b-130">可以为空</span><span class="sxs-lookup"><span data-stu-id="6085b-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="6085b-131">False</span><span class="sxs-lookup"><span data-stu-id="6085b-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6085b-132">另请参阅</span><span class="sxs-lookup"><span data-stu-id="6085b-132">See also</span></span>



[<span data-ttu-id="6085b-133">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="6085b-133">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="6085b-134">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="6085b-134">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)
