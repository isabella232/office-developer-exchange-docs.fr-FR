---
title: Opération UninstallApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7707aa6a-381d-43f7-a454-54f6343ed127
description: Opération de recherche plus d’informations sur la UninstallApp EWS.
ms.openlocfilehash: 4f44224651993023336eef5540ec29b7f6a6e32e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838808"
---
# <a name="uninstallapp-operation"></a><span data-ttu-id="ccec5-103">Opération UninstallApp</span><span class="sxs-lookup"><span data-stu-id="ccec5-103">UninstallApp operation</span></span>

<span data-ttu-id="ccec5-104">Trouvez des informations sur l’opération EWS **UninstallApp** .</span><span class="sxs-lookup"><span data-stu-id="ccec5-104">Find information about the **UninstallApp** EWS operation.</span></span> 
  
<span data-ttu-id="ccec5-105">L’opération **UninstallApp** désinstalle une application de messagerie pour Outlook.</span><span class="sxs-lookup"><span data-stu-id="ccec5-105">The **UninstallApp** operation uninstalls a mail app for Outlook.</span></span> 
  
<span data-ttu-id="ccec5-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ccec5-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-uninstallapp-operation"></a><span data-ttu-id="ccec5-107">Utilisation de l’opération UninstallApp</span><span class="sxs-lookup"><span data-stu-id="ccec5-107">Using the UninstallApp operation</span></span>

<span data-ttu-id="ccec5-108">L’opération **UninstallApp** prend un argument dans la demande qui identifie l’application de messagerie pour désinstaller.</span><span class="sxs-lookup"><span data-stu-id="ccec5-108">The **UninstallApp** operation takes one argument in the request that identifies the mail app to uninstall.</span></span> 
  
### <a name="uninstallapp-operation-soap-headers"></a><span data-ttu-id="ccec5-109">En-têtes SOAP UninstallApp opération</span><span class="sxs-lookup"><span data-stu-id="ccec5-109">UninstallApp operation SOAP headers</span></span>

<span data-ttu-id="ccec5-110">L’opération **UninstallApp** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="ccec5-110">The **UninstallApp** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="ccec5-111">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="ccec5-111">**Header name**</span></span>|<span data-ttu-id="ccec5-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ccec5-112">**Element**</span></span>|<span data-ttu-id="ccec5-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="ccec5-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ccec5-114">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="ccec5-114">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="ccec5-115">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="ccec5-115">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="ccec5-116">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="ccec5-116">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="ccec5-117">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="ccec5-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="ccec5-118">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="ccec5-118">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="ccec5-119">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ccec5-119">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="ccec5-120">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="ccec5-120">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="ccec5-121">Cet en-tête est applicable à une réponse.</span><span class="sxs-lookup"><span data-stu-id="ccec5-121">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="uninstallapp-operation-request-example-uninstall-a-mail-app-in-a-mailbox"></a><span data-ttu-id="ccec5-122">Exemple de requête d’opération UninstallApp : désinstaller une application de messagerie dans une boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="ccec5-122">UninstallApp operation request example: Uninstall a mail app in a mailbox</span></span>

<span data-ttu-id="ccec5-123">L’exemple suivant d’une opération **UninstallApp** demande montre comment à une désinstallation une application de messagerie à l’aide de l’identificateur de l’application.</span><span class="sxs-lookup"><span data-stu-id="ccec5-123">The following example of an **UninstallApp** operation request shows how to a uninstall a mail app by using the app identifier.</span></span> <span data-ttu-id="ccec5-124">L’identificateur de l’application peut être trouvé dans le manifeste d’application qui est retourné par l' [opération GetAppManifests](getappmanifests-operation.md).</span><span class="sxs-lookup"><span data-stu-id="ccec5-124">The app identifier can be found in the app manifest that is returned by the [GetAppManifests operation](getappmanifests-operation.md).</span></span>
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:UninstallApp>
         <m:ID>1C50226D-04B5-4AB2-9FCD-42E236B59E4B</m:ID>
      </m:UninstallApp>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="ccec5-125">La demande SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="ccec5-125">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="ccec5-126">UninstallApp</span><span class="sxs-lookup"><span data-stu-id="ccec5-126">UninstallApp</span></span>](uninstallapp.md)
    
- [<span data-ttu-id="ccec5-127">ID (chaîne)</span><span class="sxs-lookup"><span data-stu-id="ccec5-127">ID (String)</span></span>](id-string.md)
    
## <a name="successful-uninstallapp-operation-response"></a><span data-ttu-id="ccec5-128">Réponse d’opération UninstallApp réussie</span><span class="sxs-lookup"><span data-stu-id="ccec5-128">Successful UninstallApp operation response</span></span>

<span data-ttu-id="ccec5-129">L’exemple suivant montre une réponse positive à une demande d’opération **UninstallApp** pour désinstaller une application de messagerie.</span><span class="sxs-lookup"><span data-stu-id="ccec5-129">The following example shows a successful response to an **UninstallApp** operation request to uninstall a mail app.</span></span> 
  
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
      <UninstallAppResponse ResponseClass="Success" 
                            xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </UninstallAppResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="ccec5-130">La réponse SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="ccec5-130">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="ccec5-131">UninstallAppResponse</span><span class="sxs-lookup"><span data-stu-id="ccec5-131">UninstallAppResponse</span></span>](uninstallappresponse.md)
    
- [<span data-ttu-id="ccec5-132">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ccec5-132">ResponseCode</span></span>](responsecode.md)
    
## <a name="uninstallapp-operation-error-response"></a><span data-ttu-id="ccec5-133">Réponse d’erreur d’opération UninstallApp</span><span class="sxs-lookup"><span data-stu-id="ccec5-133">UninstallApp operation error response</span></span>

<span data-ttu-id="ccec5-134">L’exemple suivant montre une réponse d’erreur à une demande d’opération **UninstallApp** .</span><span class="sxs-lookup"><span data-stu-id="ccec5-134">The following example shows an error response to an **UninstallApp** operation request.</span></span> <span data-ttu-id="ccec5-135">Il s’agit d’une réponse à une demande pour désinstaller une application de messagerie qui a déjà été désinstallée.</span><span class="sxs-lookup"><span data-stu-id="ccec5-135">This is a response to a request to uninstall a mail app that has already been uninstalled.</span></span> 
  
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
      <UninstallAppResponse ResponseClass="Error" 
                            xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Extension ID 1c50226d-04b5-4ab2-9fcd-42e236b59e4b can't be found.</MessageText>
         <ResponseCode>ErrorInternalServerError</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </UninstallAppResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="ccec5-136">La réponse d’erreur corps SOAP contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="ccec5-136">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="ccec5-137">UninstallAppResponse</span><span class="sxs-lookup"><span data-stu-id="ccec5-137">UninstallAppResponse</span></span>](uninstallappresponse.md)
    
- [<span data-ttu-id="ccec5-138">MessageText</span><span class="sxs-lookup"><span data-stu-id="ccec5-138">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="ccec5-139">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ccec5-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ccec5-140">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="ccec5-140">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="ccec5-141">Pour les codes d’erreur générique à EWS, spécifiques à cette opération, consultez la rubrique [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="ccec5-141">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="ccec5-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ccec5-142">See also</span></span>

- [<span data-ttu-id="ccec5-143">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ccec5-143">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="ccec5-144">Opération InstallApp</span><span class="sxs-lookup"><span data-stu-id="ccec5-144">InstallApp operation</span></span>](installapp-operation.md)
    
- [<span data-ttu-id="ccec5-145">Opération DisableApp</span><span class="sxs-lookup"><span data-stu-id="ccec5-145">DisableApp operation</span></span>](disableapp-operation.md)
    
- [<span data-ttu-id="ccec5-146">GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="ccec5-146">GetAppManifests</span></span>](getappmanifests.md)
    
- [<span data-ttu-id="ccec5-147">Opération GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="ccec5-147">GetAppMarketplaceUrl operation</span></span>](getappmarketplaceurl-operation.md)
    

