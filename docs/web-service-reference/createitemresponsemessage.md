---
title: CreateItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItemResponseMessage
api_type:
- schema
ms.assetid: 595d36c2-f87a-4d50-8e8b-f58d7641564b
description: CreateItemResponseMessage 元素包含单个 CreateItem 操作请求的状态和结果。
ms.openlocfilehash: 6304d2c7a3c9253c03c07eb37e9a57226e794a24
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457849"
---
# <a name="createitemresponsemessage"></a>CreateItemResponseMessage

**CreateItemResponseMessage**元素包含单个[CreateItem 操作](createitem-operation.md)请求的状态和结果。 
  
- [CreateItemResponse](createitemresponse.md)  
- [ResponseMessages](responsemessages.md) 
- [CreateItemResponseMessage](createitemresponsemessage.md)
  
```xml
<CreateItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
</CreateItemResponseMessage>
```

 **ItemInfoResponseMessageType**
## <a name="attributes-and-elements"></a>属性和元素

下面各部分介绍了属性、子元素和父元素。
  
### <a name="attributes"></a>Attributes

|**属性**|**说明**|
|:-----|:-----|
|**ResponseClass** <br/> | 描述[CreateItem 操作](createitem-operation.md)响应的状态。<br/><br/>以下值对此属性有效：<br/><br/>-成功  <br/>-警告  <br/>-错误  <br/> |
   
#### <a name="responseclass-attribute-values"></a>ResponseClass 属性值

|**值**|**说明**|
|:-----|:-----|
|**Success** <br/> |描述已完成的请求。  <br/> |
|**警告** <br/> | 介绍未处理的请求。 如果在处理请求中的项目时出现错误，并且无法处理后续项目，则可能会返回一个警告。<br/><br/>以下是警告源的示例：<br/><br/>-Exchange 存储在批处理过程中处于脱机状态。  <br/>-Active Directory 域服务（AD DS）处于脱机状态。  <br/>-移动邮箱。  <br/>-邮件数据库（MDB）处于脱机状态。  <br/>-密码已过期。  <br/>-超出配额。  <br/> |
|**Error** <br/> | 介绍无法满足的请求。<br/><br/>以下是错误源的示例：  <br/><br/>-属性或元素无效  <br/>-属性或元素越界  <br/>-未知标记  <br/>-Context 中的属性或元素无效  <br/>-任何客户端的未经授权访问尝试  <br/>-响应有效客户端调用的服务器端故障<br/><br/>  有关错误的信息可以在[ResponseCode](responsecode.md)和[MessageText](messagetext.md)元素中找到。  <br/> |
   
### <a name="child-elements"></a>子元素

|**元素**|**描述**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |提供响应状态的文本说明。  <br/> |
|[ResponseCode](responsecode.md) <br/> |提供用于标识请求遇到的特定错误的错误代码。  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |当前未使用，并保留以供将来使用。 它包含值0。  <br/> |
|[MessageXml](messagexml.md) <br/> |提供其他错误响应信息。  <br/> |
|[Items](items.md) <br/> |包含已创建项的数组。  <br/> |
   
### <a name="parent-elements"></a>父元素

|**元素**|**描述**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |包含 Exchange Web 服务请求的响应消息。  <br/> |
   
## <a name="remarks"></a>备注

描述此元素的架构位于运行 Microsoft Exchange Server 2010 且安装了客户端访问服务器角色的计算机的 EWS 虚拟目录中。
  
## <a name="element-information"></a>元素信息

|||
|:-----|:-----|
|命名空间  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|架构名称  <br/> |消息架构  <br/> |
|验证文件  <br/> |Messages.xsd  <br/> |
|可以为空  <br/> |False  <br/> |
   
## <a name="see-also"></a>另请参阅

- [CreateItem 操作](createitem-operation.md)
- [Exchange 的 EWS 引用](ews-reference-for-exchange.md)
- [Exchange 中的 EWS XML 元素](ews-xml-elements-in-exchange.md)

