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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829412"
---
# <a name="setholdonmailboxes-operation"></a><span data-ttu-id="8ef69-103">Opération SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="8ef69-103">SetHoldOnMailboxes operation</span></span>

<span data-ttu-id="8ef69-104">Trouvez des informations sur l’opération EWS **SetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="8ef69-104">Find information about the **SetHoldOnMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="8ef69-105">L’opération **SetHoldOnMailboxes** définit une stratégie de blocage de boîtes aux lettres sur les boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="8ef69-105">The **SetHoldOnMailboxes** operation sets a mailbox hold policy on mailboxes.</span></span> 
  
<span data-ttu-id="8ef69-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="8ef69-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-setholdonmailboxes-operation"></a><span data-ttu-id="8ef69-107">Utilisation de l’opération SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="8ef69-107">Using the SetHoldOnMailboxes operation</span></span>

<span data-ttu-id="8ef69-108">L’opération **SetHoldOnMailboxes** définit un blocage de boîtes aux lettres sur un ou plusieurs boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="8ef69-108">The **SetHoldOnMailboxes** operation sets a mailbox hold on to one or more mailboxes.</span></span> 
  
### <a name="setholdonmailboxes-operation-soap-headers"></a><span data-ttu-id="8ef69-109">En-têtes SOAP SetHoldOnMailboxes opération</span><span class="sxs-lookup"><span data-stu-id="8ef69-109">SetHoldOnMailboxes operation SOAP headers</span></span>

<span data-ttu-id="8ef69-110">L’opération **SetHoldOnMailboxes** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="8ef69-110">The **SetHoldOnMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="8ef69-111">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="8ef69-111">**Header name**</span></span>|<span data-ttu-id="8ef69-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8ef69-112">**Element**</span></span>|<span data-ttu-id="8ef69-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="8ef69-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="8ef69-114">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="8ef69-114">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="8ef69-115">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="8ef69-115">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="8ef69-116">Identifie les rôles de serveur qui sont nécessaires pour l’appelant effectuer la demande.</span><span class="sxs-lookup"><span data-stu-id="8ef69-116">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="8ef69-117">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="8ef69-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="8ef69-118">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="8ef69-118">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="8ef69-119">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="8ef69-119">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="8ef69-120">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="8ef69-120">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="8ef69-121">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="8ef69-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="8ef69-122">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="8ef69-122">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="8ef69-123">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="8ef69-123">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="8ef69-124">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="8ef69-124">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="8ef69-125">Cet en-tête est applicable à une réponse.</span><span class="sxs-lookup"><span data-stu-id="8ef69-125">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="setholdonmailboxes-operation-request-example-apply-a-hold-on-a-mailbox"></a><span data-ttu-id="8ef69-126">Exemple de requête d’opération SetHoldOnMailboxes : appliquer un blocage sur une boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="8ef69-126">SetHoldOnMailboxes operation request example: Apply a hold on a mailbox</span></span>

<span data-ttu-id="8ef69-127">Une demande d’opération **SetHoldOnMailboxes** l’exemple suivant montre comment appliquer un blocage sur deux boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="8ef69-127">The following example of a **SetHoldOnMailboxes** operation request shows how to apply a hold on two mailboxes.</span></span> <span data-ttu-id="8ef69-128">La suspension de la boîte aux lettres a été créée à l’aide de la commande [New-MailboxSearch](http://technet.microsoft.com/en-us/library/dd298064.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8ef69-128">The mailbox hold was created by using the [New-MailboxSearch](http://technet.microsoft.com/en-us/library/dd298064.aspx) command.</span></span> 
  
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

<span data-ttu-id="8ef69-129">La demande SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="8ef69-129">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="8ef69-130">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="8ef69-130">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
    
- [<span data-ttu-id="8ef69-131">ActionType (HoldActionType)</span><span class="sxs-lookup"><span data-stu-id="8ef69-131">ActionType (HoldActionType)</span></span>](actiontype-holdactiontype.md)
    
- [<span data-ttu-id="8ef69-132">HoldId</span><span class="sxs-lookup"><span data-stu-id="8ef69-132">HoldId</span></span>](holdid.md)
    
- [<span data-ttu-id="8ef69-133">Query</span><span class="sxs-lookup"><span data-stu-id="8ef69-133">Query</span></span>](query.md)
    
- [<span data-ttu-id="8ef69-134">Boîtes aux lettres (ArrayOfStringsType)</span><span class="sxs-lookup"><span data-stu-id="8ef69-134">Mailboxes (ArrayOfStringsType)</span></span>](mailboxes-arrayofstringstype.md)
    
- [<span data-ttu-id="8ef69-135">Chaîne</span><span class="sxs-lookup"><span data-stu-id="8ef69-135">String</span></span>](string.md)
    
- [<span data-ttu-id="8ef69-136">Language</span><span class="sxs-lookup"><span data-stu-id="8ef69-136">Language</span></span>](language.md)
    
- [<span data-ttu-id="8ef69-137">IncludeNonIndexableItems</span><span class="sxs-lookup"><span data-stu-id="8ef69-137">IncludeNonIndexableItems</span></span>](includenonindexableitems.md)
    
- [<span data-ttu-id="8ef69-138">Déduplication</span><span class="sxs-lookup"><span data-stu-id="8ef69-138">Deduplication</span></span>](deduplication.md)
    
## <a name="successful-setholdonmailboxes-operation-response"></a><span data-ttu-id="8ef69-139">Réponse d’opération SetHoldOnMailboxes réussie</span><span class="sxs-lookup"><span data-stu-id="8ef69-139">Successful SetHoldOnMailboxes operation response</span></span>

<span data-ttu-id="8ef69-140">L’exemple suivant montre une réponse positive à une demande d’opération **SetHoldOnMailboxes** pour mettre les deux boîtes aux lettres en attente.</span><span class="sxs-lookup"><span data-stu-id="8ef69-140">The following example shows a successful response to a **SetHoldOnMailboxes** operation request to put two mailboxes on hold.</span></span> 
  
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

<span data-ttu-id="8ef69-141">La réponse SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="8ef69-141">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="8ef69-142">SetHoldOnMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="8ef69-142">SetHoldOnMailboxesResponse</span></span>](setholdonmailboxesresponse.md)
    
- [<span data-ttu-id="8ef69-143">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="8ef69-143">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="8ef69-144">MailboxHoldResult</span><span class="sxs-lookup"><span data-stu-id="8ef69-144">MailboxHoldResult</span></span>](mailboxholdresult.md)
    
- [<span data-ttu-id="8ef69-145">HoldId</span><span class="sxs-lookup"><span data-stu-id="8ef69-145">HoldId</span></span>](holdid.md)
    
- [<span data-ttu-id="8ef69-146">Query</span><span class="sxs-lookup"><span data-stu-id="8ef69-146">Query</span></span>](query.md)
    
- [<span data-ttu-id="8ef69-147">MailboxHoldStatuses</span><span class="sxs-lookup"><span data-stu-id="8ef69-147">MailboxHoldStatuses</span></span>](mailboxholdstatuses.md)
    
- [<span data-ttu-id="8ef69-148">MailboxHoldStatus</span><span class="sxs-lookup"><span data-stu-id="8ef69-148">MailboxHoldStatus</span></span>](mailboxholdstatus.md)
    
- [<span data-ttu-id="8ef69-149">Boîte aux lettres (chaîne)</span><span class="sxs-lookup"><span data-stu-id="8ef69-149">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="8ef69-150">État (HoldStatusType)</span><span class="sxs-lookup"><span data-stu-id="8ef69-150">Status (HoldStatusType)</span></span>](status-holdstatustype.md)
    
- [<span data-ttu-id="8ef69-151">AdditionalInfo</span><span class="sxs-lookup"><span data-stu-id="8ef69-151">AdditionalInfo</span></span>](additionalinfo.md)
    
## <a name="setholdonmailboxes-operation-error-response"></a><span data-ttu-id="8ef69-152">Réponse d’erreur d’opération SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="8ef69-152">SetHoldOnMailboxes operation error response</span></span>

<span data-ttu-id="8ef69-153">L’exemple suivant montre une réponse d’erreur à une demande d’opération **SetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="8ef69-153">The following example shows an error response to a **SetHoldOnMailboxes** operation request.</span></span> <span data-ttu-id="8ef69-154">Il s’agit d’une réponse à une demande qui contient un identificateur de boîte aux lettres spécifiée est incorrecte.</span><span class="sxs-lookup"><span data-stu-id="8ef69-154">This is a response to a request that contains an incorrectly specified mailbox identifier.</span></span> 
  
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

<span data-ttu-id="8ef69-155">La réponse d’erreur corps SOAP contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="8ef69-155">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="8ef69-156">SetHoldOnMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="8ef69-156">SetHoldOnMailboxesResponse</span></span>](setholdonmailboxesresponse.md)
    
- [<span data-ttu-id="8ef69-157">MessageText</span><span class="sxs-lookup"><span data-stu-id="8ef69-157">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="8ef69-158">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="8ef69-158">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="8ef69-159">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="8ef69-159">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="8ef69-160">Pour les codes d’erreur générique à EWS, spécifiques à cette opération, consultez la rubrique [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="8ef69-160">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="8ef69-161">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8ef69-161">See also</span></span>

- [<span data-ttu-id="8ef69-162">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8ef69-162">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="8ef69-163">Opération GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="8ef69-163">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="8ef69-164">Opération SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="8ef69-164">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)
    
- [<span data-ttu-id="8ef69-165">Opération GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="8ef69-165">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)
    
- [<span data-ttu-id="8ef69-166">Opération GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ef69-166">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="8ef69-167">Opération GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="8ef69-167">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    
- [<span data-ttu-id="8ef69-168">Opération GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="8ef69-168">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

