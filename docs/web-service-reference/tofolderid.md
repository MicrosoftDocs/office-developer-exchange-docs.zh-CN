---
title: ToFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ToFolderId
api_type:
- schema
ms.assetid: bd6a4265-ad40-43f6-bcc4-0bf5df4e984c
description: ToFolderId 元素表示复制或移动的项或文件夹的目标文件夹。
ms.openlocfilehash: c9cceb17fd55b7357d54b37bf4c8da1137d39b6a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468773"
---
# <a name="tofolderid"></a>ToFolderId

**ToFolderId**元素表示复制或移动的项或文件夹的目标文件夹。 
  
```xml
<ToFolderId>
   <FolderId/>
</ToFolderId>
```

```xml
<ToFolderId>
   <DistinguishedFolderId/>
</ToFolderId>
```

**TargetFolderIdType**

## <a name="attributes-and-elements"></a>属性和元素

下面各部分介绍了属性、子元素和父元素。
  
### <a name="attributes"></a>Attributes

无。
  
### <a name="child-elements"></a>子元素

|**元素**|**说明**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |包含用于复制或移动的项或文件夹的目标文件夹的标识符。  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |标识命名的目标文件夹复制或移动的项或文件夹。  <br/> |
   
### <a name="parent-elements"></a>父元素

|**元素**|**说明**|
|:-----|:-----|
|[MoveFolder](movefolder.md) <br/> |定义在 Exchange 存储中移动文件夹的请求。  <br/> 下面是此元素的 XPath 表达式：   <br/>  `/MoveFolder` <br/> |
|[CopyFolder](copyfolder.md) <br/> |定义在 Exchange 存储中复制文件夹的请求。  <br/> 下面是此元素的 XPath 表达式：   <br/>  `/CopyFolder` <br/> |
|[MoveItem](moveitem.md) <br/> |定义在 Exchange 存储中移动项目的请求。  <br/> 下面是此元素的 XPath 表达式：   <br/>  `/MoveItem` <br/> |
|[CopyItem](copyitem.md) <br/> |定义在 Exchange 存储中复制项目的请求。  <br/> 下面是此元素的 XPath 表达式：   <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a>说明

描述此元素的架构位于正在运行 MicrosoftExchange Server 2007 的计算机（已安装客户端访问服务器角色）的 EWS 虚拟目录中。
  
## <a name="element-information"></a>元素信息

|||
|:-----|:-----|
|命名空间  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|架构名称  <br/> |消息架构  <br/> |
|验证文件  <br/> |Messages.xsd  <br/> |
|可以为空  <br/> |False  <br/> |
   
## <a name="see-also"></a>另请参阅

- [MoveFolder 操作](movefolder-operation.md)  
- [CopyFolder 操作](copyfolder-operation.md) 
- [MoveItem 操作](moveitem-operation.md) 
- [CopyItem 操作](copyitem-operation.md)

