---
title: InternalReply
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InternalReply
api_type:
- schema
ms.assetid: 1d784ded-b874-4eb1-8f6d-2e0e03330e1e
description: InternalReply 元素包含外出 (oof) 响应发送给用户的域或受信任的域中的其他用户。
ms.openlocfilehash: ac5e9eadac7f45c233007ffb05f4d2430875ec52
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825955"
---
# <a name="internalreply"></a><span data-ttu-id="88baa-103">InternalReply</span><span class="sxs-lookup"><span data-stu-id="88baa-103">InternalReply</span></span>

<span data-ttu-id="88baa-104">**InternalReply**元素包含外出 (oof) 响应发送给用户的域或受信任的域中的其他用户。</span><span class="sxs-lookup"><span data-stu-id="88baa-104">The **InternalReply** element contains the out of office (OOF) response sent to other users in the user's domain or trusted domains.</span></span> 
  
```XML
<InternalReply>
   <Message/> 
</InternalReply>
```

 <span data-ttu-id="88baa-105">**ReplyBody**</span><span class="sxs-lookup"><span data-stu-id="88baa-105">**ReplyBody**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="88baa-106">属性和元素</span><span class="sxs-lookup"><span data-stu-id="88baa-106">Attributes and elements</span></span>

<span data-ttu-id="88baa-107">如下章节中介绍了属性、子元素和父元素。</span><span class="sxs-lookup"><span data-stu-id="88baa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="88baa-108">属性</span><span class="sxs-lookup"><span data-stu-id="88baa-108">Attributes</span></span>

|<span data-ttu-id="88baa-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="88baa-109">**Attribute**</span></span>|<span data-ttu-id="88baa-110">**说明**</span><span class="sxs-lookup"><span data-stu-id="88baa-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="88baa-111">xml: lang</span><span class="sxs-lookup"><span data-stu-id="88baa-111">xml:lang</span></span>  <br/> |<span data-ttu-id="88baa-112">指定**InternalReply**消息中使用的语言。</span><span class="sxs-lookup"><span data-stu-id="88baa-112">Specifies the language used in the **InternalReply** message.</span></span> <span data-ttu-id="88baa-113">此属性的可能值由 IETF RFC 3066 定义。</span><span class="sxs-lookup"><span data-stu-id="88baa-113">The possible values of this attribute are defined by IETF RFC 3066.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="88baa-114">子元素</span><span class="sxs-lookup"><span data-stu-id="88baa-114">Child elements</span></span>

|<span data-ttu-id="88baa-115">**元素**</span><span class="sxs-lookup"><span data-stu-id="88baa-115">**Element**</span></span>|<span data-ttu-id="88baa-116">**说明**</span><span class="sxs-lookup"><span data-stu-id="88baa-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88baa-117">消息 （可用性）</span><span class="sxs-lookup"><span data-stu-id="88baa-117">Message (Availability)</span></span>](message-availability.md) <br/> |<span data-ttu-id="88baa-118">包含 OOF 响应。</span><span class="sxs-lookup"><span data-stu-id="88baa-118">Contains the OOF response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="88baa-119">父元素</span><span class="sxs-lookup"><span data-stu-id="88baa-119">Parent elements</span></span>

|<span data-ttu-id="88baa-120">**元素**</span><span class="sxs-lookup"><span data-stu-id="88baa-120">**Element**</span></span>|<span data-ttu-id="88baa-121">**说明**</span><span class="sxs-lookup"><span data-stu-id="88baa-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88baa-122">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="88baa-122">UserOofSettings</span></span>](useroofsettings.md) <br/> |<span data-ttu-id="88baa-123">指定 OOF 设置。</span><span class="sxs-lookup"><span data-stu-id="88baa-123">Specifies the OOF settings.</span></span>  <br/> <span data-ttu-id="88baa-124">以下是此元素的 XPath 表达式：</span><span class="sxs-lookup"><span data-stu-id="88baa-124">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[<span data-ttu-id="88baa-125">OofSettings</span><span class="sxs-lookup"><span data-stu-id="88baa-125">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="88baa-126">包含 OOF 设置。</span><span class="sxs-lookup"><span data-stu-id="88baa-126">Contains the OOF settings.</span></span>  <br/> <span data-ttu-id="88baa-127">以下是此元素的 XPath 表达式：</span><span class="sxs-lookup"><span data-stu-id="88baa-127">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsResponse/OofSettings` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="88baa-128">备注</span><span class="sxs-lookup"><span data-stu-id="88baa-128">Remarks</span></span>

<span data-ttu-id="88baa-129">描述此元素的架构位于承载 Exchange Web Services 的 IIS 虚拟目录中。</span><span class="sxs-lookup"><span data-stu-id="88baa-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="88baa-130">示例</span><span class="sxs-lookup"><span data-stu-id="88baa-130">Example</span></span>

<span data-ttu-id="88baa-131">SetUserOofSettings 请求的下面的示例将[OofState](oofstate.md)设置为**已启用**，将 OOF 的持续时间设置为 10 天，并设置内部和外部 OOF 邮件。</span><span class="sxs-lookup"><span data-stu-id="88baa-131">The following example of a SetUserOofSettings request sets the [OofState](oofstate.md) to **Enabled**, sets the duration of OOF for 10 days, and sets the internal and external OOF messages.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetUserOofSettingsRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <Name>David Alexander</Name>
        <Address>someone@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
      <UserOofSettings xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <OofState>Enabled</OofState>
        <ExternalAudience>All</ExternalAudience>
        <Duration>
          <StartTime>2005-10-05T00:00:00</StartTime>
          <EndTime>2005-10-25T00:00:00</EndTime>
        </Duration>
        <InternalReply>
          <Message>I am out of office.  This is my internal reply.</Message>
        </InternalReply>
        <ExternalReply>
          <Message>I am out of office. This is my external reply.</Message>
        </ExternalReply>
      </UserOofSettings>
    </SetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="88baa-132">元素信息</span><span class="sxs-lookup"><span data-stu-id="88baa-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="88baa-133">命名空间</span><span class="sxs-lookup"><span data-stu-id="88baa-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="88baa-134">架构名称</span><span class="sxs-lookup"><span data-stu-id="88baa-134">Schema Name</span></span>  <br/> |<span data-ttu-id="88baa-135">类型架构</span><span class="sxs-lookup"><span data-stu-id="88baa-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="88baa-136">验证文件</span><span class="sxs-lookup"><span data-stu-id="88baa-136">Validation File</span></span>  <br/> |<span data-ttu-id="88baa-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="88baa-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="88baa-138">可以为空</span><span class="sxs-lookup"><span data-stu-id="88baa-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="88baa-139">False</span><span class="sxs-lookup"><span data-stu-id="88baa-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="88baa-140">另请参阅</span><span class="sxs-lookup"><span data-stu-id="88baa-140">See also</span></span>



[<span data-ttu-id="88baa-141">GetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="88baa-141">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
  
[<span data-ttu-id="88baa-142">SetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="88baa-142">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)
