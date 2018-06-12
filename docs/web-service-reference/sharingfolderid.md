---
title: SharingFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SharingFolderId
api_type:
- schema
ms.assetid: 5ad37ceb-2922-4420-9051-c29d0d57c420
description: SharingFolderId 元素均表示共享关系中的本地文件夹的标识符。
ms.openlocfilehash: e0eb1fbd7155040508daf253f5eb4b1352d7426d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827485"
---
# <a name="sharingfolderid"></a>SharingFolderId

**SharingFolderId**元素均表示共享关系中的本地文件夹的标识符。 
  
```xml
<SharingFolderId Id="" ChangeKey="" />
```

 **FolderIdType**
## <a name="attributes-and-elements"></a>属性和元素

如下章节中介绍了属性、子元素和父元素。
  
### <a name="attributes"></a>属性

|**属性**|**说明**|
|:-----|:-----|
|Id  <br/> |包含一个字符串，标识 Exchange 存储中的文件夹。 此属性是必需的。  <br/> |
|更改密钥  <br/> |包含一个字符串，标识的文件夹的 Id 属性标识的版本。 此属性是可选的。 使用此属性以确保正确版本的文件夹使用。  <br/> |
   
### <a name="child-elements"></a>子元素

无。
  
### <a name="parent-elements"></a>父元素

|**元素**|**说明**|
|:-----|:-----|
|[RefreshSharingFolder](refreshsharingfolder.md) <br/> |定义一个请求刷新指定的本地文件夹。  <br/> |
|[GetSharingFolderResponse](getsharingfolderresponse.md) <br/> |定义[GetSharingFolder 操作](getsharingfolder-operation.md)请求的响应。  <br/> |
|[GetSharingFolderResponseMessage](getsharingfolderresponsemessage.md) <br/> |包含状态和的单个结果[GetSharingFolder 操作](getsharingfolder-operation.md)请求。  <br/> |
   
## <a name="remarks"></a>备注

描述该元素的架构位于 IIS 虚拟目录正在运行 Microsoft Exchange Server 的计算机的主机交换 Web 服务已安装了客户端访问服务器角色。
  
## <a name="element-information"></a>元素信息

|||
|:-----|:-----|
|命名空间  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|架构名称  <br/> |消息架构  <br/> |
|验证文件  <br/> |Messages.xsd  <br/> |
|可以为空  <br/> |False  <br/> |
   
## <a name="see-also"></a>另请参阅



- [在交换 EWS XML 元素](ews-xml-elements-in-exchange.md)
