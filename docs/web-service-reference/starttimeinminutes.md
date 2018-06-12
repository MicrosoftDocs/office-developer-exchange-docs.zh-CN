---
title: StartTimeInMinutes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StartTimeInMinutes
api_type:
- schema
ms.assetid: 0fb60a78-6e79-4601-8e2f-5bd245c46d69
description: StartTimeInMinutes 元素均表示邮箱用户的工作日的开始。
ms.openlocfilehash: f3f1d26731d0406ff8a0fd45fc0243a9feabf886
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827558"
---
# <a name="starttimeinminutes"></a>StartTimeInMinutes

**StartTimeInMinutes**元素均表示邮箱用户的工作日的开始。 
  
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
- [FreeBusyResponseArray](freebusyresponsearray.md)
  
- [FreeBusyResponse](freebusyresponse.md)
  
- [FreeBusyView](freebusyview.md)
  
- [WorkingHours](workinghours-ex15websvcsotherref.md)
  
- [WorkingPeriodArray](workingperiodarray.md)
  
- [WorkingPeriod](workingperiod.md)
  
- [StartTimeInMinutes](starttimeinminutes.md)
  
```xml
<StartTimeInMinutes>...</StartTimeInMinutes>
```

**int**

## <a name="attributes-and-elements"></a>属性和元素

如下章节中介绍了属性、子元素和父元素。
  
### <a name="attributes"></a>属性

无。
  
### <a name="child-elements"></a>子元素

无。
  
### <a name="parent-elements"></a>父元素

|**元素**|**说明**|
|:-----|:-----|
|[WorkingPeriod](workingperiod.md) <br/> |包含工作周的那几天和邮箱用户的时间。  <br/> 以下是此元素的 XPath 表达式：  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray/WorkingPeriod` <br/> |
   
## <a name="text-value"></a>文本值

文本值是必需的。 文本值的某一天开始以来经过多少分钟表示工作日的开始。 例如，上午 8 点开始时间 表示由 480 分钟。
  
此元素的可能值的范围是 0 到 1440年。
  
## <a name="remarks"></a>备注

描述此元素的架构位于正在运行 MicrosoftExchange Server 2007 的计算机（已安装客户端访问服务器角色）的 EWS 虚拟目录中。
  
## <a name="element-information"></a>元素信息

|||
|:-----|:-----|
|命名空间  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|架构名称  <br/> |类型架构  <br/> |
|验证文件  <br/> |Types.xsd  <br/> |
|可以为空  <br/> |False  <br/> |
   
## <a name="see-also"></a>另请参阅

- [GetUserAvailability 操作](getuseravailability-operation.md)
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)
- [Getting User Availability](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)
