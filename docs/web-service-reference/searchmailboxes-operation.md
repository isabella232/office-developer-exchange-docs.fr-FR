---
title: Opération SearchMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8a67c1d8-d021-4e68-aa62-35f7d9c2edc7
description: Trouvez des informations sur l’opération EWS SearchMailboxes.
ms.openlocfilehash: 9ec7e9dd4ef17f22f236e64ca1fdbeb65e6e56fe
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456763"
---
# <a name="searchmailboxes-operation"></a><span data-ttu-id="de0d4-103">Opération SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="de0d4-103">SearchMailboxes operation</span></span>

> [!NOTE]
> <span data-ttu-id="de0d4-104">Cette opération est déconseillée et n’est plus prise en charge par Microsoft.</span><span class="sxs-lookup"><span data-stu-id="de0d4-104">This operation is deprecated, and no longer supported by Microsoft.</span></span>  <span data-ttu-id="de0d4-105">Pour remplacer, utilisez l’opération [FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="de0d4-105">As a replacement, please use the [FindItem](finditem-operation.md) operation.</span></span>

<span data-ttu-id="de0d4-106">Trouvez des informations sur l’opération EWS **SearchMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="de0d4-106">Find information about the **SearchMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="de0d4-107">L’opération **SearchMailboxes** recherche des occurrences de termes dans des éléments de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="de0d4-107">The **SearchMailboxes** operation searches mailboxes for occurrences of terms in mailbox items.</span></span> 
  
<span data-ttu-id="de0d4-108">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="de0d4-108">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-searchmailboxes-operation"></a><span data-ttu-id="de0d4-109">Utilisation de l’opération SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="de0d4-109">Using the SearchMailboxes operation</span></span>

<span data-ttu-id="de0d4-110">L’opération **SearchMailboxes** peut utiliser plusieurs requêtes de recherche simultanées pour effectuer une recherche de découverte sur plusieurs boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="de0d4-110">The **SearchMailboxes** operation can use many simultaneous search queries to perform discovery search on multiple mailboxes.</span></span> <span data-ttu-id="de0d4-111">Les résultats peuvent être des informations statistiques sur le nombre de termes de recherche, ou un aperçu des éléments qui contiennent les termes de recherche.</span><span class="sxs-lookup"><span data-stu-id="de0d4-111">The results can be either statistical information about the number of times search terms occur, or a preview of the items that contain the search terms.</span></span> 
  
### <a name="searchmailboxes-operation-soap-headers"></a><span data-ttu-id="de0d4-112">En-têtes SOAP d’opération SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="de0d4-112">SearchMailboxes operation SOAP headers</span></span>

<span data-ttu-id="de0d4-113">L’opération **SearchMailboxes** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="de0d4-113">The **SearchMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="de0d4-114">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="de0d4-114">**Header name**</span></span>|<span data-ttu-id="de0d4-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="de0d4-115">**Element**</span></span>|<span data-ttu-id="de0d4-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="de0d4-116">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="de0d4-117">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="de0d4-117">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="de0d4-118">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="de0d4-118">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="de0d4-119">Identifie les rôles serveur nécessaires pour que l’appelant effectue la demande.</span><span class="sxs-lookup"><span data-stu-id="de0d4-119">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="de0d4-120">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="de0d4-120">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="de0d4-121">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="de0d4-121">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="de0d4-122">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="de0d4-122">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="de0d4-123">Identifie la version de schéma de la demande d’opération.</span><span class="sxs-lookup"><span data-stu-id="de0d4-123">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="de0d4-124">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="de0d4-124">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="de0d4-125">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="de0d4-125">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="de0d4-126">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="de0d4-126">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="de0d4-127">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="de0d4-127">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="de0d4-128">Cet en-tête s’applique à une réponse.</span><span class="sxs-lookup"><span data-stu-id="de0d4-128">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="searchmailboxes-operation-request-example-search-mailboxes-for-number-of-search-term-hits"></a><span data-ttu-id="de0d4-129">Exemple de requête d’opération SearchMailboxes : boîtes aux lettres de recherche pour le nombre d’accès aux termes de recherche</span><span class="sxs-lookup"><span data-stu-id="de0d4-129">SearchMailboxes operation request example: Search mailboxes for number of search term hits</span></span>

<span data-ttu-id="de0d4-130">L’exemple suivant de demande d’opération **SearchMailboxes** montre comment utiliser deux requêtes différentes pour effectuer une recherche dans trois boîtes aux lettres différentes pour obtenir des informations statistiques sur le nombre de fois qu’un terme est affiché dans chaque boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="de0d4-130">The following example of a **SearchMailboxes** operation request shows how to use two different queries to search three different mailboxes for statistical information about how many times a term appears in each mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="de0d4-131">Dans cet exemple, l’élément [query](query.md) est intentionnellement laissé vide.</span><span class="sxs-lookup"><span data-stu-id="de0d4-131">In this example, the [Query](query.md) element is intentionaly left blank.</span></span> <span data-ttu-id="de0d4-132">Cela indique comment une demande réussie peut contenir des conditions d’erreur en fonction de la recherche par boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="de0d4-132">This shows how a successful request can contain error conditions on a per mailbox search basis.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:SearchMailboxes>
         <m:SearchQueries>
            <t:MailboxQuery>
               <t:Query>Test Item</t:Query>
               <t:MailboxSearchScopes>
                  <t:MailboxSearchScope>
                     <t:Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=12311a742f0e47e392c8201a60d13ecf-Steve</t:Mailbox>
                     <t:SearchScope>All</t:SearchScope>
                  </t:MailboxSearchScope>
                  <t:MailboxSearchScope>
                     <t:Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=f00c9f70539844beb52341d8f40c572e-Antho</t:Mailbox>
                     <t:SearchScope>PrimaryOnly</t:SearchScope>
                  </t:MailboxSearchScope>
               </t:MailboxSearchScopes>
            </t:MailboxQuery>
            <t:MailboxQuery>
               <t:Query></t:Query>
               <t:MailboxSearchScopes>
                  <t:MailboxSearchScope>
                     <t:Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=accba4fd5ddf12214a0e82ce1645f4e-Danie</t:Mailbox>
                     <t:SearchScope>ArchiveOnly</t:SearchScope>
                  </t:MailboxSearchScope>
               </t:MailboxSearchScopes>
            </t:MailboxQuery>
         </m:SearchQueries>
         <m:ResultType>StatisticsOnly</m:ResultType>
      </m:SearchMailboxes>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="de0d4-133">Le corps SOAP de la demande contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="de0d4-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="de0d4-134">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="de0d4-134">SearchMailboxes</span></span>](searchmailboxes.md)
    
- [<span data-ttu-id="de0d4-135">SearchQueries</span><span class="sxs-lookup"><span data-stu-id="de0d4-135">SearchQueries</span></span>](searchqueries.md)
    
- [<span data-ttu-id="de0d4-136">MailboxQuery</span><span class="sxs-lookup"><span data-stu-id="de0d4-136">MailboxQuery</span></span>](mailboxquery.md)
    
- [<span data-ttu-id="de0d4-137">Query</span><span class="sxs-lookup"><span data-stu-id="de0d4-137">Query</span></span>](query.md)
    
- [<span data-ttu-id="de0d4-138">MailboxSearchScopes</span><span class="sxs-lookup"><span data-stu-id="de0d4-138">MailboxSearchScopes</span></span>](mailboxsearchscopes.md)
    
- [<span data-ttu-id="de0d4-139">MailboxSearchScope</span><span class="sxs-lookup"><span data-stu-id="de0d4-139">MailboxSearchScope</span></span>](mailboxsearchscope.md)
    
- [<span data-ttu-id="de0d4-140">Mailbox (String)</span><span class="sxs-lookup"><span data-stu-id="de0d4-140">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="de0d4-141">SearchScope</span><span class="sxs-lookup"><span data-stu-id="de0d4-141">SearchScope</span></span>](searchscope.md)
    
- [<span data-ttu-id="de0d4-142">ResultType</span><span class="sxs-lookup"><span data-stu-id="de0d4-142">ResultType</span></span>](resulttype.md)
    
## <a name="successful-searchmailboxes-operation-response"></a><span data-ttu-id="de0d4-143">Réponse de l’opération SearchMailboxes réussie</span><span class="sxs-lookup"><span data-stu-id="de0d4-143">Successful SearchMailboxes operation response</span></span>

<span data-ttu-id="de0d4-144">L’exemple suivant montre une réponse réussie à une demande d’opération **SearchMailboxes** afin d’obtenir des informations statistiques sur le nombre de termes de recherche trouvés dans les boîtes aux lettres cibles.</span><span class="sxs-lookup"><span data-stu-id="de0d4-144">The following example shows a successful response to a **SearchMailboxes** operation request to get statistical information about the number of times search terms are found in the target mailboxes.</span></span> <span data-ttu-id="de0d4-145">La dernière requête contient un élément de **requête** vide, qui affiche une recherche de boîte aux lettres ayant échoué.</span><span class="sxs-lookup"><span data-stu-id="de0d4-145">The last query contains an empty **Query** element, which shows a failed mailbox search.</span></span> 
  
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
      <m:SearchMailboxesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:SearchMailboxesResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:SearchMailboxesResult>
                  <t:SearchQueries>
                     <t:MailboxQuery>
                        <t:Query>Test Item</t:Query>
                        <t:MailboxSearchScopes>
                           <t:MailboxSearchScope>
                              <t:Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYPDLT)/cn=Recipients/cn=35181a94327e392c8201a60d13ecf-Steve</t:Mailbox>
                              <t:SearchScope>All</t:SearchScope>
                           </t:MailboxSearchScope>
                           <t:MailboxSearchScope>
                              <t:Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYPDLT)/cn=Recipients/cn=f00c9f789572-beb04001d8f40c572e-Antho</t:Mailbox>
                              <t:SearchScope>PrimaryOnly</t:SearchScope>
                           </t:MailboxSearchScope>
                        </t:MailboxSearchScopes>
                     </t:MailboxQuery>
                  </t:SearchQueries>
                  <t:ResultType>StatisticsOnly</t:ResultType>
                  <t:ItemCount>2</t:ItemCount>
                  <t:Size>20206</t:Size>
                  <t:PageItemCount>0</t:PageItemCount>
                  <t:PageItemSize>0</t:PageItemSize>
                  <t:KeywordStats>
                     <t:KeywordStat>
                        <t:Keyword>Test Item</t:Keyword>
                        <t:ItemHits>2</t:ItemHits>
                        <t:Size>20206</t:Size>
                     </t:KeywordStat>
                  </t:KeywordStats>
                  <t:FailedMailboxes>
                     <t:FailedMailbox>
                        <t:Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYPDLT)/cn=Recipients/cn=accba4as3df234234a0e82ce1645f4e-Danie</t:Mailbox>
                        <t:ErrorCode>0</t:ErrorCode>
                        <t:ErrorMessage>The search query can't be empty.</t:ErrorMessage>
                        <t:IsArchive>true</t:IsArchive>
                     </t:FailedMailbox>
                  </t:FailedMailboxes>
               </m:SearchMailboxesResult>
            </m:SearchMailboxesResponseMessage>
         </m:ResponseMessages>
      </m:SearchMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="de0d4-146">Le corps SOAP de réponse contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="de0d4-146">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="de0d4-147">SearchMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="de0d4-147">SearchMailboxesResponse</span></span>](searchmailboxesresponse.md)
    
- [<span data-ttu-id="de0d4-148">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="de0d4-148">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="de0d4-149">SearchMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="de0d4-149">SearchMailboxesResponseMessage</span></span>](searchmailboxesresponsemessage.md)
    
- [<span data-ttu-id="de0d4-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="de0d4-150">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="de0d4-151">SearchMailboxesResult</span><span class="sxs-lookup"><span data-stu-id="de0d4-151">SearchMailboxesResult</span></span>](searchmailboxesresult.md)
    
- [<span data-ttu-id="de0d4-152">SearchQueries</span><span class="sxs-lookup"><span data-stu-id="de0d4-152">SearchQueries</span></span>](searchqueries.md)
    
- [<span data-ttu-id="de0d4-153">MailboxQuery</span><span class="sxs-lookup"><span data-stu-id="de0d4-153">MailboxQuery</span></span>](mailboxquery.md)
    
- [<span data-ttu-id="de0d4-154">Query</span><span class="sxs-lookup"><span data-stu-id="de0d4-154">Query</span></span>](query.md)
    
- [<span data-ttu-id="de0d4-155">MailboxSearchScopes</span><span class="sxs-lookup"><span data-stu-id="de0d4-155">MailboxSearchScopes</span></span>](mailboxsearchscopes.md)
    
- [<span data-ttu-id="de0d4-156">MailboxSearchScope</span><span class="sxs-lookup"><span data-stu-id="de0d4-156">MailboxSearchScope</span></span>](mailboxsearchscope.md)
    
- [<span data-ttu-id="de0d4-157">Mailbox (String)</span><span class="sxs-lookup"><span data-stu-id="de0d4-157">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="de0d4-158">SearchScope</span><span class="sxs-lookup"><span data-stu-id="de0d4-158">SearchScope</span></span>](searchscope.md)
    
- [<span data-ttu-id="de0d4-159">ResultType</span><span class="sxs-lookup"><span data-stu-id="de0d4-159">ResultType</span></span>](resulttype.md)
    
- [<span data-ttu-id="de0d4-160">ItemCount</span><span class="sxs-lookup"><span data-stu-id="de0d4-160">ItemCount</span></span>](itemcount.md)
    
- [<span data-ttu-id="de0d4-161">Taille (long)</span><span class="sxs-lookup"><span data-stu-id="de0d4-161">Size (long)</span></span>](size-long.md)
    
- [<span data-ttu-id="de0d4-162">PageItemCount</span><span class="sxs-lookup"><span data-stu-id="de0d4-162">PageItemCount</span></span>](pageitemcount.md)
    
- [<span data-ttu-id="de0d4-163">KeywordStats</span><span class="sxs-lookup"><span data-stu-id="de0d4-163">KeywordStats</span></span>](keywordstats.md)
    
- [<span data-ttu-id="de0d4-164">KeywordStat</span><span class="sxs-lookup"><span data-stu-id="de0d4-164">KeywordStat</span></span>](keywordstat.md)
    
- [<span data-ttu-id="de0d4-165">Mot clé</span><span class="sxs-lookup"><span data-stu-id="de0d4-165">Keyword</span></span>](keyword.md)
    
- [<span data-ttu-id="de0d4-166">ItemHits</span><span class="sxs-lookup"><span data-stu-id="de0d4-166">ItemHits</span></span>](itemhits.md)
    
- [<span data-ttu-id="de0d4-167">FailedMailboxes</span><span class="sxs-lookup"><span data-stu-id="de0d4-167">FailedMailboxes</span></span>](failedmailboxes.md)
    
- [<span data-ttu-id="de0d4-168">FailedMailbox</span><span class="sxs-lookup"><span data-stu-id="de0d4-168">FailedMailbox</span></span>](failedmailbox.md)
    
- [<span data-ttu-id="de0d4-169">Mailbox (String)</span><span class="sxs-lookup"><span data-stu-id="de0d4-169">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="de0d4-170">ErrorCode (int)</span><span class="sxs-lookup"><span data-stu-id="de0d4-170">ErrorCode (int)</span></span>](errorcode-int.md)
    
- [<span data-ttu-id="de0d4-171">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="de0d4-171">ErrorMessage</span></span>](errormessage.md)
    
- [<span data-ttu-id="de0d4-172">IsArchive</span><span class="sxs-lookup"><span data-stu-id="de0d4-172">IsArchive</span></span>](isarchive.md)
    
## <a name="searchmailboxes-operation-error-response"></a><span data-ttu-id="de0d4-173">Réponse d’erreur d’opération SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="de0d4-173">SearchMailboxes operation error response</span></span>

<span data-ttu-id="de0d4-174">L’exemple suivant montre une réponse d’erreur à une demande d’opération **SearchMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="de0d4-174">The following example shows an error response to a **SearchMailboxes** operation request.</span></span> <span data-ttu-id="de0d4-175">Il s’agit d’une réponse à une demande de recherche dans une boîte aux lettres lorsque l’identificateur de la boîte aux lettres est incorrect.</span><span class="sxs-lookup"><span data-stu-id="de0d4-175">This is a response to a request to search a mailbox when the mailbox identifier is incorrect.</span></span> 
  
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
      <m:SearchMailboxesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:SearchMailboxesResponseMessage ResponseClass="Error">
               <m:MessageText>No mailbox is specified for search operation. If specified in the request, 
               then it could be due to permission issue.</m:MessageText>
               <m:ResponseCode>ErrorInvalidOperation</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
               <m:SearchMailboxesResult>
                  <t:SearchQueries>
                     <t:MailboxQuery>
                        <t:Query>subject:Test Item</t:Query>
                        <t:MailboxSearchScopes>
                           <t:MailboxSearchScope>
                              <t:Mailbox>sbrown@contoso.com</t:Mailbox>
                              <t:SearchScope>All</t:SearchScope>
                           </t:MailboxSearchScope>
                        </t:MailboxSearchScopes>
                     </t:MailboxQuery>
                  </t:SearchQueries>
                  <t:ResultType>StatisticsOnly</t:ResultType>
                  <t:ItemCount>0</t:ItemCount>
                  <t:Size>0</t:Size>
                  <t:PageItemCount>0</t:PageItemCount>
                  <t:PageItemSize>0</t:PageItemSize>
                  <t:FailedMailboxes>
                     <t:FailedMailbox>
                        <t:Mailbox>sbrown@contoso.com</t:Mailbox>
                        <t:ErrorCode>0</t:ErrorCode>
                        <t:ErrorMessage>No mailbox is specified for search operation. If specified in the request, 
                        then it could be due to permission issue.</t:ErrorMessage>
                        <t:IsArchive>false</t:IsArchive>
                     </t:FailedMailbox>
                  </t:FailedMailboxes>
               </m:SearchMailboxesResult>
            </m:SearchMailboxesResponseMessage>
         </m:ResponseMessages>
      </m:SearchMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="de0d4-176">Le corps SOAP de la réponse d’erreur contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="de0d4-176">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="de0d4-177">SearchMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="de0d4-177">SearchMailboxesResponse</span></span>](searchmailboxesresponse.md)
    
- [<span data-ttu-id="de0d4-178">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="de0d4-178">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="de0d4-179">SearchMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="de0d4-179">SearchMailboxesResponseMessage</span></span>](searchmailboxesresponsemessage.md)
    
- [<span data-ttu-id="de0d4-180">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="de0d4-180">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="de0d4-181">SearchMailboxesResult</span><span class="sxs-lookup"><span data-stu-id="de0d4-181">SearchMailboxesResult</span></span>](searchmailboxesresult.md)
    
- [<span data-ttu-id="de0d4-182">SearchQueries</span><span class="sxs-lookup"><span data-stu-id="de0d4-182">SearchQueries</span></span>](searchqueries.md)
    
- [<span data-ttu-id="de0d4-183">MailboxQuery</span><span class="sxs-lookup"><span data-stu-id="de0d4-183">MailboxQuery</span></span>](mailboxquery.md)
    
- [<span data-ttu-id="de0d4-184">Query</span><span class="sxs-lookup"><span data-stu-id="de0d4-184">Query</span></span>](query.md)
    
- [<span data-ttu-id="de0d4-185">MailboxSearchScopes</span><span class="sxs-lookup"><span data-stu-id="de0d4-185">MailboxSearchScopes</span></span>](mailboxsearchscopes.md)
    
- [<span data-ttu-id="de0d4-186">MailboxSearchScope</span><span class="sxs-lookup"><span data-stu-id="de0d4-186">MailboxSearchScope</span></span>](mailboxsearchscope.md)
    
- [<span data-ttu-id="de0d4-187">Mailbox (String)</span><span class="sxs-lookup"><span data-stu-id="de0d4-187">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="de0d4-188">SearchScope</span><span class="sxs-lookup"><span data-stu-id="de0d4-188">SearchScope</span></span>](searchscope.md)
    
- [<span data-ttu-id="de0d4-189">ResultType</span><span class="sxs-lookup"><span data-stu-id="de0d4-189">ResultType</span></span>](resulttype.md)
    
- [<span data-ttu-id="de0d4-190">ItemCount</span><span class="sxs-lookup"><span data-stu-id="de0d4-190">ItemCount</span></span>](itemcount.md)
    
- [<span data-ttu-id="de0d4-191">Taille (long)</span><span class="sxs-lookup"><span data-stu-id="de0d4-191">Size (long)</span></span>](size-long.md)
    
- [<span data-ttu-id="de0d4-192">PageItemCount</span><span class="sxs-lookup"><span data-stu-id="de0d4-192">PageItemCount</span></span>](pageitemcount.md)
    
- [<span data-ttu-id="de0d4-193">PageItemSize</span><span class="sxs-lookup"><span data-stu-id="de0d4-193">PageItemSize</span></span>](pageitemsize.md)
    
- [<span data-ttu-id="de0d4-194">FailedMailboxes</span><span class="sxs-lookup"><span data-stu-id="de0d4-194">FailedMailboxes</span></span>](failedmailboxes.md)
    
- [<span data-ttu-id="de0d4-195">FailedMailbox</span><span class="sxs-lookup"><span data-stu-id="de0d4-195">FailedMailbox</span></span>](failedmailbox.md)
    
- [<span data-ttu-id="de0d4-196">Mailbox (String)</span><span class="sxs-lookup"><span data-stu-id="de0d4-196">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="de0d4-197">ErrorCode (int)</span><span class="sxs-lookup"><span data-stu-id="de0d4-197">ErrorCode (int)</span></span>](errorcode-int.md)
    
- [<span data-ttu-id="de0d4-198">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="de0d4-198">ErrorMessage</span></span>](errormessage.md)
    
- [<span data-ttu-id="de0d4-199">IsArchive</span><span class="sxs-lookup"><span data-stu-id="de0d4-199">IsArchive</span></span>](isarchive.md)
    
<span data-ttu-id="de0d4-200">Pour les autres codes d’erreur qui sont génériques à EWS et spécifiques à cette opération, voir [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="de0d4-200">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="de0d4-201">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="de0d4-201">See also</span></span>

- [<span data-ttu-id="de0d4-202">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="de0d4-202">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="de0d4-203">Opération GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="de0d4-203">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="de0d4-204">Opération SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="de0d4-204">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)
    
- [<span data-ttu-id="de0d4-205">Opération GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="de0d4-205">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)
    
- [<span data-ttu-id="de0d4-206">Opération GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="de0d4-206">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="de0d4-207">Opération GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="de0d4-207">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    
- [<span data-ttu-id="de0d4-208">Opération GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="de0d4-208">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

