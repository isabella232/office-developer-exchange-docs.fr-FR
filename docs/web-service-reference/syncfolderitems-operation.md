---
title: Opération SyncFolderItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderItems
api_type:
- schema
ms.assetid: 7f0de089-8876-47ec-a871-df118ceae75d
description: L’opération SyncFolderItems synchronise les éléments entre le serveur Exchange et le client.
ms.openlocfilehash: 1a28d895eda11dd43f77ec2662a60a426cfc463c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468144"
---
# <a name="syncfolderitems-operation"></a><span data-ttu-id="9a915-103">Opération SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="9a915-103">SyncFolderItems operation</span></span>

<span data-ttu-id="9a915-104">L’opération SyncFolderItems synchronise les éléments entre le serveur Exchange et le client.</span><span class="sxs-lookup"><span data-stu-id="9a915-104">The SyncFolderItems operation synchronizes items between the Exchange server and the client.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9a915-105">Remarques</span><span class="sxs-lookup"><span data-stu-id="9a915-105">Remarks</span></span>

<span data-ttu-id="9a915-106">L’opération SyncFolderItems renvoie un maximum de 512 modifications.</span><span class="sxs-lookup"><span data-stu-id="9a915-106">The SyncFolderItems operation will return a maximum of 512 changes.</span></span> <span data-ttu-id="9a915-107">Des demandes SyncFolderItems suivantes doivent être effectuées pour obtenir des modifications supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="9a915-107">Subsequent SyncFolderItems requests must be performed to get additional changes.</span></span> 
  
<span data-ttu-id="9a915-108">SyncFolderItems est similaire à l’opération FindItem, car elle ne peut pas renvoyer de propriétés comme Body ou Attachments.</span><span class="sxs-lookup"><span data-stu-id="9a915-108">SyncFolderItems is similar to the FindItem operation in that it cannot return properties like Body or Attachments.</span></span> <span data-ttu-id="9a915-109">Si l’opération SyncFolderItems ne retourne pas les propriétés dont vous avez besoin, vous pouvez utiliser l' [opération GetItem](getitem-operation.md) pour obtenir un ensemble spécifique de propriétés pour chaque élément renvoyé par SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="9a915-109">If the SyncFolderItems operation does not return the properties that you need, you can use the [GetItem operation](getitem-operation.md) to get a specific set of properties for each item that it returned by SyncFolderItems.</span></span> 
  
## <a name="syncfolderitems-request-example"></a><span data-ttu-id="9a915-110">Exemple de requête SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="9a915-110">SyncFolderItems request example</span></span>

### <a name="description"></a><span data-ttu-id="9a915-111">Description</span><span class="sxs-lookup"><span data-stu-id="9a915-111">Description</span></span>

<span data-ttu-id="9a915-112">L’exemple de requête SyncFolderItems suivant montre comment synchroniser des éléments dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="9a915-112">The following example of a SyncFolderItems request shows how to synchronize items in a folder.</span></span> <span data-ttu-id="9a915-113">Cet exemple illustre la synchronisation d’un élément de dossier qui n’est pas la première synchronisation effectuée pour le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="9a915-113">This example shows a folder item's synchronization that is not the first synchronization to have occurred for the Sent Items folder.</span></span> <span data-ttu-id="9a915-114">L’élément [SyncState](syncstate-ex15websvcsotherref.md) n’est pas inclus dans la demande de la première tentative de synchronisation d’un client avec le serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="9a915-114">The [SyncState](syncstate-ex15websvcsotherref.md) element is not included in the request for the first attempt to synchronize a client with the Exchange server.</span></span> <span data-ttu-id="9a915-115">La première tentative de synchronisation des éléments dans une hiérarchie de dossiers renverra tous les éléments de la boîte aux lettres, à l’exclusion des éléments identifiés dans l’élément [ignore](ignore.md) .</span><span class="sxs-lookup"><span data-stu-id="9a915-115">The first attempt to synchronize the items in a folder hierarchy will return all the items in the mailbox, excluding items that are identified in the [Ignore](ignore.md) element.</span></span> <span data-ttu-id="9a915-116">Cette requête SyncFolderItems essaiera de synchroniser toutes les modifications apportées aux éléments de dossier depuis la dernière synchronisation.</span><span class="sxs-lookup"><span data-stu-id="9a915-116">This SyncFolderItems request will try to synchronize all changes to the folder items since the last synchronization.</span></span> <span data-ttu-id="9a915-117">Cette demande ignorera la tentative de synchronisation de l’élément identifié dans l’élément [ignore](ignore.md) .</span><span class="sxs-lookup"><span data-stu-id="9a915-117">This request will ignore the attempt to synchronize the one item that is identified in the [Ignore](ignore.md) element.</span></span> 
  
### <a name="code"></a><span data-ttu-id="9a915-118">Code</span><span class="sxs-lookup"><span data-stu-id="9a915-118">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SyncFolderItems xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemShape>
        <t:BaseShape>Default</t:BaseShape>
      </ItemShape>
      <SyncFolderId>
        <t:DistinguishedFolderId Id="sentitems"/>
      </SyncFolderId>
      <SyncState>AEbJ94eMOAAA=</SyncState>
      <Ignore>
        <t:ItemId Id="AQApAHRAA==" ChangeKey="CQAAABY"/>
      </Ignore>
      <MaxChangesReturned>100</MaxChangesReturned>
    </SyncFolderItems>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="9a915-119">Commentaires</span><span class="sxs-lookup"><span data-stu-id="9a915-119">Comments</span></span>

<span data-ttu-id="9a915-120">L’élément [SyncState](syncstate-ex15websvcsotherref.md) les données codées en base64 et l’attribut d' **ID** d’élément [ItemId](itemid.md) ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="9a915-120">The [SyncState](syncstate-ex15websvcsotherref.md) element base64-encoded data and the [ItemId](itemid.md) element **Id** attribute have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="9a915-121">Demander des éléments</span><span class="sxs-lookup"><span data-stu-id="9a915-121">Request elements</span></span>

<span data-ttu-id="9a915-122">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="9a915-122">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="9a915-123">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="9a915-123">SyncFolderItems</span></span>](syncfolderitems.md)
    
- [<span data-ttu-id="9a915-124">ItemShape</span><span class="sxs-lookup"><span data-stu-id="9a915-124">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="9a915-125">BaseShape</span><span class="sxs-lookup"><span data-stu-id="9a915-125">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="9a915-126">SyncFolderId</span><span class="sxs-lookup"><span data-stu-id="9a915-126">SyncFolderId</span></span>](syncfolderid.md)
    
- [<span data-ttu-id="9a915-127">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="9a915-127">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="9a915-128">SyncState</span><span class="sxs-lookup"><span data-stu-id="9a915-128">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
- [<span data-ttu-id="9a915-129">Ignore</span><span class="sxs-lookup"><span data-stu-id="9a915-129">Ignore</span></span>](ignore.md)
    
- [<span data-ttu-id="9a915-130">ItemId</span><span class="sxs-lookup"><span data-stu-id="9a915-130">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="9a915-131">MaxChangesReturned</span><span class="sxs-lookup"><span data-stu-id="9a915-131">MaxChangesReturned</span></span>](maxchangesreturned.md)
    
## <a name="successful-syncfolderitems-response"></a><span data-ttu-id="9a915-132">Réponse SyncFolderItems réussie</span><span class="sxs-lookup"><span data-stu-id="9a915-132">Successful SyncFolderItems Response</span></span>

### <a name="description"></a><span data-ttu-id="9a915-133">Description</span><span class="sxs-lookup"><span data-stu-id="9a915-133">Description</span></span>

<span data-ttu-id="9a915-134">L’exemple suivant montre une réponse réussie à la demande SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="9a915-134">The following example shows a successful response to the SyncFolderItems request.</span></span> <span data-ttu-id="9a915-135">Dans cet exemple, une demande de réunion est synchronisée à partir du dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="9a915-135">In this example, a meeting request is synchronized from the Sent Items folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="9a915-136">Code</span><span class="sxs-lookup"><span data-stu-id="9a915-136">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SyncFolderItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SyncFolderItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAAAAA=</m:SyncState>
          <m:IncludesLastItemInRange>true</m:IncludesLastItemInRange>
          <m:Changes>
            <t:Create>
              <t:MeetingRequest>
                <t:ItemId Id="AQApAHRwA==" ChangeKey="CwAAABYA" />
                <t:Subject>Budget Q3</t:Subject>
                <t:Sensitivity>Normal</t:Sensitivity>
                <t:IsOutOfDate>false</t:IsOutOfDate>
                <t:HasBeenProcessed>true</t:HasBeenProcessed>
                <t:ResponseType>NoResponseReceived</t:ResponseType>
                <t:IntendedFreeBusyStatus>Busy</t:IntendedFreeBusyStatus>
                <t:Start>2006-08-02T17:30:00Z</t:Start>
                <t:End>2006-08-02T19:30:00Z</t:End>
                <t:Location>Conference Room 2</t:Location>
                <t:Organizer>
                  <t:Mailbox>
                    <t:Name>Dan Park</t:Name>
                    <t:EmailAddress>dpark@example.com</t:EmailAddress>
                    <t:RoutingType>SMTP</t:RoutingType>
                  </t:Mailbox>
                </t:Organizer>
              </t:MeetingRequest>
            </t:Create>
          </m:Changes>
        </m:SyncFolderItemsResponseMessage>
      </m:ResponseMessages>
    </SyncFolderItemsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="9a915-137">Commentaires</span><span class="sxs-lookup"><span data-stu-id="9a915-137">Comments</span></span>

<span data-ttu-id="9a915-138">L’élément [SyncState](syncstate-ex15websvcsotherref.md) les données codées en base64 et l’attribut d' **ID** d’élément [ItemId](itemid.md) ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="9a915-138">The [SyncState](syncstate-ex15websvcsotherref.md) element base64-encoded data and the [ItemId](itemid.md) element **Id** attribute have been shortened to preserve readability.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="9a915-139">Éléments de réponse réussis</span><span class="sxs-lookup"><span data-stu-id="9a915-139">Successful response elements</span></span>

<span data-ttu-id="9a915-140">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="9a915-140">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="9a915-141">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="9a915-141">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="9a915-142">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="9a915-142">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md)
    
- [<span data-ttu-id="9a915-143">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="9a915-143">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="9a915-144">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9a915-144">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)
    
- [<span data-ttu-id="9a915-145">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="9a915-145">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="9a915-146">SyncState</span><span class="sxs-lookup"><span data-stu-id="9a915-146">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
- [<span data-ttu-id="9a915-147">IncludesLastItemInRange</span><span class="sxs-lookup"><span data-stu-id="9a915-147">IncludesLastItemInRange</span></span>](includeslastiteminrange.md)
    
- [<span data-ttu-id="9a915-148">Changes (éléments)</span><span class="sxs-lookup"><span data-stu-id="9a915-148">Changes (Items)</span></span>](changes-items.md)
    
- [<span data-ttu-id="9a915-149">Créer (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="9a915-149">Create (ItemSync)</span></span>](create-itemsync.md)
    
- [<span data-ttu-id="9a915-150">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="9a915-150">MeetingRequest</span></span>](meetingrequest.md)
    
- [<span data-ttu-id="9a915-151">ItemId</span><span class="sxs-lookup"><span data-stu-id="9a915-151">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="9a915-152">Subject</span><span class="sxs-lookup"><span data-stu-id="9a915-152">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="9a915-153">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="9a915-153">Sensitivity</span></span>](sensitivity.md)
    
- [<span data-ttu-id="9a915-154">IsOutOfDate</span><span class="sxs-lookup"><span data-stu-id="9a915-154">IsOutOfDate</span></span>](isoutofdate.md)
    
- [<span data-ttu-id="9a915-155">HasBeenProcessed</span><span class="sxs-lookup"><span data-stu-id="9a915-155">HasBeenProcessed</span></span>](hasbeenprocessed.md)
    
- [<span data-ttu-id="9a915-156">ResponseType</span><span class="sxs-lookup"><span data-stu-id="9a915-156">ResponseType</span></span>](responsetype.md)
    
- [<span data-ttu-id="9a915-157">IntendedFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="9a915-157">IntendedFreeBusyStatus</span></span>](intendedfreebusystatus.md)
    
- [<span data-ttu-id="9a915-158">Démarrage</span><span class="sxs-lookup"><span data-stu-id="9a915-158">Start</span></span>](start.md)
    
- [<span data-ttu-id="9a915-159">Fin</span><span class="sxs-lookup"><span data-stu-id="9a915-159">End </span></span>](end-ex15websvcsotherref.md)
    
- [<span data-ttu-id="9a915-160">Emplacement</span><span class="sxs-lookup"><span data-stu-id="9a915-160">Location</span></span>](location.md)
    
- [<span data-ttu-id="9a915-161">Organizer</span><span class="sxs-lookup"><span data-stu-id="9a915-161">Organizer</span></span>](organizer.md)
    
- [<span data-ttu-id="9a915-162">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="9a915-162">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="9a915-163">Nom (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="9a915-163">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="9a915-164">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="9a915-164">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="9a915-165">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="9a915-165">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
## <a name="syncfolderitems-error-response"></a><span data-ttu-id="9a915-166">Réponse d’erreur SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="9a915-166">SyncFolderItems error response</span></span>

### <a name="description"></a><span data-ttu-id="9a915-167">Description</span><span class="sxs-lookup"><span data-stu-id="9a915-167">Description</span></span>

<span data-ttu-id="9a915-168">L’exemple suivant montre une réponse d’erreur à une requête SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="9a915-168">The following example shows an error response to a SyncFolderItems request.</span></span> <span data-ttu-id="9a915-169">Cette erreur a été causée par un SyncState non valide.</span><span class="sxs-lookup"><span data-stu-id="9a915-169">This error was caused by an invalid SyncState.</span></span>
  
### <a name="code"></a><span data-ttu-id="9a915-170">Code</span><span class="sxs-lookup"><span data-stu-id="9a915-170">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SyncFolderItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SyncFolderItemsResponseMessage ResponseClass="Error">
          <m:MessageText>Synchronization state data is corrupt or otherwise invalid.</m:MessageText>
          <m:ResponseCode>ErrorInvalidSyncStateData</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:SyncState />
          <m:IncludesLastItemInRange>true</m:IncludesLastItemInRange>
        </m:SyncFolderItemsResponseMessage>
      </m:ResponseMessages>
    </SyncFolderItemsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="9a915-171">Éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="9a915-171">Error response elements</span></span>

<span data-ttu-id="9a915-172">Les éléments suivants sont utilisés dans la réponse d'erreur :</span><span class="sxs-lookup"><span data-stu-id="9a915-172">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="9a915-173">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="9a915-173">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="9a915-174">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="9a915-174">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md)
    
- [<span data-ttu-id="9a915-175">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="9a915-175">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="9a915-176">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9a915-176">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)
    
- [<span data-ttu-id="9a915-177">MessageText</span><span class="sxs-lookup"><span data-stu-id="9a915-177">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="9a915-178">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="9a915-178">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="9a915-179">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="9a915-179">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="9a915-180">SyncState</span><span class="sxs-lookup"><span data-stu-id="9a915-180">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
- [<span data-ttu-id="9a915-181">IncludesLastItemInRange</span><span class="sxs-lookup"><span data-stu-id="9a915-181">IncludesLastItemInRange</span></span>](includeslastiteminrange.md)
    
## <a name="see-also"></a><span data-ttu-id="9a915-182">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9a915-182">See also</span></span>



- [<span data-ttu-id="9a915-183">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9a915-183">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

