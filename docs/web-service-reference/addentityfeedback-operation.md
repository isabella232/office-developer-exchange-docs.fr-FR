---
title: Opération AddEntityFeedback
manager: luken
ms.date: 4/18/2016
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 00e40197-5794-4268-b937-bd65aa044890
description: L’opération AddEntityFeedback renvoie les informations d’erreur correspondant aux problèmes côté serveur.
ms.openlocfilehash: a1027a0a1ee06cf3e83833b1d84c13d77b07c0b9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458438"
---
# <a name="addentityfeedback-operation"></a><span data-ttu-id="c1a44-103">Opération AddEntityFeedback</span><span class="sxs-lookup"><span data-stu-id="c1a44-103">AddEntityFeedback operation</span></span>

<span data-ttu-id="c1a44-104">L’opération **AddEntityFeedback** renvoie les informations d’erreur correspondant aux problèmes côté serveur.</span><span class="sxs-lookup"><span data-stu-id="c1a44-104">The **AddEntityFeedback** operation returns error information corresponding to server-side issues.</span></span> 
  
<span data-ttu-id="c1a44-105">Cette opération repose sur le type d’événement enregistré.</span><span class="sxs-lookup"><span data-stu-id="c1a44-105">This operation relies on the type of event being logged.</span></span> <span data-ttu-id="c1a44-106">L’un des événements les plus importants est **EntityAdded**, ce qui correspond à une entité sélectionnée.</span><span class="sxs-lookup"><span data-stu-id="c1a44-106">One of the most important events is **EntityAdded**, which corresponds to an entity being selected.</span></span> <span data-ttu-id="c1a44-107">Cette opération étant un traitement par lots, elle peut être utilisée pour enregistrer des lots d’entrées dans une demande unique.</span><span class="sxs-lookup"><span data-stu-id="c1a44-107">This operation is batch, so it can be used to log batches of entries in a single request.</span></span> 
  
## <a name="findpeople-request-examples"></a><span data-ttu-id="c1a44-108">Exemples de requête FindPeople</span><span class="sxs-lookup"><span data-stu-id="c1a44-108">FindPeople request examples</span></span>

<span data-ttu-id="c1a44-109">L’opération **AddEntityFeedback** permet aux clients de consigner les détails de l’interaction avec les entités renvoyées par le service.</span><span class="sxs-lookup"><span data-stu-id="c1a44-109">The **AddEntityFeedback** operation provides a way for clients to log details of interaction with entities returned by the service.</span></span> <span data-ttu-id="c1a44-110">Cela peut être utilisé en tant que signal pour améliorer la pertinence en arrière-plan pour chaque client.</span><span class="sxs-lookup"><span data-stu-id="c1a44-110">This can be used as a signal to improve relevance behind the scenes for each client.</span></span> <span data-ttu-id="c1a44-111">Par exemple, les clients peuvent utiliser cette opération pour envoyer des commentaires sur les entités de personnes retournées à partir de **FindPeople**.</span><span class="sxs-lookup"><span data-stu-id="c1a44-111">E.g., Clients can use this operation to provide feedback on people entities returned from **FindPeople**.</span></span>
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
                             xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                             xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="the-request-soap-body-contents"></a><span data-ttu-id="c1a44-112">Contenu du corps SOAP de la demande</span><span class="sxs-lookup"><span data-stu-id="c1a44-112">The request SOAP body contents</span></span>

<span data-ttu-id="c1a44-113">La demande SOAP contient un seul élément **EntityFeedbackEntries**.</span><span class="sxs-lookup"><span data-stu-id="c1a44-113">The soap request contains a single element **EntityFeedbackEntries**.</span></span> <span data-ttu-id="c1a44-114">Il contient à son tour un tableau d’objets **EntityFeedbackEntry** .</span><span class="sxs-lookup"><span data-stu-id="c1a44-114">This in turn contains an array of **EntityFeedbackEntry** objects.</span></span> <span data-ttu-id="c1a44-115">Chaque entrée du tableau peut contenir les éléments suivants.</span><span class="sxs-lookup"><span data-stu-id="c1a44-115">Each entry in the array can contain the following elements.</span></span> 
  
|<span data-ttu-id="c1a44-116">**Paramètres de la demande**</span><span class="sxs-lookup"><span data-stu-id="c1a44-116">**Request Parameters**</span></span>|<span data-ttu-id="c1a44-117">**Obligatoire**</span><span class="sxs-lookup"><span data-stu-id="c1a44-117">**Required**</span></span>|<span data-ttu-id="c1a44-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="c1a44-118">**Description**</span></span>|<span data-ttu-id="c1a44-119">**Type**</span><span class="sxs-lookup"><span data-stu-id="c1a44-119">**Type**</span></span>|
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="c1a44-120">**ClientEventTimeUtc**</span><span class="sxs-lookup"><span data-stu-id="c1a44-120">**ClientEventTimeUtc**</span></span> <br/> |<span data-ttu-id="c1a44-121">Oui</span><span class="sxs-lookup"><span data-stu-id="c1a44-121">Yes</span></span>  <br/> |<span data-ttu-id="c1a44-122">Heure UTC à laquelle l’événement s’est produit côté client.</span><span class="sxs-lookup"><span data-stu-id="c1a44-122">The UTC time the event occurred on the client-side.</span></span>  <br/> |<span data-ttu-id="c1a44-123">DateTime
</span><span class="sxs-lookup"><span data-stu-id="c1a44-123">DateTime</span></span>  <br/> |
|<span data-ttu-id="c1a44-124">**ClientEventTimeLocal**</span><span class="sxs-lookup"><span data-stu-id="c1a44-124">**ClientEventTimeLocal**</span></span> <br/> |<span data-ttu-id="c1a44-125">Oui</span><span class="sxs-lookup"><span data-stu-id="c1a44-125">Yes</span></span>  <br/> |<span data-ttu-id="c1a44-126">Heure locale à laquelle l’événement s’est produit côté client.</span><span class="sxs-lookup"><span data-stu-id="c1a44-126">The local time the event occurred on the client side.</span></span>  <br/> |<span data-ttu-id="c1a44-127">DateTime
</span><span class="sxs-lookup"><span data-stu-id="c1a44-127">DateTime</span></span>  <br/> |
|<span data-ttu-id="c1a44-128">**Identifi**</span><span class="sxs-lookup"><span data-stu-id="c1a44-128">**ClientId**</span></span> <br/> |<span data-ttu-id="c1a44-129">Oui</span><span class="sxs-lookup"><span data-stu-id="c1a44-129">Yes</span></span>  <br/> |<span data-ttu-id="c1a44-130">Type de client (par exemple, Outlook, OWA, etc.).</span><span class="sxs-lookup"><span data-stu-id="c1a44-130">Type of Client (E.g., Outlook, OWA, etc.).</span></span>  <br/> |<span data-ttu-id="c1a44-131">ClientIDType, énumération</span><span class="sxs-lookup"><span data-stu-id="c1a44-131">ClientIDType Enumeration</span></span>  <br/> |
|<span data-ttu-id="c1a44-132">**ClientSessionId**</span><span class="sxs-lookup"><span data-stu-id="c1a44-132">**ClientSessionId**</span></span> <br/> |<span data-ttu-id="c1a44-133">Oui</span><span class="sxs-lookup"><span data-stu-id="c1a44-133">Yes</span></span>  <br/> |<span data-ttu-id="c1a44-134">GUID identifiant l’ID de session.</span><span class="sxs-lookup"><span data-stu-id="c1a44-134">GUID Identifying the session ID.</span></span> <span data-ttu-id="c1a44-135">Généré sur le client.</span><span class="sxs-lookup"><span data-stu-id="c1a44-135">Generated on the client.</span></span>  <br/> |<span data-ttu-id="c1a44-136">GUID</span><span class="sxs-lookup"><span data-stu-id="c1a44-136">GUID</span></span>  <br/> |
|<span data-ttu-id="c1a44-137">**ClientVersion**</span><span class="sxs-lookup"><span data-stu-id="c1a44-137">**ClientVersion**</span></span> <br/> |<span data-ttu-id="c1a44-138">Oui</span><span class="sxs-lookup"><span data-stu-id="c1a44-138">Yes</span></span>  <br/> |<span data-ttu-id="c1a44-139">Version du client (par exemple, 15.01.0101.000).</span><span class="sxs-lookup"><span data-stu-id="c1a44-139">Version of the client (E.g., 15.01.0101.000).</span></span>  <br/> |<span data-ttu-id="c1a44-140">Chaîne</span><span class="sxs-lookup"><span data-stu-id="c1a44-140">String</span></span>  <br/> |
|<span data-ttu-id="c1a44-141">**EntityAddSource**</span><span class="sxs-lookup"><span data-stu-id="c1a44-141">**EntityAddSource**</span></span> <br/> |<span data-ttu-id="c1a44-142">Non</span><span class="sxs-lookup"><span data-stu-id="c1a44-142">No</span></span>  <br/> |<span data-ttu-id="c1a44-143">Source pour EntityAded (par exemple, EntityRelevanceAPI, types, collés).</span><span class="sxs-lookup"><span data-stu-id="c1a44-143">Source for EntityAded (E.g., EntityRelevanceAPI, types, pasted).</span></span>  <br/> |<span data-ttu-id="c1a44-144">EntityAddSource, énumération</span><span class="sxs-lookup"><span data-stu-id="c1a44-144">EntityAddSource Enumeration</span></span>  <br/> |
|<span data-ttu-id="c1a44-145">**EntrySequenceNumber**</span><span class="sxs-lookup"><span data-stu-id="c1a44-145">**EntrySequenceNumber**</span></span> <br/> |<span data-ttu-id="c1a44-146">Oui</span><span class="sxs-lookup"><span data-stu-id="c1a44-146">Yes</span></span>  <br/> |<span data-ttu-id="c1a44-147">Entier incrémentiel par session cliente.</span><span class="sxs-lookup"><span data-stu-id="c1a44-147">An incremental integer per client session.</span></span> <span data-ttu-id="c1a44-148">Utilisé pour détecter la perte de données.</span><span class="sxs-lookup"><span data-stu-id="c1a44-148">Used for detecting data loss.</span></span>  <br/> |<span data-ttu-id="c1a44-149">Int</span><span class="sxs-lookup"><span data-stu-id="c1a44-149">Int</span></span>  <br/> |
|<span data-ttu-id="c1a44-150">**EventType**</span><span class="sxs-lookup"><span data-stu-id="c1a44-150">**EventType**</span></span> <br/> |<span data-ttu-id="c1a44-151">Oui</span><span class="sxs-lookup"><span data-stu-id="c1a44-151">Yes</span></span>  <br/> |<span data-ttu-id="c1a44-152">Type d’événement (par exemple, entité ajoutée, entité supprimée).</span><span class="sxs-lookup"><span data-stu-id="c1a44-152">Type of event (E.g., Entity Added, Entity Removed).</span></span>  <br/> |<span data-ttu-id="c1a44-153">Chaîne</span><span class="sxs-lookup"><span data-stu-id="c1a44-153">String</span></span>  <br/> |
|<span data-ttu-id="c1a44-154">**JSONPropertyBag**</span><span class="sxs-lookup"><span data-stu-id="c1a44-154">**JSONPropertyBag**</span></span> <br/> |<span data-ttu-id="c1a44-155">Non</span><span class="sxs-lookup"><span data-stu-id="c1a44-155">No</span></span>  <br/> |<span data-ttu-id="c1a44-156">Propriétés supplémentaires associées à l’événement (BLOB JSON des paires clé/valeur).</span><span class="sxs-lookup"><span data-stu-id="c1a44-156">Additional properties associated with the event (JSON blob of key/value pairs).</span></span>  <br/> |<span data-ttu-id="c1a44-157">BLOB JSON</span><span class="sxs-lookup"><span data-stu-id="c1a44-157">JSON Blob</span></span>  <br/> |
|<span data-ttu-id="c1a44-158">**TargetEntityList**</span><span class="sxs-lookup"><span data-stu-id="c1a44-158">**TargetEntityList**</span></span> <br/> |<span data-ttu-id="c1a44-159">Non</span><span class="sxs-lookup"><span data-stu-id="c1a44-159">No</span></span>  <br/> |<span data-ttu-id="c1a44-160">Liste des entités associées à l’événement.</span><span class="sxs-lookup"><span data-stu-id="c1a44-160">List of entities associated with the event.</span></span>  <br/> |<span data-ttu-id="c1a44-161">Chaîne JSON</span><span class="sxs-lookup"><span data-stu-id="c1a44-161">JSON String</span></span>  <br/> |
|<span data-ttu-id="c1a44-162">**TransactionId**</span><span class="sxs-lookup"><span data-stu-id="c1a44-162">**TransactionId**</span></span> <br/> |<span data-ttu-id="c1a44-163">Non</span><span class="sxs-lookup"><span data-stu-id="c1a44-163">No</span></span>  <br/> |<span data-ttu-id="c1a44-164">ID (GUID) corrélation de l’ID dans les journaux de requêtes.</span><span class="sxs-lookup"><span data-stu-id="c1a44-164">ID (GUID) correlating the ID in query logs.</span></span>  <br/> |<span data-ttu-id="c1a44-165">Chaîne</span><span class="sxs-lookup"><span data-stu-id="c1a44-165">String</span></span>  <br/> |
   
### <a name="successful-addentityfeedback-operation-response"></a><span data-ttu-id="c1a44-166">Réponse de l’opération AddEntityFeedback réussie</span><span class="sxs-lookup"><span data-stu-id="c1a44-166">Successful AddEntityFeedback operation response</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" 
                                MinorVersion="1" 
                                MajorBuildNumber="228" 
                                MinorBuildNumber="0" 
                                Version="V2_49" 
                                xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                                xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                                xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <AddEntityFeedbackResponse ResponseClass="Success" 
                                                              xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                                              xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                                                              xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <ErrorCount>0</ErrorCount>
            <ErrorDetails />
        </AddEntityFeedbackResponse>
    </s:Body>
</s:Envelope> 

```

### <a name="the-response-soap-body-contains-the-following-elements"></a><span data-ttu-id="c1a44-167">Le corps SOAP de réponse contient les éléments suivants</span><span class="sxs-lookup"><span data-stu-id="c1a44-167">The response SOAP body contains the following elements</span></span>

#### <a name="errors"></a><span data-ttu-id="c1a44-168">Erreurs</span><span class="sxs-lookup"><span data-stu-id="c1a44-168">Errors</span></span> 
  
<span data-ttu-id="c1a44-169">L’API peut journaliser un lot d’entrées de commentaires, Nous consignerons tout ce que nous pouvons faire.</span><span class="sxs-lookup"><span data-stu-id="c1a44-169">The API can log a batch of feedback entries, we log all that we can.</span></span> <span data-ttu-id="c1a44-170">Ce champ indique le nombre d’entrées d’erreur qui n’ont pas été journalisées.</span><span class="sxs-lookup"><span data-stu-id="c1a44-170">This field represents the number of error entries that were not logged.</span></span>
    
#### <a name="errordetails"></a><span data-ttu-id="c1a44-171">ErrorDetails</span><span class="sxs-lookup"><span data-stu-id="c1a44-171">ErrorDetails</span></span>
  
<span data-ttu-id="c1a44-172">Les détails relatifs aux erreurs ci-dessus sont séparés par `;` .</span><span class="sxs-lookup"><span data-stu-id="c1a44-172">Details pertaining to the errors above separates by `;`.</span></span>
    
### <a name="currently-supported-values"></a><span data-ttu-id="c1a44-173">Valeurs actuellement prises en charge</span><span class="sxs-lookup"><span data-stu-id="c1a44-173">Currently supported values</span></span>

|<span data-ttu-id="c1a44-174">**ClientIdType, énumération**</span><span class="sxs-lookup"><span data-stu-id="c1a44-174">**ClientIdType Enumeration**</span></span>|
|:-----|
|<span data-ttu-id="c1a44-175">Desktop</span><span class="sxs-lookup"><span data-stu-id="c1a44-175">Desktop</span></span>  <br/> |
|<span data-ttu-id="c1a44-176">Exchange</span><span class="sxs-lookup"><span data-stu-id="c1a44-176">Exchange</span></span>  <br/> |
|<span data-ttu-id="c1a44-177">CONSÉQUENT</span><span class="sxs-lookup"><span data-stu-id="c1a44-177">IMAP4</span></span>  <br/> |
|<span data-ttu-id="c1a44-178">Lync</span><span class="sxs-lookup"><span data-stu-id="c1a44-178">Lync</span></span>  <br/> |
|<span data-ttu-id="c1a44-179">MacMail</span><span class="sxs-lookup"><span data-stu-id="c1a44-179">MacMail</span></span>  <br/> |
|<span data-ttu-id="c1a44-180">MacOutlook</span><span class="sxs-lookup"><span data-stu-id="c1a44-180">MacOutlook</span></span>  <br/> |
|<span data-ttu-id="c1a44-181">Mobile</span><span class="sxs-lookup"><span data-stu-id="c1a44-181">Mobile</span></span>  <br/> |
|<span data-ttu-id="c1a44-182">Autres</span><span class="sxs-lookup"><span data-stu-id="c1a44-182">Other</span></span>  <br/> |
|<span data-ttu-id="c1a44-183">Outlook</span><span class="sxs-lookup"><span data-stu-id="c1a44-183">Outlook</span></span>  <br/> |
|<span data-ttu-id="c1a44-184">OutlookService</span><span class="sxs-lookup"><span data-stu-id="c1a44-184">OutlookService</span></span>  <br/> |
|<span data-ttu-id="c1a44-185">POP3</span><span class="sxs-lookup"><span data-stu-id="c1a44-185">POP3</span></span>  <br/> |
|<span data-ttu-id="c1a44-186">Tablet</span><span class="sxs-lookup"><span data-stu-id="c1a44-186">Tablet</span></span>  <br/> |
|<span data-ttu-id="c1a44-187">Web</span><span class="sxs-lookup"><span data-stu-id="c1a44-187">Web</span></span>  <br/> |
   
|<span data-ttu-id="c1a44-188">**EntityAddSource, énumération**</span><span class="sxs-lookup"><span data-stu-id="c1a44-188">**EntityAddSource Enumeration**</span></span>|
|:-----|
|<span data-ttu-id="c1a44-189">ActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="c1a44-189">ActiveDirectory</span></span>  <br/> |
|<span data-ttu-id="c1a44-190">EntityRelevanceApi</span><span class="sxs-lookup"><span data-stu-id="c1a44-190">EntityRelevanceApi</span></span>  <br/> |
|<span data-ttu-id="c1a44-191">EntityRelevanceApiCache</span><span class="sxs-lookup"><span data-stu-id="c1a44-191">EntityRelevanceApiCache</span></span>  <br/> |
|<span data-ttu-id="c1a44-192">ExplicitTyping</span><span class="sxs-lookup"><span data-stu-id="c1a44-192">ExplicitTyping</span></span>  <br/> |
|<span data-ttu-id="c1a44-193">LocalCache</span><span class="sxs-lookup"><span data-stu-id="c1a44-193">LocalCache</span></span>  <br/> |
|<span data-ttu-id="c1a44-194">LocalCacheAndEntityRelevanceAPI</span><span class="sxs-lookup"><span data-stu-id="c1a44-194">LocalCacheAndEntityRelevanceAPI</span></span>  <br/> |
|<span data-ttu-id="c1a44-195">Aucun</span><span class="sxs-lookup"><span data-stu-id="c1a44-195">None</span></span>  <br/> |
|<span data-ttu-id="c1a44-196">Autres</span><span class="sxs-lookup"><span data-stu-id="c1a44-196">Other</span></span>  <br/> |
|<span data-ttu-id="c1a44-197">Coller</span><span class="sxs-lookup"><span data-stu-id="c1a44-197">Paste</span></span>  <br/> |
   
### <a name="addentityfeedback-operation-error-response"></a><span data-ttu-id="c1a44-198">Réponse d’erreur d’opération AddEntityFeedback</span><span class="sxs-lookup"><span data-stu-id="c1a44-198">AddEntityFeedback operation error response</span></span>

<span data-ttu-id="c1a44-199">Pour les codes d’erreur qui sont génériques à EWS, voir [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="c1a44-199">For error codes that are generic to EWS, see [ResponseCode](responsecode.md).</span></span>
  
### <a name="example-of-addentityfeedback-in-conjunction-with-findpeople"></a><span data-ttu-id="c1a44-200">Exemple de AddEntityFeedback en association avec FindPeople</span><span class="sxs-lookup"><span data-stu-id="c1a44-200">Example of AddEntityFeedback in conjunction with FindPeople</span></span>

#### <a name="findpeople-request"></a><span data-ttu-id="c1a44-201">Demande FindPeople</span><span class="sxs-lookup"><span data-stu-id="c1a44-201">FindPeople request</span></span>
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

#### <a name="findpeople-response"></a><span data-ttu-id="c1a44-202">Réponse FindPeople</span><span class="sxs-lookup"><span data-stu-id="c1a44-202">FindPeople response</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" MinorVersion="1" MajorBuildNumber="302" MinorBuildNumber="0" Version="V2_68" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <FindPeopleResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <People>
                <Persona xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

#### <a name="addentityfeedback-request"></a><span data-ttu-id="c1a44-203">Demande AddEntityFeedback</span><span class="sxs-lookup"><span data-stu-id="c1a44-203">AddEntityFeedback request</span></span>

```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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
> <span data-ttu-id="c1a44-204">Utilisation de l’ID de transaction de réponse FindPeople comme ID de transaction de demande AddEntityFeedback.</span><span class="sxs-lookup"><span data-stu-id="c1a44-204">Using FindPeople response transaction ID as the AddEntityFeedback request transaction ID.</span></span> 
  
#### <a name="addentityfeedback-response"></a><span data-ttu-id="c1a44-205">Réponse AddEntityFeedback</span><span class="sxs-lookup"><span data-stu-id="c1a44-205">AddEntityFeedback response</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" MinorVersion="1" MajorBuildNumber="302" MinorBuildNumber="0" Version="V2_68" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <AddEntityFeedbackResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <ErrorCount>0</ErrorCount>
            <ErrorDetails />
        </AddEntityFeedbackResponse>
    </s:Body>
</s:Envelope>

```


