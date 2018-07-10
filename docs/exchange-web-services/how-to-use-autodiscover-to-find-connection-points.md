---
title: 使用 Autodiscover 以查找连接点
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 03896542-549b-4c45-973c-98f9025ea26c
description: 了解如何使用自动发现服务来定向客户端应用程序，到正确的 Exchange 服务器。
ms.openlocfilehash: 653fcd1c094c23c3e89e903b7194b96720802b51
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752895"
---
# <a name="use-autodiscover-to-find-connection-points"></a><span data-ttu-id="e228c-103">使用 Autodiscover 以查找连接点</span><span class="sxs-lookup"><span data-stu-id="e228c-103">Use Autodiscover to find connection points</span></span>

<span data-ttu-id="e228c-104">了解如何使用自动发现服务来定向客户端应用程序，到正确的 Exchange 服务器。</span><span class="sxs-lookup"><span data-stu-id="e228c-104">Find out how to use the Autodiscover service to direct your client application to the correct Exchange server.</span></span>
  
<span data-ttu-id="e228c-105">Exchange 自动发现服务客户端应用程序提供承载的电子邮件帐户配置设置 Exchange Online、 Exchange Online 作为 Office 365 的一部分或运行的 Exchange 版本的 Exchange 服务器上启动与 Exchange2013。</span><span class="sxs-lookup"><span data-stu-id="e228c-105">The Exchange Autodiscover service provides your client application with configuration settings for email accounts that are hosted on Exchange Online, Exchange Online as part of Office 365, or an Exchange server running a version of Exchange starting with Exchange 2013.</span></span> <span data-ttu-id="e228c-106">自动发现服务是一种 web 服务，提供配置设置。</span><span class="sxs-lookup"><span data-stu-id="e228c-106">The Autodiscover service is a web service that provides configuration settings.</span></span> <span data-ttu-id="e228c-107">自动发现服务是一种 web 服务，提供 Exchange 服务器到客户端应用程序的配置信息。</span><span class="sxs-lookup"><span data-stu-id="e228c-107">The Autodiscover service is a web service that provides Exchange server configuration information to your client application.</span></span> <span data-ttu-id="e228c-108">客户端应用程序使用自动发现可确定特定邮箱的自动发现服务的终结点。</span><span class="sxs-lookup"><span data-stu-id="e228c-108">Client applications use Autodiscover to determine the endpoint of the Autodiscover service for a specific mailbox.</span></span> <span data-ttu-id="e228c-109">本文介绍如何执行从 Exchange 服务器以查找正确的终结点的响应。</span><span class="sxs-lookup"><span data-stu-id="e228c-109">This article explains how to follow the responses from an Exchange server to find the correct endpoint.</span></span> 
  
<span data-ttu-id="e228c-110">有关如何获取电子邮件地址配置设置的信息，请参阅[获取使用自动发现 Exchange 中的用户设置](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)和[获取从 Exchange 服务器的域设置](how-to-get-domain-settings-from-an-exchange-server.md)。</span><span class="sxs-lookup"><span data-stu-id="e228c-110">For information about how to get email address configuration settings, see [Get user settings from Exchange by using Autodiscover](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) and [Get domain settings from an Exchange server](how-to-get-domain-settings-from-an-exchange-server.md).</span></span>
  
> [!NOTE]
> <span data-ttu-id="e228c-111">查找正确的终结点的过程的用户或域设置请求的一部分。</span><span class="sxs-lookup"><span data-stu-id="e228c-111">The process for finding the correct endpoint is part of the request for user or domain settings.</span></span> <span data-ttu-id="e228c-112">自动发现服务使用的重定向响应的一系列发送电子邮件地址的正确终结点将客户端应用程序。</span><span class="sxs-lookup"><span data-stu-id="e228c-112">The Autodiscover service uses a series of redirect responses to send the client application to the correct endpoint for an email address.</span></span> 
  
<span data-ttu-id="e228c-113">您可以使用以下 Exchange 开发技术之一访问自动发现服务：</span><span class="sxs-lookup"><span data-stu-id="e228c-113">You can use one of the following Exchange development technologies to access the Autodiscover service:</span></span>
  
> [!NOTE]
> <span data-ttu-id="e228c-114">有关这些 Exchange 开发技术的详细信息，请参阅[在 Exchange 浏览 EWS 托管 API 和 EWS，web services](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)。</span><span class="sxs-lookup"><span data-stu-id="e228c-114">For more information about these Exchange development technologies, see [Explore the EWS Managed API, EWS, and web services in Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md).</span></span> 
  
- <span data-ttu-id="e228c-115">Exchange Web Services (EWS) 托管的 API</span><span class="sxs-lookup"><span data-stu-id="e228c-115">The Exchange Web Services (EWS) Managed API</span></span>
    
- <span data-ttu-id="e228c-116">EWS</span><span class="sxs-lookup"><span data-stu-id="e228c-116">EWS</span></span>
    
    <span data-ttu-id="e228c-117">如果您使用 EWS，您可以使用以下方法检索用户设置：</span><span class="sxs-lookup"><span data-stu-id="e228c-117">If you are using EWS, you can use the following methods to retrieve user settings:</span></span>
    
  - <span data-ttu-id="e228c-118">基于 SOAP 的自动发现服务</span><span class="sxs-lookup"><span data-stu-id="e228c-118">The SOAP-based Autodiscover service</span></span>
    
  - <span data-ttu-id="e228c-119">XML (POX) 自动发现服务</span><span class="sxs-lookup"><span data-stu-id="e228c-119">The XML (POX) Autodiscover service</span></span>
    
  - <span data-ttu-id="e228c-120">生成从 SOAP 或 XML 自动发现服务自动生成代理</span><span class="sxs-lookup"><span data-stu-id="e228c-120">An autogenerated proxy generated from the SOAP or XML Autodiscover service</span></span>
    
    <span data-ttu-id="e228c-121">有关这些方法的详细信息，请参阅[exchange 自动发现](autodiscover-for-exchange.md)。</span><span class="sxs-lookup"><span data-stu-id="e228c-121">For more information about these methods, see [Autodiscover for Exchange](autodiscover-for-exchange.md).</span></span>
    
<span data-ttu-id="e228c-122">EWS 托管 API 以检索用户设置提供基于对象的接口。</span><span class="sxs-lookup"><span data-stu-id="e228c-122">The EWS Managed API provides an object-based interface for retrieving user settings.</span></span> <span data-ttu-id="e228c-123">如果您的客户端应用程序使用托管的代码，我们建议您使用 EWS 托管 API。</span><span class="sxs-lookup"><span data-stu-id="e228c-123">If your client application uses managed code, we recommend that you use the EWS Managed API.</span></span> <span data-ttu-id="e228c-124">EWS 托管 API 界面更好地专为一个简单的对象模型比典型的自动生成 web 服务代理。</span><span class="sxs-lookup"><span data-stu-id="e228c-124">The EWS Managed API interface is better optimized for a simple object model than the typical autogenerated web service proxy.</span></span> 
  
<span data-ttu-id="e228c-125">如果您使用 EWS，我们建议您使用 SOAP 自动发现服务，因为它支持比 POX 自动发现服务更丰富的功能。</span><span class="sxs-lookup"><span data-stu-id="e228c-125">If you are using EWS, we suggest that you use the SOAP Autodiscover service, because it supports a richer set of features than the POX Autodiscover service.</span></span>
  
## <a name="prerequisites-for-finding-an-endpoint"></a><span data-ttu-id="e228c-126">查找终结点的先决条件</span><span class="sxs-lookup"><span data-stu-id="e228c-126">Prerequisites for finding an endpoint</span></span>
<span data-ttu-id="e228c-127"><a name="bk_Prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="e228c-127"></span></span>

<span data-ttu-id="e228c-128">您可以创建使用自动发现服务的客户端应用程序之前，您需要有权访问以下：</span><span class="sxs-lookup"><span data-stu-id="e228c-128">Before you can create a client application that uses the Autodiscover service, you need to have access to the following:</span></span>
  
- <span data-ttu-id="e228c-129">Exchange Online 或正在运行的 Exchange 版本开始 Exchange 2007 sp1 的服务器。</span><span class="sxs-lookup"><span data-stu-id="e228c-129">Exchange Online or a server that is running a version of Exchange starting with Exchange 2007 SP1.</span></span> <span data-ttu-id="e228c-130">如果您使用基于 SOAP 的自动发现服务、 Exchange Online 或 Exchange 启动与 Exchange 2010 的版本。</span><span class="sxs-lookup"><span data-stu-id="e228c-130">If you are using the SOAP-based Autodiscover service, Exchange Online or a version of Exchange starting with Exchange 2010.</span></span>
    
- <span data-ttu-id="e228c-131">Exchange 服务器配置为接受来自客户端应用程序的连接。</span><span class="sxs-lookup"><span data-stu-id="e228c-131">An Exchange server that is configured to accept connections from your client application.</span></span> <span data-ttu-id="e228c-132">有关如何配置您的 Exchange 服务器的信息，请参阅[在 Exchange 控制客户端应用程序访问 EWS](controlling-client-application-access-to-ews-in-exchange.md)。</span><span class="sxs-lookup"><span data-stu-id="e228c-132">For information about how to configure your Exchange server, see [Controlling client application access to EWS in Exchange](controlling-client-application-access-to-ews-in-exchange.md).</span></span>
    
- <span data-ttu-id="e228c-133">有权使用 EWS 帐户。</span><span class="sxs-lookup"><span data-stu-id="e228c-133">An account that is authorized to use EWS.</span></span> <span data-ttu-id="e228c-134">有关如何配置帐户的信息，请参阅[在 Exchange 控制客户端应用程序访问 EWS](controlling-client-application-access-to-ews-in-exchange.md)。</span><span class="sxs-lookup"><span data-stu-id="e228c-134">For information about how to configure an account, see [Controlling client application access to EWS in Exchange](controlling-client-application-access-to-ews-in-exchange.md).</span></span>
    
> [!NOTE]
> <span data-ttu-id="e228c-135">如果您使用 EWS 托管 API，您必须提供在某些情况下证书验证回调。</span><span class="sxs-lookup"><span data-stu-id="e228c-135">If you are using the EWS Managed API, you must provide a certificate validation callback in some circumstances.</span></span> <span data-ttu-id="e228c-136">您可能还需要使用某些生成的代理库，如那些通过 Visual Studio 创建的证书验证回调。</span><span class="sxs-lookup"><span data-stu-id="e228c-136">You may also need a certificate validation callback with some generated proxy libraries, such as those created by Visual Studio.</span></span> <span data-ttu-id="e228c-137">有关详细信息，请参阅[验证 EWS 托管 API 服务器证书](how-to-validate-a-server-certificate-for-the-ews-managed-api.md)。</span><span class="sxs-lookup"><span data-stu-id="e228c-137">For more information, see [Validate a server certificate for the EWS Managed API](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).</span></span> 
  
### <a name="core-concepts-for-finding-an-endpoint"></a><span data-ttu-id="e228c-138">查找终结点的核心概念</span><span class="sxs-lookup"><span data-stu-id="e228c-138">Core concepts for finding an endpoint</span></span>
<span data-ttu-id="e228c-139"><a name="bk_Core"> </a></span><span class="sxs-lookup"><span data-stu-id="e228c-139"></span></span>

<span data-ttu-id="e228c-140">您使用自动发现查找终结点之前，您应熟悉以下表中列出的概念。</span><span class="sxs-lookup"><span data-stu-id="e228c-140">Before you use Autodiscover to find an endpoint, you should be familiar with the concepts listed in the following table.</span></span>
  
|<span data-ttu-id="e228c-141">**概念**</span><span class="sxs-lookup"><span data-stu-id="e228c-141">**Concept**</span></span>|<span data-ttu-id="e228c-142">**说明**</span><span class="sxs-lookup"><span data-stu-id="e228c-142">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e228c-143">Exchange 自动发现</span><span class="sxs-lookup"><span data-stu-id="e228c-143">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md) <br/> |<span data-ttu-id="e228c-144">提供自动发现服务的工作原理的概述。</span><span class="sxs-lookup"><span data-stu-id="e228c-144">Provides an overview of how the Autodiscover service works.</span></span>  <br/> |
   
<span data-ttu-id="e228c-145">如果您使用 EWS 托管 API，您使用[Microsoft.Exchange.WebServices.Data.ExchangeService](http://msdn.microsoft.com/zh-cn/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)类[Microsoft.Exchange.WebServices.Data](http://msdn.microsoft.com/zh-cn/library/dd633907%28v=exchg.80%29.aspx)命名空间中管理与 EWS 的连接。</span><span class="sxs-lookup"><span data-stu-id="e228c-145">If you are using the EWS Managed API, you use the [Microsoft.Exchange.WebServices.Data.ExchangeService](http://msdn.microsoft.com/zh-cn/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) class in the [Microsoft.Exchange.WebServices.Data](http://msdn.microsoft.com/zh-cn/library/dd633907%28v=exchg.80%29.aspx) namespace to manage your connection to EWS.</span></span> <span data-ttu-id="e228c-146">要使用本文中的 EWS 托管 API 代码示例，您需要以引用您的代码中的以下命名空间：</span><span class="sxs-lookup"><span data-stu-id="e228c-146">To use the EWS Managed API code samples in this article, you need to reference the following namespaces in your code:</span></span> 
  
- <span data-ttu-id="e228c-147">**System.Net**</span><span class="sxs-lookup"><span data-stu-id="e228c-147">**System.Net**</span></span>
    
- <span data-ttu-id="e228c-148">**Microsoft.Exchange.WebServices.Data.ExchangeService**</span><span class="sxs-lookup"><span data-stu-id="e228c-148">**Microsoft.Exchange.WebServices.Data.ExchangeService**</span></span>
    
## <a name="find-the-correct-endpoint-by-using-the-ews-managed-api"></a><span data-ttu-id="e228c-149">使用 EWS 托管 API 来查找正确的终结点</span><span class="sxs-lookup"><span data-stu-id="e228c-149">Find the correct endpoint by using the EWS Managed API</span></span>
<span data-ttu-id="e228c-150"><a name="bk_Managed"> </a></span><span class="sxs-lookup"><span data-stu-id="e228c-150"></span></span>

<span data-ttu-id="e228c-151">如果您使用 EWS 托管 API，由**ExchangeService**类处理对自动发现服务的调用。</span><span class="sxs-lookup"><span data-stu-id="e228c-151">If you are using the EWS Managed API, calls to the Autodiscover service are handled by the **ExchangeService** class.</span></span> <span data-ttu-id="e228c-152">若要确定正确的终结点的电子邮件帐户，请 **[ExchangeService]** 对象上调用**AutodiscoverUrl**方法。</span><span class="sxs-lookup"><span data-stu-id="e228c-152">To determine the correct endpoint for an email account, you call the **AutodiscoverUrl** method on an **[ExchangeService]** object.</span></span> <span data-ttu-id="e228c-153">下面的代码示例演示如何使用 EWS 托管 API Exchange.asmx 文件正确的客户端访问服务器上设置电子邮件地址的 EWS web 服务终结点。</span><span class="sxs-lookup"><span data-stu-id="e228c-153">The following code example shows how to set the EWS web service endpoint for an email address to the Exchange.asmx file on the correct Client Access server by using the EWS Managed API.</span></span> 
  
```cs
NetworkCredential credentials = new NetworkCredential(securelyStoredEmail, securelyStoredPassword);
ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2013);
service.Credentials = credentials;
service.AutodiscoverUrl("User1@contoso.com");
```

## <a name="find-the-correct-endpoint-by-using-ews"></a><span data-ttu-id="e228c-154">使用 EWS 查找正确的终结点</span><span class="sxs-lookup"><span data-stu-id="e228c-154">Find the correct endpoint by using EWS</span></span>
<span data-ttu-id="e228c-155"><a name="bk_SOAP"> </a></span><span class="sxs-lookup"><span data-stu-id="e228c-155"></span></span>

<span data-ttu-id="e228c-156">SOAP 自动发现服务可能使用的请求和响应的一系列定向到正确的终结点 EWS 的应用程序。</span><span class="sxs-lookup"><span data-stu-id="e228c-156">The SOAP Autodiscover service may use a series of requests and responses to direct your application to the correct endpoint for EWS.</span></span> <span data-ttu-id="e228c-157">有关确定的电子邮件帐户的正确终结点的过程的信息，请参阅[exchange 自动发现](autodiscover-for-exchange.md)。</span><span class="sxs-lookup"><span data-stu-id="e228c-157">For information about the process for determining the correct endpoint for an email account, see [Autodiscover for Exchange](autodiscover-for-exchange.md).</span></span> <span data-ttu-id="e228c-158">下面的 XML 示例演示请求和响应，您可以预期发出 SOAP 自动发现请求以查找正确的终结点时的系列。</span><span class="sxs-lookup"><span data-stu-id="e228c-158">The following XML examples show the series of requests and responses that you can expect when making a SOAP Autodiscover request to find the correct endpoint.</span></span>
  
### <a name="soap-autodiscover-endpoint-request"></a><span data-ttu-id="e228c-159">SOAP 自动发现终结点请求</span><span class="sxs-lookup"><span data-stu-id="e228c-159">SOAP Autodiscover endpoint request</span></span>

<span data-ttu-id="e228c-160">下面的示例演示发送到自动发现服务以查找正确的终结点的 XML 请求。</span><span class="sxs-lookup"><span data-stu-id="e228c-160">The following example shows an XML request that is sent to the Autodiscover service to find the correct endpoint.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:wsa="http://www.w3.org/2005/08/addressing" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2013</a:RequestedServerVersion>
    <wsa:Action>http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://mail.microsoft.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <a:Request>
        <a:Users>
          <a:User>
            <a:Mailbox>User1@Contoso.com</a:Mailbox>
          </a:User>
        </a:Users>
        <a:RequestedSettings>
          <a:Setting>InternalEwsUrl</a:Setting>
          <a:Setting>ExternalEwsUrl</a:Setting>
        </a:RequestedSettings>
      </a:Request>
    </a:GetUserSettingsRequestMessage>
  </soap:Body>
</soap:Envelope>

```

### <a name="soap-autodiscover-redirection-response"></a><span data-ttu-id="e228c-161">SOAP 自动发现重定向响应</span><span class="sxs-lookup"><span data-stu-id="e228c-161">SOAP Autodiscover redirection response</span></span>

<span data-ttu-id="e228c-162">自动发现服务会使用两种重定向响应之一响应： HTTP 302 重定向或 SOAP 重定向响应。</span><span class="sxs-lookup"><span data-stu-id="e228c-162">The Autodiscover service may respond with one of two redirection responses: an HTTP 302 redirect, or a SOAP redirection response.</span></span> <span data-ttu-id="e228c-163">如果从 Exchange 服务器响应 HTTP 302 重定向，客户端应用程序应验证重定向地址是可以接受，然后按照重定向响应。</span><span class="sxs-lookup"><span data-stu-id="e228c-163">If the response from the Exchange server is an HTTP 302 redirect, the client application should validate that the redirection address is acceptable and then follow the redirection response.</span></span>
  
> [!安全注释]<span data-ttu-id="e228c-164"> 条件验证重定向响应，请参阅[exchange 自动发现](autodiscover-for-exchange.md)。</span><span class="sxs-lookup"><span data-stu-id="e228c-164"> For criteria for validating a redirection response, see [Autodiscover for Exchange](autodiscover-for-exchange.md).</span></span> 
  
<span data-ttu-id="e228c-165">如果自动发现服务将返回一个重定向响应，指示[错误代码](http://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx)元素**用户回音**元素的客户端应用程序应使用**RedirectTarget**元素来构建是新设置请求发送到指定的重定向响应中的服务器。</span><span class="sxs-lookup"><span data-stu-id="e228c-165">If the Autodiscover service returns a redirection response, indicated by the [ErrorCode](http://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) element of the **UserResponse** element, your client application should use the **RedirectTarget** element to construct a new settings request that is sent to the server specified in the redirection response.</span></span> <span data-ttu-id="e228c-166">下面的示例显示服务器的重定向响应。</span><span class="sxs-lookup"><span data-stu-id="e228c-166">The following example shows a redirection response from the server.</span></span> 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>15</h:MajorVersion>
      <h:MinorVersion>0</h:MinorVersion>
      <h:MajorBuildNumber>682</h:MajorBuildNumber>
      <h:MinorBuildNumber>1</h:MinorBuildNumber>
      <h:Version>Exchange2013</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetUserSettingsResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
        <ErrorCode>NoError</ErrorCode>
        <ErrorMessage />
        <UserResponses>
          <UserResponse>
            <ErrorCode>RedirectAddress</ErrorCode>
            <ErrorMessage>Redirection address.</ErrorMessage>
            <RedirectTarget>User1@mail.Contoso.com</RedirectTarget>
            <UserSettingErrors />
            <UserSettings />
          </UserResponse>
        </UserResponses>
      </Response>
    </GetUserSettingsResponseMessage>
  </s:Body>
</s:Envelope>

```

<span data-ttu-id="e228c-167">后重定向，客户端使用的重定向 URL 准备另一个请求。</span><span class="sxs-lookup"><span data-stu-id="e228c-167">After a redirection, the client uses the redirection URL to prepare another request.</span></span> <span data-ttu-id="e228c-168">下面的代码演示的请求重定向响应中创建的示例。</span><span class="sxs-lookup"><span data-stu-id="e228c-168">The following code shows an example of the request that you create from the redirection response.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:wsa="http://www.w3.org/2005/08/addressing" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2013</a:RequestedServerVersion>
    <wsa:Action>http://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://autodiscover.exchange.microsoft.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <a:Request>
        <a:Users>
          <a:User>
            <a:Mailbox>User1@mail.Contoso.com</a:Mailbox>
          </a:User>
        </a:Users>
        <a:RequestedSettings>
          <a:Setting>InternalEwsUrl</a:Setting>
          <a:Setting>ExternalEwsUrl</a:Setting>
        </a:RequestedSettings>
      </a:Request>
    </a:GetUserSettingsRequestMessage>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="e228c-169">当客户端应用程序具有已定向到的正确的终结点的自动发现服务时，服务器将发送与[ErrorCode](http://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx)元素**用户回音**元素设置为**NoError**和包含请求的响应用户设置。</span><span class="sxs-lookup"><span data-stu-id="e228c-169">When the client application has been directed to the correct endpoint for the Autodiscover service, the server will send a response with the [ErrorCode](http://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) element of the **UserResponse** element set to **NoError** and containing the requested user settings.</span></span> <span data-ttu-id="e228c-170">仅请求的用户设置， **InternalEwsUrl**和**ExternalEwsUrl**，则返回。</span><span class="sxs-lookup"><span data-stu-id="e228c-170">Only the requested user settings, **InternalEwsUrl** and **ExternalEwsUrl**, are returned.</span></span> <span data-ttu-id="e228c-171">下面的示例显示来自服务器的响应。</span><span class="sxs-lookup"><span data-stu-id="e228c-171">The following example shows the response from the server.</span></span> 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" 
        xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>15</h:MajorVersion>
      <h:MinorVersion>0</h:MinorVersion>
      <h:MajorBuildNumber>160</h:MajorBuildNumber>
      <h:MinorBuildNumber>4</h:MinorBuildNumber>
      <h:Version>Exchange2013</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetUserSettingsResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
        <ErrorCode>NoError</ErrorCode>
        <ErrorMessage />
        <UserResponses>
          <UserResponse>
            <ErrorCode>NoError</ErrorCode>
            <ErrorMessage>No error.</ErrorMessage>
            <RedirectTarget i:nil="true" />
            <UserSettingErrors />
            <UserSettings>
              <UserSetting i:type="StringSetting">
                <Name>InternalEwsUrl</Name>
                <Value>https://server.Contoso.com/ews/exchange.asmx</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>ExternalEwsUrl</Name>
                <Value>https://server.Contoso.com/ews/exchange.asmx</Value>
              </UserSetting>
            </UserSettings>
          </UserResponse>
        </UserResponses>
      </Response>
    </GetUserSettingsResponseMessage>
  </s:Body>
</s:Envelope>
```

## <a name="next-steps"></a><span data-ttu-id="e228c-172">后续步骤</span><span class="sxs-lookup"><span data-stu-id="e228c-172">Next steps</span></span>
<span data-ttu-id="e228c-173"><a name="bk_Next"> </a></span><span class="sxs-lookup"><span data-stu-id="e228c-173"></span></span>

<span data-ttu-id="e228c-174">按照自动发现过程查找终结点返回请求的域或用户设置。</span><span class="sxs-lookup"><span data-stu-id="e228c-174">Finding the endpoint by following the Autodiscover process returns the requested domain or user settings.</span></span> <span data-ttu-id="e228c-175">有关发出请求的特定设置的信息，请参阅以下文章：</span><span class="sxs-lookup"><span data-stu-id="e228c-175">For information about making a request for specific settings, see the following articles:</span></span>
  
- [<span data-ttu-id="e228c-176">从 Exchange 服务器获取域设置</span><span class="sxs-lookup"><span data-stu-id="e228c-176">Get domain settings from an Exchange server</span></span>](how-to-get-domain-settings-from-an-exchange-server.md)
    
- [<span data-ttu-id="e228c-177">通过使用自动发现 Exchange 中获取用户设置</span><span class="sxs-lookup"><span data-stu-id="e228c-177">Get user settings from Exchange by using Autodiscover</span></span>](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
## <a name="see-also"></a><span data-ttu-id="e228c-178">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e228c-178">See also</span></span>


- [<span data-ttu-id="e228c-179">EWS 应用程序设置</span><span class="sxs-lookup"><span data-stu-id="e228c-179">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)
    
- [<span data-ttu-id="e228c-180">Exchange 自动发现</span><span class="sxs-lookup"><span data-stu-id="e228c-180">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md)
    
- [<span data-ttu-id="e228c-181">Exchange 的自动发现 web 服务引用</span><span class="sxs-lookup"><span data-stu-id="e228c-181">Autodiscover web service reference for Exchange</span></span>](http://msdn.microsoft.com/library/a01124a8-a8cf-4b80-8625-d7ee05690bca%28Office.15%29.aspx)
    
- [<span data-ttu-id="e228c-182">Exchange 的 EWS 引用</span><span class="sxs-lookup"><span data-stu-id="e228c-182">EWS reference for Exchange</span></span>](http://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx)
    
