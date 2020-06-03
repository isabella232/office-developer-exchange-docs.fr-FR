---
title: Opération RefreshSharingFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RefreshSharingFolder
api_type:
- schema
ms.assetid: 1b047e34-40f0-459f-ac9e-e9f8e7349479
description: L’opération RefreshSharingFolder actualise le dossier local spécifié avec les données les plus récentes du dossier partagé.
ms.openlocfilehash: dd7136ae82353841db09497d23eabe450c1c8b13
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456744"
---
# <a name="refreshsharingfolder-operation"></a><span data-ttu-id="e1039-103">Opération RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="e1039-103">RefreshSharingFolder operation</span></span>

<span data-ttu-id="e1039-104">L’opération **RefreshSharingFolder** actualise le dossier local spécifié avec les données les plus récentes du dossier partagé.</span><span class="sxs-lookup"><span data-stu-id="e1039-104">The **RefreshSharingFolder** operation refreshes the specified local folder with the latest data from the folder that is being shared.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="e1039-105">En-têtes SOAP</span><span class="sxs-lookup"><span data-stu-id="e1039-105">SOAP Headers</span></span>

<span data-ttu-id="e1039-106">L’opération **RefreshSharingFolder** peut utiliser les en-têtes SOAP répertoriés et décrits dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="e1039-106">The **RefreshSharingFolder** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="e1039-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="e1039-107">**Header**</span></span>|<span data-ttu-id="e1039-108">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e1039-108">**Element**</span></span>|<span data-ttu-id="e1039-109">**Description**</span><span class="sxs-lookup"><span data-stu-id="e1039-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="e1039-110">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="e1039-110">RequestVersion</span></span>  <br/> |[<span data-ttu-id="e1039-111">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="e1039-111">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="e1039-112">Identifie la version de schéma de la demande d’opération.</span><span class="sxs-lookup"><span data-stu-id="e1039-112">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="e1039-113">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="e1039-113">ServerVersion</span></span>  <br/> |[<span data-ttu-id="e1039-114">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="e1039-114">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="e1039-115">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="e1039-115">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="refreshsharingfolder-request-example"></a><span data-ttu-id="e1039-116">Exemple de requête RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="e1039-116">RefreshSharingFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="e1039-117">Description</span><span class="sxs-lookup"><span data-stu-id="e1039-117">Description</span></span>

<span data-ttu-id="e1039-118">L’exemple suivant montre comment créer une demande pour actualiser le dossier local spécifié avec les données les plus récentes du dossier partagé.</span><span class="sxs-lookup"><span data-stu-id="e1039-118">The following example shows how to form a request to refresh the specified local folder with the latest data from the folder that is being shared.</span></span> <span data-ttu-id="e1039-119">L’élément [SharingFolderId](sharingfolderid.md) spécifie l’identificateur du dossier local à actualiser.</span><span class="sxs-lookup"><span data-stu-id="e1039-119">The [SharingFolderId](sharingfolderid.md) element specifies the identifier of the local folder to be refreshed.</span></span> 
  
### <a name="code"></a><span data-ttu-id="e1039-120">Code</span><span class="sxs-lookup"><span data-stu-id="e1039-120">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <RefreshSharingFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:SharingFolderId Id="AAMkAD=" ChangeKey="AwAAA=" />
    </RefreshSharingFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="e1039-121">Demander des éléments</span><span class="sxs-lookup"><span data-stu-id="e1039-121">Request elements</span></span>

<span data-ttu-id="e1039-122">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="e1039-122">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="e1039-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="e1039-123">RequestServerVersion</span></span>](requestserverversion.md)
    
- [<span data-ttu-id="e1039-124">RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="e1039-124">RefreshSharingFolder</span></span>](refreshsharingfolder.md)
    
- [<span data-ttu-id="e1039-125">SharingFolderId</span><span class="sxs-lookup"><span data-stu-id="e1039-125">SharingFolderId</span></span>](sharingfolderid.md)
    
## <a name="successful-refreshsharingfolder-response"></a><span data-ttu-id="e1039-126">Réponse RefreshSharingFolder réussie</span><span class="sxs-lookup"><span data-stu-id="e1039-126">Successful RefreshSharingFolder Response</span></span>

### <a name="description"></a><span data-ttu-id="e1039-127">Description</span><span class="sxs-lookup"><span data-stu-id="e1039-127">Description</span></span>

<span data-ttu-id="e1039-128">L’exemple suivant montre une réponse réussie à une demande **RefreshSharingFolder** .</span><span class="sxs-lookup"><span data-stu-id="e1039-128">The following example shows a successful response to a **RefreshSharingFolder** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="e1039-129">Code</span><span class="sxs-lookup"><span data-stu-id="e1039-129">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <RefreshSharingFolderResponseMessage ResponseClass="Success"
                                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
    </RefreshSharingFolderResponseMessage>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="e1039-130">Éléments de réponse réussis</span><span class="sxs-lookup"><span data-stu-id="e1039-130">Successful response elements</span></span>

<span data-ttu-id="e1039-131">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="e1039-131">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="e1039-132">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="e1039-132">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="e1039-133">RefreshSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e1039-133">RefreshSharingFolderResponseMessage</span></span>](refreshsharingfolderresponsemessage.md)
    
- [<span data-ttu-id="e1039-134">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e1039-134">ResponseCode</span></span>](responsecode.md)
    
## <a name="refreshsharingfolder-error-response"></a><span data-ttu-id="e1039-135">Réponse d’erreur RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="e1039-135">RefreshSharingFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="e1039-136">Description</span><span class="sxs-lookup"><span data-stu-id="e1039-136">Description</span></span>

<span data-ttu-id="e1039-137">L’exemple suivant montre une réponse d’erreur à une requête **RefreshSharingFolder** .</span><span class="sxs-lookup"><span data-stu-id="e1039-137">The following example shows an error response to a **RefreshSharingFolder** request.</span></span> <span data-ttu-id="e1039-138">Dans cet exemple, la demande **RefreshSharingFolder** a échoué car un abonnement correspondant au dossier local spécifié est introuvable.</span><span class="sxs-lookup"><span data-stu-id="e1039-138">In this example, the **RefreshSharingFolder** request failed because a subscription that corresponds to the specified local folder was not found.</span></span> 
  
### <a name="code"></a><span data-ttu-id="e1039-139">Code</span><span class="sxs-lookup"><span data-stu-id="e1039-139">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <RefreshSharingFolderResponseMessage ResponseClass="Error"
                                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:MessageText>Failed to synchronize the sharing folder.</m:MessageText>
      <m:ResponseCode>ErrorSharingSynchronizationFailed</m:ResponseCode>
      <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
      <m:MessageXml>
        <t:Value Name="ErrorDetails">Microsoft.Exchange.InfoWorker.Common.Sharing.SubscriptionNotFoundException: The subscription wasn't found.;</t:Value>
      </m:MessageXml>
    </RefreshSharingFolderResponseMessage>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="e1039-140">Éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="e1039-140">Error response elements</span></span>

<span data-ttu-id="e1039-141">Les éléments suivants sont utilisés dans la réponse d'erreur :</span><span class="sxs-lookup"><span data-stu-id="e1039-141">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="e1039-142">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="e1039-142">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="e1039-143">RefreshSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e1039-143">RefreshSharingFolderResponseMessage</span></span>](refreshsharingfolderresponsemessage.md)
    
- [<span data-ttu-id="e1039-144">MessageText</span><span class="sxs-lookup"><span data-stu-id="e1039-144">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="e1039-145">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e1039-145">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="e1039-146">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="e1039-146">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="e1039-147">MessageXml</span><span class="sxs-lookup"><span data-stu-id="e1039-147">MessageXml</span></span>](messagexml.md)
    
## <a name="see-also"></a><span data-ttu-id="e1039-148">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e1039-148">See also</span></span>



[<span data-ttu-id="e1039-149">RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="e1039-149">RefreshSharingFolder</span></span>](refreshsharingfolder.md)
  
[<span data-ttu-id="e1039-150">RefreshSharingFolderType</span><span class="sxs-lookup"><span data-stu-id="e1039-150">RefreshSharingFolderType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.RefreshSharingFolderType.aspx)
  
[<span data-ttu-id="e1039-151">RefreshSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e1039-151">RefreshSharingFolderResponseMessage</span></span>](refreshsharingfolderresponsemessage.md)
  
[<span data-ttu-id="e1039-152">RefreshSharingFolderResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="e1039-152">RefreshSharingFolderResponseMessageType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.RefreshSharingFolderResponseMessageType.aspx)


[<span data-ttu-id="e1039-153">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e1039-153">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="e1039-154">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e1039-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

