---
title: EndTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndTime
api_type:
- schema
ms.assetid: 82e4ef4f-a557-4044-b9b7-d91622f4ac55
description: EndTime 元素表示时间跨度的结束。
ms.openlocfilehash: 5a30b32ecfeafe582cd07dd662aacb0a960257c9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462990"
---
# <a name="endtime"></a>EndTime

**EndTime**元素表示时间跨度的结束。 
  
```xml
<EndTime>dateTime</EndTime>
```

 **dateTime**
## <a name="attributes-and-elements"></a>属性和元素

下面各部分介绍了属性、子元素和父元素。
  
### <a name="attributes"></a>Attributes

无。
  
### <a name="child-elements"></a>子元素

无。
  
### <a name="parent-elements"></a>父元素

|**元素**|**说明**|
|:-----|:-----|
|[TimeWindow](timewindow.md) <br/> |标识查询的用户可用性信息的时间跨度。<br/><br/> 下面是此元素的 XPath 表达式： <br/><br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions/TimeWindow` <br/> |
|[DetailedSuggestionsWindow](detailedsuggestionswindow.md) <br/> |标识查询的时间跨度，以获取有关建议会议时间的详细信息。<br/><br/> 下面是此元素的 XPath 表达式： <br/><br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow`.  <br/> |
|[持续时间（UserOofSettings）](duration-useroofsettings.md) <br/> | 指定在[OofState](oofstate.md)元素设置为 "已**计划**" 时启用 "外出" （OOF）状态的持续时间。  <br/><br/>  以下是此元素的可能的 XPath 表达式：<br/><br/>  `/SetUserOofSettingsRequest/UserOofSettings/Duration` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/Duration` <br/> |
|[重复](occurrence.md) <br/> |代表定期日历项目的单个修改事件。  <br/> |
|[CalendarEvent](calendarevent.md) <br/> |代表唯一的日历项目事件。 这用于可用性查询。 **CalendarEvent**元素中的**EndTime**元素是必需的。 **CalendarEvent**元素中的**EndTime**元素对于**CalendarEvent**类型是唯一的。<br/><br/> 下面是此元素的 XPath 表达式： <br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a>文本值

文本值是必需的。
  
## <a name="remarks"></a>说明

[StartTime](starttime.md)元素表示时间范围的开始。 
  
结束时间表示客户端的时间。
  
架构包含许多[EndTime](endtime.md)元素。 
  
> [!NOTE]
> 描述此元素的架构位于正在运行 MicrosoftExchange Server 2007 的计算机（已安装客户端访问服务器角色）的 EWS 虚拟目录中。 
  
## <a name="element-information"></a>元素信息

|||
|:-----|:-----|
|命名空间  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|架构名称  <br/> |类型架构  <br/> |
|验证文件  <br/> |Types.xsd  <br/> |
|可以为空  <br/> |False  <br/> |
   
## <a name="see-also"></a>另请参阅

- [GetUserAvailability 操作](getuseravailability-operation.md)
- [获取用户可用性](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

