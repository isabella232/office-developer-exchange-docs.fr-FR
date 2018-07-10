---
title: Opération SetHoldOnMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9015a0d8-3495-461b-aa79-797d23169585
description: Opération de recherche plus d’informations sur la SetHoldOnMailboxes EWS.
ms.openlocfilehash: 1091ed14ceb25dfd275499b9db47ae4e41b5f1a0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829412"
---
# <a name="setholdonmailboxes-operation"></a><span data-ttu-id="bfeba-103">Opération SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="bfeba-103">SetHoldOnMailboxes operation</span></span>

<span data-ttu-id="bfeba-104">Trouvez des informations sur l’opération EWS **SetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="bfeba-104">Find information about the **SetHoldOnMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="bfeba-105">L’opération **SetHoldOnMailboxes** définit une stratégie de blocage de boîtes aux lettres sur les boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="bfeba-105">The **SetHoldOnMailboxes** operation sets a mailbox hold policy on mailboxes.</span></span> 
  
<span data-ttu-id="bfeba-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="bfeba-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-setholdonmailboxes-operation"></a><span data-ttu-id="bfeba-107">Utilisation de l’opération SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="bfeba-107">Using the SetHoldOnMailboxes operation</span></span>

<span data-ttu-id="bfeba-108">L’opération **SetHoldOnMailboxes** définit un blocage de boîtes aux lettres sur un ou plusieurs boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="bfeba-108">The **SetHoldOnMailboxes** operation sets a mailbox hold on to one or more mailboxes.</span></span> 
  
### <a name="setholdonmailboxes-operation-soap-headers"></a><span data-ttu-id="bfeba-109">En-têtes SOAP SetHoldOnMailboxes opération</span><span class="sxs-lookup"><span data-stu-id="bfeba-109">SetHoldOnMailboxes operation SOAP headers</span></span>

<span data-ttu-id="bfeba-110">L’opération **SetHoldOnMailboxes** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="bfeba-110">The **SetHoldOnMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="bfeba-111">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="bfeba-111">**Header name**</span></span>|<span data-ttu-id="bfeba-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bfeba-112">**Element**</span></span>|<span data-ttu-id="bfeba-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="bfeba-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="bfeba-114">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="bfeba-114">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="bfeba-115">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="bfeba-115">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="bfeba-116">Identifie les rôles de serveur qui sont nécessaires pour l’appelant effectuer la demande.</span><span class="sxs-lookup"><span data-stu-id="bfeba-116">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="bfeba-117">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="bfeba-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="bfeba-118">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="bfeba-118">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="bfeba-119">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="bfeba-119">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="bfeba-120">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="bfeba-120">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="bfeba-121">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="bfeba-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="bfeba-122">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="bfeba-122">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="bfeba-123">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="bfeba-123">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="bfeba-124">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="bfeba-124">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="bfeba-125">Cet en-tête est applicable à une réponse.</span><span class="sxs-lookup"><span data-stu-id="bfeba-125">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="setholdonmailboxes-operation-request-example-apply-a-hold-on-a-mailbox"></a><span data-ttu-id="bfeba-126">Exemple de requête d’opération SetHoldOnMailboxes : appliquer un blocage sur une boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="bfeba-126">SetHoldOnMailboxes operation request example: Apply a hold on a mailbox</span></span>

<span data-ttu-id="bfeba-127">Une demande d’opération **SetHoldOnMailboxes** l’exemple suivant montre comment appliquer un blocage sur deux boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="bfeba-127">The following example of a **SetHoldOnMailboxes** operation request shows how to apply a hold on two mailboxes.</span></span> <span data-ttu-id="bfeba-128">La suspension de la boîte aux lettres a été créée à l’aide de la commande [New-MailboxSearch](http://technet.microsoft.com/fr-fr/library/dd298064.aspx) .</span><span class="sxs-lookup"><span data-stu-id="bfeba-128">The mailbox hold was created by using the [New-MailboxSearch](http://technet.microsoft.com/fr-fr/library/dd298064.aspx) command.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:SetHoldOnMailboxes>
         <m:ActionType>Create</m:ActionType>
         <m:HoldId>HoldId2</m:HoldId>
         <m:Query>test</m:Query>
         <m:Mailboxes>
            <t:String>/o=First/ou=Exchange(DLT)/cn=Recipients/cn=1fa441ff5e4749ba43ecc0fd94c21adf-Willi</t:String>
            <t:String>/o=First/ou=Exchange(DLT)/cn=Recipients/cn=aed2346adaa34ffc9f0f339917e8de95-Micha</t:String>
         </m:Mailboxes>
         <m:Language>English</m:Language>
         <m:IncludeNonIndexableItems>false</m:IncludeNonIndexableItems>
         <m:Deduplication>true</m:Deduplication>
      </m:SetHoldOnMailboxes>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="bfeba-129">La demande SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="bfeba-129">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="bfeba-130">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="bfeba-130">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
    
- [<span data-ttu-id="bfeba-131">ActionType (HoldActionType)</span><span class="sxs-lookup"><span data-stu-id="bfeba-131">ActionType (HoldActionType)</span></span>](actiontype-holdactiontype.md)
    
- [<span data-ttu-id="bfeba-132">HoldId</span><span class="sxs-lookup"><span data-stu-id="bfeba-132">HoldId</span></span>](holdid.md)
    
- [<span data-ttu-id="bfeba-133">Query</span><span class="sxs-lookup"><span data-stu-id="bfeba-133">Query</span></span>](query.md)
    
- [<span data-ttu-id="bfeba-134">Boîtes aux lettres (ArrayOfStringsType)</span><span class="sxs-lookup"><span data-stu-id="bfeba-134">Mailboxes (ArrayOfStringsType)</span></span>](mailboxes-arrayofstringstype.md)
    
- [<span data-ttu-id="bfeba-135">Chaîne</span><span class="sxs-lookup"><span data-stu-id="bfeba-135">String</span></span>](string.md)
    
- [<span data-ttu-id="bfeba-136">Language</span><span class="sxs-lookup"><span data-stu-id="bfeba-136">Language</span></span>](language.md)
    
- [<span data-ttu-id="bfeba-137">IncludeNonIndexableItems</span><span class="sxs-lookup"><span data-stu-id="bfeba-137">IncludeNonIndexableItems</span></span>](includenonindexableitems.md)
    
- [<span data-ttu-id="bfeba-138">Déduplication</span><span class="sxs-lookup"><span data-stu-id="bfeba-138">Deduplication</span></span>](deduplication.md)
    
## <a name="successful-setholdonmailboxes-operation-response"></a><span data-ttu-id="bfeba-139">Réponse d’opération SetHoldOnMailboxes réussie</span><span class="sxs-lookup"><span data-stu-id="bfeba-139">Successful SetHoldOnMailboxes operation response</span></span>

<span data-ttu-id="bfeba-140">L’exemple suivant montre une réponse positive à une demande d’opération **SetHoldOnMailboxes** pour mettre les deux boîtes aux lettres en attente.</span><span class="sxs-lookup"><span data-stu-id="bfeba-140">The following example shows a successful response to a **SetHoldOnMailboxes** operation request to put two mailboxes on hold.</span></span> 
  
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
      <SetHoldOnMailboxesResponse ResponseClass="Success" 
                                  xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <MailboxHoldResult>
            <HoldId xmlns="http://schemas.microsoft.com/exchange/services/2006/types">HoldId2</HoldId>
            <Query xmlns="http://schemas.microsoft.com/exchange/services/2006/types">test</Query>
            <MailboxHoldStatuses xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <MailboxHoldStatus>
                  <Mailbox>o=First/ou=Exchange(DLT)/cn=Recipients/cn=1fa441ff5e4749ba43ecc0fd94c21adf-Willi</Mailbox>
                  <Status>Pending</Status>
                  <AdditionalInfo/>
               </MailboxHoldStatus>
               <MailboxHoldStatus>
                  <Mailbox>/o=First/ou=Exchange(DLT)/cn=Recipients/cn=aed2346adaa34ffc9f0f339917e8de95-Micha</Mailbox>
                  <Status>Pending</Status>
                  <AdditionalInfo/>
               </MailboxHoldStatus>
            </MailboxHoldStatuses>
         </MailboxHoldResult>
      </SetHoldOnMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="bfeba-141">La réponse SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="bfeba-141">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="bfeba-142">SetHoldOnMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="bfeba-142">SetHoldOnMailboxesResponse</span></span>](setholdonmailboxesresponse.md)
    
- [<span data-ttu-id="bfeba-143">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="bfeba-143">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="bfeba-144">MailboxHoldResult</span><span class="sxs-lookup"><span data-stu-id="bfeba-144">MailboxHoldResult</span></span>](mailboxholdresult.md)
    
- [<span data-ttu-id="bfeba-145">HoldId</span><span class="sxs-lookup"><span data-stu-id="bfeba-145">HoldId</span></span>](holdid.md)
    
- [<span data-ttu-id="bfeba-146">Query</span><span class="sxs-lookup"><span data-stu-id="bfeba-146">Query</span></span>](query.md)
    
- [<span data-ttu-id="bfeba-147">MailboxHoldStatuses</span><span class="sxs-lookup"><span data-stu-id="bfeba-147">MailboxHoldStatuses</span></span>](mailboxholdstatuses.md)
    
- [<span data-ttu-id="bfeba-148">MailboxHoldStatus</span><span class="sxs-lookup"><span data-stu-id="bfeba-148">MailboxHoldStatus</span></span>](mailboxholdstatus.md)
    
- [<span data-ttu-id="bfeba-149">Boîte aux lettres (chaîne)</span><span class="sxs-lookup"><span data-stu-id="bfeba-149">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="bfeba-150">État (HoldStatusType)</span><span class="sxs-lookup"><span data-stu-id="bfeba-150">Status (HoldStatusType)</span></span>](status-holdstatustype.md)
    
- [<span data-ttu-id="bfeba-151">AdditionalInfo</span><span class="sxs-lookup"><span data-stu-id="bfeba-151">AdditionalInfo</span></span>](additionalinfo.md)
    
## <a name="setholdonmailboxes-operation-error-response"></a><span data-ttu-id="bfeba-152">Réponse d’erreur d’opération SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="bfeba-152">SetHoldOnMailboxes operation error response</span></span>

<span data-ttu-id="bfeba-153">L’exemple suivant montre une réponse d’erreur à une demande d’opération **SetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="bfeba-153">The following example shows an error response to a **SetHoldOnMailboxes** operation request.</span></span> <span data-ttu-id="bfeba-154">Il s’agit d’une réponse à une demande qui contient un identificateur de boîte aux lettres spécifiée est incorrecte.</span><span class="sxs-lookup"><span data-stu-id="bfeba-154">This is a response to a request that contains an incorrectly specified mailbox identifier.</span></span> 
  
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
      <SetHoldOnMailboxesResponse ResponseClass="Error" 
                                  xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>No mailbox is specified for hold operation. If specified in the request, then it could be the object does not exist in AD or is a Distribution Group.</MessageText>
         <ResponseCode>ErrorInvalidOperation</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </SetHoldOnMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="bfeba-155">La réponse d’erreur corps SOAP contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="bfeba-155">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="bfeba-156">SetHoldOnMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="bfeba-156">SetHoldOnMailboxesResponse</span></span>](setholdonmailboxesresponse.md)
    
- [<span data-ttu-id="bfeba-157">MessageText</span><span class="sxs-lookup"><span data-stu-id="bfeba-157">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="bfeba-158">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="bfeba-158">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="bfeba-159">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="bfeba-159">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="bfeba-160">Pour les codes d’erreur générique à EWS, spécifiques à cette opération, consultez la rubrique [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="bfeba-160">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="bfeba-161">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bfeba-161">See also</span></span>

- [<span data-ttu-id="bfeba-162">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="bfeba-162">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="bfeba-163">Opération GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="bfeba-163">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="bfeba-164">Opération SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="bfeba-164">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)
    
- [<span data-ttu-id="bfeba-165">Opération GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="bfeba-165">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)
    
- [<span data-ttu-id="bfeba-166">Opération GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="bfeba-166">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="bfeba-167">Opération GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="bfeba-167">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    
- [<span data-ttu-id="bfeba-168">Opération GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="bfeba-168">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

