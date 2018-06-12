---
title: InternalUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 4649baa9-eec9-426d-952b-361818c25fe0
description: InternalUrl 元素包含使用 MAPI/HTTP 协议客户端连接到通讯簿服务器或从用户的组织内部的用户的邮箱的 URL。
ms.openlocfilehash: 3823236081961128b31bb2c0f563062897c55814
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825950"
---
# <a name="internalurl-pox"></a>InternalUrl (POX)

**InternalUrl**元素包含使用 MAPI/HTTP 协议客户端连接到通讯簿服务器或从用户的组织内部的用户的邮箱的 URL。 
  
```XML
<InternalUrl/>
```

## <a name="attributes-and-elements"></a>属性和元素

如下章节中介绍了属性、子元素和父元素。
  
### <a name="attributes"></a>属性

无。
  
### <a name="child-elements"></a>子元素

无。
  
### <a name="parent-elements"></a>父元素

|**元素**|**说明**|
|:-----|:-----|
|[通讯簿 (POX)](addressbook-pox.md) <br/> |包含使用 MAPI/HTTP 协议客户端连接到通讯簿服务器的规范。  <br/> |
|[MailStore (POX)](mailstore-pox.md) <br/> |包含使用 MAPI/HTTP 协议来连接到用户邮箱的客户端的规范。  <br/> |
   
## <a name="text-value"></a>文本值

文本值表示可用于访问通讯簿服务器或从用户的组织内部的用户的邮箱的 URL。
  
## <a name="remarks"></a>备注

**InternalUrl**元素中可能存在一个响应，其中具有与**Type**属性值为"mapiHttp"[协议 (POX)](protocol-pox.md)元素。 
  
**InternalUrl**元素是可用于实现 MAPI/HTTP 协议和目标 Exchange Online、 Exchange Online 作为 Office 365 的一部分的客户端和 Exchange 开头的本地版本构建 15.00.0847.032 (Exchange Server 2013 SP1). 
  
## <a name="see-also"></a>另请参阅



[Exchange POX 自动发现 XML 元素](pox-autodiscover-xml-elements-for-exchange.md)
