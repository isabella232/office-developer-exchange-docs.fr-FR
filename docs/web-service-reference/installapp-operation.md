---
title: Opération InstallApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 596eae95-3e78-489a-8bb2-d2dd4a026405
description: Opération de recherche plus d’informations sur la InstallApp EWS.
ms.openlocfilehash: ccc5d2dde949070bae905ff1ebb182c892f07fcb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827951"
---
# <a name="installapp-operation"></a><span data-ttu-id="0ad5e-103">Opération InstallApp</span><span class="sxs-lookup"><span data-stu-id="0ad5e-103">InstallApp operation</span></span>

<span data-ttu-id="0ad5e-104">Trouvez des informations sur l’opération EWS **InstallApp** .</span><span class="sxs-lookup"><span data-stu-id="0ad5e-104">Find information about the **InstallApp** EWS operation.</span></span> 
  
<span data-ttu-id="0ad5e-105">L’opération **InstallApp** installe une application de messagerie pour Outlook dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="0ad5e-105">The **InstallApp** operation installs a mail app for Outlook in a mailbox.</span></span> 
  
<span data-ttu-id="0ad5e-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0ad5e-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-installapp-operation"></a><span data-ttu-id="0ad5e-107">Utilisation de l’opération InstallApp</span><span class="sxs-lookup"><span data-stu-id="0ad5e-107">Using the InstallApp operation</span></span>

<span data-ttu-id="0ad5e-108">L’opération **InstallApp** prend un argument unique qui identifie une application de messagerie à installer.</span><span class="sxs-lookup"><span data-stu-id="0ad5e-108">The **InstallApp** operation takes a single argument that identifies a mail app to install.</span></span> <span data-ttu-id="0ad5e-109">L’argument contient le manifeste pour une application de messagerie codé en base64.</span><span class="sxs-lookup"><span data-stu-id="0ad5e-109">The argument contains the base64-encoded manifest for a mail app.</span></span> 
  
### <a name="installapp-operation-soap-headers"></a><span data-ttu-id="0ad5e-110">En-têtes SOAP InstallApp opération</span><span class="sxs-lookup"><span data-stu-id="0ad5e-110">InstallApp operation SOAP headers</span></span>

<span data-ttu-id="0ad5e-111">L’opération **InstallApp** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="0ad5e-111">The **InstallApp** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="0ad5e-112">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="0ad5e-112">**Header name**</span></span>|<span data-ttu-id="0ad5e-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0ad5e-113">**Element**</span></span>|<span data-ttu-id="0ad5e-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="0ad5e-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="0ad5e-115">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="0ad5e-115">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="0ad5e-116">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="0ad5e-116">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="0ad5e-117">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="0ad5e-117">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="0ad5e-118">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="0ad5e-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="0ad5e-119">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="0ad5e-119">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="0ad5e-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="0ad5e-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="0ad5e-121">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="0ad5e-121">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="0ad5e-122">Cet en-tête est applicable à une réponse.</span><span class="sxs-lookup"><span data-stu-id="0ad5e-122">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="installapp-operation-request-example-install-a-mail-app-in-a-mailbox"></a><span data-ttu-id="0ad5e-123">Exemple de requête d’opération InstallApp : installer une application de messagerie dans une boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="0ad5e-123">InstallApp operation request example: Install a mail app in a mailbox</span></span>

<span data-ttu-id="0ad5e-124">Une requête d’opération **InstallApp** l’exemple suivant montre comment installer une application de messagerie pour Outlook.</span><span class="sxs-lookup"><span data-stu-id="0ad5e-124">The following example of an **InstallApp** operation request shows how to install a mail app for Outlook.</span></span> <span data-ttu-id="0ad5e-125">Vous trouverez le manifeste d’application à l’aide de l' [opération GetAppManifests](getappmanifests-operation.md).</span><span class="sxs-lookup"><span data-stu-id="0ad5e-125">The app manifest can be found by using the [GetAppManifests operation](getappmanifests-operation.md).</span></span>
  
> [!NOTE]
> <span data-ttu-id="0ad5e-126">Le manifeste d’application codé en base64 a été tronqué arbitrairement afin de préserver la lisibilité et ne représente pas un manifeste valid.</span><span class="sxs-lookup"><span data-stu-id="0ad5e-126">The base64-encoded app manifest has been arbitrarily truncated to preserve readability and does not represent a valid manifest.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:InstallApp>
         <m:Manifest>TUwiIC8+CiAgPC9SdWxlPgo8L09mZmljZUFwcD4=</m:Manifest>
      </m:InstallApp>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="0ad5e-127">La demande SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="0ad5e-127">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="0ad5e-128">InstallApp</span><span class="sxs-lookup"><span data-stu-id="0ad5e-128">InstallApp</span></span>](installapp.md)
    
- [<span data-ttu-id="0ad5e-129">Manifeste</span><span class="sxs-lookup"><span data-stu-id="0ad5e-129">Manifest</span></span>](manifest.md)
    
## <a name="successful-installapp-operation-response"></a><span data-ttu-id="0ad5e-130">Réponse d’opération InstallApp réussie</span><span class="sxs-lookup"><span data-stu-id="0ad5e-130">Successful InstallApp operation response</span></span>

<span data-ttu-id="0ad5e-131">L’exemple suivant montre une réponse positive à une demande d’opération **InstallApp** pour installer une application de messagerie.</span><span class="sxs-lookup"><span data-stu-id="0ad5e-131">The following example shows a successful response to an **InstallApp** operation request to install a mail app.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <InstallAppResponse ResponseClass="Success" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </InstallAppResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="0ad5e-132">La réponse SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="0ad5e-132">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="0ad5e-133">InstallAppResponse</span><span class="sxs-lookup"><span data-stu-id="0ad5e-133">InstallAppResponse</span></span>](installappresponse.md)
    
- [<span data-ttu-id="0ad5e-134">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0ad5e-134">ResponseCode</span></span>](responsecode.md)
    
## <a name="installapp-operation-error-response"></a><span data-ttu-id="0ad5e-135">Réponse d’erreur d’opération InstallApp</span><span class="sxs-lookup"><span data-stu-id="0ad5e-135">InstallApp operation error response</span></span>

<span data-ttu-id="0ad5e-136">L’exemple suivant montre une réponse d’erreur à une demande d’opération **InstallApp** .</span><span class="sxs-lookup"><span data-stu-id="0ad5e-136">The following example shows an error response to an **InstallApp** operation request.</span></span> <span data-ttu-id="0ad5e-137">Il s’agit d’une réponse à une demande qui contient un manifeste non valide.</span><span class="sxs-lookup"><span data-stu-id="0ad5e-137">This is a response to a request that contains an invalid manifest.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <InstallAppResponse ResponseClass="Error" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>This app can't be installed. Missing OfficeApp element.</MessageText>
         <ResponseCode>ErrorInternalServerError</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </InstallAppResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="0ad5e-138">La réponse d’erreur corps SOAP contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="0ad5e-138">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="0ad5e-139">InstallAppResponse</span><span class="sxs-lookup"><span data-stu-id="0ad5e-139">InstallAppResponse</span></span>](installappresponse.md)
    
- [<span data-ttu-id="0ad5e-140">MessageText</span><span class="sxs-lookup"><span data-stu-id="0ad5e-140">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="0ad5e-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0ad5e-141">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0ad5e-142">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="0ad5e-142">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="0ad5e-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0ad5e-143">See also</span></span>

- [<span data-ttu-id="0ad5e-144">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0ad5e-144">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="0ad5e-145">Opération DisableApp</span><span class="sxs-lookup"><span data-stu-id="0ad5e-145">DisableApp operation</span></span>](disableapp-operation.md)
    
- [<span data-ttu-id="0ad5e-146">Opération UninstallApp</span><span class="sxs-lookup"><span data-stu-id="0ad5e-146">UninstallApp operation</span></span>](uninstallapp-operation.md)
    
- [<span data-ttu-id="0ad5e-147">GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="0ad5e-147">GetAppManifests</span></span>](getappmanifests.md)
    
- [<span data-ttu-id="0ad5e-148">Opération GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="0ad5e-148">GetAppMarketplaceUrl operation</span></span>](getappmarketplaceurl-operation.md)
    

