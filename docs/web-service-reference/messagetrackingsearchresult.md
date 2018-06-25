---
title: MessageTrackingSearchResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageTrackingSearchResult
api_type:
- schema
ms.assetid: 8ea77aa8-b93f-4287-be36-0a9da06e0946
description: L’élément MessageTrackingSearchResult contient un résultat de message unique d’un élément FindMessageTrackingReportResponse.
ms.openlocfilehash: ad4fb9d9e2266222303bd2015a7afba0bb46721b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828460"
---
# <a name="messagetrackingsearchresult"></a><span data-ttu-id="60daa-103">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="60daa-103">MessageTrackingSearchResult</span></span>

<span data-ttu-id="60daa-104">L’élément **MessageTrackingSearchResult** contient un résultat de message unique d’un élément [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="60daa-104">The **MessageTrackingSearchResult** element contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span> 
  
```xml
<MessageTrackingSearchResult>
   <Subject/>
   <Sender/>
   <PurportedSender/>
   <Recipients/>
   <SubmittedTime/>
   <MessageTrackingReportId/>
   <PreviousHopServer/>
   <FirstHopServer/>
   <Properties/>
</MessageTrackingSearchResult>
```

 <span data-ttu-id="60daa-105">**FindMessageTrackingSearchResultType**</span><span class="sxs-lookup"><span data-stu-id="60daa-105">**FindMessageTrackingSearchResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="60daa-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="60daa-106">Attributes and elements</span></span>

<span data-ttu-id="60daa-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="60daa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="60daa-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="60daa-108">Attributes</span></span>

<span data-ttu-id="60daa-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="60daa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="60daa-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="60daa-110">Child elements</span></span>

|<span data-ttu-id="60daa-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="60daa-111">**Element**</span></span>|<span data-ttu-id="60daa-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="60daa-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="60daa-113">Objet</span><span class="sxs-lookup"><span data-stu-id="60daa-113">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="60daa-114">Contient l’objet du message électronique.</span><span class="sxs-lookup"><span data-stu-id="60daa-114">Contains the e-mail message subject.</span></span>  <br/> |
|[<span data-ttu-id="60daa-115">Expéditeur (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="60daa-115">Sender (EmailAddressType)</span></span>](sender-emailaddresstype.md) <br/> |<span data-ttu-id="60daa-116">Contient l’adresse de l’expéditeur du message électronique.</span><span class="sxs-lookup"><span data-stu-id="60daa-116">Contains the e-mail message sender's address.</span></span>  <br/> |
|[<span data-ttu-id="60daa-117">PurportedSender</span><span class="sxs-lookup"><span data-stu-id="60daa-117">PurportedSender</span></span>](purportedsender.md) <br/> |<span data-ttu-id="60daa-118">Contient des informations de contact pour l’expéditeur présumé d’un message électronique.</span><span class="sxs-lookup"><span data-stu-id="60daa-118">Contains contact information for the alleged sender of an e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="60daa-119">Destinataires (ArrayOfRecipientsType)</span><span class="sxs-lookup"><span data-stu-id="60daa-119">Recipients (ArrayOfRecipientsType)</span></span>](recipients-arrayofrecipientstype.md) <br/> |<span data-ttu-id="60daa-120">Contient une liste d’adresses de messagerie qui a reçu ce message.</span><span class="sxs-lookup"><span data-stu-id="60daa-120">Contains a list of e-mail addresses that received this message.</span></span>  <br/> |
|[<span data-ttu-id="60daa-121">SubmittedTime</span><span class="sxs-lookup"><span data-stu-id="60daa-121">SubmittedTime</span></span>](submittedtime.md) <br/> |<span data-ttu-id="60daa-122">Contient l’heure à laquelle le message a été envoyé.</span><span class="sxs-lookup"><span data-stu-id="60daa-122">Contains the time that the message was submitted.</span></span>  <br/> |
|[<span data-ttu-id="60daa-123">MessageTrackingReportId</span><span class="sxs-lookup"><span data-stu-id="60daa-123">MessageTrackingReportId</span></span>](messagetrackingreportid.md) <br/> |<span data-ttu-id="60daa-124">Contient un ID interne qui identifie le message dans la base de données de transport.</span><span class="sxs-lookup"><span data-stu-id="60daa-124">Contains an internal ID that identifies the message in the transport database.</span></span>  <br/> |
|[<span data-ttu-id="60daa-125">PreviousHopServer</span><span class="sxs-lookup"><span data-stu-id="60daa-125">PreviousHopServer</span></span>](previoushopserver.md) <br/> |<span data-ttu-id="60daa-126">Contient le nom du serveur dans la forêt qui précédemment accepté le message.</span><span class="sxs-lookup"><span data-stu-id="60daa-126">Contains the name of the server in the forest that previously accepted the message.</span></span>  <br/> |
|[<span data-ttu-id="60daa-127">FirstHopServer</span><span class="sxs-lookup"><span data-stu-id="60daa-127">FirstHopServer</span></span>](firsthopserver.md) <br/> |<span data-ttu-id="60daa-128">Contient le nom du serveur dans la forêt qui a accepté tout d’abord le message.</span><span class="sxs-lookup"><span data-stu-id="60daa-128">Contains the name of the server in the forest that first accepted the message.</span></span>  <br/> |
|[<span data-ttu-id="60daa-129">Propriétés (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="60daa-129">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="60daa-130">Contient une liste d’un ou plusieurs des propriétés de suivi.</span><span class="sxs-lookup"><span data-stu-id="60daa-130">Contains a list of one or more tracking properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="60daa-131">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="60daa-131">Parent elements</span></span>

|<span data-ttu-id="60daa-132">**Élément**</span><span class="sxs-lookup"><span data-stu-id="60daa-132">**Element**</span></span>|<span data-ttu-id="60daa-133">**Description**</span><span class="sxs-lookup"><span data-stu-id="60daa-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="60daa-134">MessageTrackingSearchResults</span><span class="sxs-lookup"><span data-stu-id="60daa-134">MessageTrackingSearchResults</span></span>](messagetrackingsearchresults.md) <br/> |<span data-ttu-id="60daa-135">Contient une liste des messages qui correspondent aux critères de recherche.</span><span class="sxs-lookup"><span data-stu-id="60daa-135">Contains a list of messages that match the search criteria.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="60daa-136">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="60daa-136">Text value</span></span>

<span data-ttu-id="60daa-137">Aucun.</span><span class="sxs-lookup"><span data-stu-id="60daa-137">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="60daa-138">Remarques</span><span class="sxs-lookup"><span data-stu-id="60daa-138">Remarks</span></span>

<span data-ttu-id="60daa-139">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="60daa-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="60daa-140">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="60daa-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="60daa-141">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="60daa-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="60daa-142">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="60daa-142">Schema Name</span></span>  <br/> |<span data-ttu-id="60daa-143">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="60daa-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="60daa-144">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="60daa-144">Validation File</span></span>  <br/> |<span data-ttu-id="60daa-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="60daa-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="60daa-146">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="60daa-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="60daa-147">False</span><span class="sxs-lookup"><span data-stu-id="60daa-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="60daa-148">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="60daa-148">See also</span></span>



[<span data-ttu-id="60daa-149">Opération FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="60daa-149">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)


- [<span data-ttu-id="60daa-150">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="60daa-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

