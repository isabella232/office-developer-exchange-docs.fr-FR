---
title: Utilisation de la découverte automatique pour trouver des points de connexion
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 03896542-549b-4c45-973c-98f9025ea26c
description: Découvrez comment utiliser le service de découverte automatique pour diriger votre application cliente vers le serveur Exchange approprié.
localization_priority: Priority
ms.openlocfilehash: c1895fa0d2cce489467a726614e9457052624ef6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527592"
---
# <a name="use-autodiscover-to-find-connection-points"></a><span data-ttu-id="cc336-103">Utilisation de la découverte automatique pour trouver des points de connexion</span><span class="sxs-lookup"><span data-stu-id="cc336-103">Use Autodiscover to find connection points</span></span>

<span data-ttu-id="cc336-104">Découvrez comment utiliser le service de découverte automatique pour diriger votre application cliente vers le serveur Exchange approprié.</span><span class="sxs-lookup"><span data-stu-id="cc336-104">Find out how to use the Autodiscover service to direct your client application to the correct Exchange server.</span></span>
  
<span data-ttu-id="cc336-105">Le service de découverte automatique Exchange fournit à votre application cliente des paramètres de configuration pour les comptes de messagerie hébergés sur Exchange Online, Exchange Online dans le cadre d’Office 365 ou un serveur Exchange exécutant une version d’Exchange à partir d’Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="cc336-105">The Exchange Autodiscover service provides your client application with configuration settings for email accounts that are hosted on Exchange Online, Exchange Online as part of Office 365, or an Exchange server running a version of Exchange starting with Exchange 2013.</span></span> <span data-ttu-id="cc336-106">Le service de découverte automatique est un service Web qui fournit des paramètres de configuration.</span><span class="sxs-lookup"><span data-stu-id="cc336-106">The Autodiscover service is a web service that provides configuration settings.</span></span> <span data-ttu-id="cc336-107">Le service de découverte automatique est un service Web qui fournit des informations de configuration Exchange Server à votre application cliente.</span><span class="sxs-lookup"><span data-stu-id="cc336-107">The Autodiscover service is a web service that provides Exchange server configuration information to your client application.</span></span> <span data-ttu-id="cc336-108">Les applications clientes utilisent la découverte automatique pour déterminer le point de terminaison du service de découverte automatique pour une boîte aux lettres spécifique.</span><span class="sxs-lookup"><span data-stu-id="cc336-108">Client applications use Autodiscover to determine the endpoint of the Autodiscover service for a specific mailbox.</span></span> <span data-ttu-id="cc336-109">Cet article explique comment suivre les réponses d’un serveur Exchange pour trouver le point de terminaison correct.</span><span class="sxs-lookup"><span data-stu-id="cc336-109">This article explains how to follow the responses from an Exchange server to find the correct endpoint.</span></span> 
  
<span data-ttu-id="cc336-110">Pour plus d’informations sur la façon d’obtenir les paramètres de configuration des adresses de messagerie, consultez la rubrique [obtenir les paramètres utilisateur à partir d’Exchange à l’aide de la découverte automatique](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) et [obtenir les paramètres de domaine à partir d’un serveur Exchange](how-to-get-domain-settings-from-an-exchange-server.md).</span><span class="sxs-lookup"><span data-stu-id="cc336-110">For information about how to get email address configuration settings, see [Get user settings from Exchange by using Autodiscover](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) and [Get domain settings from an Exchange server](how-to-get-domain-settings-from-an-exchange-server.md).</span></span>
  
> [!NOTE]
> <span data-ttu-id="cc336-111">Le processus de recherche du point de terminaison correct fait partie de la demande pour les paramètres de l’utilisateur ou du domaine.</span><span class="sxs-lookup"><span data-stu-id="cc336-111">The process for finding the correct endpoint is part of the request for user or domain settings.</span></span> <span data-ttu-id="cc336-112">Le service de découverte automatique utilise une série de réponses de redirection pour envoyer l’application cliente au point de terminaison approprié pour une adresse de messagerie.</span><span class="sxs-lookup"><span data-stu-id="cc336-112">The Autodiscover service uses a series of redirect responses to send the client application to the correct endpoint for an email address.</span></span> 
  
<span data-ttu-id="cc336-113">Vous pouvez utiliser l’une des technologies de développement Exchange suivantes pour accéder au service de découverte automatique :</span><span class="sxs-lookup"><span data-stu-id="cc336-113">You can use one of the following Exchange development technologies to access the Autodiscover service:</span></span>

- <span data-ttu-id="cc336-114">API managée des services web Exchange (EWS)</span><span class="sxs-lookup"><span data-stu-id="cc336-114">The Exchange Web Services (EWS) Managed API</span></span>
    
- <span data-ttu-id="cc336-115">EWS</span><span class="sxs-lookup"><span data-stu-id="cc336-115">EWS</span></span>
    
<span data-ttu-id="cc336-116">Si vous utilisez EWS, recourez aux méthodes suivantes pour extraire des paramètres utilisateur :</span><span class="sxs-lookup"><span data-stu-id="cc336-116">If you are using EWS, you can use the following methods to retrieve user settings:</span></span>
    
- <span data-ttu-id="cc336-117">Service de découverte automatique basé sur SOAP</span><span class="sxs-lookup"><span data-stu-id="cc336-117">The SOAP-based Autodiscover service</span></span>
    
- <span data-ttu-id="cc336-118">Service de découverte automatique XML (POX)</span><span class="sxs-lookup"><span data-stu-id="cc336-118">The XML (POX) Autodiscover service</span></span>
    
- <span data-ttu-id="cc336-119">Proxy généré automatiquement à partir du service de détection automatique SOAP ou XML</span><span class="sxs-lookup"><span data-stu-id="cc336-119">An autogenerated proxy generated from the SOAP or XML Autodiscover service</span></span>
    
<span data-ttu-id="cc336-120">Pour plus d'informations sur ces méthodes, reportez-vous à la section [Découverte automatique pour Exchange](autodiscover-for-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="cc336-120">For more information about these methods, see [Autodiscover for Exchange](autodiscover-for-exchange.md).</span></span>

<span data-ttu-id="cc336-121">Pour plus d’informations sur ces technologies de développement Exchange, voir [Explorer l’API managée EWS, EWS et les services Web dans Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="cc336-121">For more information about these Exchange development technologies, see [Explore the EWS Managed API, EWS, and web services in Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md).</span></span> 

<span data-ttu-id="cc336-p103">L’API managée EWS fournit une interface basée sur des objets pour récupérer les paramètres de l’utilisateur. Si votre application cliente utilise du code managé, nous vous recommandons de choisir l’API managée EWS. L’interface API managée EWS optimisée pour un modèle d’objet simple présente des performances supérieures au proxy de service web généré automatiquement par défaut.</span><span class="sxs-lookup"><span data-stu-id="cc336-p103">The EWS Managed API provides an object-based interface for retrieving user settings. If your client application uses managed code, we recommend that you use the EWS Managed API. The EWS Managed API interface is better optimized for a simple object model than the typical autogenerated web service proxy.</span></span> 
  
<span data-ttu-id="cc336-125">Si vous utilisez EWS, nous vous conseillons d’opter pour le service de découverte automatique SOAP, car il prend en charge un ensemble de fonctionnalités plus riche que le service de découverte automatique POX.</span><span class="sxs-lookup"><span data-stu-id="cc336-125">If you are using EWS, we suggest that you use the SOAP Autodiscover service, because it supports a richer set of features than the POX Autodiscover service.</span></span>
  
## <a name="prerequisites-for-finding-an-endpoint"></a><span data-ttu-id="cc336-126">Conditions préalables à la recherche d’un point de terminaison</span><span class="sxs-lookup"><span data-stu-id="cc336-126">Prerequisites for finding an endpoint</span></span>
<span data-ttu-id="cc336-127"><a name="bk_Prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="cc336-127"><a name="bk_Prereq"> </a></span></span>

<span data-ttu-id="cc336-128">Pour pouvoir créer une application cliente qui utilise le service de découverte automatique, vous devez avoir accès à ce qui suit :</span><span class="sxs-lookup"><span data-stu-id="cc336-128">Before you can create a client application that uses the Autodiscover service, you need to have access to the following:</span></span>
  
- <span data-ttu-id="cc336-129">Exchange Online ou un serveur qui exécute une version d’Exchange à partir d’Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="cc336-129">Exchange Online or a server that is running a version of Exchange starting with Exchange 2007 SP1.</span></span> <span data-ttu-id="cc336-130">Si vous utilisez le service de découverte automatique basé sur SOAP, Exchange Online ou une version d’Exchange commençant par Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="cc336-130">If you are using the SOAP-based Autodiscover service, Exchange Online or a version of Exchange starting with Exchange 2010.</span></span>
    
- <span data-ttu-id="cc336-p105">Un serveur Exchange qui est configuré pour accepter les connexions depuis votre application cliente. Pour plus d'informations sur la configuration de votre serveur Exchange, reportez-vous à la rubrique [Contrôle de l'accès aux applications de client pour EWS dans Exchange](controlling-client-application-access-to-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="cc336-p105">An Exchange server that is configured to accept connections from your client application. For information about how to configure your Exchange server, see [Controlling client application access to EWS in Exchange](controlling-client-application-access-to-ews-in-exchange.md).</span></span>
    
- <span data-ttu-id="cc336-p106">Un compte autorisé à utiliser EWS. Pour plus d'informations sur la configuration d'un compte, reportez-vous à la rubrique [Contrôle de l'accès aux applications de client pour EWS dans Exchange](controlling-client-application-access-to-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="cc336-p106">An account that is authorized to use EWS. For information about how to configure an account, see [Controlling client application access to EWS in Exchange](controlling-client-application-access-to-ews-in-exchange.md).</span></span>
    
> [!NOTE]
> <span data-ttu-id="cc336-135">Si vous utilisez l’API managée EWS, vous devez fournir un rappel de validation de certificat dans certains cas.</span><span class="sxs-lookup"><span data-stu-id="cc336-135">If you are using the EWS Managed API, you must provide a certificate validation callback in some circumstances.</span></span> <span data-ttu-id="cc336-136">Vous aurez peut-être également besoin d’un rappel de validation de certificat avec certaines bibliothèques proxy générées, telles que celles créées par Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="cc336-136">You may also need a certificate validation callback with some generated proxy libraries, such as those created by Visual Studio.</span></span> <span data-ttu-id="cc336-137">Pour plus d'informations, reportez-vous à la rubrique [Valider un certificat de serveur pour l'API managée EWS](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).</span><span class="sxs-lookup"><span data-stu-id="cc336-137">For more information, see [Validate a server certificate for the EWS Managed API](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).</span></span> 
  
### <a name="core-concepts-for-finding-an-endpoint"></a><span data-ttu-id="cc336-138">Concepts de base pour trouver un point de terminaison</span><span class="sxs-lookup"><span data-stu-id="cc336-138">Core concepts for finding an endpoint</span></span>
<span data-ttu-id="cc336-139"><a name="bk_Core"> </a></span><span class="sxs-lookup"><span data-stu-id="cc336-139"><a name="bk_Core"> </a></span></span>

<span data-ttu-id="cc336-140">Avant d’utiliser la découverte automatique pour trouver un point de terminaison, vous devez être familiarisé avec les concepts présentés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="cc336-140">Before you use Autodiscover to find an endpoint, you should be familiar with the concepts listed in the following table.</span></span>
  
|<span data-ttu-id="cc336-141">**Concept**</span><span class="sxs-lookup"><span data-stu-id="cc336-141">**Concept**</span></span>|<span data-ttu-id="cc336-142">**Description**</span><span class="sxs-lookup"><span data-stu-id="cc336-142">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cc336-143">Découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="cc336-143">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md) <br/> |<span data-ttu-id="cc336-144">Fournit une vue d’ensemble du fonctionnement du service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="cc336-144">Provides an overview of how the Autodiscover service works.</span></span>  <br/> |
   
<span data-ttu-id="cc336-145">Si vous utilisez l'API managée EWS, vous gérez votre connexion à EWS à l'aide de la classe [Microsoft.Exchange.WebServices.Data.ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) dans l'espace de noms [Microsoft.Exchange.WebServices.Data](https://msdn.microsoft.com/library/dd633907%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="cc336-145">If you are using the EWS Managed API, you use the [Microsoft.Exchange.WebServices.Data.ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) class in the [Microsoft.Exchange.WebServices.Data](https://msdn.microsoft.com/library/dd633907%28v=exchg.80%29.aspx) namespace to manage your connection to EWS.</span></span> <span data-ttu-id="cc336-146">Pour utiliser les exemples de code de l’API managée EWS dans cet article, vous devez référencer les espaces de noms suivants dans votre code :</span><span class="sxs-lookup"><span data-stu-id="cc336-146">To use the EWS Managed API code samples in this article, you need to reference the following namespaces in your code:</span></span> 
  
- <span data-ttu-id="cc336-147">**System.Net**</span><span class="sxs-lookup"><span data-stu-id="cc336-147">**System.Net**</span></span>
    
- <span data-ttu-id="cc336-148">**Microsoft.Exchange.WebServices.Data.ExchangeService**</span><span class="sxs-lookup"><span data-stu-id="cc336-148">**Microsoft.Exchange.WebServices.Data.ExchangeService**</span></span>
    
## <a name="find-the-correct-endpoint-by-using-the-ews-managed-api"></a><span data-ttu-id="cc336-149">Trouver le point de terminaison correct à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="cc336-149">Find the correct endpoint by using the EWS Managed API</span></span>
<span data-ttu-id="cc336-150"><a name="bk_Managed"> </a></span><span class="sxs-lookup"><span data-stu-id="cc336-150"><a name="bk_Managed"> </a></span></span>

<span data-ttu-id="cc336-151">Si vous utilisez l’API managée EWS, les appels au service de découverte automatique sont gérés par la classe **ExchangeService** .</span><span class="sxs-lookup"><span data-stu-id="cc336-151">If you are using the EWS Managed API, calls to the Autodiscover service are handled by the **ExchangeService** class.</span></span> <span data-ttu-id="cc336-152">Pour déterminer le point de terminaison approprié pour un compte de messagerie, vous appelez la méthode **AutodiscoverUrl** sur un objet **[ExchangeService]** .</span><span class="sxs-lookup"><span data-stu-id="cc336-152">To determine the correct endpoint for an email account, you call the **AutodiscoverUrl** method on an **[ExchangeService]** object.</span></span> <span data-ttu-id="cc336-153">L’exemple de code suivant montre comment définir le point de terminaison du service Web EWS pour une adresse de messagerie dans le fichier Exchange. asmx sur le serveur d’accès au client approprié à l’aide de l’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="cc336-153">The following code example shows how to set the EWS web service endpoint for an email address to the Exchange.asmx file on the correct Client Access server by using the EWS Managed API.</span></span> 
  
```cs
NetworkCredential credentials = new NetworkCredential(securelyStoredEmail, securelyStoredPassword);
ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2013);
service.Credentials = credentials;
service.AutodiscoverUrl("User1@contoso.com");
```

## <a name="find-the-correct-endpoint-by-using-ews"></a><span data-ttu-id="cc336-154">Trouver le point de terminaison correct à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="cc336-154">Find the correct endpoint by using EWS</span></span>
<span data-ttu-id="cc336-155"><a name="bk_SOAP"> </a></span><span class="sxs-lookup"><span data-stu-id="cc336-155"><a name="bk_SOAP"> </a></span></span>

<span data-ttu-id="cc336-156">Le service de découverte automatique SOAP peut utiliser une série de demandes et de réponses pour diriger votre application vers le point de terminaison correct pour EWS.</span><span class="sxs-lookup"><span data-stu-id="cc336-156">The SOAP Autodiscover service may use a series of requests and responses to direct your application to the correct endpoint for EWS.</span></span> <span data-ttu-id="cc336-157">Pour plus d’informations sur le processus permettant de déterminer le point de terminaison correct pour un compte de messagerie, consultez la rubrique [découverte automatique pour Exchange](autodiscover-for-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="cc336-157">For information about the process for determining the correct endpoint for an email account, see [Autodiscover for Exchange](autodiscover-for-exchange.md).</span></span> <span data-ttu-id="cc336-158">Les exemples XML suivants montrent la série de demandes et de réponses que vous pouvez vous attendre lors de la création d’une demande de découverte automatique SOAP pour trouver le point de terminaison approprié.</span><span class="sxs-lookup"><span data-stu-id="cc336-158">The following XML examples show the series of requests and responses that you can expect when making a SOAP Autodiscover request to find the correct endpoint.</span></span>
  
### <a name="soap-autodiscover-endpoint-request"></a><span data-ttu-id="cc336-159">Demande de point de terminaison de découverte automatique SOAP</span><span class="sxs-lookup"><span data-stu-id="cc336-159">SOAP Autodiscover endpoint request</span></span>

<span data-ttu-id="cc336-160">L’exemple suivant montre une requête XML qui est envoyée au service de découverte automatique pour trouver le point de terminaison correct.</span><span class="sxs-lookup"><span data-stu-id="cc336-160">The following example shows an XML request that is sent to the Autodiscover service to find the correct endpoint.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:wsa="http://www.w3.org/2005/08/addressing" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2013</a:RequestedServerVersion>
    <wsa:Action>https://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://mail.microsoft.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover">
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

### <a name="soap-autodiscover-redirection-response"></a><span data-ttu-id="cc336-161">Réponse de redirection de la découverte automatique SOAP</span><span class="sxs-lookup"><span data-stu-id="cc336-161">SOAP Autodiscover redirection response</span></span>

<span data-ttu-id="cc336-162">Le service de découverte automatique peut répondre avec une des deux réponses de redirection : une redirection HTTP 302 ou une réponse de redirection SOAP.</span><span class="sxs-lookup"><span data-stu-id="cc336-162">The Autodiscover service may respond with one of two redirection responses: an HTTP 302 redirect, or a SOAP redirection response.</span></span> <span data-ttu-id="cc336-163">Si la réponse du serveur Exchange est une redirection HTTP 302, l’application cliente doit vérifier que l’adresse de redirection est acceptable, puis suivre la réponse de redirection.</span><span class="sxs-lookup"><span data-stu-id="cc336-163">If the response from the Exchange server is an HTTP 302 redirect, the client application should validate that the redirection address is acceptable and then follow the redirection response.</span></span>
  
> [!IMPORTANT]
> <span data-ttu-id="cc336-164">Pour obtenir les critères de validation d’une réponse de redirection, consultez la rubrique [découverte automatique pour Exchange](autodiscover-for-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="cc336-164">For criteria for validating a redirection response, see [Autodiscover for Exchange](autodiscover-for-exchange.md).</span></span> 
  
<span data-ttu-id="cc336-165">Si le service de découverte automatique renvoie une réponse de redirection, indiquée par l’élément [ErrorCode](https://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) de l’élément **UserResponse** , votre application cliente doit utiliser l’élément **RedirectTarget** pour créer une nouvelle demande de paramètres qui est envoyée au serveur spécifié dans la réponse de redirection.</span><span class="sxs-lookup"><span data-stu-id="cc336-165">If the Autodiscover service returns a redirection response, indicated by the [ErrorCode](https://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) element of the **UserResponse** element, your client application should use the **RedirectTarget** element to construct a new settings request that is sent to the server specified in the redirection response.</span></span> <span data-ttu-id="cc336-166">L’exemple suivant montre une réponse de redirection du serveur.</span><span class="sxs-lookup"><span data-stu-id="cc336-166">The following example shows a redirection response from the server.</span></span> 
  
```XML
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/" xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">https://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="https://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>15</h:MajorVersion>
      <h:MinorVersion>0</h:MinorVersion>
      <h:MajorBuildNumber>682</h:MajorBuildNumber>
      <h:MinorBuildNumber>1</h:MinorBuildNumber>
      <h:Version>Exchange2013</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetUserSettingsResponseMessage xmlns="https://schemas.microsoft.com/exchange/2010/Autodiscover">
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

<span data-ttu-id="cc336-167">Après une redirection, le client utilise l’URL de redirection pour préparer une autre demande.</span><span class="sxs-lookup"><span data-stu-id="cc336-167">After a redirection, the client uses the redirection URL to prepare another request.</span></span> <span data-ttu-id="cc336-168">Le code suivant illustre un exemple de la requête que vous créez à partir de la réponse de redirection.</span><span class="sxs-lookup"><span data-stu-id="cc336-168">The following code shows an example of the request that you create from the redirection response.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:wsa="http://www.w3.org/2005/08/addressing" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2013</a:RequestedServerVersion>
    <wsa:Action>https://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://autodiscover.exchange.microsoft.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover">
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

<span data-ttu-id="cc336-169">Lorsque l’application cliente a été dirigée vers le point de terminaison approprié pour le service de découverte automatique, le serveur envoie une réponse avec l’élément [ErrorCode](https://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) de l’élément **UserResponse** défini sur **NOERROR** et contenant les paramètres utilisateur demandés.</span><span class="sxs-lookup"><span data-stu-id="cc336-169">When the client application has been directed to the correct endpoint for the Autodiscover service, the server will send a response with the [ErrorCode](https://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) element of the **UserResponse** element set to **NoError** and containing the requested user settings.</span></span> <span data-ttu-id="cc336-170">Seuls les paramètres utilisateur demandés, **InternalEwsUrl** et **ExternalEwsUrl**, sont renvoyés.</span><span class="sxs-lookup"><span data-stu-id="cc336-170">Only the requested user settings, **InternalEwsUrl** and **ExternalEwsUrl**, are returned.</span></span> <span data-ttu-id="cc336-171">L’exemple suivant montre la réponse du serveur.</span><span class="sxs-lookup"><span data-stu-id="cc336-171">The following example shows the response from the server.</span></span> 
  
```XML
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/" 
        xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">https://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="https://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>15</h:MajorVersion>
      <h:MinorVersion>0</h:MinorVersion>
      <h:MajorBuildNumber>160</h:MajorBuildNumber>
      <h:MinorBuildNumber>4</h:MinorBuildNumber>
      <h:Version>Exchange2013</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetUserSettingsResponseMessage xmlns="https://schemas.microsoft.com/exchange/2010/Autodiscover">
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

## <a name="next-steps"></a><span data-ttu-id="cc336-172">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="cc336-172">Next steps</span></span>
<span data-ttu-id="cc336-173"><a name="bk_Next"> </a></span><span class="sxs-lookup"><span data-stu-id="cc336-173"><a name="bk_Next"> </a></span></span>

<span data-ttu-id="cc336-174">La recherche du point de terminaison en suivant le processus de découverte automatique renvoie les paramètres de domaine ou d’utilisateur demandés.</span><span class="sxs-lookup"><span data-stu-id="cc336-174">Finding the endpoint by following the Autodiscover process returns the requested domain or user settings.</span></span> <span data-ttu-id="cc336-175">Pour plus d’informations sur la demande de paramètres spécifiques, consultez les articles suivants :</span><span class="sxs-lookup"><span data-stu-id="cc336-175">For information about making a request for specific settings, see the following articles:</span></span>
  
- [<span data-ttu-id="cc336-176">Obtenir des paramètres de domaine à partir d’un serveur Exchange</span><span class="sxs-lookup"><span data-stu-id="cc336-176">Get domain settings from an Exchange server</span></span>](how-to-get-domain-settings-from-an-exchange-server.md)    
- [<span data-ttu-id="cc336-177">Obtenir les paramètres de l'utilisateur Exchange à l'aide de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="cc336-177">Get user settings from Exchange by using Autodiscover</span></span>](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
## <a name="see-also"></a><span data-ttu-id="cc336-178">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="cc336-178">See also</span></span>

- [<span data-ttu-id="cc336-179">Configuration de votre application EWS</span><span class="sxs-lookup"><span data-stu-id="cc336-179">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)   
- [<span data-ttu-id="cc336-180">Découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="cc336-180">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md)    
- [<span data-ttu-id="cc336-181">Référence de service web de découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="cc336-181">Autodiscover web service reference for Exchange</span></span>](https://msdn.microsoft.com/library/a01124a8-a8cf-4b80-8625-d7ee05690bca%28Office.15%29.aspx)    
- [<span data-ttu-id="cc336-182">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="cc336-182">EWS reference for Exchange</span></span>](https://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx)
    

