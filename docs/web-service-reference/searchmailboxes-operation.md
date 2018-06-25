---
title: Opération SearchMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8a67c1d8-d021-4e68-aa62-35f7d9c2edc7
description: Opération de recherche plus d’informations sur la SearchMailboxes EWS.
ms.openlocfilehash: 141ea466a24f3cb400a8e0b63e2162c1eae5d7f8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829296"
---
# <a name="searchmailboxes-operation"></a><span data-ttu-id="21ab4-103">Opération SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="21ab4-103">SearchMailboxes operation</span></span>

<span data-ttu-id="21ab4-104">Trouvez des informations sur l’opération EWS **SearchMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="21ab4-104">Find information about the **SearchMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="21ab4-105">L’opération **SearchMailboxes** recherche des boîtes aux lettres des occurrences des termes dans les éléments de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="21ab4-105">The **SearchMailboxes** operation searches mailboxes for occurrences of terms in mailbox items.</span></span> 
  
<span data-ttu-id="21ab4-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="21ab4-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-searchmailboxes-operation"></a><span data-ttu-id="21ab4-107">Utilisation de l’opération SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="21ab4-107">Using the SearchMailboxes operation</span></span>

<span data-ttu-id="21ab4-108">L’opération **SearchMailboxes** permettre utiliser le nombre de requêtes simultanées recherche pour effectuer une recherche de découverte sur plusieurs boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="21ab4-108">The **SearchMailboxes** operation can use many simultaneous search queries to perform discovery search on multiple mailboxes.</span></span> <span data-ttu-id="21ab4-109">Les résultats peuvent être soit des informations statistiques sur le nombre de termes de recherche se produisent, ou un aperçu des éléments qui contiennent les termes de recherche.</span><span class="sxs-lookup"><span data-stu-id="21ab4-109">The results can be either statistical information about the number of times search terms occur, or a preview of the items that contain the search terms.</span></span> 
  
### <a name="searchmailboxes-operation-soap-headers"></a><span data-ttu-id="21ab4-110">En-têtes SOAP SearchMailboxes opération</span><span class="sxs-lookup"><span data-stu-id="21ab4-110">SearchMailboxes operation SOAP headers</span></span>

<span data-ttu-id="21ab4-111">L’opération **SearchMailboxes** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="21ab4-111">The **SearchMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="21ab4-112">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="21ab4-112">**Header name**</span></span>|<span data-ttu-id="21ab4-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="21ab4-113">**Element**</span></span>|<span data-ttu-id="21ab4-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="21ab4-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="21ab4-115">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="21ab4-115">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="21ab4-116">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="21ab4-116">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="21ab4-117">Identifie les rôles de serveur qui sont nécessaires pour l’appelant effectuer la demande.</span><span class="sxs-lookup"><span data-stu-id="21ab4-117">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="21ab4-118">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="21ab4-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="21ab4-119">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="21ab4-119">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="21ab4-120">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="21ab4-120">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="21ab4-121">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="21ab4-121">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="21ab4-122">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="21ab4-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="21ab4-123">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="21ab4-123">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="21ab4-124">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="21ab4-124">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="21ab4-125">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="21ab4-125">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="21ab4-126">Cet en-tête est applicable à une réponse.</span><span class="sxs-lookup"><span data-stu-id="21ab4-126">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="searchmailboxes-operation-request-example-search-mailboxes-for-number-of-search-term-hits"></a><span data-ttu-id="21ab4-127">Exemple de requête d’opération SearchMailboxes : boîtes aux lettres pour le nombre de résultats de la recherche de termes de recherche</span><span class="sxs-lookup"><span data-stu-id="21ab4-127">SearchMailboxes operation request example: Search mailboxes for number of search term hits</span></span>

<span data-ttu-id="21ab4-128">Une demande d’opération **SearchMailboxes** l’exemple suivant montre comment utiliser deux requêtes différentes pour rechercher les trois boîtes aux lettres pour des informations statistiques sur le nombre de fois un terme apparaît dans chaque boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="21ab4-128">The following example of a **SearchMailboxes** operation request shows how to use two different queries to search three different mailboxes for statistical information about how many times a term appears in each mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="21ab4-129">Dans cet exemple, l’élément [Query](query.md) est intentionaly vide.</span><span class="sxs-lookup"><span data-stu-id="21ab4-129">In this example, the [Query](query.md) element is intentionaly left blank.</span></span> <span data-ttu-id="21ab4-130">Indique comment une demande réussie peut contenir des conditions d’erreur dans une base de recherche de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="21ab4-130">This shows how a successful request can contain error conditions on a per mailbox search basis.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="21ab4-131">La demande SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="21ab4-131">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="21ab4-132">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="21ab4-132">SearchMailboxes</span></span>](searchmailboxes.md)
    
- [<span data-ttu-id="21ab4-133">SearchQueries</span><span class="sxs-lookup"><span data-stu-id="21ab4-133">SearchQueries</span></span>](searchqueries.md)
    
- [<span data-ttu-id="21ab4-134">MailboxQuery</span><span class="sxs-lookup"><span data-stu-id="21ab4-134">MailboxQuery</span></span>](mailboxquery.md)
    
- [<span data-ttu-id="21ab4-135">Query</span><span class="sxs-lookup"><span data-stu-id="21ab4-135">Query</span></span>](query.md)
    
- [<span data-ttu-id="21ab4-136">MailboxSearchScopes</span><span class="sxs-lookup"><span data-stu-id="21ab4-136">MailboxSearchScopes</span></span>](mailboxsearchscopes.md)
    
- [<span data-ttu-id="21ab4-137">MailboxSearchScope</span><span class="sxs-lookup"><span data-stu-id="21ab4-137">MailboxSearchScope</span></span>](mailboxsearchscope.md)
    
- [<span data-ttu-id="21ab4-138">Boîte aux lettres (chaîne)</span><span class="sxs-lookup"><span data-stu-id="21ab4-138">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="21ab4-139">SearchScope</span><span class="sxs-lookup"><span data-stu-id="21ab4-139">SearchScope</span></span>](searchscope.md)
    
- [<span data-ttu-id="21ab4-140">ResultType</span><span class="sxs-lookup"><span data-stu-id="21ab4-140">ResultType</span></span>](resulttype.md)
    
## <a name="successful-searchmailboxes-operation-response"></a><span data-ttu-id="21ab4-141">Réponse d’opération SearchMailboxes réussie</span><span class="sxs-lookup"><span data-stu-id="21ab4-141">Successful SearchMailboxes operation response</span></span>

<span data-ttu-id="21ab4-142">L’exemple suivant montre une réponse positive à une demande d’opération **SearchMailboxes** pour obtenir des informations statistiques sur le nombre de termes de recherche figurent dans les boîtes aux lettres cible.</span><span class="sxs-lookup"><span data-stu-id="21ab4-142">The following example shows a successful response to a **SearchMailboxes** operation request to get statistical information about the number of times search terms are found in the target mailboxes.</span></span> <span data-ttu-id="21ab4-143">La dernière requête contient un élément de **requête** vide, ce qui indique une recherche de boîte aux lettres ayant échoué.</span><span class="sxs-lookup"><span data-stu-id="21ab4-143">The last query contains an empty **Query** element, which shows a failed mailbox search.</span></span> 
  
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
      <m:SearchMailboxesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="21ab4-144">La réponse SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="21ab4-144">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="21ab4-145">SearchMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="21ab4-145">SearchMailboxesResponse</span></span>](searchmailboxesresponse.md)
    
- [<span data-ttu-id="21ab4-146">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="21ab4-146">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="21ab4-147">SearchMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="21ab4-147">SearchMailboxesResponseMessage</span></span>](searchmailboxesresponsemessage.md)
    
- [<span data-ttu-id="21ab4-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="21ab4-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="21ab4-149">SearchMailboxesResult</span><span class="sxs-lookup"><span data-stu-id="21ab4-149">SearchMailboxesResult</span></span>](searchmailboxesresult.md)
    
- [<span data-ttu-id="21ab4-150">SearchQueries</span><span class="sxs-lookup"><span data-stu-id="21ab4-150">SearchQueries</span></span>](searchqueries.md)
    
- [<span data-ttu-id="21ab4-151">MailboxQuery</span><span class="sxs-lookup"><span data-stu-id="21ab4-151">MailboxQuery</span></span>](mailboxquery.md)
    
- [<span data-ttu-id="21ab4-152">Query</span><span class="sxs-lookup"><span data-stu-id="21ab4-152">Query</span></span>](query.md)
    
- [<span data-ttu-id="21ab4-153">MailboxSearchScopes</span><span class="sxs-lookup"><span data-stu-id="21ab4-153">MailboxSearchScopes</span></span>](mailboxsearchscopes.md)
    
- [<span data-ttu-id="21ab4-154">MailboxSearchScope</span><span class="sxs-lookup"><span data-stu-id="21ab4-154">MailboxSearchScope</span></span>](mailboxsearchscope.md)
    
- [<span data-ttu-id="21ab4-155">Boîte aux lettres (chaîne)</span><span class="sxs-lookup"><span data-stu-id="21ab4-155">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="21ab4-156">SearchScope</span><span class="sxs-lookup"><span data-stu-id="21ab4-156">SearchScope</span></span>](searchscope.md)
    
- [<span data-ttu-id="21ab4-157">ResultType</span><span class="sxs-lookup"><span data-stu-id="21ab4-157">ResultType</span></span>](resulttype.md)
    
- [<span data-ttu-id="21ab4-158">ItemCount</span><span class="sxs-lookup"><span data-stu-id="21ab4-158">ItemCount</span></span>](itemcount.md)
    
- [<span data-ttu-id="21ab4-159">Taille (long)</span><span class="sxs-lookup"><span data-stu-id="21ab4-159">Size (long)</span></span>](size-long.md)
    
- [<span data-ttu-id="21ab4-160">PageItemCount</span><span class="sxs-lookup"><span data-stu-id="21ab4-160">PageItemCount</span></span>](pageitemcount.md)
    
- [<span data-ttu-id="21ab4-161">KeywordStats</span><span class="sxs-lookup"><span data-stu-id="21ab4-161">KeywordStats</span></span>](keywordstats.md)
    
- [<span data-ttu-id="21ab4-162">KeywordStat</span><span class="sxs-lookup"><span data-stu-id="21ab4-162">KeywordStat</span></span>](keywordstat.md)
    
- [<span data-ttu-id="21ab4-163">Mot clé</span><span class="sxs-lookup"><span data-stu-id="21ab4-163">Keyword</span></span>](keyword.md)
    
- [<span data-ttu-id="21ab4-164">ItemHits</span><span class="sxs-lookup"><span data-stu-id="21ab4-164">ItemHits</span></span>](itemhits.md)
    
- [<span data-ttu-id="21ab4-165">FailedMailboxes</span><span class="sxs-lookup"><span data-stu-id="21ab4-165">FailedMailboxes</span></span>](failedmailboxes.md)
    
- [<span data-ttu-id="21ab4-166">FailedMailbox</span><span class="sxs-lookup"><span data-stu-id="21ab4-166">FailedMailbox</span></span>](failedmailbox.md)
    
- [<span data-ttu-id="21ab4-167">Boîte aux lettres (chaîne)</span><span class="sxs-lookup"><span data-stu-id="21ab4-167">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="21ab4-168">ErrorCode (int)</span><span class="sxs-lookup"><span data-stu-id="21ab4-168">ErrorCode (int)</span></span>](errorcode-int.md)
    
- [<span data-ttu-id="21ab4-169">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="21ab4-169">ErrorMessage</span></span>](errormessage.md)
    
- [<span data-ttu-id="21ab4-170">IsArchive</span><span class="sxs-lookup"><span data-stu-id="21ab4-170">IsArchive</span></span>](isarchive.md)
    
## <a name="searchmailboxes-operation-error-response"></a><span data-ttu-id="21ab4-171">Réponse d’erreur d’opération SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="21ab4-171">SearchMailboxes operation error response</span></span>

<span data-ttu-id="21ab4-172">L’exemple suivant montre une réponse d’erreur à une demande d’opération **SearchMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="21ab4-172">The following example shows an error response to a **SearchMailboxes** operation request.</span></span> <span data-ttu-id="21ab4-173">Il s’agit d’une réponse à une demande de recherche dans une boîte aux lettres lors de l’identificateur de la boîte aux lettres est incorrect.</span><span class="sxs-lookup"><span data-stu-id="21ab4-173">This is a response to a request to search a mailbox when the mailbox identifier is incorrect.</span></span> 
  
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
      <m:SearchMailboxesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="21ab4-174">La réponse d’erreur corps SOAP contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="21ab4-174">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="21ab4-175">SearchMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="21ab4-175">SearchMailboxesResponse</span></span>](searchmailboxesresponse.md)
    
- [<span data-ttu-id="21ab4-176">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="21ab4-176">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="21ab4-177">SearchMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="21ab4-177">SearchMailboxesResponseMessage</span></span>](searchmailboxesresponsemessage.md)
    
- [<span data-ttu-id="21ab4-178">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="21ab4-178">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="21ab4-179">SearchMailboxesResult</span><span class="sxs-lookup"><span data-stu-id="21ab4-179">SearchMailboxesResult</span></span>](searchmailboxesresult.md)
    
- [<span data-ttu-id="21ab4-180">SearchQueries</span><span class="sxs-lookup"><span data-stu-id="21ab4-180">SearchQueries</span></span>](searchqueries.md)
    
- [<span data-ttu-id="21ab4-181">MailboxQuery</span><span class="sxs-lookup"><span data-stu-id="21ab4-181">MailboxQuery</span></span>](mailboxquery.md)
    
- [<span data-ttu-id="21ab4-182">Query</span><span class="sxs-lookup"><span data-stu-id="21ab4-182">Query</span></span>](query.md)
    
- [<span data-ttu-id="21ab4-183">MailboxSearchScopes</span><span class="sxs-lookup"><span data-stu-id="21ab4-183">MailboxSearchScopes</span></span>](mailboxsearchscopes.md)
    
- [<span data-ttu-id="21ab4-184">MailboxSearchScope</span><span class="sxs-lookup"><span data-stu-id="21ab4-184">MailboxSearchScope</span></span>](mailboxsearchscope.md)
    
- [<span data-ttu-id="21ab4-185">Boîte aux lettres (chaîne)</span><span class="sxs-lookup"><span data-stu-id="21ab4-185">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="21ab4-186">SearchScope</span><span class="sxs-lookup"><span data-stu-id="21ab4-186">SearchScope</span></span>](searchscope.md)
    
- [<span data-ttu-id="21ab4-187">ResultType</span><span class="sxs-lookup"><span data-stu-id="21ab4-187">ResultType</span></span>](resulttype.md)
    
- [<span data-ttu-id="21ab4-188">ItemCount</span><span class="sxs-lookup"><span data-stu-id="21ab4-188">ItemCount</span></span>](itemcount.md)
    
- [<span data-ttu-id="21ab4-189">Taille (long)</span><span class="sxs-lookup"><span data-stu-id="21ab4-189">Size (long)</span></span>](size-long.md)
    
- [<span data-ttu-id="21ab4-190">PageItemCount</span><span class="sxs-lookup"><span data-stu-id="21ab4-190">PageItemCount</span></span>](pageitemcount.md)
    
- [<span data-ttu-id="21ab4-191">PageItemSize</span><span class="sxs-lookup"><span data-stu-id="21ab4-191">PageItemSize</span></span>](pageitemsize.md)
    
- [<span data-ttu-id="21ab4-192">FailedMailboxes</span><span class="sxs-lookup"><span data-stu-id="21ab4-192">FailedMailboxes</span></span>](failedmailboxes.md)
    
- [<span data-ttu-id="21ab4-193">FailedMailbox</span><span class="sxs-lookup"><span data-stu-id="21ab4-193">FailedMailbox</span></span>](failedmailbox.md)
    
- [<span data-ttu-id="21ab4-194">Boîte aux lettres (chaîne)</span><span class="sxs-lookup"><span data-stu-id="21ab4-194">Mailbox (string)</span></span>](mailbox-string.md)
    
- [<span data-ttu-id="21ab4-195">ErrorCode (int)</span><span class="sxs-lookup"><span data-stu-id="21ab4-195">ErrorCode (int)</span></span>](errorcode-int.md)
    
- [<span data-ttu-id="21ab4-196">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="21ab4-196">ErrorMessage</span></span>](errormessage.md)
    
- [<span data-ttu-id="21ab4-197">IsArchive</span><span class="sxs-lookup"><span data-stu-id="21ab4-197">IsArchive</span></span>](isarchive.md)
    
<span data-ttu-id="21ab4-198">Pour les codes d’erreur générique à EWS, spécifiques à cette opération, consultez la rubrique [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="21ab4-198">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="21ab4-199">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="21ab4-199">See also</span></span>

- [<span data-ttu-id="21ab4-200">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="21ab4-200">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="21ab4-201">Opération GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="21ab4-201">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md)
    
- [<span data-ttu-id="21ab4-202">Opération SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="21ab4-202">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)
    
- [<span data-ttu-id="21ab4-203">Opération GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="21ab4-203">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)
    
- [<span data-ttu-id="21ab4-204">Opération GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="21ab4-204">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="21ab4-205">Opération GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="21ab4-205">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    
- [<span data-ttu-id="21ab4-206">Opération GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="21ab4-206">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

