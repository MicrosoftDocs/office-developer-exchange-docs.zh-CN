---
title: JournalFolderPermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- JournalFolderPermissionLevel
api_type:
- schema
ms.assetid: 564525fa-cd95-4c1a-9d6c-3806be664579
description: JournalFolderPermissionLevel 元素包含默认日记文件夹的权限。 在 Microsoft Exchange Server 2007 Service Pack 1 (SP1) 引入了此元素。
ms.openlocfilehash: 5c0f30932eb3fbbeef1a8e34611deeb1ffef402c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529047"
---
# <a name="journalfolderpermissionlevel"></a>JournalFolderPermissionLevel

**JournalFolderPermissionLevel**元素包含默认日记文件夹的权限。 在 Microsoft Exchange Server 2007 Service Pack 1 (SP1) 引入了此元素。 
  
```xml
<JournalFolderPermissionLevel>
   None or Editor or Reviewer or Author or Custom
</JournalFolderPermissionLevel>
```

 **DelegateFolderPermissionLevelType**
## <a name="attributes-and-elements"></a>属性和元素

下面各部分介绍了属性、子元素和父元素。
  
### <a name="attributes"></a>Attributes

无。
  
### <a name="child-elements"></a>子元素

无。
  
### <a name="parent-elements"></a>父元素

|**元素**|**说明**|
|:-----|:-----|
|[DelegatePermissions](delegatepermissions.md) <br/> |包含用户的代理权限级别设置。 在 Exchange 2007 SP1 引入了此元素。  <br/> |
   
## <a name="text-value"></a>文本值

下表列出了表示权限级别的文本值。
  
**权限级别文本值**

|**权限级别**|**说明**|
|:-----|:-----|
|无  <br/> |代理用户对 "日记" 文件夹没有访问权限。  <br/> |
|Reviewer  <br/> |代理用户可以读取 "日记" 文件夹中的项目。  <br/> |
|作者  <br/> |代理用户可以读取和创建 "日记" 文件夹中的项目。  <br/> |
|编辑器  <br/> |代理用户可以读取、创建和修改 "日记" 文件夹中的项目。  <br/> |
|自定义警报  <br/> |代理用户对 "日记" 文件夹具有自定义访问权限。  <br/> |
   
## <a name="remarks"></a>说明

描述此元素的架构位于正在运行 Microsoft Exchange Server 2007 的计算机（已安装客户端访问服务器角色）的 EWS 虚拟目录中。
  
## <a name="element-information"></a>元素信息

|||
|:-----|:-----|
|命名空间  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|架构名称  <br/> |类型架构  <br/> |
|验证文件  <br/> |Types.xsd  <br/> |
|可以为空  <br/> |False  <br/> |
   
## <a name="see-also"></a>另请参阅



[AddDelegate 操作](adddelegate-operation.md)
  
[UpdateDelegate 操作](updatedelegate-operation.md)


- [Exchange 中的 EWS XML 元素](ews-xml-elements-in-exchange.md)


[添加委派](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

