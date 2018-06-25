---
title: Opération GetNonIndexableItemDetails
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9279c3ad-f7c8-4bbc-b0a7-2c78416cb39a
description: Opération de recherche plus d’informations sur la GetNonIndexableItemDetails EWS.
ms.openlocfilehash: 6b0c5afd54ac98f89bc6c5199300c20862c6f207
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756683"
---
# <a name="getnonindexableitemdetails-operation"></a><span data-ttu-id="9df22-103">Opération GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="9df22-103">GetNonIndexableItemDetails operation</span></span>

<span data-ttu-id="9df22-104">Trouvez des informations sur l’opération EWS **GetNonIndexableItemDetails** .</span><span class="sxs-lookup"><span data-stu-id="9df22-104">Find information about the **GetNonIndexableItemDetails** EWS operation.</span></span> 
  
<span data-ttu-id="9df22-105">L’opération **GetNonIndexableItemDetails** récupère plus d’informations sur les éléments qui ne peuvent pas être indexés.</span><span class="sxs-lookup"><span data-stu-id="9df22-105">The **GetNonIndexableItemDetails** operation retrieves details about items that cannot be indexed.</span></span> <span data-ttu-id="9df22-106">Cela inclut, mais n’est pas limité à l’identificateur d’élément, un code d’erreur, une description de l’erreur lors de la tentative d’index de l’élément et des informations supplémentaires sur le fichier.</span><span class="sxs-lookup"><span data-stu-id="9df22-106">This includes, but is not limited to, the item identifier, an error code, an error description, when an attempt was made to index the item, and additional information about the file.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="9df22-107">Bien que le schéma indique que plusieurs boîtes aux lettres pouvant être recherchées, dans la version initiale d’Exchange 2013, le service prend uniquement en charge les détails des éléments lors de l’obtention des éléments nonindexable dans une seule boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="9df22-107">Although the schema indicates that more than one mailbox can be searched, in the initial release version of Exchange 2013, the service only supports getting item details for nonindexable items in a single mailbox.</span></span> 
  
<span data-ttu-id="9df22-108">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9df22-108">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getnonindexableitemdetails-operation"></a><span data-ttu-id="9df22-109">Utilisation de l’opération GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="9df22-109">Using the GetNonIndexableItemDetails operation</span></span>

<span data-ttu-id="9df22-110">L’opération **GetNonIndexableItemDetails** identifie les éléments de boîte aux lettres qui ne peuvent pas être indexés et fournit des informations sur la raison pour laquelle les éléments ne peuvent pas être indexés.</span><span class="sxs-lookup"><span data-stu-id="9df22-110">The **GetNonIndexableItemDetails** operation identifies mailbox items that cannot be indexed and provides information about why the items cannot be indexed.</span></span> <span data-ttu-id="9df22-111">Éléments qui ne peuvent pas être indexés ne sont pas recherchés lors d’une recherche de découverte.</span><span class="sxs-lookup"><span data-stu-id="9df22-111">Items that cannot be indexed are not searched during a discovery search.</span></span> 
  
### <a name="getnonindexableitemdetails-operation-soap-headers"></a><span data-ttu-id="9df22-112">En-têtes SOAP GetNonIndexableItemDetails opération</span><span class="sxs-lookup"><span data-stu-id="9df22-112">GetNonIndexableItemDetails operation SOAP headers</span></span>

<span data-ttu-id="9df22-113">L’opération **GetNonIndexableItemDetails** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="9df22-113">The **GetNonIndexableItemDetails** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="9df22-114">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="9df22-114">**Header name**</span></span>|<span data-ttu-id="9df22-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9df22-115">**Element**</span></span>|<span data-ttu-id="9df22-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="9df22-116">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="9df22-117">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="9df22-117">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="9df22-118">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="9df22-118">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="9df22-119">Identifie les rôles de serveur qui sont nécessaires pour l’appelant effectuer la demande.</span><span class="sxs-lookup"><span data-stu-id="9df22-119">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="9df22-120">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="9df22-120">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="9df22-121">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="9df22-121">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="9df22-122">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="9df22-122">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="9df22-123">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="9df22-123">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="9df22-124">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="9df22-124">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="9df22-125">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="9df22-125">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="9df22-126">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="9df22-126">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="9df22-127">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="9df22-127">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="9df22-128">Cet en-tête est applicable à une réponse.</span><span class="sxs-lookup"><span data-stu-id="9df22-128">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getnonindexableitemdetails-operation-request-example-get-the-details-of-an-item-that-cannot-be-indexed"></a><span data-ttu-id="9df22-129">Exemple de requête d’opération GetNonIndexableItemDetails : obtenir les détails d’un élément qui ne peuvent pas être indexés</span><span class="sxs-lookup"><span data-stu-id="9df22-129">GetNonIndexableItemDetails operation request example: Get the details of an item that cannot be indexed</span></span>

<span data-ttu-id="9df22-130">Une demande d’opération **GetNonIndexableItemDetails** l’exemple suivant montre comment demander les détails des éléments qui ne peuvent pas être indexés pour une boîte aux lettres unique.</span><span class="sxs-lookup"><span data-stu-id="9df22-130">The following example of a **GetNonIndexableItemDetails** operation request shows how to request the details for items that cannot be indexed for a single mailbox.</span></span> <span data-ttu-id="9df22-131">La recherche est effectuée sur les deux principal et d’archivage de boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="9df22-131">The search is performed across both primary and archive mailboxes.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="9df22-132">Tous les noms de domaine hérité dans cet exemple ont être raccourcie afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="9df22-132">All legacy domain names in this example have be shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetNonIndexableItemDetails>
         <m:Mailboxes>
            <t:LegacyDN>/o=First Organization/ou=Exchange Administrative Group (FYT)/cn=Recipients/cn=35-Steve</t:LegacyDN>
         </m:Mailboxes>
         <m:SearchArchiveOnly>false</m:SearchArchiveOnly>
      </m:GetNonIndexableItemDetails>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="9df22-133">La demande SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="9df22-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="9df22-134">GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="9df22-134">GetNonIndexableItemDetails</span></span>](getnonindexableitemdetails.md)
    
- [<span data-ttu-id="9df22-135">Boîtes aux lettres (NonEmptyArrayOfLegacyDNsType)</span><span class="sxs-lookup"><span data-stu-id="9df22-135">Mailboxes (NonEmptyArrayOfLegacyDNsType)</span></span>](mailboxes-nonemptyarrayoflegacydnstype.md)
    
- [<span data-ttu-id="9df22-136">LegacyDN</span><span class="sxs-lookup"><span data-stu-id="9df22-136">LegacyDN</span></span>](legacydn.md)
    
- [<span data-ttu-id="9df22-137">SearchArchiveOnly</span><span class="sxs-lookup"><span data-stu-id="9df22-137">SearchArchiveOnly</span></span>](searcharchiveonly.md)
    
## <a name="successful-getnonindexableitemdetails-operation-response"></a><span data-ttu-id="9df22-138">Réponse d’opération GetNonIndexableItemDetails réussie</span><span class="sxs-lookup"><span data-stu-id="9df22-138">Successful GetNonIndexableItemDetails operation response</span></span>

<span data-ttu-id="9df22-139">L’exemple suivant montre une réponse positive à une demande d’opération **GetNonIndexableItemDetails** pour obtenir les éléments qui ne peuvent pas être indexés pour une boîte aux lettres unique.</span><span class="sxs-lookup"><span data-stu-id="9df22-139">The following example shows a successful response to a **GetNonIndexableItemDetails** operation request to get items that cannot be indexed for a single mailbox.</span></span> <span data-ttu-id="9df22-140">L’élément dans cet exemple ne peuvent pas être indexé est le fichier binaryfile.abc, qui est d’un format inconnu.</span><span class="sxs-lookup"><span data-stu-id="9df22-140">The item in this example that cannot be indexed is the binaryfile.abc file, which is of an unknown format.</span></span> 
  
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
      <GetNonIndexableItemDetailsResponse ResponseClass="Success" 
                                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <NonIndexableItemDetailsResult>
            <Items xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <NonIndexableItemDetail>
                  <ItemId Id="AQMkAGVmNDAyOQAAAY2fUAAAAA==" ChangeKey="CQAAAA=="/>
                  <ErrorCode>DocumentParserFailure</ErrorCode>
                  <ErrorDescription>The document parser encountered a processing error.</ErrorDescription>
                  <IsPartiallyIndexed>false</IsPartiallyIndexed>
                  <IsPermanentFailure>true</IsPermanentFailure>
                  <SortValue>502511175756</SortValue>
                  <AttemptCount>0</AttemptCount>
                  <LastAttemptTime>2012-11-15T01:56:11Z</LastAttemptTime>
                  <AdditionalInfo> 301002 Error parsing document 'exchange://localhost/Attachment/d987b1f4-9aa7-42b3-aa8c-9515a35dfa1a/1f3047d4-c287-41e4-910c-feb70c1a59f0/ef402830-3d33-4a0d-a4e9-d8576900060d/85b83861-0026-418f-8464-be2036696333/502511175756.0/binaryfile.abc'. Document has an undetectable format and will not be parsed.</AdditionalInfo>
               </NonIndexableItemDetail>
            </Items>
         </NonIndexableItemDetailsResult>
      </GetNonIndexableItemDetailsResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="9df22-141">La réponse SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="9df22-141">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="9df22-142">GetNonIndexableItemDetailsResponse</span><span class="sxs-lookup"><span data-stu-id="9df22-142">GetNonIndexableItemDetailsResponse</span></span>](getnonindexableitemdetailsresponse.md)
    
- [<span data-ttu-id="9df22-143">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="9df22-143">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="9df22-144">NonIndexableItemDetailsResult</span><span class="sxs-lookup"><span data-stu-id="9df22-144">NonIndexableItemDetailsResult</span></span>](nonindexableitemdetailsresult.md)
    
- [<span data-ttu-id="9df22-145">NonIndexableItemDetail</span><span class="sxs-lookup"><span data-stu-id="9df22-145">NonIndexableItemDetail</span></span>](nonindexableitemdetail.md)
    
- [<span data-ttu-id="9df22-146">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="9df22-146">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="9df22-147">ErrorCode (ItemIndexErrorType)</span><span class="sxs-lookup"><span data-stu-id="9df22-147">ErrorCode (ItemIndexErrorType)</span></span>](errorcode-itemindexerrortype.md)
    
- [<span data-ttu-id="9df22-148">ErrorDescription</span><span class="sxs-lookup"><span data-stu-id="9df22-148">ErrorDescription</span></span>](errordescription.md)
    
- [<span data-ttu-id="9df22-149">IsPartiallyIndexed</span><span class="sxs-lookup"><span data-stu-id="9df22-149">IsPartiallyIndexed</span></span>](ispartiallyindexed.md)
    
- [<span data-ttu-id="9df22-150">IsPermanentFailure</span><span class="sxs-lookup"><span data-stu-id="9df22-150">IsPermanentFailure</span></span>](ispermanentfailure.md)
    
- [<span data-ttu-id="9df22-151">SortValue</span><span class="sxs-lookup"><span data-stu-id="9df22-151">SortValue</span></span>](sortvalue.md)
    
- [<span data-ttu-id="9df22-152">AttemptCount</span><span class="sxs-lookup"><span data-stu-id="9df22-152">AttemptCount</span></span>](attemptcount.md)
    
- [<span data-ttu-id="9df22-153">LastAttemptTime</span><span class="sxs-lookup"><span data-stu-id="9df22-153">LastAttemptTime</span></span>](lastattempttime.md)
    
- [<span data-ttu-id="9df22-154">AdditionalInfo</span><span class="sxs-lookup"><span data-stu-id="9df22-154">AdditionalInfo</span></span>](additionalinfo.md)
    
## <a name="getnonindexableitemdetails-operation-error-response"></a><span data-ttu-id="9df22-155">Réponse d’erreur d’opération GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="9df22-155">GetNonIndexableItemDetails operation error response</span></span>

<span data-ttu-id="9df22-156">L’exemple suivant montre une réponse d’erreur à une demande d’opération **GetNonIndexableItemDetails** .</span><span class="sxs-lookup"><span data-stu-id="9df22-156">The following example shows an error response to a **GetNonIndexableItemDetails** operation request.</span></span> <span data-ttu-id="9df22-157">Il s’agit d’une réponse à une demande pour obtenir des détails des éléments pour les éléments qui ne peuvent pas être indexés à partir de plusieurs boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="9df22-157">This is a response to a request to get item details for items that cannot be indexed from more than one mailbox.</span></span> 
  
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
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetNonIndexableItemDetailsResponse ResponseClass="Error" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Multiple mailboxes is currently not supported, only single mailbox is supported.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetNonIndexableItemDetailsResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="9df22-158">La réponse d’erreur corps SOAP contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="9df22-158">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="9df22-159">GetNonIndexableItemDetailsResponse</span><span class="sxs-lookup"><span data-stu-id="9df22-159">GetNonIndexableItemDetailsResponse</span></span>](getnonindexableitemdetailsresponse.md)
    
- [<span data-ttu-id="9df22-160">MessageText</span><span class="sxs-lookup"><span data-stu-id="9df22-160">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="9df22-161">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="9df22-161">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="9df22-162">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="9df22-162">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="9df22-163">Pour les codes d’erreur générique à EWS, spécifiques à cette opération, consultez la rubrique [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="9df22-163">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="9df22-164">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9df22-164">See also</span></span>

- [<span data-ttu-id="9df22-165">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9df22-165">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="9df22-166">Opération GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="9df22-166">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="9df22-167">Opération SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="9df22-167">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)
    
- [<span data-ttu-id="9df22-168">Opération GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="9df22-168">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)
    
- [<span data-ttu-id="9df22-169">Opération SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="9df22-169">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)
    
- [<span data-ttu-id="9df22-170">Opération GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="9df22-170">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="9df22-171">Opération GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="9df22-171">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

