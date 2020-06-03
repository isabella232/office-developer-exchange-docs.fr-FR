---
title: Opération SetHoldOnMailboxes
manager: sethgros
ms.date: 01/24/2020
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9015a0d8-3495-461b-aa79-797d23169585
description: Trouvez des informations sur l’opération EWS SetHoldOnMailboxes.
ms.openlocfilehash: 4d79ba9f616974b9415ae9eae23b8f5fdb0ab205
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44448393"
---
# <a name="setholdonmailboxes-operation"></a><span data-ttu-id="160ef-103">Opération SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="160ef-103">SetHoldOnMailboxes operation</span></span>

> [!IMPORTANT]
> <span data-ttu-id="160ef-104">À partir du 1er avril 2020, l’opération SetHoldOnMailboxes ne sera plus disponible dans Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="160ef-104">Starting on April 1, 2020, the SetHoldOnMailboxes operation will no longer be available in Exchange Online.</span></span> <span data-ttu-id="160ef-105">Cette opération ne sera pas affectée dans les versions locales d’Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="160ef-105">This operation won't be affected in on-premises versions of Exchange Server.</span></span> <span data-ttu-id="160ef-106">Pour plus d’informations, reportez-vous à la section [retraite des outils eDiscovery hérités dans Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#getsearchablemailboxes-setholdonmailboxes-and-getholdonmailboxes-operations-in-the-ews-api).</span><span class="sxs-lookup"><span data-stu-id="160ef-106">For more information, see [Retirement of legacy eDiscovery tools in Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#getsearchablemailboxes-setholdonmailboxes-and-getholdonmailboxes-operations-in-the-ews-api).</span></span>

<span data-ttu-id="160ef-107">Trouvez des informations sur l’opération EWS **SetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="160ef-107">Find information about the **SetHoldOnMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="160ef-108">L’opération **SetHoldOnMailboxes** définit une stratégie de blocage de boîte aux lettres sur les boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="160ef-108">The **SetHoldOnMailboxes** operation sets a mailbox hold policy on mailboxes.</span></span> 
  
<span data-ttu-id="160ef-109">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="160ef-109">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-setholdonmailboxes-operation"></a><span data-ttu-id="160ef-110">Utilisation de l’opération SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="160ef-110">Using the SetHoldOnMailboxes operation</span></span>

<span data-ttu-id="160ef-111">L’opération **SetHoldOnMailboxes** définit la conservation d’une boîte aux lettres sur une ou plusieurs boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="160ef-111">The **SetHoldOnMailboxes** operation sets a mailbox hold on to one or more mailboxes.</span></span> 
  
### <a name="setholdonmailboxes-operation-soap-headers"></a><span data-ttu-id="160ef-112">En-têtes SOAP d’opération SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="160ef-112">SetHoldOnMailboxes operation SOAP headers</span></span>

<span data-ttu-id="160ef-113">L’opération **SetHoldOnMailboxes** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="160ef-113">The **SetHoldOnMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="160ef-114">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="160ef-114">**Header name**</span></span>|<span data-ttu-id="160ef-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="160ef-115">**Element**</span></span>|<span data-ttu-id="160ef-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="160ef-116">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="160ef-117">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="160ef-117">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="160ef-118">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="160ef-118">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="160ef-119">Identifie les rôles serveur nécessaires pour que l’appelant effectue la demande.</span><span class="sxs-lookup"><span data-stu-id="160ef-119">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="160ef-120">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="160ef-120">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="160ef-121">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="160ef-121">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="160ef-122">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="160ef-122">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="160ef-123">Identifie la version de schéma de la demande d’opération.</span><span class="sxs-lookup"><span data-stu-id="160ef-123">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="160ef-124">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="160ef-124">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="160ef-125">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="160ef-125">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="160ef-126">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="160ef-126">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="160ef-127">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="160ef-127">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="160ef-128">Cet en-tête s’applique à une réponse.</span><span class="sxs-lookup"><span data-stu-id="160ef-128">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="setholdonmailboxes-operation-request-example-apply-a-hold-on-a-mailbox"></a><span data-ttu-id="160ef-129">Exemple de requête d’opération SetHoldOnMailboxes : appliquer une conservation sur une boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="160ef-129">SetHoldOnMailboxes operation request example: Apply a hold on a mailbox</span></span>

<span data-ttu-id="160ef-130">L’exemple suivant de demande d’opération **SetHoldOnMailboxes** montre comment appliquer une conservation sur deux boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="160ef-130">The following example of a **SetHoldOnMailboxes** operation request shows how to apply a hold on two mailboxes.</span></span> <span data-ttu-id="160ef-131">La conservation de la boîte aux lettres a été créée à l’aide de la commande [New-MailboxSearch](https://technet.microsoft.com/library/dd298064.aspx) .</span><span class="sxs-lookup"><span data-stu-id="160ef-131">The mailbox hold was created by using the [New-MailboxSearch](https://technet.microsoft.com/library/dd298064.aspx) command.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="160ef-132">Le corps SOAP de la demande contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="160ef-132">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="160ef-133">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="160ef-133">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
    
- [<span data-ttu-id="160ef-134">ActionType (HoldActionType)</span><span class="sxs-lookup"><span data-stu-id="160ef-134">ActionType (HoldActionType)</span></span>](actiontype-holdactiontype.md)
    
- [<span data-ttu-id="160ef-135">HoldId</span><span class="sxs-lookup"><span data-stu-id="160ef-135">HoldId</span></span>](holdid.md)
    
- [<span data-ttu-id="160ef-136">Query</span><span class="sxs-lookup"><span data-stu-id="160ef-136">Query</span></span>](query.md)
    
- [<span data-ttu-id="160ef-137">Boîtes aux lettres (ArrayOfStringsType)</span><span class="sxs-lookup"><span data-stu-id="160ef-137">Mailboxes (ArrayOfStringsType)</span></span>](mailboxes-arrayofstringstype.md)
    
- [<span data-ttu-id="160ef-138">String</span><span class="sxs-lookup"><span data-stu-id="160ef-138">String</span></span>](string.md)
    
- [<span data-ttu-id="160ef-139">Language</span><span class="sxs-lookup"><span data-stu-id="160ef-139">Language</span></span>](language.md)
    
- [<span data-ttu-id="160ef-140">IncludeNonIndexableItems</span><span class="sxs-lookup"><span data-stu-id="160ef-140">IncludeNonIndexableItems</span></span>](includenonindexableitems.md)
    
- [<span data-ttu-id="160ef-141">Déduplication</span><span class="sxs-lookup"><span data-stu-id="160ef-141">Deduplication</span></span>](deduplication.md)
    
## <a name="successful-setholdonmailboxes-operation-response"></a><span data-ttu-id="160ef-142">Réponse de l’opération SetHoldOnMailboxes réussie</span><span class="sxs-lookup"><span data-stu-id="160ef-142">Successful SetHoldOnMailboxes operation response</span></span>

<span data-ttu-id="160ef-143">L’exemple suivant montre une réponse réussie à une demande d’opération **SetHoldOnMailboxes** afin de mettre en attente deux boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="160ef-143">The following example shows a successful response to a **SetHoldOnMailboxes** operation request to put two mailboxes on hold.</span></span> 
  
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
      <SetHoldOnMailboxesResponse ResponseClass="Success" 
                                  xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <MailboxHoldResult>
            <HoldId xmlns="https://schemas.microsoft.com/exchange/services/2006/types">HoldId2</HoldId>
            <Query xmlns="https://schemas.microsoft.com/exchange/services/2006/types">test</Query>
            <MailboxHoldStatuses xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="160ef-144">Le corps SOAP de réponse contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="160ef-144">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="160ef-145">SetHoldOnMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="160ef-145">SetHoldOnMailboxesResponse</span></span>](setholdonmailboxesresponse.md)
    
- [<span data-ttu-id="160ef-146">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="160ef-146">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="160ef-147">MailboxHoldResult</span><span class="sxs-lookup"><span data-stu-id="160ef-147">MailboxHoldResult</span></span>](mailboxholdresult.md)
    
- [<span data-ttu-id="160ef-148">HoldId</span><span class="sxs-lookup"><span data-stu-id="160ef-148">HoldId</span></span>](holdid.md)
    
- [<span data-ttu-id="160ef-149">Query</span><span class="sxs-lookup"><span data-stu-id="160ef-149">Query</span></span>](query.md)
    
- [<span data-ttu-id="160ef-150">MailboxHoldStatuses</span><span class="sxs-lookup"><span data-stu-id="160ef-150">MailboxHoldStatuses</span></span>](mailboxholdstatuses.md)
    
- [<span data-ttu-id="160ef-151">MailboxHoldStatus</span><span class="sxs-lookup"><span data-stu-id="160ef-151">MailboxHoldStatus</span></span>](mailboxholdstatus.md)
    
- [<span data-ttu-id="160ef-152">Mailbox (String)</span><span class="sxs-lookup"><span data-stu-id="160ef-152">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="160ef-153">État (HoldStatusType)</span><span class="sxs-lookup"><span data-stu-id="160ef-153">Status (HoldStatusType)</span></span>](status-holdstatustype.md)
    
- [<span data-ttu-id="160ef-154">AdditionalInfo</span><span class="sxs-lookup"><span data-stu-id="160ef-154">AdditionalInfo</span></span>](additionalinfo.md)
    
## <a name="setholdonmailboxes-operation-error-response"></a><span data-ttu-id="160ef-155">Réponse d’erreur d’opération SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="160ef-155">SetHoldOnMailboxes operation error response</span></span>

<span data-ttu-id="160ef-156">L’exemple suivant montre une réponse d’erreur à une demande d’opération **SetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="160ef-156">The following example shows an error response to a **SetHoldOnMailboxes** operation request.</span></span> <span data-ttu-id="160ef-157">Il s’agit d’une réponse à une demande contenant un identificateur de boîte aux lettres spécifié de manière incorrecte.</span><span class="sxs-lookup"><span data-stu-id="160ef-157">This is a response to a request that contains an incorrectly specified mailbox identifier.</span></span> 
  
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
      <SetHoldOnMailboxesResponse ResponseClass="Error" 
                                  xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>No mailbox is specified for hold operation. If specified in the request, then it could be the object does not exist in AD or is a Distribution Group.</MessageText>
         <ResponseCode>ErrorInvalidOperation</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </SetHoldOnMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="160ef-158">Le corps SOAP de la réponse d’erreur contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="160ef-158">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="160ef-159">SetHoldOnMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="160ef-159">SetHoldOnMailboxesResponse</span></span>](setholdonmailboxesresponse.md)
    
- [<span data-ttu-id="160ef-160">MessageText</span><span class="sxs-lookup"><span data-stu-id="160ef-160">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="160ef-161">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="160ef-161">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="160ef-162">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="160ef-162">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="160ef-163">Pour les autres codes d’erreur qui sont génériques à EWS et spécifiques à cette opération, voir [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="160ef-163">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="160ef-164">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="160ef-164">See also</span></span>

- [<span data-ttu-id="160ef-165">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="160ef-165">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="160ef-166">Opération GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="160ef-166">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="160ef-167">Opération SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="160ef-167">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)
    
- [<span data-ttu-id="160ef-168">Opération GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="160ef-168">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)
    
- [<span data-ttu-id="160ef-169">Opération GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="160ef-169">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="160ef-170">Opération GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="160ef-170">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    
- [<span data-ttu-id="160ef-171">Opération GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="160ef-171">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

