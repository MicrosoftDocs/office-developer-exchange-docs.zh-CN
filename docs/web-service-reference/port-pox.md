---
title: 端口（POX）
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 4046821a-d6f3-4764-82be-4011221ce7a3
description: Port 元素指定用于连接到存储区的端口。
ms.openlocfilehash: 2da59e03a57b44fb12d14368d1b585ba845eacfe
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464012"
---
# <a name="port-pox"></a>端口（POX）

**Port**元素指定用于连接到存储区的端口。 
  
[自动发现（POX）](autodiscover-pox.md)
  
[响应（POX）](response-pox.md)
  
[帐户（POX）](account-pox.md)
  
[协议（POX）](protocol-pox.md)
  
[端口（POX）](port-pox.md)
  
```xml
<Port/>
```

## <a name="attributes-and-elements"></a>属性和元素

下面各部分介绍了属性、子元素和父元素。
  
### <a name="attributes"></a>Attributes

无。
  
### <a name="child-elements"></a>子元素

无。
  
### <a name="parent-elements"></a>父元素

|**元素**|**说明**|
|:-----|:-----|
|[协议（POX）](protocol-pox.md) <br/> |包含用于将客户端连接到运行 Microsoft Exchange Server 2007 且安装了客户端访问服务器角色的计算机的规范。  <br/> |
   
## <a name="text-value"></a>文本值

该文本值表示用于访问 Exchange 服务器的端口。
  
## <a name="remarks"></a>备注

如果[Server （POX）](server-pox.md)元素包含 URL，则不使用该**端口**值。 
  
## <a name="see-also"></a>另请参阅



[Exchange 的 POX 自动发现 XML 元素](pox-autodiscover-xml-elements-for-exchange.md)

