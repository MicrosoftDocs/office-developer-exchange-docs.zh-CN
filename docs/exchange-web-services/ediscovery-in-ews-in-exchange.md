---
title: 在交换中 EWS eDiscovery
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3128419f-dd5f-46d2-bb0d-0940738d0bb6
description: 了解 Exchange 中 EWS 的电子数据展示。
ms.openlocfilehash: 48e3fdb3a2f21f7dcfcb7eed21b586e099b249a3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456092"
---
# <a name="ediscovery-in-ews-in-exchange"></a>在交换中 EWS eDiscovery

了解 Exchange 中 EWS 的电子数据展示。
  
电子数据展示是一种联合查询 web 服务，它使外部应用程序能够执行 Exchange 数据的查询。
  
发现包括几个阶段，包括标识和保留关键数据、在法庭中剔除和查看数据以及生成数据。 电子数据展示查询通过跨 Exchange 和 SharePoint 提供单个发现工作流来促进发现过程。
  
## <a name="ediscovery-operations"></a>电子数据展示操作

通过 Exchange Online 中引入的操作、Exchange Online （作为 Office 365 的一部分）和从 Exchange 2013 开始的 Exchange 版本提供了由 EWS 公开的电子数据展示功能。 
  
**表1。电子数据展示的新操作**

|**操作名称**|**说明**|
|:-----|:-----|
|[GetDiscoverySearchConfiguration](https://msdn.microsoft.com/library/8a54a6dc-110c-4972-a8bc-5ddb43c4b857%28Office.15%29.aspx) <br/> |获取就地保留的配置信息、已保存的发现搜索以及为发现搜索启用的邮箱。  <br/> |
|[GetHoldOnMailboxes](https://msdn.microsoft.com/library/9157f329-80b4-4cd0-a158-378064966ae6%28Office.15%29.aspx) <br/> |获取基于查询的保留的状态，它是通过使用[SetHoldOnMailboxes 操作](https://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx)设置的。  <br/> |
|[GetNonIndexableItemDetails](https://msdn.microsoft.com/library/9279c3ad-f7c8-4bbc-b0a7-2c78416cb39a%28Office.15%29.aspx) <br/> |检索有关无法编制索引的项目的详细信息。 这包括但不限于项目标识符、错误代码、错误说明、对项目编制索引时，以及有关文件的其他信息。  <br/> |
|[GetNonIndexableItemStatistics](https://msdn.microsoft.com/library/ed077877-9d98-4434-b8b6-a4a905e7f7a6%28Office.15%29.aspx) <br/> |检索邮箱中无法编制索引的项目数。  <br/> |
|[GetSearchableMailboxes](https://msdn.microsoft.com/library/47f8ff57-4835-4d2d-9136-44afb31a4cbe%28Office.15%29.aspx) <br/> |获取客户端有权搜索或执行电子数据展示的邮箱的列表。  <br/> |
|[SearchMailboxes](https://msdn.microsoft.com/library/8a67c1d8-d021-4e68-aa62-35f7d9c2edc7%28Office.15%29.aspx) <br/> |搜索与查询关键字匹配的特定邮箱中的项目。  <br/> |
|[SetHoldOnMailboxes](https://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx) <br/> |设置项目的基于查询的保留。  <br/> |
   
## <a name="see-also"></a>另请参阅

- [开发 Exchange Web 服务客户端](develop-web-service-clients-for-exchange.md)
    
- [Start using web services in Exchange](start-using-web-services-in-exchange.md)
    
- [Exchange 的 EWS 客户端设计概述](ews-client-design-overview-for-exchange.md)
    

