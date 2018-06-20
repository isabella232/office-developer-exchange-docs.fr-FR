---
title: Opération AddEntityFeedback
manager: luken
ms.date: 4/18/2016
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 00e40197-5794-4268-b937-bd65aa044890
description: L’opération AddEntityFeedback renvoie des informations d’erreur correspondant à des problèmes côté serveur.
ms.openlocfilehash: b695806f543827d78aea139ffcbd7e4af58b9fef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755169"
---
# <a name="addentityfeedback-operation"></a><span data-ttu-id="ccdad-103">Opération AddEntityFeedback</span><span class="sxs-lookup"><span data-stu-id="ccdad-103">AddEntityFeedback operation</span></span>

<span data-ttu-id="ccdad-104">L’opération **AddEntityFeedback** renvoie des informations d’erreur correspondant à des problèmes côté serveur.</span><span class="sxs-lookup"><span data-stu-id="ccdad-104">The **AddEntityFeedback** operation returns error information corresponding to server-side issues.</span></span> 
  
<span data-ttu-id="ccdad-105">Cette opération s’appuie sur le type d’événement en cours de journalisation.</span><span class="sxs-lookup"><span data-stu-id="ccdad-105">This operation relies on the type of event being logged.</span></span> <span data-ttu-id="ccdad-106">Un des événements plus importants est **EntityAdded**, qui correspond à une entité sélectionnée.</span><span class="sxs-lookup"><span data-stu-id="ccdad-106">One of the most important events is **EntityAdded**, which corresponds to an entity being selected.</span></span> <span data-ttu-id="ccdad-107">Cette opération est lot, afin qu’il peut être utilisé pour journaliser les lots d’entrées dans une demande unique.</span><span class="sxs-lookup"><span data-stu-id="ccdad-107">This operation is batch, so it can be used to log batches of entries in a single request.</span></span> 
  
## <a name="findpeople-request-examples"></a><span data-ttu-id="ccdad-108">Exemples de requêtes FindPeople</span><span class="sxs-lookup"><span data-stu-id="ccdad-108">FindPeople request examples</span></span>

<span data-ttu-id="ccdad-109">L’opération **AddEntityFeedback** offre un moyen pour les clients journaliser les détails de l’interaction avec les entités retournées par le service.</span><span class="sxs-lookup"><span data-stu-id="ccdad-109">The **AddEntityFeedback** operation provides a way for clients to log details of interaction with entities returned by the service.</span></span> <span data-ttu-id="ccdad-110">Cela peut servir comme un signal pour améliorer la pertinence dans les coulisses pour chaque client.</span><span class="sxs-lookup"><span data-stu-id="ccdad-110">This can be used as a signal to improve relevance behind the scenes for each client.</span></span> <span data-ttu-id="ccdad-111">Par exemple, les Clients peuvent utiliser cette opération pour fournir des commentaires sur les entités de personnes renvoyées à partir de **FindPeople**.</span><span class="sxs-lookup"><span data-stu-id="ccdad-111">E.g., Clients can use this operation to provide feedback on people entities returned from **FindPeople**.</span></span>
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
                             xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                             xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:AddEntityFeedback>
            <m:EntityFeedbackEntries>
                  <t:EntityFeedbackEntry>
                        <t:ClientEventTimeUTC> 2015-07-05T22:16:18+00:00</t:ClientEventTimeUTC>
                        <t:ClientEventTimeLocal> 2015-07-05T22:16:18+00:00</t:ClientEventTimeLocal>
                        <t:ClientSessionId>00000000-0000-0000-0000-000000000012</t:ClientSessionId>
                        <t:ClientVersion>15.01.0101.01</t:ClientVersion>
                        <t:ClientId>Web</t:ClientId>
                        <t:TransactionId>123456789</t:TransactionId>
                        <t:EventType>EntityAdded</t:EventType>
                        <t:TargetEntityList>["a","b","c"]</t:TargetEntityList>
                        <t:SourceOfEntityAdded></t:SourceOfEntityAdded>
                        <t:JSONPropertyBag></t:JSONPropertyBag>
                  </t:EntityFeedbackEntry>
                  <t:EntityFeedbackEntry>
                  …
                  </t:EntityFeedbackEntry>
            </m:EntityFeedbackEntries>
      </m:AddEntityFeedback>
   </soap:Body>
</soap:Envelope>

```

### <a name="the-request-soap-body-contents"></a><span data-ttu-id="ccdad-112">Le contenu du corps demande SOAP</span><span class="sxs-lookup"><span data-stu-id="ccdad-112">The request SOAP body contents</span></span>

<span data-ttu-id="ccdad-113">La demande soap contient un élément unique **EntityFeedbackEntries**.</span><span class="sxs-lookup"><span data-stu-id="ccdad-113">The soap request contains a single element **EntityFeedbackEntries**.</span></span> <span data-ttu-id="ccdad-114">À son tour, il contient un tableau d’objets **EntityFeedbackEntry** .</span><span class="sxs-lookup"><span data-stu-id="ccdad-114">This in turn contains an array of **EntityFeedbackEntry** objects.</span></span> <span data-ttu-id="ccdad-115">Chaque entrée du tableau peut contenir les éléments suivants.</span><span class="sxs-lookup"><span data-stu-id="ccdad-115">Each entry in the array can contain the following elements.</span></span> 
  
|<span data-ttu-id="ccdad-116">**Paramètres de la demande**</span><span class="sxs-lookup"><span data-stu-id="ccdad-116">**Request Parameters**</span></span>|<span data-ttu-id="ccdad-117">**Obligatoire**</span><span class="sxs-lookup"><span data-stu-id="ccdad-117">**Required**</span></span>|<span data-ttu-id="ccdad-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="ccdad-118">**Description**</span></span>|<span data-ttu-id="ccdad-119">**Type**</span><span class="sxs-lookup"><span data-stu-id="ccdad-119">**Type**</span></span>|
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="ccdad-120">**ClientEventTimeUtc**</span><span class="sxs-lookup"><span data-stu-id="ccdad-120">**ClientEventTimeUtc**</span></span> <br/> |<span data-ttu-id="ccdad-121">Oui</span><span class="sxs-lookup"><span data-stu-id="ccdad-121">Yes</span></span>  <br/> |<span data-ttu-id="ccdad-122">L’heure UTC l’événement s’est produite sur le côté client.</span><span class="sxs-lookup"><span data-stu-id="ccdad-122">The UTC time the event occurred on the client-side.</span></span>  <br/> |<span data-ttu-id="ccdad-123">Date/heure</span><span class="sxs-lookup"><span data-stu-id="ccdad-123">DateTime</span></span>  <br/> |
|<span data-ttu-id="ccdad-124">**ClientEventTimeLocal**</span><span class="sxs-lookup"><span data-stu-id="ccdad-124">**ClientEventTimeLocal**</span></span> <br/> |<span data-ttu-id="ccdad-125">Oui</span><span class="sxs-lookup"><span data-stu-id="ccdad-125">Yes</span></span>  <br/> |<span data-ttu-id="ccdad-126">L’heure locale de l’événement côté client.</span><span class="sxs-lookup"><span data-stu-id="ccdad-126">The local time the event occurred on the client side.</span></span>  <br/> |<span data-ttu-id="ccdad-127">Date/heure</span><span class="sxs-lookup"><span data-stu-id="ccdad-127">DateTime</span></span>  <br/> |
|<span data-ttu-id="ccdad-128">**ClientId**</span><span class="sxs-lookup"><span data-stu-id="ccdad-128">**ClientId**</span></span> <br/> |<span data-ttu-id="ccdad-129">Oui</span><span class="sxs-lookup"><span data-stu-id="ccdad-129">Yes</span></span>  <br/> |<span data-ttu-id="ccdad-130">Type de Client (par exemple, Outlook, OWA, etc.).</span><span class="sxs-lookup"><span data-stu-id="ccdad-130">Type of Client (E.g., Outlook, OWA, etc.).</span></span>  <br/> |<span data-ttu-id="ccdad-131">Énumération ClientIDType</span><span class="sxs-lookup"><span data-stu-id="ccdad-131">ClientIDType Enumeration</span></span>  <br/> |
|<span data-ttu-id="ccdad-132">**ClientSessionId**</span><span class="sxs-lookup"><span data-stu-id="ccdad-132">**ClientSessionId**</span></span> <br/> |<span data-ttu-id="ccdad-133">Oui</span><span class="sxs-lookup"><span data-stu-id="ccdad-133">Yes</span></span>  <br/> |<span data-ttu-id="ccdad-134">GUID qui identifie l’ID de session.</span><span class="sxs-lookup"><span data-stu-id="ccdad-134">GUID Identifying the session ID.</span></span> <span data-ttu-id="ccdad-135">Généré sur le client.</span><span class="sxs-lookup"><span data-stu-id="ccdad-135">Generated on the client.</span></span>  <br/> |<span data-ttu-id="ccdad-136">GUID</span><span class="sxs-lookup"><span data-stu-id="ccdad-136">GUID</span></span>  <br/> |
|<span data-ttu-id="ccdad-137">**ClientVersion**</span><span class="sxs-lookup"><span data-stu-id="ccdad-137">**ClientVersion**</span></span> <br/> |<span data-ttu-id="ccdad-138">Oui</span><span class="sxs-lookup"><span data-stu-id="ccdad-138">Yes</span></span>  <br/> |<span data-ttu-id="ccdad-139">Version du client (par exemple, 15.01.0101.000).</span><span class="sxs-lookup"><span data-stu-id="ccdad-139">Version of the client (E.g., 15.01.0101.000).</span></span>  <br/> |<span data-ttu-id="ccdad-140">Chaîne</span><span class="sxs-lookup"><span data-stu-id="ccdad-140">String</span></span>  <br/> |
|<span data-ttu-id="ccdad-141">**EntityAddSource**</span><span class="sxs-lookup"><span data-stu-id="ccdad-141">**EntityAddSource**</span></span> <br/> |<span data-ttu-id="ccdad-142">Non</span><span class="sxs-lookup"><span data-stu-id="ccdad-142">No</span></span>  <br/> |<span data-ttu-id="ccdad-143">Source de EntityAded (par exemple, EntityRelevanceAPI, types, collés).</span><span class="sxs-lookup"><span data-stu-id="ccdad-143">Source for EntityAded (E.g., EntityRelevanceAPI, types, pasted).</span></span>  <br/> |<span data-ttu-id="ccdad-144">Énumération EntityAddSource</span><span class="sxs-lookup"><span data-stu-id="ccdad-144">EntityAddSource Enumeration</span></span>  <br/> |
|<span data-ttu-id="ccdad-145">**EntrySequenceNumber**</span><span class="sxs-lookup"><span data-stu-id="ccdad-145">**EntrySequenceNumber**</span></span> <br/> |<span data-ttu-id="ccdad-146">Oui</span><span class="sxs-lookup"><span data-stu-id="ccdad-146">Yes</span></span>  <br/> |<span data-ttu-id="ccdad-147">Un entier incrémenté par session client.</span><span class="sxs-lookup"><span data-stu-id="ccdad-147">An incremental integer per client session.</span></span> <span data-ttu-id="ccdad-148">Utilisé pour détecter la perte de données.</span><span class="sxs-lookup"><span data-stu-id="ccdad-148">Used for detecting data loss.</span></span>  <br/> |<span data-ttu-id="ccdad-149">Int</span><span class="sxs-lookup"><span data-stu-id="ccdad-149">Int</span></span>  <br/> |
|<span data-ttu-id="ccdad-150">**EventType**</span><span class="sxs-lookup"><span data-stu-id="ccdad-150">**EventType**</span></span> <br/> |<span data-ttu-id="ccdad-151">Oui</span><span class="sxs-lookup"><span data-stu-id="ccdad-151">Yes</span></span>  <br/> |<span data-ttu-id="ccdad-152">Type d’événement (par exemple, ajout de l’entité, entité supprimée).</span><span class="sxs-lookup"><span data-stu-id="ccdad-152">Type of event (E.g., Entity Added, Entity Removed).</span></span>  <br/> |<span data-ttu-id="ccdad-153">Chaîne</span><span class="sxs-lookup"><span data-stu-id="ccdad-153">String</span></span>  <br/> |
|<span data-ttu-id="ccdad-154">**JSONPropertyBag**</span><span class="sxs-lookup"><span data-stu-id="ccdad-154">**JSONPropertyBag**</span></span> <br/> |<span data-ttu-id="ccdad-155">Non</span><span class="sxs-lookup"><span data-stu-id="ccdad-155">No</span></span>  <br/> |<span data-ttu-id="ccdad-156">Propriétés supplémentaires associées à l’événement (blob JSON de paires clé/valeur).</span><span class="sxs-lookup"><span data-stu-id="ccdad-156">Additional properties associated with the event (JSON blob of key/value pairs).</span></span>  <br/> |<span data-ttu-id="ccdad-157">Blob JSON</span><span class="sxs-lookup"><span data-stu-id="ccdad-157">JSON Blob</span></span>  <br/> |
|<span data-ttu-id="ccdad-158">**TargetEntityList**</span><span class="sxs-lookup"><span data-stu-id="ccdad-158">**TargetEntityList**</span></span> <br/> |<span data-ttu-id="ccdad-159">Non</span><span class="sxs-lookup"><span data-stu-id="ccdad-159">No</span></span>  <br/> |<span data-ttu-id="ccdad-160">Liste des entités associées à l’événement.</span><span class="sxs-lookup"><span data-stu-id="ccdad-160">List of entities associated with the event.</span></span>  <br/> |<span data-ttu-id="ccdad-161">Chaîne JSON</span><span class="sxs-lookup"><span data-stu-id="ccdad-161">JSON String</span></span>  <br/> |
|<span data-ttu-id="ccdad-162">**TransactionId**</span><span class="sxs-lookup"><span data-stu-id="ccdad-162">**TransactionId**</span></span> <br/> |<span data-ttu-id="ccdad-163">Non</span><span class="sxs-lookup"><span data-stu-id="ccdad-163">No</span></span>  <br/> |<span data-ttu-id="ccdad-164">ID (GUID) corrélation l’ID dans les journaux de requête.</span><span class="sxs-lookup"><span data-stu-id="ccdad-164">ID (GUID) correlating the ID in query logs.</span></span>  <br/> |<span data-ttu-id="ccdad-165">Chaîne</span><span class="sxs-lookup"><span data-stu-id="ccdad-165">String</span></span>  <br/> |
   
### <a name="successful-addentityfeedback-operation-response"></a><span data-ttu-id="ccdad-166">Réponse d’opération AddEntityFeedback réussie</span><span class="sxs-lookup"><span data-stu-id="ccdad-166">Successful AddEntityFeedback operation response</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" 
                                MinorVersion="1" 
                                MajorBuildNumber="228" 
                                MinorBuildNumber="0" 
                                Version="V2_49" 
                                xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                                xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                                xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <AddEntityFeedbackResponse ResponseClass="Success" 
                                                              xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                                              xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                                                              xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <ErrorCount>0</ErrorCount>
            <ErrorDetails />
        </AddEntityFeedbackResponse>
    </s:Body>
</s:Envelope> 

```

### <a name="the-response-soap-body-contains-the-following-elements"></a><span data-ttu-id="ccdad-167">La réponse SOAP body contient les éléments suivants</span><span class="sxs-lookup"><span data-stu-id="ccdad-167">The response SOAP body contains the following elements</span></span>

#### <a name="errors"></a><span data-ttu-id="ccdad-168">Erreurs</span><span class="sxs-lookup"><span data-stu-id="ccdad-168">Errors</span></span> 
  
<span data-ttu-id="ccdad-169">L’API peut se connecter à un lot d’entrées de la part de vos commentaires, nous tout ce que vous pouvez ouvrir une session.</span><span class="sxs-lookup"><span data-stu-id="ccdad-169">The API can log a batch of feedback entries, we log all that we can.</span></span> <span data-ttu-id="ccdad-170">Ce champ représente le nombre d’entrées d’erreur qui ne sont pas connectés.</span><span class="sxs-lookup"><span data-stu-id="ccdad-170">This field represents the number of error entries that were not logged.</span></span>
    
#### <a name="errordetails"></a><span data-ttu-id="ccdad-171">ErrorDetails</span><span class="sxs-lookup"><span data-stu-id="ccdad-171">ErrorDetails</span></span>
  
<span data-ttu-id="ccdad-172">Plus d’informations concernant les erreurs ci-dessus séparant en `;`.</span><span class="sxs-lookup"><span data-stu-id="ccdad-172">Details pertaining to the errors above separates by `;`.</span></span>
    
### <a name="currently-supported-values"></a><span data-ttu-id="ccdad-173">Valeurs prises en charge actuellement</span><span class="sxs-lookup"><span data-stu-id="ccdad-173">Currently supported values</span></span>

|<span data-ttu-id="ccdad-174">**Énumération ClientIdType**</span><span class="sxs-lookup"><span data-stu-id="ccdad-174">**ClientIdType Enumeration**</span></span>|
|:-----|
|<span data-ttu-id="ccdad-175">Ordinateur de bureau</span><span class="sxs-lookup"><span data-stu-id="ccdad-175">Desktop</span></span>  <br/> |
|<span data-ttu-id="ccdad-176">Exchange</span><span class="sxs-lookup"><span data-stu-id="ccdad-176">Exchange</span></span>  <br/> |
|<span data-ttu-id="ccdad-177">IMAP4</span><span class="sxs-lookup"><span data-stu-id="ccdad-177">IMAP4</span></span>  <br/> |
|<span data-ttu-id="ccdad-178">Lync</span><span class="sxs-lookup"><span data-stu-id="ccdad-178">Lync</span></span>  <br/> |
|<span data-ttu-id="ccdad-179">Messagerie</span><span class="sxs-lookup"><span data-stu-id="ccdad-179">MacMail</span></span>  <br/> |
|<span data-ttu-id="ccdad-180">MacOutlook</span><span class="sxs-lookup"><span data-stu-id="ccdad-180">MacOutlook</span></span>  <br/> |
|<span data-ttu-id="ccdad-181">Mobile</span><span class="sxs-lookup"><span data-stu-id="ccdad-181">Mobile</span></span>  <br/> |
|<span data-ttu-id="ccdad-182">Other</span><span class="sxs-lookup"><span data-stu-id="ccdad-182">Other</span></span>  <br/> |
|<span data-ttu-id="ccdad-183">Outlook</span><span class="sxs-lookup"><span data-stu-id="ccdad-183">Outlook</span></span>  <br/> |
|<span data-ttu-id="ccdad-184">OutlookService</span><span class="sxs-lookup"><span data-stu-id="ccdad-184">OutlookService</span></span>  <br/> |
|<span data-ttu-id="ccdad-185">POP3</span><span class="sxs-lookup"><span data-stu-id="ccdad-185">POP3</span></span>  <br/> |
|<span data-ttu-id="ccdad-186">Tablette</span><span class="sxs-lookup"><span data-stu-id="ccdad-186">Tablet</span></span>  <br/> |
|<span data-ttu-id="ccdad-187">Web</span><span class="sxs-lookup"><span data-stu-id="ccdad-187">Web</span></span>  <br/> |
   
|<span data-ttu-id="ccdad-188">**Énumération EntityAddSource**</span><span class="sxs-lookup"><span data-stu-id="ccdad-188">**EntityAddSource Enumeration**</span></span>|
|:-----|
|<span data-ttu-id="ccdad-189">ActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="ccdad-189">ActiveDirectory</span></span>  <br/> |
|<span data-ttu-id="ccdad-190">EntityRelevanceApi</span><span class="sxs-lookup"><span data-stu-id="ccdad-190">EntityRelevanceApi</span></span>  <br/> |
|<span data-ttu-id="ccdad-191">EntityRelevanceApiCache</span><span class="sxs-lookup"><span data-stu-id="ccdad-191">EntityRelevanceApiCache</span></span>  <br/> |
|<span data-ttu-id="ccdad-192">ExplicitTyping</span><span class="sxs-lookup"><span data-stu-id="ccdad-192">ExplicitTyping</span></span>  <br/> |
|<span data-ttu-id="ccdad-193">LocalCache</span><span class="sxs-lookup"><span data-stu-id="ccdad-193">LocalCache</span></span>  <br/> |
|<span data-ttu-id="ccdad-194">LocalCacheAndEntityRelevanceAPI</span><span class="sxs-lookup"><span data-stu-id="ccdad-194">LocalCacheAndEntityRelevanceAPI</span></span>  <br/> |
|<span data-ttu-id="ccdad-195">Aucun</span><span class="sxs-lookup"><span data-stu-id="ccdad-195">None</span></span>  <br/> |
|<span data-ttu-id="ccdad-196">Other</span><span class="sxs-lookup"><span data-stu-id="ccdad-196">Other</span></span>  <br/> |
|<span data-ttu-id="ccdad-197">Coller</span><span class="sxs-lookup"><span data-stu-id="ccdad-197">Paste</span></span>  <br/> |
   
### <a name="addentityfeedback-operation-error-response"></a><span data-ttu-id="ccdad-198">Réponse d’erreur d’opération AddEntityFeedback</span><span class="sxs-lookup"><span data-stu-id="ccdad-198">AddEntityFeedback operation error response</span></span>

<span data-ttu-id="ccdad-199">Pour les codes d’erreur qui sont génériques pour EWS, voir [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="ccdad-199">For error codes that are generic to EWS, see [ResponseCode](responsecode.md).</span></span>
  
### <a name="example-of-addentityfeedback-in-conjunction-with-findpeople"></a><span data-ttu-id="ccdad-200">Exemple de AddEntityFeedback en association avec FindPeople</span><span class="sxs-lookup"><span data-stu-id="ccdad-200">Example of AddEntityFeedback in conjunction with FindPeople</span></span>

#### <a name="findpeople-request"></a><span data-ttu-id="ccdad-201">Demande FindPeople</span><span class="sxs-lookup"><span data-stu-id="ccdad-201">FindPeople request</span></span>
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
<soap:Body >
    <m:FindPeople>
      <m:IndexedPageItemView BasePoint="Beginning" MaxEntriesReturned="100" Offset="0"/>
      <m:QueryString>user1</m:QueryString>
      <m:SearchPeopleSuggestionIndex>true</m:SearchPeopleSuggestionIndex>
    </m:FindPeople>
  </soap:Body>
</soap:Envelope>    
    
```

#### <a name="findpeople-response"></a><span data-ttu-id="ccdad-202">Réponse FindPeople</span><span class="sxs-lookup"><span data-stu-id="ccdad-202">FindPeople response</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" MinorVersion="1" MajorBuildNumber="302" MinorBuildNumber="0" Version="V2_68" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <FindPeopleResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <People>
                <Persona xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                    <PersonaId Id="AAUQAFjZ4UxX8SZCqSPFsmh0cSo=" />
                    <PersonaType>Person</PersonaType>
                    <CreationTime>2015-10-02T23:25:42</CreationTime>
                    <DisplayName>user2</DisplayName>
…
                  </Persona>
            </People>
            <TotalNumberOfPeopleInView>0</TotalNumberOfPeopleInView>
            <FirstMatchingRowIndex>0</FirstMatchingRowIndex>
            <FirstLoadedRowIndex>0</FirstLoadedRowIndex>
            <TransactionId>b56ad16e-5d5a-4574-90f8-b8dd57382be6</TransactionId>
        </FindPeopleResponse>
    </s:Body>
</s:Envelope>

```

#### <a name="addentityfeedback-request"></a><span data-ttu-id="ccdad-203">Demande AddEntityFeedback</span><span class="sxs-lookup"><span data-stu-id="ccdad-203">AddEntityFeedback request</span></span>

```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:AddEntityFeedback>
<m:EntityFeedbackEntries>
<t:EntityFeedbackEntry>
         <t:ClientEventTimeUtc>2015-07-05T22:16:18+00:00</t:ClientEventTimeUtc>
         <t:ClientEventTimeLocal>2015-07-05T22:16:18+00:00</t:ClientEventTimeLocal>
         <t:ClientSessionId>00000000-0000-0000-0000-000000000012</t:ClientSessionId>
         <t:ClientVersion>15.01.0101.01</t:ClientVersion>
         <t:ClientId>Web</t:ClientId>
         <t:TransactionId>b56ad16e-5d5a-4574-90f8-b8dd57382be6</t:TransactionId>
         <t:EventType>EntityAdded</t:EventType>
         <t:TargetEntityList>["user1@ms7.com"]</t:TargetEntityList>
         <t:SourceOfEntityAdded>EntityRelevanceApi</t:SourceOfEntityAdded>
         <t:JSONPropertyBag></t:JSONPropertyBag>
</t:EntityFeedbackEntry>
</m:EntityFeedbackEntries>
      </m:AddEntityFeedback>
   </soap:Body>
</soap:Envelope>

```

> [!NOTE]
> <span data-ttu-id="ccdad-204">ID ID de transaction de réponse en tant que la transaction de demande AddEntityFeedback à l’aide de FindPeople d'.</span><span class="sxs-lookup"><span data-stu-id="ccdad-204">Using FindPeople response transaction ID as the AddEntityFeedback request transaction ID.</span></span> 
  
#### <a name="addentityfeedback-response"></a><span data-ttu-id="ccdad-205">Réponse AddEntityFeedback</span><span class="sxs-lookup"><span data-stu-id="ccdad-205">AddEntityFeedback response</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" MinorVersion="1" MajorBuildNumber="302" MinorBuildNumber="0" Version="V2_68" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <AddEntityFeedbackResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <ErrorCount>0</ErrorCount>
            <ErrorDetails />
        </AddEntityFeedbackResponse>
    </s:Body>
</s:Envelope>

```


