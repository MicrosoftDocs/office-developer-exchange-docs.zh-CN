---
title: 项目
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Item
api_type:
- schema
ms.assetid: 4dfe8f48-e7b4-444d-bdf9-a34e180f598b
description: Item 元素表示 Exchange 存储中的一般项目。
ms.openlocfilehash: 72d8b1344bea3bcd105a0e293365b17f37193ac3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460314"
---
# <a name="item"></a>项目

**Item**元素表示 Exchange 存储中的一般项目。 
  
```xml
<Item>
   <MimeContent/>
   <ItemId/>
   <ParentFolderId/>
   <ItemClass/>
   <Subject/>
   <Sensitivity/>
   <Body/>
   <Attachments/>
   <DateTimeReceived/>
   <Size/>
   <Categories/>
   <Importance/>
   <InReplyTo/>
   <IsSubmitted/>
   <IsDraft/>
   <IsFromMe/>
   <IsResend/>
   <IsUnmodified/>
   <InternetMessageHeaders/>
   <DateTimeSent/>
   <DateTimeCreated/>
   <ResponseObjects/>
   <ReminderDueBy/>
   <ReminderIsSet/>
   <ReminderMinutesBeforeStart/>
   <DisplayCc/>
   <DisplayTo/>
   <HasAttachments/>
   <ExtendedProperty/>
   <Culture/>
   <EffectiveRights/>
   <LastModifiedName/>
   <LastModifiedTime/>
   <IsAssociated/>
   <WebClientReadFormQueryString/>
   <WebClientEditFormQueryString/>
   <ConversationId/>
   <UniqueBody/>
</Item>
```

 **ItemType**
## <a name="attributes-and-elements"></a>属性和元素

下面各部分介绍了属性、子元素和父元素。
  
### <a name="attributes"></a>Attributes

无。
  
### <a name="child-elements"></a>子元素

|**元素**|**说明**|
|:-----|:-----|
|[MimeContent](mimecontent.md) <br/> |包含以 base64Binary 格式表示的对象的本机多用途 Internet 邮件扩展（MIME）流。  <br/> |
|[ItemId](itemid.md) <br/> |包含 Exchange 存储中某项的唯一标识符和更改键。 此属性是只读的。  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |表示包含项或文件夹的父文件夹的标识符。 此属性是只读的。  <br/> |
|[ItemClass](itemclass.md) <br/> |表示项目的邮件类。  <br/> |
|[主题](subject.md) <br/> |表示 Exchange 存储项和响应对象的主题。 主题限制为255个字符。  <br/> |
|[Sensitivity](sensitivity.md) <br/> |指示项的敏感度级别。  <br/> |
|[Body](body.md) <br/> |表示邮件的实际正文内容。  <br/> |
|[附件](attachments-ex15websvcsotherref.md) <br/> |包含附加到 Exchange 存储中的项目的项目或文件。  <br/> |
|[DateTimeReceived](datetimereceived.md) <br/> |表示邮箱中的项目的接收日期和时间。  <br/> |
|[大小](size.md) <br/> |表示项的大小（以字节为单位）。 此属性是只读的。  <br/> |
|[类别](categories-ex15websvcsotherref.md) <br/> |表示一个字符串集合，这些字符串标识邮箱中的项目所属的类别。  <br/> |
|[Importance](importance.md) <br/> |介绍项的重要性。  <br/> |
|[InReplyTo](inreplyto.md) <br/> |表示此项是其回复项的标识符。  <br/> |
|[IsSubmitted](issubmitted.md) <br/> |指示是否已将项目提交到 "发件箱" 默认文件夹。  <br/> |
|[IsDraft](isdraft.md) <br/> |表示是否尚未发送某个项目。  <br/> |
|[IsFromMe](isfromme.md) <br/> |指示用户是否向其自身发送了项目。  <br/> |
|[IsResend](isresend.md) <br/> |指示以前是否已发送过该项目。  <br/> |
|[IsUnmodified](isunmodified.md) <br/> |指示项目是否已被修改。  <br/> |
|[Message](internetmessageheaders.md) <br/> |表示邮箱中的项目中包含的所有 Internet 邮件头的集合。  <br/> |
|[DateTimeSent](datetimesent.md) <br/> |表示邮箱中的项目的发送日期和时间。  <br/> |
|[DateTimeCreated](datetimecreated.md) <br/> |表示邮箱中的给定项目的创建日期和时间。  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |包含与 Exchange 存储中的项目关联的所有响应对象的集合。  <br/> |
|[ReminderDueBy](reminderdueby.md) <br/> |表示事件发生的日期和时间。 [ReminderMinutesBeforeStart](reminderminutesbeforestart.md)元素使用此元素来确定何时显示提醒。  <br/> |
|[ReminderIsSet](reminderisset.md) <br/> |指示是否已为 Exchange 存储中的某个项目设置提醒。  <br/> |
|[ReminderMinutesBeforeStart](reminderminutesbeforestart.md) <br/> |表示在显示提醒时事件之前的分钟数。  <br/> |
|[DisplayCc](displaycc.md) <br/> |表示用于 "抄送" 框中的内容的显示字符串。 这是所有 Cc 收件人显示名称的串联字符串。  <br/> |
|[DisplayTo](displayto.md) <br/> |表示用于 "To" 框中的内容的显示字符串。 这是所有收件人显示名称的串联字符串。  <br/> |
|[HasAttachments](hasattachments.md) <br/> |表示一个属性，如果一个项目至少有一个可见的附件，则设置为**true** 。 此属性是只读的。  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |标识文件夹和项的扩展属性。  <br/> |
|[Culture](culture.md) <br/> |表示邮箱中给定项目的区域性。  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |包含客户端的权利基础的项或文件夹的权限设置。此元素是只读的。  <br/> |
|[LastModifiedName](lastmodifiedname.md) <br/> |包含上次修改项目的用户的显示名称。  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |指示项目的上次修改时间。  <br/> |
|[IsAssociated](isassociated.md) <br/> |指示项目是否与文件夹相关联。  <br/> |
|[WebClientReadFormQueryString](webclientreadformquerystring.md) <br/> |表示连接到 Microsoft Office Outlook Web App 终结点以在 Outlook Web App 中读取项目的 URL。  <br/> |
|[WebClientEditFormQueryString](webclienteditformquerystring.md) <br/> |表示用于连接到 Outlook web App 终结点以在 Outlook Web App 中编辑项目的 URL。  <br/> |
|[ConversationId](conversationid.md) <br/> |包含项或对话的标识符。  <br/> |
|[UniqueBody](uniquebody.md) <br/> |表示一个 HTML 片段或纯文本，它表示此对话的唯一正文。  <br/> |
   
### <a name="parent-elements"></a>父元素

|**元素**|**说明**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> |介绍与会议时间相邻的所有日历项目。  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |标识在[UpdateItem 操作](updateitem-operation.md)过程中追加到项目/文件夹的单个属性的数据。  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |标识与会议时间冲突的所有项目。  <br/> |
|[创建（ItemSync）](create-itemsync.md) <br/> |标识要在本地客户端存储中创建的单个项目。  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |表示附加到另一个 Exchange 项目的 Exchange 项目。  <br/> |
|[Items](items.md) <br/> |包含项的数组。  <br/> |
|[项目（NonEmptyArrayOfAllItemsType）](items-nonemptyarrayofallitemstype.md) <br/> |包含要在由[ParentFolderId （TargetFolderIdType）](parentfolderid-targetfolderidtype.md)元素标识的文件夹中创建的项的数组。  <br/> |
|[SetItemField](setitemfield.md) <br/> |表示对[UpdateItem 操作](updateitem-operation.md)中项的单个属性的更新。  <br/> |
|[Update （ItemSync）](update-itemsync.md) <br/> |标识要在本地客户端存储中更新的单个项目。  <br/> |
   
## <a name="text-value"></a>文本值

无。
  
## <a name="remarks"></a>说明

请务必注意， **ItemType**是[Task](task.md)、 [CalendarItem](calendaritem.md)、 [Contact](contact.md)、 [DistributionList](distributionlist.md)和[Message](message-ex15websvcsotherref.md)的基本类型。
  
[Message](message-ex15websvcsotherref.md)元素表示电子邮件以及 Exchange Web 服务（EWS）架构未强类型化的所有其他项目。 项目，如 IPM。共享和 IPM. InfoPath 以**邮件**元素的形式返回。 Microsoft Exchange Server 2010 不会在响应中返回基本**项目**元素。 
  
描述此元素的架构位于承载 Exchange Web Services 的 IIS 虚拟目录中。
  
## <a name="element-information"></a>元素信息

|||
|:-----|:-----|
|命名空间  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|架构名称  <br/> |类型架构  <br/> |
|验证文件  <br/> |Types.xsd  <br/> |
|可以为空  <br/> |False  <br/> |
   
## <a name="see-also"></a>另请参阅



- [在交换 EWS XML 元素](ews-xml-elements-in-exchange.md)
  
[Exchange 的 EWS 引用](ews-reference-for-exchange.md)

