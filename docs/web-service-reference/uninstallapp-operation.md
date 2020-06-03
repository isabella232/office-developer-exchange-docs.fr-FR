---
title: Opération UninstallApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7707aa6a-381d-43f7-a454-54f6343ed127
description: Trouvez des informations sur l’opération EWS UninstallApp.
ms.openlocfilehash: 27931636ee13a251fb03fe804987d7b01a325230
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467150"
---
# <a name="uninstallapp-operation"></a><span data-ttu-id="cb631-103">Opération UninstallApp</span><span class="sxs-lookup"><span data-stu-id="cb631-103">UninstallApp operation</span></span>

<span data-ttu-id="cb631-104">Trouvez des informations sur l’opération EWS **UninstallApp** .</span><span class="sxs-lookup"><span data-stu-id="cb631-104">Find information about the **UninstallApp** EWS operation.</span></span> 
  
<span data-ttu-id="cb631-105">L’opération **UninstallApp** désinstalle une application de messagerie pour Outlook.</span><span class="sxs-lookup"><span data-stu-id="cb631-105">The **UninstallApp** operation uninstalls a mail app for Outlook.</span></span> 
  
<span data-ttu-id="cb631-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="cb631-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-uninstallapp-operation"></a><span data-ttu-id="cb631-107">Utilisation de l’opération UninstallApp</span><span class="sxs-lookup"><span data-stu-id="cb631-107">Using the UninstallApp operation</span></span>

<span data-ttu-id="cb631-108">L’opération **UninstallApp** prend un argument dans la demande qui identifie l’application de messagerie à désinstaller.</span><span class="sxs-lookup"><span data-stu-id="cb631-108">The **UninstallApp** operation takes one argument in the request that identifies the mail app to uninstall.</span></span> 
  
### <a name="uninstallapp-operation-soap-headers"></a><span data-ttu-id="cb631-109">En-têtes SOAP d’opération UninstallApp</span><span class="sxs-lookup"><span data-stu-id="cb631-109">UninstallApp operation SOAP headers</span></span>

<span data-ttu-id="cb631-110">L’opération **UninstallApp** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="cb631-110">The **UninstallApp** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="cb631-111">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="cb631-111">**Header name**</span></span>|<span data-ttu-id="cb631-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="cb631-112">**Element**</span></span>|<span data-ttu-id="cb631-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="cb631-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="cb631-114">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="cb631-114">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="cb631-115">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="cb631-115">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="cb631-116">Identifie la version de schéma de la demande d’opération.</span><span class="sxs-lookup"><span data-stu-id="cb631-116">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="cb631-117">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="cb631-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="cb631-118">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="cb631-118">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="cb631-119">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="cb631-119">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="cb631-120">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="cb631-120">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="cb631-121">Cet en-tête s’applique à une réponse.</span><span class="sxs-lookup"><span data-stu-id="cb631-121">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="uninstallapp-operation-request-example-uninstall-a-mail-app-in-a-mailbox"></a><span data-ttu-id="cb631-122">Exemple de requête d’opération UninstallApp : désinstaller une application de messagerie dans une boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="cb631-122">UninstallApp operation request example: Uninstall a mail app in a mailbox</span></span>

<span data-ttu-id="cb631-123">L’exemple suivant de demande d’opération **UninstallApp** montre comment désinstaller une application de messagerie à l’aide de l’identificateur d’application.</span><span class="sxs-lookup"><span data-stu-id="cb631-123">The following example of an **UninstallApp** operation request shows how to a uninstall a mail app by using the app identifier.</span></span> <span data-ttu-id="cb631-124">L’identificateur de l’application se trouve dans le manifeste de l’application qui est renvoyé par l' [opération GetAppManifests](getappmanifests-operation.md).</span><span class="sxs-lookup"><span data-stu-id="cb631-124">The app identifier can be found in the app manifest that is returned by the [GetAppManifests operation](getappmanifests-operation.md).</span></span>
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="cb631-125">Le corps SOAP de la demande contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="cb631-125">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="cb631-126">UninstallApp</span><span class="sxs-lookup"><span data-stu-id="cb631-126">UninstallApp</span></span>](uninstallapp.md)
    
- [<span data-ttu-id="cb631-127">ID (chaîne)</span><span class="sxs-lookup"><span data-stu-id="cb631-127">ID (String)</span></span>](id-string.md)
    
## <a name="successful-uninstallapp-operation-response"></a><span data-ttu-id="cb631-128">Réponse de l’opération UninstallApp réussie</span><span class="sxs-lookup"><span data-stu-id="cb631-128">Successful UninstallApp operation response</span></span>

<span data-ttu-id="cb631-129">L’exemple suivant montre une réponse réussie à une demande d’opération **UninstallApp** pour désinstaller une application de messagerie.</span><span class="sxs-lookup"><span data-stu-id="cb631-129">The following example shows a successful response to an **UninstallApp** operation request to uninstall a mail app.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <UninstallAppResponse ResponseClass="Success" 
                            xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </UninstallAppResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="cb631-130">Le corps SOAP de réponse contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="cb631-130">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="cb631-131">UninstallAppResponse</span><span class="sxs-lookup"><span data-stu-id="cb631-131">UninstallAppResponse</span></span>](uninstallappresponse.md)
    
- [<span data-ttu-id="cb631-132">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="cb631-132">ResponseCode</span></span>](responsecode.md)
    
## <a name="uninstallapp-operation-error-response"></a><span data-ttu-id="cb631-133">Réponse d’erreur d’opération UninstallApp</span><span class="sxs-lookup"><span data-stu-id="cb631-133">UninstallApp operation error response</span></span>

<span data-ttu-id="cb631-134">L’exemple suivant montre une réponse d’erreur à une demande d’opération **UninstallApp** .</span><span class="sxs-lookup"><span data-stu-id="cb631-134">The following example shows an error response to an **UninstallApp** operation request.</span></span> <span data-ttu-id="cb631-135">Il s’agit d’une réponse à une demande de désinstallation d’une application de messagerie qui a déjà été désinstallée.</span><span class="sxs-lookup"><span data-stu-id="cb631-135">This is a response to a request to uninstall a mail app that has already been uninstalled.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <UninstallAppResponse ResponseClass="Error" 
                            xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Extension ID 1c50226d-04b5-4ab2-9fcd-42e236b59e4b can't be found.</MessageText>
         <ResponseCode>ErrorInternalServerError</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </UninstallAppResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="cb631-136">Le corps SOAP de la réponse d’erreur contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="cb631-136">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="cb631-137">UninstallAppResponse</span><span class="sxs-lookup"><span data-stu-id="cb631-137">UninstallAppResponse</span></span>](uninstallappresponse.md)
    
- [<span data-ttu-id="cb631-138">MessageText</span><span class="sxs-lookup"><span data-stu-id="cb631-138">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="cb631-139">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="cb631-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="cb631-140">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="cb631-140">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="cb631-141">Pour les autres codes d’erreur qui sont génériques à EWS et spécifiques à cette opération, voir [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="cb631-141">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="cb631-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="cb631-142">See also</span></span>

- [<span data-ttu-id="cb631-143">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="cb631-143">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="cb631-144">Opération InstallApp</span><span class="sxs-lookup"><span data-stu-id="cb631-144">InstallApp operation</span></span>](installapp-operation.md)
    
- [<span data-ttu-id="cb631-145">Opération DisableApp</span><span class="sxs-lookup"><span data-stu-id="cb631-145">DisableApp operation</span></span>](disableapp-operation.md)
    
- [<span data-ttu-id="cb631-146">GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="cb631-146">GetAppManifests</span></span>](getappmanifests.md)
    
- [<span data-ttu-id="cb631-147">Opération GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="cb631-147">GetAppMarketplaceUrl operation</span></span>](getappmarketplaceurl-operation.md)
    

