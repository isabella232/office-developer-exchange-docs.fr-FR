---
title: Opération DisableApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 211731a3-2470-49af-bda3-1ddfc15a8e46
description: Opération de recherche plus d’informations sur la DisableApp EWS.
ms.openlocfilehash: be9e124d7464012ffa797a69192893d85804a004
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755940"
---
# <a name="disableapp-operation"></a><span data-ttu-id="6b819-103">Opération DisableApp</span><span class="sxs-lookup"><span data-stu-id="6b819-103">DisableApp operation</span></span>

<span data-ttu-id="6b819-104">Trouvez des informations sur l’opération EWS **DisableApp** .</span><span class="sxs-lookup"><span data-stu-id="6b819-104">Find information about the **DisableApp** EWS operation.</span></span> 
  
<span data-ttu-id="6b819-105">L’opération **DisableApp** désactive une application de messagerie pour Outlook.</span><span class="sxs-lookup"><span data-stu-id="6b819-105">The **DisableApp** operation disables a mail app for Outlook.</span></span> 
  
<span data-ttu-id="6b819-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6b819-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-disableapp-operation"></a><span data-ttu-id="6b819-107">Utilisation de l’opération DisableApp</span><span class="sxs-lookup"><span data-stu-id="6b819-107">Using the DisableApp operation</span></span>

<span data-ttu-id="6b819-108">L’opération **DisableApp** prend deux arguments qui identifient l’application de messagerie pour désactiver la demande et la raison pourquoi il a été désactivé.</span><span class="sxs-lookup"><span data-stu-id="6b819-108">The **DisableApp** operation takes two arguments in the request that identify the mail app to disable and the reason why it was disabled.</span></span> 
  
### <a name="disableapp-operation-soap-headers"></a><span data-ttu-id="6b819-109">En-têtes SOAP DisableApp opération</span><span class="sxs-lookup"><span data-stu-id="6b819-109">DisableApp operation SOAP headers</span></span>

<span data-ttu-id="6b819-110">L’opération **DisableApp** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="6b819-110">The **DisableApp** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="6b819-111">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="6b819-111">**Header name**</span></span>|<span data-ttu-id="6b819-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6b819-112">**Element**</span></span>|<span data-ttu-id="6b819-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="6b819-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="6b819-114">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="6b819-114">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="6b819-115">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="6b819-115">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="6b819-116">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="6b819-116">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="6b819-117">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="6b819-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="6b819-118">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="6b819-118">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="6b819-119">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="6b819-119">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="6b819-120">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="6b819-120">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="6b819-121">Cet en-tête est applicable à une réponse.</span><span class="sxs-lookup"><span data-stu-id="6b819-121">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="disableapp-operation-request-example-disable-a-mail-app-installed-in-a-mailbox"></a><span data-ttu-id="6b819-122">Exemple de requête d’opération DisableApp : désactiver une application de messagerie installée dans une boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="6b819-122">DisableApp operation request example: Disable a mail app installed in a mailbox</span></span>

<span data-ttu-id="6b819-123">L’exemple suivant d’une opération **DisableApp** demande montre comment un désactiver une application de messagerie.</span><span class="sxs-lookup"><span data-stu-id="6b819-123">The following example of a **DisableApp** operation request shows how to a disable a mail app.</span></span> <span data-ttu-id="6b819-124">Vous trouverez l’identificateur de l’application dans le manifeste d’application qui est retourné dans une réponse de [l’opération GetAppManifests](getappmanifests-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="6b819-124">The app identifier can be found in the app manifest that is returned in a [GetAppManifests operation](getappmanifests-operation.md) response.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
      <t:TimeZoneContext>
         <t:TimeZoneDefinition Id="GMT Standard Time"/>
      </t:TimeZoneContext>
   </soap:Header>
   <soap:Body >
      <m:DisableApp>
         <m:ID>1C50226D-04B5-4AB2-9FCD-42E236B59E4B</m:ID>
         <m:DisableReason>NoReason</m:DisableReason>
      </m:DisableApp>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="6b819-125">La demande SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="6b819-125">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="6b819-126">DisableApp</span><span class="sxs-lookup"><span data-stu-id="6b819-126">DisableApp</span></span>](disableapp.md)
    
- [<span data-ttu-id="6b819-127">ID (chaîne)</span><span class="sxs-lookup"><span data-stu-id="6b819-127">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="6b819-128">DisableReason</span><span class="sxs-lookup"><span data-stu-id="6b819-128">DisableReason</span></span>](disablereason.md)
    
## <a name="successful-disableapp-operation-response"></a><span data-ttu-id="6b819-129">Réponse d’opération DisableApp réussie</span><span class="sxs-lookup"><span data-stu-id="6b819-129">Successful DisableApp operation response</span></span>

<span data-ttu-id="6b819-130">L’exemple suivant montre une réponse positive à une demande d’opération **DisableApp** pour désactiver une application de messagerie.</span><span class="sxs-lookup"><span data-stu-id="6b819-130">The following example shows a successful response to a **DisableApp** operation request to disable a mail app.</span></span> 
  
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
      <DisableAppResponse ResponseClass="Success" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </DisableAppResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="6b819-131">La réponse SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="6b819-131">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="6b819-132">DisableAppResponse</span><span class="sxs-lookup"><span data-stu-id="6b819-132">DisableAppResponse</span></span>](disableappresponse.md)
    
- [<span data-ttu-id="6b819-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="6b819-133">ResponseCode</span></span>](responsecode.md)
    
## <a name="disableapp-operation-error-response"></a><span data-ttu-id="6b819-134">Réponse d’erreur d’opération DisableApp</span><span class="sxs-lookup"><span data-stu-id="6b819-134">DisableApp operation error response</span></span>

<span data-ttu-id="6b819-135">L’exemple suivant montre une réponse d’erreur à une demande d’opération **DisableApp** .</span><span class="sxs-lookup"><span data-stu-id="6b819-135">The following example shows an error response to a **DisableApp** operation request.</span></span> <span data-ttu-id="6b819-136">Il s’agit d’une réponse à une demande pour désactiver une application de messagerie qui n’est pas installée dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="6b819-136">This is a response to a request to disable a mail app that is not installed in a mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="556" MinorBuildNumber="14" Version="Exchange2013" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <DisableAppResponse ResponseClass="Error" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Extension ID 1C50226D-04B5-4AB2-9FCD-42E236B59E4A can't be found.</MessageText>
         <ResponseCode>ErrorExtensionNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </DisableAppResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="6b819-137">La réponse d’erreur corps SOAP contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="6b819-137">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="6b819-138">DisableAppResponse</span><span class="sxs-lookup"><span data-stu-id="6b819-138">DisableAppResponse</span></span>](disableappresponse.md)
    
- [<span data-ttu-id="6b819-139">MessageText</span><span class="sxs-lookup"><span data-stu-id="6b819-139">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="6b819-140">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="6b819-140">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="6b819-141">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="6b819-141">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="6b819-142">Pour les codes d’erreur générique à EWS, spécifiques à cette opération, consultez la rubrique [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="6b819-142">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="6b819-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6b819-143">See also</span></span>

- [<span data-ttu-id="6b819-144">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6b819-144">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)   
- [<span data-ttu-id="6b819-145">Opération InstallApp</span><span class="sxs-lookup"><span data-stu-id="6b819-145">InstallApp operation</span></span>](installapp-operation.md)   
- [<span data-ttu-id="6b819-146">Opération UninstallApp</span><span class="sxs-lookup"><span data-stu-id="6b819-146">UninstallApp operation</span></span>](uninstallapp-operation.md)   
- [<span data-ttu-id="6b819-147">GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="6b819-147">GetAppManifests</span></span>](getappmanifests.md)   
- [<span data-ttu-id="6b819-148">Opération GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="6b819-148">GetAppMarketplaceUrl operation</span></span>](getappmarketplaceurl-operation.md)   
- [<span data-ttu-id="6b819-149">Compléments Outlook</span><span class="sxs-lookup"><span data-stu-id="6b819-149">Outlook add-ins</span></span>](http://msdn.microsoft.com/library/71e64bc9-e347-4f5d-8948-0a47b5dd93e6%28Office.15%29.aspx)
    
