---
title: Opération GetAppMarketplaceUrl
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2c016fc3-0e13-4624-9a5b-d3e84577a860
description: Trouvez des informations sur l’opération EWS GetAppMarketplaceUrl.
ms.openlocfilehash: 6797af44c3aaa6653c440b3d53a282d8c90a4381
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459524"
---
# <a name="getappmarketplaceurl-operation"></a><span data-ttu-id="76f1d-103">Opération GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="76f1d-103">GetAppMarketplaceUrl operation</span></span>

<span data-ttu-id="76f1d-104">Trouvez des informations sur l’opération EWS **GetAppMarketplaceUrl** .</span><span class="sxs-lookup"><span data-stu-id="76f1d-104">Find information about the **GetAppMarketplaceUrl** EWS operation.</span></span> 
  
<span data-ttu-id="76f1d-105">L’opération **GetAppMarketplaceUrl** récupère l’URL du Marketplace d’application qu’un client peut visiter pour acquérir des applications à installer dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="76f1d-105">The **GetAppMarketplaceUrl** operation retrieves the URL for the app marketplace that a client can visit to acquire apps to install in a mailbox.</span></span> 
  
<span data-ttu-id="76f1d-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="76f1d-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getappmarketplaceurl-operation"></a><span data-ttu-id="76f1d-107">Utilisation de l’opération GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="76f1d-107">Using the GetAppMarketplaceUrl operation</span></span>

<span data-ttu-id="76f1d-108">L’opération **GetAppMarketplaceUrl** ne prend aucun argument pour demander l’URL pour la Marketplace à partir de laquelle un client peut installer des applications.</span><span class="sxs-lookup"><span data-stu-id="76f1d-108">The **GetAppMarketplaceUrl** operation does not take any arguments to request the URL for the marketplace from which a client can install apps.</span></span> <span data-ttu-id="76f1d-109">La réponse contient une URL vers le Marketplace d’application.</span><span class="sxs-lookup"><span data-stu-id="76f1d-109">The response will contain a URL to the app marketplace.</span></span> 
  
### <a name="getappmarketplaceurl-operation-soap-headers"></a><span data-ttu-id="76f1d-110">En-têtes SOAP d’opération GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="76f1d-110">GetAppMarketplaceUrl operation SOAP headers</span></span>

<span data-ttu-id="76f1d-111">L’opération **GetAppMarketplaceUrl** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="76f1d-111">The **GetAppMarketplaceUrl** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="76f1d-112">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="76f1d-112">**Header name**</span></span>|<span data-ttu-id="76f1d-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="76f1d-113">**Element**</span></span>|<span data-ttu-id="76f1d-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="76f1d-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="76f1d-115">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="76f1d-115">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="76f1d-116">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="76f1d-116">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="76f1d-117">Identifie la version de schéma de la demande d’opération.</span><span class="sxs-lookup"><span data-stu-id="76f1d-117">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="76f1d-118">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="76f1d-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="76f1d-119">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="76f1d-119">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="76f1d-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="76f1d-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="76f1d-121">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="76f1d-121">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="76f1d-122">Cet en-tête s’applique à une réponse.</span><span class="sxs-lookup"><span data-stu-id="76f1d-122">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getappmarketplaceurl-operation-request-example-get-the-app-marketplace-url-for-a-mailbox"></a><span data-ttu-id="76f1d-123">Exemple de requête d’opération GetAppMarketplaceUrl : obtenir l’URL d’application Marketplace pour une boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="76f1d-123">GetAppMarketplaceUrl operation request example: Get the app marketplace URL for a mailbox</span></span>

<span data-ttu-id="76f1d-124">L’exemple suivant de demande d’opération **GetAppMarketplaceUrl** indique comment obtenir l’URL d’application Marketplace pour une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="76f1d-124">The following example of a **GetAppMarketplaceUrl** operation request shows how to get the app marketplace URL for a mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013_SP1" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
      <t:TimeZoneContext>
         <t:TimeZoneDefinition Id="GMT Standard Time"/>
      </t:TimeZoneContext>
   </soap:Header>
   <soap:Body >
      <m:GetAppMarketplaceUrl>
        <m:ApiVersionSupported>1.0</m:ApiVersionSupported>
        <m:SchemaVersionSupported>1.0</m:SchemaVersionSupported>
      </m:GetAppMarketplaceUrl>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="76f1d-125">Le corps SOAP de la demande contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="76f1d-125">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="76f1d-126">GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="76f1d-126">GetAppMarketplaceUrl</span></span>](getappmarketplaceurl.md)
    
- [<span data-ttu-id="76f1d-127">ApiVersionSupported</span><span class="sxs-lookup"><span data-stu-id="76f1d-127">ApiVersionSupported</span></span>](apiversionsupported.md)
    
- [<span data-ttu-id="76f1d-128">SchemaVersionSupported</span><span class="sxs-lookup"><span data-stu-id="76f1d-128">SchemaVersionSupported</span></span>](schemaversionsupported.md)
    
## <a name="successful-getappmarketplaceurl-operation-response"></a><span data-ttu-id="76f1d-129">Réponse de l’opération GetAppMarketplaceUrl réussie</span><span class="sxs-lookup"><span data-stu-id="76f1d-129">Successful GetAppMarketplaceUrl operation response</span></span>

<span data-ttu-id="76f1d-130">L’exemple suivant montre une réponse réussie à une demande d’opération **GetAppMarketplaceUrl** pour obtenir l’URL d’application Marketplace pour une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="76f1d-130">The following example shows a successful response to a **GetAppMarketplaceUrl** operation request to get the app marketplace URL for a mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="76f1d-131">L’URL d’application Marketplace a été modifiée afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="76f1d-131">The app marketplace URL has been altered to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="918" 
                           MinorBuildNumber="7" 
                           Version="V2_10" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetAppMarketplaceUrlResponse ResponseClass="Success" 
                                    xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <AppMarketplaceUrl>http://marketplace.contoso.com</AppMarketplaceUrl>
      </GetAppMarketplaceUrlResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="76f1d-132">Le corps SOAP de réponse contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="76f1d-132">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="76f1d-133">GetAppMarketplaceUrlResponse</span><span class="sxs-lookup"><span data-stu-id="76f1d-133">GetAppMarketplaceUrlResponse</span></span>](getappmarketplaceurlresponse.md)
    
- [<span data-ttu-id="76f1d-134">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="76f1d-134">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="76f1d-135">AppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="76f1d-135">AppMarketplaceUrl</span></span>](appmarketplaceurl.md)
    
## <a name="getappmarketplaceurl-operation-error-response"></a><span data-ttu-id="76f1d-136">Réponse d’erreur d’opération GetAppMarketPlaceUrl</span><span class="sxs-lookup"><span data-stu-id="76f1d-136">GetAppMarketPlaceUrl operation error response</span></span>

<span data-ttu-id="76f1d-137">Les erreurs renvoyées pour cette opération sont liées à une configuration de service incorrecte ou à des erreurs EWS génériques.</span><span class="sxs-lookup"><span data-stu-id="76f1d-137">Errors returned for this operation are either related to an incorrect service configuration or are generic EWS errors.</span></span> <span data-ttu-id="76f1d-138">Pour les codes d’erreur génériques à EWS et spécifiques à cette opération, voir [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="76f1d-138">For error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span> 
  
<span data-ttu-id="76f1d-139">L’exemple suivant montre une réponse d’erreur renvoyée lorsque le panneau de configuration Exchange externe n’est pas configuré.</span><span class="sxs-lookup"><span data-stu-id="76f1d-139">The following example shows an error response that is returned when external Exchange Control Panel (ECP) is not configured.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="918" 
                           MinorBuildNumber="7" 
                           Version="V2_10" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetAppMarketplaceUrlResponse ResponseClass="Error" 
                                    xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Cannot get external ECP URL. This might happen if external ECP URL isn't configured.</MessageText>
         <ResponseCode>ErrorCannotGetExternalEcpUrl</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetAppMarketplaceUrlResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="76f1d-140">Le corps SOAP de la réponse d’erreur contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="76f1d-140">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="76f1d-141">GetAppMarketplaceUrlResponse</span><span class="sxs-lookup"><span data-stu-id="76f1d-141">GetAppMarketplaceUrlResponse</span></span>](getappmarketplaceurlresponse.md)
    
- [<span data-ttu-id="76f1d-142">MessageText</span><span class="sxs-lookup"><span data-stu-id="76f1d-142">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="76f1d-143">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="76f1d-143">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="76f1d-144">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="76f1d-144">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="76f1d-145">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="76f1d-145">See also</span></span>

- [<span data-ttu-id="76f1d-146">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="76f1d-146">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="76f1d-147">Opération DisableApp</span><span class="sxs-lookup"><span data-stu-id="76f1d-147">DisableApp operation</span></span>](disableapp-operation.md)
    
- [<span data-ttu-id="76f1d-148">Opération InstallApp</span><span class="sxs-lookup"><span data-stu-id="76f1d-148">InstallApp operation</span></span>](installapp-operation.md)
    
- [<span data-ttu-id="76f1d-149">Opération UninstallApp</span><span class="sxs-lookup"><span data-stu-id="76f1d-149">UninstallApp operation</span></span>](uninstallapp-operation.md)
    
- [<span data-ttu-id="76f1d-150">Opération GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="76f1d-150">GetAppManifests operation</span></span>](getappmanifests-operation.md)
    

