---
title: mexRuntime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- mexRuntime
api_type:
- schema
ms.assetid: eabb2f12-10a7-4ce2-ae4b-9c04010c765f
description: 上次修改时间：2015年9月17日
ms.openlocfilehash: f192965a8375eb46d1ca5b46d3b768a3299c284d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461833"
---
# <a name="mexruntime"></a>mexRuntime
  
**适用于：** Exchange Server 2013
  
**MexRuntime**元素包含定义代理监视的配置信息和安装的 SMTP 和路由代理的配置信息的元素。 
  
- [configuration](configuration.md)  
- [mexRuntime](mexruntime.md)
  
```XML
<mexRuntime>
   <monitoring/>
   <agentList/>
</mexRuntime>
```

**mexRuntimeType （复杂类型）**

## <a name="attributes-and-elements"></a>属性和元素

下面各部分介绍了属性、子元素和父元素。
  
### <a name="attributes"></a>Attributes

无。
  
### <a name="child-elements"></a>子元素

|**元素**|**说明**|
|:-----|:-----|
|[监视](monitoring.md) <br/> |包含定义如何以及何时安装的传输监视器代理的配置信息。  <br/> |
|[agentList](agentlist.md) <br/> |包含已安装的每个代理的[代理](agent.md)元素。  <br/> |
   
### <a name="parent-elements"></a>父元素

|**元素**|**说明**|
|:-----|:-----|
|[configuration](configuration.md) <br/> |代理配置文件的根元素。  <br/> |
   
## <a name="element-information"></a>元素信息

|||
|:-----|:-----|
|命名空间  <br/> |此文件不定义命名空间。  <br/> |
|架构名称  <br/> |不可用。  <br/> |
|验证文件  <br/> |不可用。  <br/> |
|可以为空  <br/> |不正确。  <br/> |
   
## <a name="see-also"></a>另请参阅

- [Exchange 2013 的代理配置文件元素](agents-configuration-file-elements-for-exchange-2013.md)

