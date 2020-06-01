---
title: Opération GetNonIndexableItemStatistics
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ed077877-9d98-4434-b8b6-a4a905e7f7a6
description: Trouvez des informations sur l’opération EWS GetNonIndexableItemStatistics.
ms.openlocfilehash: c7d49f9e0d7b4191c7403cb4d1a20e70a96c3882
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44452817"
---
# <a name="getnonindexableitemstatistics-operation"></a><span data-ttu-id="79a87-103">Opération GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="79a87-103">GetNonIndexableItemStatistics operation</span></span>

<span data-ttu-id="79a87-104">Trouvez des informations sur l’opération EWS **GetNonIndexableItemStatistics** .</span><span class="sxs-lookup"><span data-stu-id="79a87-104">Find information about the **GetNonIndexableItemStatistics** EWS operation.</span></span> 
  
<span data-ttu-id="79a87-105">L’opération **GetNonIndexableItemStatistics** récupère le nombre d’éléments qui ne peuvent pas être indexés dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="79a87-105">The **GetNonIndexableItemStatistics** operation retrieves the count of items that cannot be indexed in a mailbox.</span></span> 
  
<span data-ttu-id="79a87-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="79a87-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getnonindexableitemstatistics-operation"></a><span data-ttu-id="79a87-107">Utilisation de l’opération GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="79a87-107">Using the GetNonIndexableItemStatistics operation</span></span>

<span data-ttu-id="79a87-108">L’opération **GetNonIndexableItemStatistics** compte les éléments de boîte aux lettres qui ne peuvent pas être indexés.</span><span class="sxs-lookup"><span data-stu-id="79a87-108">The **GetNonIndexableItemStatistics** operation counts mailbox items that cannot be indexed.</span></span> <span data-ttu-id="79a87-109">Les éléments qui ne peuvent pas être indexés ne sont pas recherchés lors d’une recherche de découverte.</span><span class="sxs-lookup"><span data-stu-id="79a87-109">Items that cannot be indexed are not searched during a discovery search.</span></span> 
  
### <a name="getnonindexableitemstatistics-operation-soap-headers"></a><span data-ttu-id="79a87-110">En-têtes SOAP d’opération GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="79a87-110">GetNonIndexableItemStatistics operation SOAP headers</span></span>

<span data-ttu-id="79a87-111">L’opération **GetNonIndexableItemStatistics** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="79a87-111">The **GetNonIndexableItemStatistics** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="79a87-112">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="79a87-112">**Header name**</span></span>|<span data-ttu-id="79a87-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="79a87-113">**Element**</span></span>|<span data-ttu-id="79a87-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="79a87-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="79a87-115">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="79a87-115">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="79a87-116">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="79a87-116">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="79a87-117">Identifie les rôles serveur nécessaires pour que l’appelant effectue la demande.</span><span class="sxs-lookup"><span data-stu-id="79a87-117">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="79a87-118">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="79a87-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="79a87-119">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="79a87-119">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="79a87-120">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="79a87-120">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="79a87-121">Identifie la version de schéma de la demande d’opération.</span><span class="sxs-lookup"><span data-stu-id="79a87-121">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="79a87-122">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="79a87-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="79a87-123">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="79a87-123">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="79a87-124">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="79a87-124">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="79a87-125">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="79a87-125">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="79a87-126">Cet en-tête s’applique à une réponse.</span><span class="sxs-lookup"><span data-stu-id="79a87-126">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getnonindexableitemstatistics-operation-request-example-get-the-count-of-items-that-cannot-be-indexed-in-a-mailbox"></a><span data-ttu-id="79a87-127">Exemple de requête d’opération GetNonIndexableItemStatistics : obtenir le nombre d’éléments ne pouvant pas être indexés dans une boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="79a87-127">GetNonIndexableItemStatistics operation request example: Get the count of items that cannot be indexed in a mailbox</span></span>

<span data-ttu-id="79a87-128">L’exemple suivant de demande d’opération **GetNonIndexableItemStatistics** indique comment demander le nombre d’éléments ne pouvant pas être indexés dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="79a87-128">The following example of a **GetNonIndexableItemStatistics** operation request shows how to request the count of items that cannot be indexed in a mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="79a87-129">Tous les noms de domaine hérités de cet exemple sont raccourcis pour conserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="79a87-129">All legacy domain names in this example have be shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetNonIndexableItemStatistics>
         <m:Mailboxes>
            <t:LegacyDN>/o=First Organization/ou=Exchange Administrative Group (FYDIDLT)/cn=Recipients/cn=3518cf-Steve</t:LegacyDN>
         </m:Mailboxes>
         <m:SearchArchiveOnly>false</m:SearchArchiveOnly>
      </m:GetNonIndexableItemStatistics>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="79a87-130">Le corps SOAP de la demande contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="79a87-130">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="79a87-131">GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="79a87-131">GetNonIndexableItemStatistics</span></span>](getnonindexableitemstatistics.md)
    
- [<span data-ttu-id="79a87-132">Boîtes aux lettres (NonEmptyArrayOfLegacyDNsType)</span><span class="sxs-lookup"><span data-stu-id="79a87-132">Mailboxes (NonEmptyArrayOfLegacyDNsType)</span></span>](mailboxes-nonemptyarrayoflegacydnstype.md)
    
- [<span data-ttu-id="79a87-133">LegacyDN</span><span class="sxs-lookup"><span data-stu-id="79a87-133">LegacyDN</span></span>](legacydn.md)
    
- [<span data-ttu-id="79a87-134">SearchArchiveOnly</span><span class="sxs-lookup"><span data-stu-id="79a87-134">SearchArchiveOnly</span></span>](searcharchiveonly.md)
    
## <a name="successful-getnonindexableitemstatistics-operation-response"></a><span data-ttu-id="79a87-135">Réponse de l’opération GetNonIndexableItemStatistics réussie</span><span class="sxs-lookup"><span data-stu-id="79a87-135">Successful GetNonIndexableItemStatistics operation response</span></span>

<span data-ttu-id="79a87-136">L’exemple suivant montre une réponse réussie à une demande d’opération **GetNonIndexableItemStatistics** pour obtenir le nombre d’éléments qui ne peuvent pas être indexés dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="79a87-136">The following example shows a successful response to a **GetNonIndexableItemStatistics** operation request to get the count of items that cannot be indexed in a mailbox.</span></span> 
  
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
      <GetNonIndexableItemStatisticsResponse ResponseClass="Success" 
                                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <NonIndexableItemStatistics>
            <NonIndexableItemStatistic xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYT)/cn=Recipients/cn=35181acf-Steve</Mailbox>
               <ItemCount>2</ItemCount>
            </NonIndexableItemStatistic>
         </NonIndexableItemStatistics>
      </GetNonIndexableItemStatisticsResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="79a87-137">Le corps SOAP de réponse contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="79a87-137">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="79a87-138">GetNonIndexableItemStatisticsResponse</span><span class="sxs-lookup"><span data-stu-id="79a87-138">GetNonIndexableItemStatisticsResponse</span></span>](getnonindexableitemstatisticsresponse.md)
    
- [<span data-ttu-id="79a87-139">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="79a87-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="79a87-140">NonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="79a87-140">NonIndexableItemStatistics</span></span>](nonindexableitemstatistics.md)
    
- [<span data-ttu-id="79a87-141">NonIndexableItemStatistic</span><span class="sxs-lookup"><span data-stu-id="79a87-141">NonIndexableItemStatistic</span></span>](nonindexableitemstatistic.md)
    
- [<span data-ttu-id="79a87-142">Mailbox (String)</span><span class="sxs-lookup"><span data-stu-id="79a87-142">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="79a87-143">ItemCount</span><span class="sxs-lookup"><span data-stu-id="79a87-143">ItemCount</span></span>](itemcount.md)
    
## <a name="getnonindexableitemstatistics-operation-error-response"></a><span data-ttu-id="79a87-144">Réponse d’erreur d’opération GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="79a87-144">GetNonIndexableItemStatistics operation error response</span></span>

<span data-ttu-id="79a87-145">L’exemple suivant montre une réponse d’erreur à une demande d’opération **GetNonIndexableItemStatistics** .</span><span class="sxs-lookup"><span data-stu-id="79a87-145">The following example shows an error response to a **GetNonIndexableItemStatistics** operation request.</span></span> <span data-ttu-id="79a87-146">Il s’agit d’une réponse à une demande pour obtenir le nombre d’éléments qui ne peuvent pas être indexés à partir de plusieurs boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="79a87-146">This is a response to a request to get the count of items that cannot be indexed from more than one mailbox.</span></span> 
  
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
      <GetNonIndexableItemStatisticsResponse ResponseClass="Error" 
                                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Multiple mailboxes is currently not supported, only single mailbox is supported.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetNonIndexableItemStatisticsResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="79a87-147">Le corps SOAP de la réponse d’erreur contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="79a87-147">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="79a87-148">GetNonIndexableItemStatisticsResponse</span><span class="sxs-lookup"><span data-stu-id="79a87-148">GetNonIndexableItemStatisticsResponse</span></span>](getnonindexableitemstatisticsresponse.md)
    
- [<span data-ttu-id="79a87-149">MessageText</span><span class="sxs-lookup"><span data-stu-id="79a87-149">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="79a87-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="79a87-150">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="79a87-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="79a87-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="79a87-152">Pour les autres codes d’erreur qui sont génériques à EWS et spécifiques à cette opération, voir [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="79a87-152">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="79a87-153">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="79a87-153">See also</span></span>

- [<span data-ttu-id="79a87-154">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="79a87-154">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="79a87-155">Opération GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="79a87-155">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="79a87-156">Opération SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="79a87-156">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)
    
- [<span data-ttu-id="79a87-157">Opération GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="79a87-157">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)
    
- [<span data-ttu-id="79a87-158">Opération SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="79a87-158">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)
    
- [<span data-ttu-id="79a87-159">Opération GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="79a87-159">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="79a87-160">Opération GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="79a87-160">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    

