---
title: DescriptiveLinkKey
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DescriptiveLinkKey
api_type:
- schema
ms.assetid: f7f36749-00f3-4915-b17c-e3caa0af6e67
description: DescriptiveLinkKey 元素当前未使用，并保留以供将来使用。 它包含值0。
ms.openlocfilehash: e078d4ef4a629ea06bab0c2eb02b4f67b4fbf651
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467870"
---
# <a name="descriptivelinkkey"></a>DescriptiveLinkKey

**DescriptiveLinkKey**元素当前未使用，并保留以供将来使用。 它包含值0。 
  
```XML
<DescriptiveLinkKey/>
```

 **int**
## <a name="attributes-and-elements"></a>属性和元素

下面各部分介绍了属性、子元素和父元素。
  
### <a name="attributes"></a>Attributes

无。
  
### <a name="child-elements"></a>子元素

无。
  
### <a name="parent-elements"></a>父元素

|**元素**|**说明**|
|:-----|:-----|
|[ResponseMessage](responsemessage.md) <br/> | 提供有关响应状态的描述性信息。  <br/><br/>以下是此元素的一些可能的 XPath 表达式：<br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/ResponseMessage` <br/><br/>`/GetUserAvailabilityResponse/SuggestionsResponse/ResponseMessage` <br/><br/>`/SetUserOofSettingsResponse/ResponseMessage` <br/><br/>`/GetUserOofSettingsResponse/ResponseMessage` <br/> |
|[DeleteItemResponseMessage](deleteitemresponsemessage.md) <br/> |包含单个**DeleteItem**请求的状态和结果。  <br/> |
|[SendItemResponseMessage](senditemresponsemessage.md) <br/> |包含单个**SendItem**请求的状态和结果。  <br/> |
|[DeleteFolderResponseMessage](deletefolderresponsemessage.md) <br/> |包含单个**DeleteFolder**请求的状态和结果。  <br/> |
|[DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md) <br/> |包含单个**DeleteAttachment**请求的状态和结果。  <br/> |
|[UnsubscribeResponseMessage](unsubscriberesponsemessage.md) <br/> |包含单个**取消订阅**请求的状态和结果。  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |包含单个**CreateFolder**请求的状态和结果。  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |包含单个**GetFolder**请求的状态和结果。  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |包含单个**UpdateFolder**请求的状态和结果。  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |包含单个**MoveFolder**请求的状态和结果。  <br/> |
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |包含单个**CopyFolder**请求的状态和结果。  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |包含单个**CreateManagedFolder**请求的状态和结果。  <br/> |
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |包含单个**FindFolder**请求的状态和结果。  <br/> |
|[CreateItemResponseMessage](createitemresponsemessage.md) <br/> |包含单个**CreateItem**请求的状态和结果。  <br/> |
|[GetItemResponseMessage](getitemresponsemessage.md) <br/> |包含单个**GetItem**请求的状态和结果。  <br/> |
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |包含单个**UpdateItem**请求的状态和结果。  <br/> |
|[MoveItemResponseMessage](moveitemresponsemessage.md) <br/> |包含单个**MoveItem**请求的状态和结果。  <br/> |
|[CopyItemResponseMessage](copyitemresponsemessage.md) <br/> |包含单个**CopyItem**请求的状态和结果。  <br/> |
|[CreateAttachmentResponseMessage](createattachmentresponsemessage.md) <br/> |包含单个**CreateAttachment**请求的状态和结果。  <br/> |
|[GetAttachmentResponseMessage](getattachmentresponsemessage.md) <br/> |包含单个**GetAttachment**请求的状态和结果。  <br/> |
|[FindItemResponseMessage](finditemresponsemessage.md) <br/> |包含单个**FindItem**请求的状态和结果。  <br/> |
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |包含**ResolveNames**请求的状态和结果。  <br/> |
|[ExpandDLResponseMessage](expanddlresponsemessage.md) <br/> |包含单个**ExpandDL**请求的状态和结果。  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |包含单个**订阅**请求的状态和结果。  <br/> |
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |包含单个**GetEvents**请求的状态和结果。  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |包含单个**SendNotification**请求的状态和结果。  <br/> |
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |包含**SyncFolderHierarchy**请求的状态和结果。  <br/> |
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |包含**SyncFolderItems**请求的状态和结果。  <br/> |
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |包含**ConvertId**请求的状态和结果。  <br/> |
|[AddDelegateResponse](adddelegateresponse.md) <br/> |包含**AddDelegate**请求的状态和结果。  <br/> |
|[GetServerTimeZonesResponseMessage](getservertimezonesresponsemessage.md) <br/> |包含**GetServerTimeZones**请求的状态和结果。  <br/> |
|[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md) <br/> |包含**GetSharingFolder**请求的状态和结果。  <br/> |
|[GetSharingFolderResponse](getsharingfolderresponse.md) <br/> |定义对**GetSharingFolder**请求的响应。  <br/> |
|[GetSharingMetadataResponseMessage](getsharingmetadataresponsemessage.md) <br/> |包含**GetSharingMetadata**请求的状态和结果。  <br/> |
|[GetSharingMetadataResponse](getsharingmetadataresponse.md) <br/> |定义对**GetSharingMetadata**请求的响应。  <br/> |
|[RefreshSharingFolderResponseMessage](refreshsharingfolderresponsemessage.md) <br/> |包含**RefreshSharingFolder**请求的状态和结果。  <br/> |
|[RefreshSharingFolderResponse](refreshsharingfolderresponse.md) <br/> |定义对**RefreshSharingFolder**请求的响应。  <br/> |
|[FindConversationResponse](findconversationresponse.md) <br/> |包含**FindConversation**响应的状态和结果。  <br/> |
|[EmptyFolderResponseMessage](emptyfolderresponsemessage.md) <br/> |包含单个**EmptyFolder**请求的状态和结果。  <br/> |
|[UpdateInboxRulesResponse](updateinboxrulesresponse.md) <br/> |包含**UpdateInboxRules**请求的状态和结果。  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |包含**UploadItemsResponse**请求的状态和结果。  <br/> |
|[GetInboxRulesResponse](getinboxrulesresponse.md) <br/> |包含对**GetInboxRules**请求的响应。  <br/> |
|GetServiceConfigurationResponse  <br/> |包含对**GetServiceConfiguration**请求的响应。  <br/> |
|[ServiceConfigurationResponseMessageType](serviceconfigurationresponsemessagetype.md) <br/> |包含服务配置设置。  <br/> |
   
## <a name="text-value"></a>文本值

如果使用此元素，则需要一个 text 值。 此元素是只读的。
  
## <a name="remarks"></a>备注

此元素不是必需的，也不包含在所有响应中。
  
描述此元素的架构位于承载 Exchange Web Services 的 IIS 虚拟目录中。
  
## <a name="element-information"></a>元素信息

|||
|:-----|:-----|
|命名空间  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|架构名称  <br/> |消息架构  <br/> |
|验证文件  <br/> |Messages.xsd  <br/> |
|可以为空  <br/> |False  <br/> |
   
## <a name="see-also"></a>另请参阅

- [Exchange 的 EWS 引用](ews-reference-for-exchange.md) 
- [Exchange 中的 EWS XML 元素](ews-xml-elements-in-exchange.md)

