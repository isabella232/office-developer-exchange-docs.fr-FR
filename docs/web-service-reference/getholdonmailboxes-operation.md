---
title: Opération GetHoldOnMailboxes
manager: sethgros
ms.date: 01/24/2020
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9157f329-80b4-4cd0-a158-378064966ae6
description: Trouvez des informations sur l’opération EWS GetHoldOnMailboxes.
ms.openlocfilehash: 867f38be87e60af8708eeb0b9d0e3ac8eee6ff64
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457731"
---
# <a name="getholdonmailboxes-operation"></a><span data-ttu-id="21785-103">Opération GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="21785-103">GetHoldOnMailboxes operation</span></span>

> [!IMPORTANT]
> <span data-ttu-id="21785-104">À partir du 1er avril 2020, l’opération GetHoldOnMailboxes ne sera plus disponible dans Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="21785-104">Starting on April 1, 2020, the GetHoldOnMailboxes operation will no longer be available in Exchange Online.</span></span> <span data-ttu-id="21785-105">Cette opération ne sera pas affectée dans les versions locales d’Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="21785-105">This operation won't be affected in on-premises versions of Exchange Server.</span></span> <span data-ttu-id="21785-106">Pour plus d’informations, reportez-vous à la section [retraite des outils eDiscovery hérités dans Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#getsearchablemailboxes-setholdonmailboxes-and-getholdonmailboxes-operations-in-the-ews-api).</span><span class="sxs-lookup"><span data-stu-id="21785-106">For more information, see [Retirement of legacy eDiscovery tools in Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#getsearchablemailboxes-setholdonmailboxes-and-getholdonmailboxes-operations-in-the-ews-api).</span></span>

<span data-ttu-id="21785-107">Trouvez des informations sur l’opération EWS **GetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="21785-107">Find information about the **GetHoldOnMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="21785-108">L’opération **GetHoldOnMailboxes** obtient les boîtes aux lettres qui sont sous une conservation spécifique et la requête de suspension associée.</span><span class="sxs-lookup"><span data-stu-id="21785-108">The **GetHoldOnMailboxes** operation gets the mailboxes that are under a specific hold and the associated hold query.</span></span> 
  
<span data-ttu-id="21785-109">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="21785-109">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getholdonmailboxes-operation"></a><span data-ttu-id="21785-110">Utilisation de l’opération GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="21785-110">Using the GetHoldOnMailboxes operation</span></span>

<span data-ttu-id="21785-111">L’opération **GetHoldOnMailboxes** fournit au client des informations sur les boîtes aux lettres placées sous une conservation spécifique, des informations sur la requête de suspension associées à chaque conservation, le cas échéant, et des informations sur l’état de la suspension pour chaque boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="21785-111">The **GetHoldOnMailboxes** operation gives the client information about which mailboxes are placed under a specific hold, information about the hold query associated with each hold, if applicable, and information about the hold status for each mailbox.</span></span> <span data-ttu-id="21785-112">Pour plus d’informations sur les conservations de boîte aux lettres, y compris les conservations basées sur une requête, voir [in-place Hold](https://technet.microsoft.com/library/ff637980%28v=exchg.150%29) on technet.</span><span class="sxs-lookup"><span data-stu-id="21785-112">For more information about mailbox holds, including query-based holds, see [In-Place Hold](https://technet.microsoft.com/library/ff637980%28v=exchg.150%29) on TechNet.</span></span> 
  
### <a name="getholdonmailboxes-operation-soap-headers"></a><span data-ttu-id="21785-113">En-têtes SOAP d’opération GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="21785-113">GetHoldOnMailboxes operation SOAP headers</span></span>

<span data-ttu-id="21785-114">L’opération **GetHoldOnMailboxes** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="21785-114">The **GetHoldOnMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="21785-115">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="21785-115">**Header name**</span></span>|<span data-ttu-id="21785-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="21785-116">**Element**</span></span>|<span data-ttu-id="21785-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="21785-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="21785-118">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="21785-118">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="21785-119">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="21785-119">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="21785-120">Identifie les rôles serveur nécessaires pour que l’appelant effectue la demande.</span><span class="sxs-lookup"><span data-stu-id="21785-120">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="21785-121">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="21785-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="21785-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="21785-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="21785-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="21785-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="21785-124">Identifie la version de schéma de la demande d’opération.</span><span class="sxs-lookup"><span data-stu-id="21785-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="21785-125">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="21785-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="21785-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="21785-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="21785-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="21785-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="21785-128">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="21785-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="21785-129">Cet en-tête s’applique à une réponse.</span><span class="sxs-lookup"><span data-stu-id="21785-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getholdonmailboxes-operation-request-example-get-mailbox-hold-information"></a><span data-ttu-id="21785-130">Exemple de requête d’opération GetHoldOnMailboxes : obtenir des informations de conservation de boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="21785-130">GetHoldOnMailboxes operation request example: Get mailbox hold information</span></span>

<span data-ttu-id="21785-131">L’exemple suivant de demande d’opération **GetHoldOnMailboxes** montre comment obtenir les informations de conservation de boîte aux lettres pour la conservation de boîte aux lettres HoldId2.</span><span class="sxs-lookup"><span data-stu-id="21785-131">The following example of a **GetHoldOnMailboxes** operation request shows how to get the mailbox hold information for the HoldId2 mailbox hold.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetHoldOnMailboxes>
         <m:HoldId>HoldId2</m:HoldId>
      </m:GetHoldOnMailboxes>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="21785-132">Le corps SOAP de la demande contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="21785-132">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="21785-133">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="21785-133">GetHoldOnMailboxes</span></span>](getholdonmailboxes.md)
    
- [<span data-ttu-id="21785-134">HoldId</span><span class="sxs-lookup"><span data-stu-id="21785-134">HoldId</span></span>](holdid.md)
    
## <a name="successful-getholdonmailboxes-operation-response"></a><span data-ttu-id="21785-135">Réponse de l’opération GetHoldOnMailboxes réussie</span><span class="sxs-lookup"><span data-stu-id="21785-135">Successful GetHoldOnMailboxes operation response</span></span>

<span data-ttu-id="21785-136">L’exemple suivant montre une réponse réussie à une demande d’opération **GetHoldOnMailboxes** pour obtenir les informations de conservation de boîte aux lettres pour la conservation de boîte aux lettres HoldId2.</span><span class="sxs-lookup"><span data-stu-id="21785-136">The following example shows a successful response to a **GetHoldOnMailboxes** operation request to get the mailbox hold information for the HoldId2 mailbox hold.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetHoldOnMailboxesResponse ResponseClass="Success" 
                                  xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <MailboxHoldResult>
            <HoldId xmlns="https://schemas.microsoft.com/exchange/services/2006/types">HoldId2</HoldId>
            <Query xmlns="https://schemas.microsoft.com/exchange/services/2006/types">test</Query>
            <MailboxHoldStatuses xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <MailboxHoldStatus>
                  <Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYDIBPDLT)/cn=Recipients/cn=ecc0fd98c2cadf-Willi</Mailbox>
                  <Status>OnHold</Status>
                  <AdditionalInfo/>
               </MailboxHoldStatus>
               <MailboxHoldStatus>
                  <Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYDIBPDLT)/cn=Recipients/cn=dasdat341q8de95-Micha</Mailbox>
                  <Status>OnHold</Status>
                  <AdditionalInfo/>
               </MailboxHoldStatus>
            </MailboxHoldStatuses>
         </MailboxHoldResult>
      </GetHoldOnMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="21785-137">Le corps SOAP de réponse contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="21785-137">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="21785-138">GetHoldOnMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="21785-138">GetHoldOnMailboxesResponse</span></span>](getholdonmailboxesresponse.md)
    
- [<span data-ttu-id="21785-139">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="21785-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="21785-140">MailboxHoldResult</span><span class="sxs-lookup"><span data-stu-id="21785-140">MailboxHoldResult</span></span>](mailboxholdresult.md)
    
- [<span data-ttu-id="21785-141">HoldId</span><span class="sxs-lookup"><span data-stu-id="21785-141">HoldId</span></span>](holdid.md)
    
- [<span data-ttu-id="21785-142">Query</span><span class="sxs-lookup"><span data-stu-id="21785-142">Query</span></span>](query.md)
    
- [<span data-ttu-id="21785-143">MailboxHoldStatuses</span><span class="sxs-lookup"><span data-stu-id="21785-143">MailboxHoldStatuses</span></span>](mailboxholdstatuses.md)
    
- [<span data-ttu-id="21785-144">MailboxHoldStatus</span><span class="sxs-lookup"><span data-stu-id="21785-144">MailboxHoldStatus</span></span>](mailboxholdstatus.md)
    
- [<span data-ttu-id="21785-145">Mailbox (String)</span><span class="sxs-lookup"><span data-stu-id="21785-145">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="21785-146">État (HoldStatusType)</span><span class="sxs-lookup"><span data-stu-id="21785-146">Status (HoldStatusType)</span></span>](status-holdstatustype.md)
    
- [<span data-ttu-id="21785-147">AdditionalInfo</span><span class="sxs-lookup"><span data-stu-id="21785-147">AdditionalInfo</span></span>](additionalinfo.md)
    
## <a name="getholdonmailboxes-operation-error-response"></a><span data-ttu-id="21785-148">Réponse d’erreur d’opération GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="21785-148">GetHoldOnMailboxes operation error response</span></span>

<span data-ttu-id="21785-149">L’exemple suivant montre une réponse d’erreur à une demande d’opération **GetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="21785-149">The following example shows an error response to a **GetHoldOnMailboxes** operation request.</span></span> <span data-ttu-id="21785-150">Il s’agit d’une réponse à une demande d’obtention d’une conservation qui a été supprimée.</span><span class="sxs-lookup"><span data-stu-id="21785-150">This is a response to a request to get a hold that has been deleted.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetHoldOnMailboxesResponse ResponseClass="Error" 
                                  xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specific query-based hold is not found.</MessageText>
         <ResponseCode>ErrorMailboxHoldNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetHoldOnMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="21785-151">Le corps SOAP de la réponse d’erreur contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="21785-151">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="21785-152">GetHoldOnMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="21785-152">GetHoldOnMailboxesResponse</span></span>](getholdonmailboxesresponse.md)
    
- [<span data-ttu-id="21785-153">MessageText</span><span class="sxs-lookup"><span data-stu-id="21785-153">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="21785-154">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="21785-154">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="21785-155">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="21785-155">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="21785-156">Pour les autres codes d’erreur qui sont génériques à EWS et spécifiques à cette opération, voir [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="21785-156">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="21785-157">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="21785-157">See also</span></span>

- [<span data-ttu-id="21785-158">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="21785-158">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="21785-159">Opération GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="21785-159">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="21785-160">Opération SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="21785-160">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)
    
- [<span data-ttu-id="21785-161">Opération SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="21785-161">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)
    
- [<span data-ttu-id="21785-162">Opération GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="21785-162">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="21785-163">Opération GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="21785-163">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    
- [<span data-ttu-id="21785-164">Opération GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="21785-164">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

