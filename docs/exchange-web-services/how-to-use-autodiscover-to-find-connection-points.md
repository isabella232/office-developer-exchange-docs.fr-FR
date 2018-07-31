---
title: Utilisation de la découverte automatique pour rechercher des points de connexion
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 03896542-549b-4c45-973c-98f9025ea26c
description: Découvrez comment utiliser le service de découverte automatique pour diriger votre application cliente vers le serveur Exchange approprié.
ms.openlocfilehash: eb3fb3664e5789638c097a43cf48f757bb0713ae
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353979"
---
# <a name="use-autodiscover-to-find-connection-points"></a><span data-ttu-id="0b1f2-103">Utilisation de la découverte automatique pour rechercher des points de connexion</span><span class="sxs-lookup"><span data-stu-id="0b1f2-103">Use Autodiscover to find connection points</span></span>

<span data-ttu-id="0b1f2-104">Découvrez comment utiliser le service de découverte automatique pour diriger votre application cliente vers le serveur Exchange approprié.</span><span class="sxs-lookup"><span data-stu-id="0b1f2-104">Find out how to use the Autodiscover service to direct your client application to the correct Exchange server.</span></span>
  
<span data-ttu-id="0b1f2-105">Le service de découverte automatique Exchange fournit à votre application client avec les paramètres de configuration de comptes de messagerie qui sont hébergées sur Exchange Online, Exchange Online dans le cadre d’Office 365 ou un serveur Exchange qui exécute une version d’Exchange commençant par Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="0b1f2-105">The Exchange Autodiscover service provides your client application with configuration settings for email accounts that are hosted on Exchange Online, Exchange Online as part of Office 365, or an Exchange server running a version of Exchange starting with Exchange 2013.</span></span> <span data-ttu-id="0b1f2-106">Le service de découverte automatique est un service web qui fournit des paramètres de configuration.</span><span class="sxs-lookup"><span data-stu-id="0b1f2-106">The Autodiscover service is a web service that provides configuration settings.</span></span> <span data-ttu-id="0b1f2-107">Le service de découverte automatique est un service web qui fournit des informations de configuration Exchange server pour votre application cliente.</span><span class="sxs-lookup"><span data-stu-id="0b1f2-107">The Autodiscover service is a web service that provides Exchange server configuration information to your client application.</span></span> <span data-ttu-id="0b1f2-108">Applications clientes utilisent la découverte automatique pour déterminer le point de terminaison du service de découverte automatique pour une boîte aux lettres spécifique.</span><span class="sxs-lookup"><span data-stu-id="0b1f2-108">Client applications use Autodiscover to determine the endpoint of the Autodiscover service for a specific mailbox.</span></span> <span data-ttu-id="0b1f2-109">Cet article explique comment suivre les réponses à partir d’un serveur Exchange pour rechercher le point de terminaison correct.</span><span class="sxs-lookup"><span data-stu-id="0b1f2-109">This article explains how to follow the responses from an Exchange server to find the correct endpoint.</span></span> 
  
<span data-ttu-id="0b1f2-110">Pour plus d’informations sur la façon d’obtenir des paramètres de configuration d’adresse de messagerie, voir [obtenir les paramètres utilisateur à partir d’Exchange à l’aide de découverte automatique](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) et [obtenir les paramètres de domaine à partir d’un serveur Exchange](how-to-get-domain-settings-from-an-exchange-server.md).</span><span class="sxs-lookup"><span data-stu-id="0b1f2-110">For information about how to get email address configuration settings, see [Get user settings from Exchange by using Autodiscover](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) and [Get domain settings from an Exchange server](how-to-get-domain-settings-from-an-exchange-server.md).</span></span>
  
> [!NOTE]
> <span data-ttu-id="0b1f2-111">Le processus pour rechercher le point de terminaison correct fait partie de la demande de l’utilisateur ou les paramètres de domaine.</span><span class="sxs-lookup"><span data-stu-id="0b1f2-111">The process for finding the correct endpoint is part of the request for user or domain settings.</span></span> <span data-ttu-id="0b1f2-112">Le service de découverte automatique utilise une série de réponses de redirection pour envoyer l’application cliente au point de terminaison correct pour une adresse de messagerie.</span><span class="sxs-lookup"><span data-stu-id="0b1f2-112">The Autodiscover service uses a series of redirect responses to send the client application to the correct endpoint for an email address.</span></span> 
  
<span data-ttu-id="0b1f2-113">Vous pouvez utiliser une des technologies de développement Exchange suivantes pour accéder au service de découverte automatique :</span><span class="sxs-lookup"><span data-stu-id="0b1f2-113">You can use one of the following Exchange development technologies to access the Autodiscover service:</span></span>

- <span data-ttu-id="0b1f2-114">API managée des services web Exchange (EWS)</span><span class="sxs-lookup"><span data-stu-id="0b1f2-114">The Exchange Web Services (EWS) Managed API</span></span>
    
- <span data-ttu-id="0b1f2-115">EWS</span><span class="sxs-lookup"><span data-stu-id="0b1f2-115">EWS</span></span>
    
<span data-ttu-id="0b1f2-116">Si vous utilisez EWS, recourez aux méthodes suivantes pour extraire des paramètres utilisateur :</span><span class="sxs-lookup"><span data-stu-id="0b1f2-116">If you are using EWS, you can use the following methods to retrieve user settings:</span></span>
    
- <span data-ttu-id="0b1f2-117">Service de découverte automatique basé sur SOAP</span><span class="sxs-lookup"><span data-stu-id="0b1f2-117">The SOAP-based Autodiscover service</span></span>
    
- <span data-ttu-id="0b1f2-118">Service de découverte automatique XML (POX)</span><span class="sxs-lookup"><span data-stu-id="0b1f2-118">The XML (POX) Autodiscover service</span></span>
    
- <span data-ttu-id="0b1f2-119">Proxy généré automatiquement à partir du service de détection automatique SOAP ou XML</span><span class="sxs-lookup"><span data-stu-id="0b1f2-119">An autogenerated proxy generated from the SOAP or XML Autodiscover service</span></span>
    
<span data-ttu-id="0b1f2-120">Pour plus d'informations sur ces méthodes, reportez-vous à la section [Découverte automatique pour Exchange](autodiscover-for-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="0b1f2-120">For more information about these methods, see [Autodiscover for Exchange](autodiscover-for-exchange.md).</span></span>

<span data-ttu-id="0b1f2-121">Pour plus d’informations sur ces technologies de développement Exchange, voir [Explorer l’API managée EWS, EWS et des services web Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="0b1f2-121">For more information about these Exchange development technologies, see [Explore the EWS Managed API, EWS, and web services in Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md).</span></span> 

<span data-ttu-id="0b1f2-p103">L'API managée EWS fournit une interface basée sur des objets pour récupérer les paramètres de l'utilisateur. Si votre application cliente utilise du code managé, nous vous recommandons de choisir l'API managée EWS. L'interface API managée EWS optimisée pour un modèle d'objet simple présente des performances supérieures au proxy de service web généré automatiquement par défaut.</span><span class="sxs-lookup"><span data-stu-id="0b1f2-p103">The EWS Managed API provides an object-based interface for retrieving user settings. If your client application uses managed code, we recommend that you use the EWS Managed API. The EWS Managed API interface is better optimized for a simple object model than the typical autogenerated web service proxy.</span></span> 
  
<span data-ttu-id="0b1f2-125">Si vous utilisez EWS, nous vous conseillons d'opter pour le service de découverte automatique SOAP, car il prend en charge un ensemble de fonctionnalités plus riche que le service de découverte automatique POX.</span><span class="sxs-lookup"><span data-stu-id="0b1f2-125">If you are using EWS, we suggest that you use the SOAP Autodiscover service, because it supports a richer set of features than the POX Autodiscover service.</span></span>
  
## <a name="prerequisites-for-finding-an-endpoint"></a><span data-ttu-id="0b1f2-126">Conditions préalables pour la recherche d’un point de terminaison</span><span class="sxs-lookup"><span data-stu-id="0b1f2-126">Prerequisites for finding an endpoint</span></span>
<span data-ttu-id="0b1f2-127"><a name="bk_Prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="0b1f2-127"></span></span>

<span data-ttu-id="0b1f2-128">Avant de pouvoir créer une application cliente qui utilise le service de découverte automatique, vous devez avoir accès à ce qui suit :</span><span class="sxs-lookup"><span data-stu-id="0b1f2-128">Before you can create a client application that uses the Autodiscover service, you need to have access to the following:</span></span>
  
- <span data-ttu-id="0b1f2-129">Exchange Online ou un serveur qui exécute une version d’Exchange de démarrer avec Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="0b1f2-129">Exchange Online or a server that is running a version of Exchange starting with Exchange 2007 SP1.</span></span> <span data-ttu-id="0b1f2-130">Si vous utilisez le service Autodiscover basés sur SOAP, Exchange Online ou une version d’Exchange commençant par Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="0b1f2-130">If you are using the SOAP-based Autodiscover service, Exchange Online or a version of Exchange starting with Exchange 2010.</span></span>
    
- <span data-ttu-id="0b1f2-p105">Un serveur Exchange qui est configuré pour accepter les connexions depuis votre application cliente. Pour plus d'informations sur la configuration de votre serveur Exchange, reportez-vous à la rubrique [Contrôle de l'accès aux applications de client pour EWS dans Exchange](controlling-client-application-access-to-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="0b1f2-p105">An Exchange server that is configured to accept connections from your client application. For information about how to configure your Exchange server, see [Controlling client application access to EWS in Exchange](controlling-client-application-access-to-ews-in-exchange.md).</span></span>
    
- <span data-ttu-id="0b1f2-p106">Un compte autorisé à utiliser EWS. Pour plus d'informations sur la configuration d'un compte, reportez-vous à la rubrique [Contrôle de l'accès aux applications de client pour EWS dans Exchange](controlling-client-application-access-to-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="0b1f2-p106">An account that is authorized to use EWS. For information about how to configure an account, see [Controlling client application access to EWS in Exchange](controlling-client-application-access-to-ews-in-exchange.md).</span></span>
    
> [!NOTE]
> <span data-ttu-id="0b1f2-135">[!REMARQUE] Si vous utilisez l'API managée EWS, vous devez fournir un rappel de validation de certificat dans certains cas.</span><span class="sxs-lookup"><span data-stu-id="0b1f2-135">If you are using the EWS Managed API, you must provide a certificate validation callback in some circumstances.</span></span> <span data-ttu-id="0b1f2-136">Vous aurez peut-être également besoin d'un rappel de validation de certificat avec certaines bibliothèques proxy générées, telles que celles qui sont créées par Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="0b1f2-136">You may also need a certificate validation callback with some generated proxy libraries, such as those created by Visual Studio.</span></span> <span data-ttu-id="0b1f2-137">Pour plus d’informations, voir [valider un certificat de serveur pour l’API managée EWS](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).</span><span class="sxs-lookup"><span data-stu-id="0b1f2-137">For more information, see [Validate a server certificate for the EWS Managed API](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).</span></span> 
  
### <a name="core-concepts-for-finding-an-endpoint"></a><span data-ttu-id="0b1f2-138">Concepts de base pour la recherche d’un point de terminaison</span><span class="sxs-lookup"><span data-stu-id="0b1f2-138">Core concepts for finding an endpoint</span></span>
<span data-ttu-id="0b1f2-139"><a name="bk_Core"> </a></span><span class="sxs-lookup"><span data-stu-id="0b1f2-139"></span></span>

<span data-ttu-id="0b1f2-140">Avant d’utiliser la découverte automatique pour trouver un point de terminaison, vous devez connaître avec les concepts figurant dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="0b1f2-140">Before you use Autodiscover to find an endpoint, you should be familiar with the concepts listed in the following table.</span></span>
  
|<span data-ttu-id="0b1f2-141">**Concept**</span><span class="sxs-lookup"><span data-stu-id="0b1f2-141">**Concept**</span></span>|<span data-ttu-id="0b1f2-142">**Description**</span><span class="sxs-lookup"><span data-stu-id="0b1f2-142">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b1f2-143">Découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="0b1f2-143">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md) <br/> |<span data-ttu-id="0b1f2-144">Fournit une vue d'ensemble du fonctionnement du service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="0b1f2-144">Provides an overview of how the Autodiscover service works.</span></span>  <br/> |
   
<span data-ttu-id="0b1f2-145">Si vous utilisez l'API managée EWS, vous gérez votre connexion à EWS à l'aide de la classe [Microsoft.Exchange.WebServices.Data.ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) dans l'espace de noms [Microsoft.Exchange.WebServices.Data](http://msdn.microsoft.com/en-us/library/dd633907%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="0b1f2-145">If you are using the EWS Managed API, you use the [Microsoft.Exchange.WebServices.Data.ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) class in the [Microsoft.Exchange.WebServices.Data](http://msdn.microsoft.com/en-us/library/dd633907%28v=exchg.80%29.aspx) namespace to manage your connection to EWS.</span></span> <span data-ttu-id="0b1f2-146">Pour utiliser les exemples de code d’API managées dans cet article, vous devez faire référence les espaces de noms suivants dans votre code :</span><span class="sxs-lookup"><span data-stu-id="0b1f2-146">To use the EWS Managed API code samples in this article, you need to reference the following namespaces in your code:</span></span> 
  
- <span data-ttu-id="0b1f2-147">**System.Net**</span><span class="sxs-lookup"><span data-stu-id="0b1f2-147">**System.Net**</span></span>
    
- <span data-ttu-id="0b1f2-148">**Microsoft.Exchange.WebServices.Data.ExchangeService**</span><span class="sxs-lookup"><span data-stu-id="0b1f2-148">**Microsoft.Exchange.WebServices.Data.ExchangeService**</span></span>
    
## <a name="find-the-correct-endpoint-by-using-the-ews-managed-api"></a><span data-ttu-id="0b1f2-149">Rechercher le point de terminaison correct à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="0b1f2-149">Find the correct endpoint by using the EWS Managed API</span></span>
<span data-ttu-id="0b1f2-150"><a name="bk_Managed"> </a></span><span class="sxs-lookup"><span data-stu-id="0b1f2-150"></span></span>

<span data-ttu-id="0b1f2-151">Si vous utilisez l’API managée EWS, les appels vers le service de découverte automatique sont gérés par la classe **ExchangeService** .</span><span class="sxs-lookup"><span data-stu-id="0b1f2-151">If you are using the EWS Managed API, calls to the Autodiscover service are handled by the **ExchangeService** class.</span></span> <span data-ttu-id="0b1f2-152">Pour déterminer le point de terminaison correct pour un compte de messagerie, vous appelez la méthode **AutodiscoverUrl** sur un objet **[ExchangeService]** .</span><span class="sxs-lookup"><span data-stu-id="0b1f2-152">To determine the correct endpoint for an email account, you call the **AutodiscoverUrl** method on an **[ExchangeService]** object.</span></span> <span data-ttu-id="0b1f2-153">L’exemple de code suivant montre comment définir le point de terminaison EWS web services pour une adresse de messagerie au fichier Exchange.asmx sur le serveur d’accès au Client approprié à l’aide de l’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="0b1f2-153">The following code example shows how to set the EWS web service endpoint for an email address to the Exchange.asmx file on the correct Client Access server by using the EWS Managed API.</span></span> 
  
```cs
NetworkCredential credentials = new NetworkCredential(securelyStoredEmail, securelyStoredPassword);
ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2013);
service.Credentials = credentials;
service.AutodiscoverUrl("User1@contoso.com");
```

## <a name="find-the-correct-endpoint-by-using-ews"></a><span data-ttu-id="0b1f2-154">Rechercher le point de terminaison correct à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="0b1f2-154">Find the correct endpoint by using EWS</span></span>
<span data-ttu-id="0b1f2-155"><a name="bk_SOAP"> </a></span><span class="sxs-lookup"><span data-stu-id="0b1f2-155"></span></span>

<span data-ttu-id="0b1f2-156">Le service de découverte automatique SOAP peut utiliser une série de demandes et réponses pour diriger votre application au point de terminaison correct pour EWS.</span><span class="sxs-lookup"><span data-stu-id="0b1f2-156">The SOAP Autodiscover service may use a series of requests and responses to direct your application to the correct endpoint for EWS.</span></span> <span data-ttu-id="0b1f2-157">Pour plus d’informations sur la façon de déterminer le point de terminaison correct pour un compte de messagerie, voir [service de découverte automatique pour Exchange](autodiscover-for-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="0b1f2-157">For information about the process for determining the correct endpoint for an email account, see [Autodiscover for Exchange](autodiscover-for-exchange.md).</span></span> <span data-ttu-id="0b1f2-158">Les exemples de code XML suivants montrent la série de demandes et réponses que vous pouvez vous attendre lors d’une demande SOAP Autodiscover pour rechercher le point de terminaison correct.</span><span class="sxs-lookup"><span data-stu-id="0b1f2-158">The following XML examples show the series of requests and responses that you can expect when making a SOAP Autodiscover request to find the correct endpoint.</span></span>
  
### <a name="soap-autodiscover-endpoint-request"></a><span data-ttu-id="0b1f2-159">Demande de point de terminaison SOAP découverte automatique</span><span class="sxs-lookup"><span data-stu-id="0b1f2-159">SOAP Autodiscover endpoint request</span></span>

<span data-ttu-id="0b1f2-160">L’exemple suivant montre une requête XML qui est envoyée au service de découverte automatique pour rechercher le point de terminaison correct.</span><span class="sxs-lookup"><span data-stu-id="0b1f2-160">The following example shows an XML request that is sent to the Autodiscover service to find the correct endpoint.</span></span>
  
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

### <a name="soap-autodiscover-redirection-response"></a><span data-ttu-id="0b1f2-161">Réponse de redirection SOAP découverte automatique</span><span class="sxs-lookup"><span data-stu-id="0b1f2-161">SOAP Autodiscover redirection response</span></span>

<span data-ttu-id="0b1f2-162">Le service de découverte automatique peut répondre avec une des deux réponses de redirection : une redirection HTTP 302, ou une réponse de redirection SOAP.</span><span class="sxs-lookup"><span data-stu-id="0b1f2-162">The Autodiscover service may respond with one of two redirection responses: an HTTP 302 redirect, or a SOAP redirection response.</span></span> <span data-ttu-id="0b1f2-163">Si la réponse du serveur Exchange est une redirection HTTP 302, l’application cliente doit valider que l’adresse de la redirection est acceptable et suivez la réponse de redirection.</span><span class="sxs-lookup"><span data-stu-id="0b1f2-163">If the response from the Exchange server is an HTTP 302 redirect, the client application should validate that the redirection address is acceptable and then follow the redirection response.</span></span>
  
> [!IMPORTANT]
> <span data-ttu-id="0b1f2-164">D’après les critères de validation d’une réponse de redirection, voir [service de découverte automatique pour Exchange](autodiscover-for-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="0b1f2-164">For criteria for validating a redirection response, see [Autodiscover for Exchange](autodiscover-for-exchange.md).</span></span> 
  
<span data-ttu-id="0b1f2-165">Si le service de découverte automatique renvoie une réponse de redirection indiquée par l’élément [ErrorCode](http://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) de l’élément de **réponse utilisateur** , votre application cliente doit utiliser l’élément **RedirectTarget** pour construire une nouvelle demande de paramètres qui est envoyé au serveur spécifié dans la réponse de redirection.</span><span class="sxs-lookup"><span data-stu-id="0b1f2-165">If the Autodiscover service returns a redirection response, indicated by the [ErrorCode](http://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) element of the **UserResponse** element, your client application should use the **RedirectTarget** element to construct a new settings request that is sent to the server specified in the redirection response.</span></span> <span data-ttu-id="0b1f2-166">L’exemple suivant montre une réponse de redirection à partir du serveur.</span><span class="sxs-lookup"><span data-stu-id="0b1f2-166">The following example shows a redirection response from the server.</span></span> 
  
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

<span data-ttu-id="0b1f2-167">Après une redirection, le client utilise l’URL de redirection pour préparer une autre requête.</span><span class="sxs-lookup"><span data-stu-id="0b1f2-167">After a redirection, the client uses the redirection URL to prepare another request.</span></span> <span data-ttu-id="0b1f2-168">Le code suivant montre un exemple de la demande que vous créez à partir de la réponse de redirection.</span><span class="sxs-lookup"><span data-stu-id="0b1f2-168">The following code shows an example of the request that you create from the redirection response.</span></span>
  
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

<span data-ttu-id="0b1f2-169">Lors de l’application cliente a été demandée au point de terminaison correct pour le service de découverte automatique, le serveur envoie une réponse à l’élément [ErrorCode](http://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) de l’élément de **réponse utilisateur** définie sur **NoError** et contenant les informations demandées paramètres utilisateur.</span><span class="sxs-lookup"><span data-stu-id="0b1f2-169">When the client application has been directed to the correct endpoint for the Autodiscover service, the server will send a response with the [ErrorCode](http://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) element of the **UserResponse** element set to **NoError** and containing the requested user settings.</span></span> <span data-ttu-id="0b1f2-170">Les paramètres utilisateur demandé uniquement, **InternalEwsUrl** et **ExternalEwsUrl**, sont renvoyés.</span><span class="sxs-lookup"><span data-stu-id="0b1f2-170">Only the requested user settings, **InternalEwsUrl** and **ExternalEwsUrl**, are returned.</span></span> <span data-ttu-id="0b1f2-171">L’exemple suivant montre la réponse du serveur.</span><span class="sxs-lookup"><span data-stu-id="0b1f2-171">The following example shows the response from the server.</span></span> 
  
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

## <a name="next-steps"></a><span data-ttu-id="0b1f2-172">Étapes suivantes</span><span class="sxs-lookup"><span data-stu-id="0b1f2-172">Next steps</span></span>
<span data-ttu-id="0b1f2-173"><a name="bk_Next"> </a></span><span class="sxs-lookup"><span data-stu-id="0b1f2-173"></span></span>

<span data-ttu-id="0b1f2-174">Recherche le point de terminaison en suivant le processus de découverte automatique renvoie le domaine demandé ou les paramètres utilisateur.</span><span class="sxs-lookup"><span data-stu-id="0b1f2-174">Finding the endpoint by following the Autodiscover process returns the requested domain or user settings.</span></span> <span data-ttu-id="0b1f2-175">Pour plus d’informations sur la création d’une demande pour des paramètres spécifiques, consultez les articles suivants :</span><span class="sxs-lookup"><span data-stu-id="0b1f2-175">For information about making a request for specific settings, see the following articles:</span></span>
  
- [<span data-ttu-id="0b1f2-176">Obtenir les paramètres de domaine à partir d’un serveur Exchange</span><span class="sxs-lookup"><span data-stu-id="0b1f2-176">Get domain settings from an Exchange server</span></span>](how-to-get-domain-settings-from-an-exchange-server.md)    
- [<span data-ttu-id="0b1f2-177">Obtenir les paramètres de l’utilisateur Exchange à l’aide de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="0b1f2-177">Get user settings from Exchange by using Autodiscover</span></span>](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
## <a name="see-also"></a><span data-ttu-id="0b1f2-178">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0b1f2-178">See also</span></span>

- [<span data-ttu-id="0b1f2-179">La configuration de vos applications EWS</span><span class="sxs-lookup"><span data-stu-id="0b1f2-179">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)   
- [<span data-ttu-id="0b1f2-180">Découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="0b1f2-180">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md)    
- [<span data-ttu-id="0b1f2-181">Référence de service web de découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="0b1f2-181">Autodiscover web service reference for Exchange</span></span>](http://msdn.microsoft.com/library/a01124a8-a8cf-4b80-8625-d7ee05690bca%28Office.15%29.aspx)    
- [<span data-ttu-id="0b1f2-182">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="0b1f2-182">EWS reference for Exchange</span></span>](http://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx)
    

