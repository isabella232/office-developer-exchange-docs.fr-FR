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
description: L’opération RefreshSharingFolder actualise le dossier local spécifié avec les données les plus récentes à partir du dossier partagé.
ms.openlocfilehash: 0037de28f0720b97cd51c58a6ee7e3c06e84d642
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829041"
---
# <a name="refreshsharingfolder-operation"></a><span data-ttu-id="ea4ed-103">Opération RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="ea4ed-103">RefreshSharingFolder operation</span></span>

<span data-ttu-id="ea4ed-104">L’opération **RefreshSharingFolder** actualise le dossier local spécifié avec les données les plus récentes à partir du dossier partagé.</span><span class="sxs-lookup"><span data-stu-id="ea4ed-104">The **RefreshSharingFolder** operation refreshes the specified local folder with the latest data from the folder that is being shared.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="ea4ed-105">En-têtes SOAP</span><span class="sxs-lookup"><span data-stu-id="ea4ed-105">SOAP Headers</span></span>

<span data-ttu-id="ea4ed-106">L’opération **RefreshSharingFolder** permettre utiliser les en-têtes SOAP qui sont répertoriés et décrits dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="ea4ed-106">The **RefreshSharingFolder** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="ea4ed-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="ea4ed-107">**Header**</span></span>|<span data-ttu-id="ea4ed-108">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ea4ed-108">**Element**</span></span>|<span data-ttu-id="ea4ed-109">**Description**</span><span class="sxs-lookup"><span data-stu-id="ea4ed-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ea4ed-110">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="ea4ed-110">RequestVersion</span></span>  <br/> |[<span data-ttu-id="ea4ed-111">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="ea4ed-111">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="ea4ed-112">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="ea4ed-112">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="ea4ed-113">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="ea4ed-113">ServerVersion</span></span>  <br/> |[<span data-ttu-id="ea4ed-114">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ea4ed-114">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="ea4ed-115">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="ea4ed-115">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="refreshsharingfolder-request-example"></a><span data-ttu-id="ea4ed-116">Exemple de requête RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="ea4ed-116">RefreshSharingFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="ea4ed-117">Description</span><span class="sxs-lookup"><span data-stu-id="ea4ed-117">Description</span></span>

<span data-ttu-id="ea4ed-118">L’exemple suivant montre comment former une demande pour actualiser le dossier local spécifié avec les données les plus récentes à partir du dossier partagé.</span><span class="sxs-lookup"><span data-stu-id="ea4ed-118">The following example shows how to form a request to refresh the specified local folder with the latest data from the folder that is being shared.</span></span> <span data-ttu-id="ea4ed-119">L’élément [SharingFolderId](sharingfolderid.md) Spécifie l’identificateur du dossier local à être actualisés.</span><span class="sxs-lookup"><span data-stu-id="ea4ed-119">The [SharingFolderId](sharingfolderid.md) element specifies the identifier of the local folder to be refreshed.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ea4ed-120">Code</span><span class="sxs-lookup"><span data-stu-id="ea4ed-120">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <RefreshSharingFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:SharingFolderId Id="AAMkAD=" ChangeKey="AwAAA=" />
    </RefreshSharingFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="ea4ed-121">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="ea4ed-121">Request elements</span></span>

<span data-ttu-id="ea4ed-122">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="ea4ed-122">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="ea4ed-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="ea4ed-123">RequestServerVersion</span></span>](requestserverversion.md)
    
- [<span data-ttu-id="ea4ed-124">RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="ea4ed-124">RefreshSharingFolder</span></span>](refreshsharingfolder.md)
    
- [<span data-ttu-id="ea4ed-125">SharingFolderId</span><span class="sxs-lookup"><span data-stu-id="ea4ed-125">SharingFolderId</span></span>](sharingfolderid.md)
    
## <a name="successful-refreshsharingfolder-response"></a><span data-ttu-id="ea4ed-126">Réponse RefreshSharingFolder réussie</span><span class="sxs-lookup"><span data-stu-id="ea4ed-126">Successful RefreshSharingFolder Response</span></span>

### <a name="description"></a><span data-ttu-id="ea4ed-127">Description</span><span class="sxs-lookup"><span data-stu-id="ea4ed-127">Description</span></span>

<span data-ttu-id="ea4ed-128">L’exemple suivant montre une réponse positive à une demande de **RefreshSharingFolder** .</span><span class="sxs-lookup"><span data-stu-id="ea4ed-128">The following example shows a successful response to a **RefreshSharingFolder** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ea4ed-129">Code</span><span class="sxs-lookup"><span data-stu-id="ea4ed-129">Code</span></span>

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
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <RefreshSharingFolderResponseMessage ResponseClass="Success"
                                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
    </RefreshSharingFolderResponseMessage>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="ea4ed-130">Éléments de réponse réussie</span><span class="sxs-lookup"><span data-stu-id="ea4ed-130">Successful response elements</span></span>

<span data-ttu-id="ea4ed-131">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="ea4ed-131">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="ea4ed-132">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ea4ed-132">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="ea4ed-133">RefreshSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ea4ed-133">RefreshSharingFolderResponseMessage</span></span>](refreshsharingfolderresponsemessage.md)
    
- [<span data-ttu-id="ea4ed-134">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ea4ed-134">ResponseCode</span></span>](responsecode.md)
    
## <a name="refreshsharingfolder-error-response"></a><span data-ttu-id="ea4ed-135">Réponse d’erreur RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="ea4ed-135">RefreshSharingFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="ea4ed-136">Description</span><span class="sxs-lookup"><span data-stu-id="ea4ed-136">Description</span></span>

<span data-ttu-id="ea4ed-137">L’exemple suivant montre une réponse d’erreur à une demande de **RefreshSharingFolder** .</span><span class="sxs-lookup"><span data-stu-id="ea4ed-137">The following example shows an error response to a **RefreshSharingFolder** request.</span></span> <span data-ttu-id="ea4ed-138">Dans cet exemple, la demande de **RefreshSharingFolder** a échoué, car un abonnement correspondant dans le dossier local spécifié est introuvable.</span><span class="sxs-lookup"><span data-stu-id="ea4ed-138">In this example, the **RefreshSharingFolder** request failed because a subscription that corresponds to the specified local folder was not found.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ea4ed-139">Code</span><span class="sxs-lookup"><span data-stu-id="ea4ed-139">Code</span></span>

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
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <RefreshSharingFolderResponseMessage ResponseClass="Error"
                                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="ea4ed-140">Éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="ea4ed-140">Error response elements</span></span>

<span data-ttu-id="ea4ed-141">Les éléments suivants sont utilisés dans la réponse d'erreur :</span><span class="sxs-lookup"><span data-stu-id="ea4ed-141">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="ea4ed-142">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ea4ed-142">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="ea4ed-143">RefreshSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ea4ed-143">RefreshSharingFolderResponseMessage</span></span>](refreshsharingfolderresponsemessage.md)
    
- [<span data-ttu-id="ea4ed-144">MessageText</span><span class="sxs-lookup"><span data-stu-id="ea4ed-144">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="ea4ed-145">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ea4ed-145">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ea4ed-146">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="ea4ed-146">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="ea4ed-147">MessageXml</span><span class="sxs-lookup"><span data-stu-id="ea4ed-147">MessageXml</span></span>](messagexml.md)
    
## <a name="see-also"></a><span data-ttu-id="ea4ed-148">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ea4ed-148">See also</span></span>



[<span data-ttu-id="ea4ed-149">RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="ea4ed-149">RefreshSharingFolder</span></span>](refreshsharingfolder.md)
  
[<span data-ttu-id="ea4ed-150">RefreshSharingFolderType</span><span class="sxs-lookup"><span data-stu-id="ea4ed-150">RefreshSharingFolderType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.RefreshSharingFolderType.aspx)
  
[<span data-ttu-id="ea4ed-151">RefreshSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ea4ed-151">RefreshSharingFolderResponseMessage</span></span>](refreshsharingfolderresponsemessage.md)
  
[<span data-ttu-id="ea4ed-152">RefreshSharingFolderResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="ea4ed-152">RefreshSharingFolderResponseMessageType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.RefreshSharingFolderResponseMessageType.aspx)


[<span data-ttu-id="ea4ed-153">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ea4ed-153">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="ea4ed-154">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ea4ed-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

