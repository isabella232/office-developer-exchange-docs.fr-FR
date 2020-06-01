---
title: Opération GetAppManifests
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 21a4987c-c24d-4a6e-ace4-e81edcda6303
description: Trouvez des informations sur l’opération EWS GetAppManifests.
ms.openlocfilehash: 4d4c1d32f14cf144335ddfdf8c9cd4c88a4421d0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463005"
---
# <a name="getappmanifests-operation"></a><span data-ttu-id="d80fb-103">Opération GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="d80fb-103">GetAppManifests operation</span></span>

<span data-ttu-id="d80fb-104">Trouvez des informations sur l’opération EWS **GetAppManifests** .</span><span class="sxs-lookup"><span data-stu-id="d80fb-104">Find information about the **GetAppManifests** EWS operation.</span></span> 
  
<span data-ttu-id="d80fb-105">L’opération **GetAppManifests** récupère les manifestes d’application.</span><span class="sxs-lookup"><span data-stu-id="d80fb-105">The **GetAppManifests** operation retrieves app manifests.</span></span> 
  
<span data-ttu-id="d80fb-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d80fb-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getappmanifests-operation"></a><span data-ttu-id="d80fb-107">Utilisation de l’opération GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="d80fb-107">Using the GetAppManifests operation</span></span>

<span data-ttu-id="d80fb-108">L’opération **GetAppManifests** ne prend aucun argument pour demander les manifestes d’application pour une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d80fb-108">The **GetAppManifests** operation does not take any arguments to request the app manifests for a mailbox.</span></span> <span data-ttu-id="d80fb-109">La réponse contient des fichiers manifeste XML codés en base64 pour chaque application installée dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d80fb-109">The response will contain base64-encoded XML manifest files for each app that is installed in a mailbox.</span></span> 
  
### <a name="getappmanifests-operation-soap-headers"></a><span data-ttu-id="d80fb-110">En-têtes SOAP d’opération GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="d80fb-110">GetAppManifests operation SOAP headers</span></span>

<span data-ttu-id="d80fb-111">L’opération **GetAppManifests** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="d80fb-111">The **GetAppManifests** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="d80fb-112">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="d80fb-112">**Header name**</span></span>|<span data-ttu-id="d80fb-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d80fb-113">**Element**</span></span>|<span data-ttu-id="d80fb-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="d80fb-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d80fb-115">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="d80fb-115">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="d80fb-116">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="d80fb-116">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="d80fb-117">Identifie la version de schéma de la demande d’opération.</span><span class="sxs-lookup"><span data-stu-id="d80fb-117">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="d80fb-118">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="d80fb-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="d80fb-119">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="d80fb-119">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="d80fb-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="d80fb-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="d80fb-121">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="d80fb-121">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="d80fb-122">Cet en-tête s’applique à une réponse.</span><span class="sxs-lookup"><span data-stu-id="d80fb-122">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getappmanifests-operation-request-example-get-the-app-manifests-for-a-mailbox"></a><span data-ttu-id="d80fb-123">Exemple de requête d’opération GetAppManifests : obtenir les manifestes d’application pour une boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="d80fb-123">GetAppManifests operation request example: Get the app manifests for a mailbox</span></span>

<span data-ttu-id="d80fb-124">L’exemple suivant de demande d’opération **GetAppManifests** indique comment obtenir les manifestes d’application pour une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d80fb-124">The following example of a **GetAppManifests** operation request shows how to get the app manifests for a mailbox.</span></span> <span data-ttu-id="d80fb-125">L’élément [ApiVersionSupported](apiversionsupported.md) et l’élément [SchemaVersionSupported](schemaversionsupported.md) sont facultatifs.</span><span class="sxs-lookup"><span data-stu-id="d80fb-125">The [ApiVersionSupported](apiversionsupported.md) element and the [SchemaVersionSupported](schemaversionsupported.md) element are optional.</span></span> 
  
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
      <m:GetAppManifests>
        <m:ApiVersionSupported>1.1</m:ApiVersionSupported>
        <m:SchemaVersionSupported>1.1</m:SchemaVersionSupported>
      </m:GetAppManifests>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="d80fb-126">Le corps SOAP de la demande contient l’élément suivant :</span><span class="sxs-lookup"><span data-stu-id="d80fb-126">The request SOAP body contains the following element:</span></span>
  
- [<span data-ttu-id="d80fb-127">GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="d80fb-127">GetAppManifests</span></span>](getappmanifests.md)
    
- [<span data-ttu-id="d80fb-128">ApiVersionSupported</span><span class="sxs-lookup"><span data-stu-id="d80fb-128">ApiVersionSupported</span></span>](apiversionsupported.md)
    
- [<span data-ttu-id="d80fb-129">SchemaVersionSupported</span><span class="sxs-lookup"><span data-stu-id="d80fb-129">SchemaVersionSupported</span></span>](schemaversionsupported.md)
    
## <a name="successful-getappmanifests-operation-response"></a><span data-ttu-id="d80fb-130">Réponse de l’opération GetAppManifests réussie</span><span class="sxs-lookup"><span data-stu-id="d80fb-130">Successful GetAppManifests operation response</span></span>

<span data-ttu-id="d80fb-131">L’exemple suivant montre une réponse réussie à une demande d’opération **GetAppManifests** pour obtenir les manifestes d’application pour une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d80fb-131">The following example shows a successful response to a **GetAppManifests** operation request to get the app manifests for a mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="d80fb-132">Tous les manifestes d’application base64 ont été tronqués de manière arbitraire afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="d80fb-132">All base64 app manifests have been arbitrarily truncated to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="918" 
                           MinorBuildNumber="07" 
                           Version="V2_10" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetAppManifestsResponse ResponseClass="Success" 
                               xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <m:Apps xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
          <t:App xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
            <t:Manifest>WNlQXBwPg==</t:Manifest>
          </t:App>
         </m:Apps>
      </GetAppManifestsResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="d80fb-133">Le corps SOAP de réponse contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="d80fb-133">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="d80fb-134">GetAppManifestsResponse</span><span class="sxs-lookup"><span data-stu-id="d80fb-134">GetAppManifestsResponse</span></span>](getappmanifestsresponse.md)
    
- [<span data-ttu-id="d80fb-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d80fb-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="d80fb-136">Applications</span><span class="sxs-lookup"><span data-stu-id="d80fb-136">Apps</span></span>](apps.md)
    
- [<span data-ttu-id="d80fb-137">App</span><span class="sxs-lookup"><span data-stu-id="d80fb-137">App</span></span>](app.md)
    
- [<span data-ttu-id="d80fb-138">Manifeste</span><span class="sxs-lookup"><span data-stu-id="d80fb-138">Manifest</span></span>](manifest.md)
    
<span data-ttu-id="d80fb-139">Le corps SOAP de la réponse peut également contenir l’élément suivant :</span><span class="sxs-lookup"><span data-stu-id="d80fb-139">The response SOAP body can also contain the following element:</span></span>
  
- [<span data-ttu-id="d80fb-140">Manifestes</span><span class="sxs-lookup"><span data-stu-id="d80fb-140">Manifests</span></span>](manifests.md)
    
## <a name="getappmanifests-operation-error-response"></a><span data-ttu-id="d80fb-141">Réponse d’erreur d’opération GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="d80fb-141">GetAppManifests operation error response</span></span>

<span data-ttu-id="d80fb-142">Les erreurs renvoyées pour cette opération sont liées à un format non valide des paramètres d’entrée ou sont des erreurs EWS génériques.</span><span class="sxs-lookup"><span data-stu-id="d80fb-142">Errors returned for this operation are related to an invalid format of the input parameters or are generic EWS errors.</span></span> <span data-ttu-id="d80fb-143">Pour les codes d’erreur génériques à EWS et spécifiques à cette opération, voir [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="d80fb-143">For error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
```
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="918"
                       MinorBuildNumber="07"
                       Version="V2_10"
                       xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetAppManifestsResponse ResponseClass="Error"
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <MessageText>The apiVersionSupported parameter is invalid. 
                   It should be in the form of major version, minor 
                   version, separated by '.', for example '2.34'.</MessageText>
      <ResponseCode>ErrorInvalidRequest</ResponseCode>
      <DescriptiveLinkKey>0</DescriptiveLinkKey>
    </GetAppManifestsResponse>
  </s:Body>
</s:Envelope>

```

## <a name="see-also"></a><span data-ttu-id="d80fb-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d80fb-144">See also</span></span>

- [<span data-ttu-id="d80fb-145">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d80fb-145">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="d80fb-146">Opération DisableApp</span><span class="sxs-lookup"><span data-stu-id="d80fb-146">DisableApp operation</span></span>](disableapp-operation.md)
    
- [<span data-ttu-id="d80fb-147">Opération InstallApp</span><span class="sxs-lookup"><span data-stu-id="d80fb-147">InstallApp operation</span></span>](installapp-operation.md)
    
- [<span data-ttu-id="d80fb-148">Opération UninstallApp</span><span class="sxs-lookup"><span data-stu-id="d80fb-148">UninstallApp operation</span></span>](uninstallapp-operation.md)
    
- [<span data-ttu-id="d80fb-149">Opération GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="d80fb-149">GetAppMarketplaceUrl operation</span></span>](getappmarketplaceurl-operation.md)
    

