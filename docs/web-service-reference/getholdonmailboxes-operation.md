---
title: Opération GetHoldOnMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9157f329-80b4-4cd0-a158-378064966ae6
description: Opération de recherche plus d’informations sur la GetHoldOnMailboxes EWS.
ms.openlocfilehash: 1d0bc2f9d26e11d8d2710693d67843ad2f339a5d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756632"
---
# <a name="getholdonmailboxes-operation"></a><span data-ttu-id="af772-103">Opération GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="af772-103">GetHoldOnMailboxes operation</span></span>

<span data-ttu-id="af772-104">Trouvez des informations sur l’opération EWS **GetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="af772-104">Find information about the **GetHoldOnMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="af772-105">L’opération **GetHoldOnMailboxes** Obtient les boîtes aux lettres qui sont sous une suspension spécifique et au blocage de requête.</span><span class="sxs-lookup"><span data-stu-id="af772-105">The **GetHoldOnMailboxes** operation gets the mailboxes that are under a specific hold and the associated hold query.</span></span> 
  
<span data-ttu-id="af772-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="af772-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getholdonmailboxes-operation"></a><span data-ttu-id="af772-107">Utilisation de l’opération GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="af772-107">Using the GetHoldOnMailboxes operation</span></span>

<span data-ttu-id="af772-108">L’opération **GetHoldOnMailboxes** donne les informations sur les boîtes aux lettres sont soumis à une suspension spécifique, les informations relatives à la requête de suspension associée à chaque suspension, le cas échéant et plus d’informations sur l’état de conservation pour chaque boîte aux lettres du client.</span><span class="sxs-lookup"><span data-stu-id="af772-108">The **GetHoldOnMailboxes** operation gives the client information about which mailboxes are placed under a specific hold, information about the hold query associated with each hold, if applicable, and information about the hold status for each mailbox.</span></span> <span data-ttu-id="af772-109">Pour plus d’informations sur les suspensions de boîte aux lettres, y compris les suspensions basée sur une requête, voir [In-Place Hold](http://technet.microsoft.com/en-us/library/ff637980%28v=exchg.150%29) sur TechNet.</span><span class="sxs-lookup"><span data-stu-id="af772-109">For more information about mailbox holds, including query-based holds, see [In-Place Hold](http://technet.microsoft.com/en-us/library/ff637980%28v=exchg.150%29) on TechNet.</span></span> 
  
### <a name="getholdonmailboxes-operation-soap-headers"></a><span data-ttu-id="af772-110">En-têtes SOAP GetHoldOnMailboxes opération</span><span class="sxs-lookup"><span data-stu-id="af772-110">GetHoldOnMailboxes operation SOAP headers</span></span>

<span data-ttu-id="af772-111">L’opération **GetHoldOnMailboxes** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="af772-111">The **GetHoldOnMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="af772-112">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="af772-112">**Header name**</span></span>|<span data-ttu-id="af772-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="af772-113">**Element**</span></span>|<span data-ttu-id="af772-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="af772-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="af772-115">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="af772-115">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="af772-116">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="af772-116">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="af772-117">Identifie les rôles de serveur qui sont nécessaires pour l’appelant effectuer la demande.</span><span class="sxs-lookup"><span data-stu-id="af772-117">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="af772-118">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="af772-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="af772-119">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="af772-119">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="af772-120">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="af772-120">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="af772-121">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="af772-121">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="af772-122">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="af772-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="af772-123">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="af772-123">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="af772-124">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="af772-124">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="af772-125">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="af772-125">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="af772-126">Cet en-tête est applicable à une réponse.</span><span class="sxs-lookup"><span data-stu-id="af772-126">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getholdonmailboxes-operation-request-example-get-mailbox-hold-information"></a><span data-ttu-id="af772-127">Exemple de requête d’opération GetHoldOnMailboxes : obtenir des informations de blocage de boîtes aux lettres</span><span class="sxs-lookup"><span data-stu-id="af772-127">GetHoldOnMailboxes operation request example: Get mailbox hold information</span></span>

<span data-ttu-id="af772-128">Une demande d’opération **GetHoldOnMailboxes** l’exemple suivant montre comment obtenir les informations de blocage de boîtes aux lettres pour la suspension de la boîte aux lettres HoldId2.</span><span class="sxs-lookup"><span data-stu-id="af772-128">The following example of a **GetHoldOnMailboxes** operation request shows how to get the mailbox hold information for the HoldId2 mailbox hold.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="af772-129">La demande SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="af772-129">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="af772-130">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="af772-130">GetHoldOnMailboxes</span></span>](getholdonmailboxes.md)
    
- [<span data-ttu-id="af772-131">HoldId</span><span class="sxs-lookup"><span data-stu-id="af772-131">HoldId</span></span>](holdid.md)
    
## <a name="successful-getholdonmailboxes-operation-response"></a><span data-ttu-id="af772-132">Réponse d’opération GetHoldOnMailboxes réussie</span><span class="sxs-lookup"><span data-stu-id="af772-132">Successful GetHoldOnMailboxes operation response</span></span>

<span data-ttu-id="af772-133">L’exemple suivant montre une réponse positive à une opération **GetHoldOnMailboxes** demande pour obtenir la boîte aux lettres contiennent des informations pour la suspension de la boîte aux lettres HoldId2.</span><span class="sxs-lookup"><span data-stu-id="af772-133">The following example shows a successful response to a **GetHoldOnMailboxes** operation request to get the mailbox hold information for the HoldId2 mailbox hold.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetHoldOnMailboxesResponse ResponseClass="Success" 
                                  xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <MailboxHoldResult>
            <HoldId xmlns="http://schemas.microsoft.com/exchange/services/2006/types">HoldId2</HoldId>
            <Query xmlns="http://schemas.microsoft.com/exchange/services/2006/types">test</Query>
            <MailboxHoldStatuses xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="af772-134">La réponse SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="af772-134">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="af772-135">GetHoldOnMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="af772-135">GetHoldOnMailboxesResponse</span></span>](getholdonmailboxesresponse.md)
    
- [<span data-ttu-id="af772-136">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="af772-136">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="af772-137">MailboxHoldResult</span><span class="sxs-lookup"><span data-stu-id="af772-137">MailboxHoldResult</span></span>](mailboxholdresult.md)
    
- [<span data-ttu-id="af772-138">HoldId</span><span class="sxs-lookup"><span data-stu-id="af772-138">HoldId</span></span>](holdid.md)
    
- [<span data-ttu-id="af772-139">Query</span><span class="sxs-lookup"><span data-stu-id="af772-139">Query</span></span>](query.md)
    
- [<span data-ttu-id="af772-140">MailboxHoldStatuses</span><span class="sxs-lookup"><span data-stu-id="af772-140">MailboxHoldStatuses</span></span>](mailboxholdstatuses.md)
    
- [<span data-ttu-id="af772-141">MailboxHoldStatus</span><span class="sxs-lookup"><span data-stu-id="af772-141">MailboxHoldStatus</span></span>](mailboxholdstatus.md)
    
- [<span data-ttu-id="af772-142">Boîte aux lettres (chaîne)</span><span class="sxs-lookup"><span data-stu-id="af772-142">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="af772-143">État (HoldStatusType)</span><span class="sxs-lookup"><span data-stu-id="af772-143">Status (HoldStatusType)</span></span>](status-holdstatustype.md)
    
- [<span data-ttu-id="af772-144">AdditionalInfo</span><span class="sxs-lookup"><span data-stu-id="af772-144">AdditionalInfo</span></span>](additionalinfo.md)
    
## <a name="getholdonmailboxes-operation-error-response"></a><span data-ttu-id="af772-145">Réponse d’erreur d’opération GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="af772-145">GetHoldOnMailboxes operation error response</span></span>

<span data-ttu-id="af772-146">L’exemple suivant montre une réponse d’erreur à une demande d’opération **GetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="af772-146">The following example shows an error response to a **GetHoldOnMailboxes** operation request.</span></span> <span data-ttu-id="af772-147">Il s’agit d’une réponse à une demande pour obtenir une suspension qui a été supprimée.</span><span class="sxs-lookup"><span data-stu-id="af772-147">This is a response to a request to get a hold that has been deleted.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetHoldOnMailboxesResponse ResponseClass="Error" 
                                  xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specific query-based hold is not found.</MessageText>
         <ResponseCode>ErrorMailboxHoldNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetHoldOnMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="af772-148">La réponse d’erreur corps SOAP contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="af772-148">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="af772-149">GetHoldOnMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="af772-149">GetHoldOnMailboxesResponse</span></span>](getholdonmailboxesresponse.md)
    
- [<span data-ttu-id="af772-150">MessageText</span><span class="sxs-lookup"><span data-stu-id="af772-150">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="af772-151">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="af772-151">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="af772-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="af772-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="af772-153">Pour les codes d’erreur générique à EWS, spécifiques à cette opération, consultez la rubrique [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="af772-153">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="af772-154">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="af772-154">See also</span></span>

- [<span data-ttu-id="af772-155">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="af772-155">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="af772-156">Opération GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="af772-156">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="af772-157">Opération SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="af772-157">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)
    
- [<span data-ttu-id="af772-158">Opération SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="af772-158">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)
    
- [<span data-ttu-id="af772-159">Opération GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="af772-159">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="af772-160">Opération GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="af772-160">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    
- [<span data-ttu-id="af772-161">Opération GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="af772-161">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

