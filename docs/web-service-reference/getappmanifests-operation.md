---
title: Opération GetAppManifests
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 21a4987c-c24d-4a6e-ace4-e81edcda6303
description: Opération de recherche plus d’informations sur la GetAppManifests EWS.
ms.openlocfilehash: 9c919bac9ac0042890d1c439454b37e6b7c60876
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756509"
---
# <a name="getappmanifests-operation"></a><span data-ttu-id="db139-103">Opération GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="db139-103">GetAppManifests operation</span></span>

<span data-ttu-id="db139-104">Trouvez des informations sur l’opération EWS **GetAppManifests** .</span><span class="sxs-lookup"><span data-stu-id="db139-104">Find information about the **GetAppManifests** EWS operation.</span></span> 
  
<span data-ttu-id="db139-105">L’opération **GetAppManifests** récupère des manifestes d’application.</span><span class="sxs-lookup"><span data-stu-id="db139-105">The **GetAppManifests** operation retrieves app manifests.</span></span> 
  
<span data-ttu-id="db139-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="db139-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getappmanifests-operation"></a><span data-ttu-id="db139-107">Utilisation de l’opération GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="db139-107">Using the GetAppManifests operation</span></span>

<span data-ttu-id="db139-108">L’opération **GetAppManifests** ne prend aucun argument pour demander les manifestes d’application pour une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="db139-108">The **GetAppManifests** operation does not take any arguments to request the app manifests for a mailbox.</span></span> <span data-ttu-id="db139-109">La réponse contient codé en base64 les fichiers manifeste XML pour chaque application est installée dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="db139-109">The response will contain base64-encoded XML manifest files for each app that is installed in a mailbox.</span></span> 
  
### <a name="getappmanifests-operation-soap-headers"></a><span data-ttu-id="db139-110">En-têtes SOAP GetAppManifests opération</span><span class="sxs-lookup"><span data-stu-id="db139-110">GetAppManifests operation SOAP headers</span></span>

<span data-ttu-id="db139-111">L’opération **GetAppManifests** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="db139-111">The **GetAppManifests** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="db139-112">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="db139-112">**Header name**</span></span>|<span data-ttu-id="db139-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="db139-113">**Element**</span></span>|<span data-ttu-id="db139-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="db139-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="db139-115">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="db139-115">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="db139-116">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="db139-116">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="db139-117">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="db139-117">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="db139-118">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="db139-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="db139-119">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="db139-119">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="db139-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="db139-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="db139-121">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="db139-121">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="db139-122">Cet en-tête est applicable à une réponse.</span><span class="sxs-lookup"><span data-stu-id="db139-122">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getappmanifests-operation-request-example-get-the-app-manifests-for-a-mailbox"></a><span data-ttu-id="db139-123">Exemple de requête d’opération GetAppManifests : obtenir les manifestes d’application pour une boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="db139-123">GetAppManifests operation request example: Get the app manifests for a mailbox</span></span>

<span data-ttu-id="db139-124">Une demande d’opération **GetAppManifests** l’exemple suivant montre comment obtenir les manifestes d’application pour une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="db139-124">The following example of a **GetAppManifests** operation request shows how to get the app manifests for a mailbox.</span></span> <span data-ttu-id="db139-125">L’élément [ApiVersionSupported](apiversionsupported.md) et l’élément [SchemaVersionSupported](schemaversionsupported.md) sont facultatives.</span><span class="sxs-lookup"><span data-stu-id="db139-125">The [ApiVersionSupported](apiversionsupported.md) element and the [SchemaVersionSupported](schemaversionsupported.md) element are optional.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="db139-126">La demande SOAP body contienne l’élément suivant :</span><span class="sxs-lookup"><span data-stu-id="db139-126">The request SOAP body contains the following element:</span></span>
  
- [<span data-ttu-id="db139-127">GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="db139-127">GetAppManifests</span></span>](getappmanifests.md)
    
- [<span data-ttu-id="db139-128">ApiVersionSupported</span><span class="sxs-lookup"><span data-stu-id="db139-128">ApiVersionSupported</span></span>](apiversionsupported.md)
    
- [<span data-ttu-id="db139-129">SchemaVersionSupported</span><span class="sxs-lookup"><span data-stu-id="db139-129">SchemaVersionSupported</span></span>](schemaversionsupported.md)
    
## <a name="successful-getappmanifests-operation-response"></a><span data-ttu-id="db139-130">Réponse d’opération GetAppManifests réussie</span><span class="sxs-lookup"><span data-stu-id="db139-130">Successful GetAppManifests operation response</span></span>

<span data-ttu-id="db139-131">L’exemple suivant montre une réponse positive à une demande d’opération **GetAppManifests** pour obtenir les manifestes d’application pour une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="db139-131">The following example shows a successful response to a **GetAppManifests** operation request to get the app manifests for a mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="db139-132">Tous les manifestes d’application en base64 ont été tronquées arbitrairement afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="db139-132">All base64 app manifests have been arbitrarily truncated to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="918" 
                           MinorBuildNumber="07" 
                           Version="V2_10" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetAppManifestsResponse ResponseClass="Success" 
                               xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <m:Apps xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
          <t:App xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
            <t:Manifest>WNlQXBwPg==</t:Manifest>
          </t:App>
         </m:Apps>
      </GetAppManifestsResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="db139-133">La réponse SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="db139-133">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="db139-134">GetAppManifestsResponse</span><span class="sxs-lookup"><span data-stu-id="db139-134">GetAppManifestsResponse</span></span>](getappmanifestsresponse.md)
    
- [<span data-ttu-id="db139-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="db139-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="db139-136">Applications</span><span class="sxs-lookup"><span data-stu-id="db139-136">Apps</span></span>](apps.md)
    
- [<span data-ttu-id="db139-137">App</span><span class="sxs-lookup"><span data-stu-id="db139-137">App</span></span>](app.md)
    
- [<span data-ttu-id="db139-138">Manifeste</span><span class="sxs-lookup"><span data-stu-id="db139-138">Manifest</span></span>](manifest.md)
    
<span data-ttu-id="db139-139">La réponse SOAP body peut également contenir l’élément suivant :</span><span class="sxs-lookup"><span data-stu-id="db139-139">The response SOAP body can also contain the following element:</span></span>
  
- [<span data-ttu-id="db139-140">Manifestes</span><span class="sxs-lookup"><span data-stu-id="db139-140">Manifests</span></span>](manifests.md)
    
## <a name="getappmanifests-operation-error-response"></a><span data-ttu-id="db139-141">Réponse d’erreur d’opération GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="db139-141">GetAppManifests operation error response</span></span>

<span data-ttu-id="db139-142">Erreurs renvoyées pour cette opération sont liés à un format non valide pour les paramètres d’entrée ou sont erreurs EWS génériques.</span><span class="sxs-lookup"><span data-stu-id="db139-142">Errors returned for this operation are related to an invalid format of the input parameters or are generic EWS errors.</span></span> <span data-ttu-id="db139-143">Codes d’erreur générique à EWS sont spécifiques à cette opération, consultez la rubrique [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="db139-143">For error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
```
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="918"
                       MinorBuildNumber="07"
                       Version="V2_10"
                       xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetAppManifestsResponse ResponseClass="Error"
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <MessageText>The apiVersionSupported parameter is invalid. 
                   It should be in the form of major version, minor 
                   version, separated by '.', for example '2.34'.</MessageText>
      <ResponseCode>ErrorInvalidRequest</ResponseCode>
      <DescriptiveLinkKey>0</DescriptiveLinkKey>
    </GetAppManifestsResponse>
  </s:Body>
</s:Envelope>

```

## <a name="see-also"></a><span data-ttu-id="db139-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="db139-144">See also</span></span>

- [<span data-ttu-id="db139-145">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="db139-145">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="db139-146">Opération DisableApp</span><span class="sxs-lookup"><span data-stu-id="db139-146">DisableApp operation</span></span>](disableapp-operation.md)
    
- [<span data-ttu-id="db139-147">Opération InstallApp</span><span class="sxs-lookup"><span data-stu-id="db139-147">InstallApp operation</span></span>](installapp-operation.md)
    
- [<span data-ttu-id="db139-148">Opération UninstallApp</span><span class="sxs-lookup"><span data-stu-id="db139-148">UninstallApp operation</span></span>](uninstallapp-operation.md)
    
- [<span data-ttu-id="db139-149">Opération GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="db139-149">GetAppMarketplaceUrl operation</span></span>](getappmarketplaceurl-operation.md)
    

