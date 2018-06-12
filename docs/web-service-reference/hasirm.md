---
title: HasIrm
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fedc04e0-cfd2-4652-a2a8-51de859ae847
description: HasIrm 元素指定对话和当前文件夹中的至少一个邮件是否 IRM 受保护的邮件。
ms.openlocfilehash: c129370d7920da7cf1f9f32eed2f075e6c21cf8b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825803"
---
# <a name="hasirm"></a>HasIrm

**HasIrm**元素指定对话和当前文件夹中的至少一个邮件是否 IRM 受保护的邮件。 
  
```XML
<HasIrm> true | false </HasIrm>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性和元素

如下章节中介绍了属性、子元素和父元素。
  
### <a name="attributes"></a>属性

无。
  
### <a name="child-elements"></a>子元素

无。
  
### <a name="parent-elements"></a>父元素

[对话 (ConversationType)](conversation-conversationtype.md)
  
## <a name="text-value"></a>文本值

如果对话和当前文件夹中的至少一个邮件具有 IRM， **HasIrm**元素的文本值为**true** 。 否则，值为**false**。
  
## <a name="remarks"></a>备注

Exchange Server 2013 Service Pack 1 (SP1) 中引入了此元素。
  
描述此元素的架构位于承载 Exchange Web Services 的 IIS 虚拟目录中。
  
## <a name="element-information"></a>元素信息

|||
|:-----|:-----|
|命名空间  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|架构名称  <br/> |类型架构  <br/> |
|验证文件  <br/> |Types.xsd  <br/> |
|可以为空  <br/> |True  <br/> |
   
## <a name="see-also"></a>另请参阅



[对话 (ConversationType)](conversation-conversationtype.md)


- [在交换 EWS XML 元素](ews-xml-elements-in-exchange.md)
