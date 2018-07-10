---
title: SetTelephoneAccessFolderEmail （UM web 服务）
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetTelephoneAccessFolderEmail
api_type:
- schema
ms.assetid: 90759da7-6dba-499e-b8c8-e44a016b3198
description: SetTelephoneAccessFolderEmail 元素定义设置默认的电子邮件文件夹从其统一消息将阅读邮件通过电话的请求。
ms.openlocfilehash: e19f151e364411717d5129cbef8c5cc097689f89
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827461"
---
# <a name="settelephoneaccessfolderemail-um-web-service"></a><span data-ttu-id="5c168-103">SetTelephoneAccessFolderEmail （UM web 服务）</span><span class="sxs-lookup"><span data-stu-id="5c168-103">SetTelephoneAccessFolderEmail (UM web service)</span></span>

<span data-ttu-id="5c168-104">**SetTelephoneAccessFolderEmail**元素定义设置默认的电子邮件文件夹从其统一消息将阅读邮件通过电话的请求。</span><span class="sxs-lookup"><span data-stu-id="5c168-104">The **SetTelephoneAccessFolderEmail** element defines a request to set the default e-mail folder from which Unified Messaging will read messages over the telephone.</span></span> 
  
[<span data-ttu-id="5c168-105">SetTelephoneAccessFolderEmail （UM web 服务）</span><span class="sxs-lookup"><span data-stu-id="5c168-105">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md)
  
```xml
<SetTelephoneAccessFolderEmail>
  <base64FolderId>   </base64FolderId>
</SetTelephoneAccessFolderEmail>
```

 <span data-ttu-id="5c168-106">**complexType**</span><span class="sxs-lookup"><span data-stu-id="5c168-106">**complexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5c168-107">属性和元素</span><span class="sxs-lookup"><span data-stu-id="5c168-107">Attributes and elements</span></span>

<span data-ttu-id="5c168-108">如下章节中介绍了属性、子元素和父元素。</span><span class="sxs-lookup"><span data-stu-id="5c168-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5c168-109">属性</span><span class="sxs-lookup"><span data-stu-id="5c168-109">Attributes</span></span>

<span data-ttu-id="5c168-110">无。</span><span class="sxs-lookup"><span data-stu-id="5c168-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5c168-111">子元素</span><span class="sxs-lookup"><span data-stu-id="5c168-111">Child elements</span></span>

|<span data-ttu-id="5c168-112">**元素**</span><span class="sxs-lookup"><span data-stu-id="5c168-112">**Element**</span></span>|<span data-ttu-id="5c168-113">**说明**</span><span class="sxs-lookup"><span data-stu-id="5c168-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c168-114">base64FolderId （UM web 服务）</span><span class="sxs-lookup"><span data-stu-id="5c168-114">base64FolderId (UM web service)</span></span>](base64folderid-um-web-service.md) <br/> |<span data-ttu-id="5c168-115">电子邮件文件夹的标识符。</span><span class="sxs-lookup"><span data-stu-id="5c168-115">The identifier of the e-mail folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5c168-116">父元素</span><span class="sxs-lookup"><span data-stu-id="5c168-116">Parent elements</span></span>

<span data-ttu-id="5c168-117">无。</span><span class="sxs-lookup"><span data-stu-id="5c168-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="5c168-118">文本值</span><span class="sxs-lookup"><span data-stu-id="5c168-118">Text value</span></span>

<span data-ttu-id="5c168-119">无。</span><span class="sxs-lookup"><span data-stu-id="5c168-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5c168-120">元素信息</span><span class="sxs-lookup"><span data-stu-id="5c168-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5c168-121">命名空间</span><span class="sxs-lookup"><span data-stu-id="5c168-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5c168-122">架构名称</span><span class="sxs-lookup"><span data-stu-id="5c168-122">Schema Name</span></span>  <br/> |<span data-ttu-id="5c168-123">邮件</span><span class="sxs-lookup"><span data-stu-id="5c168-123">Messages</span></span>  <br/> |
|<span data-ttu-id="5c168-124">验证文件</span><span class="sxs-lookup"><span data-stu-id="5c168-124">Validation File</span></span>  <br/> |<span data-ttu-id="5c168-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5c168-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5c168-126">可以为空</span><span class="sxs-lookup"><span data-stu-id="5c168-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="5c168-127">False</span><span class="sxs-lookup"><span data-stu-id="5c168-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5c168-128">另请参阅</span><span class="sxs-lookup"><span data-stu-id="5c168-128">See also</span></span>



[<span data-ttu-id="5c168-129">SetTelephoneAccessFolderEmail 操作 （UM web 服务）</span><span class="sxs-lookup"><span data-stu-id="5c168-129">SetTelephoneAccessFolderEmail operation (UM web service)</span></span>](settelephoneaccessfolderemail-operation-um-web-service.md)
