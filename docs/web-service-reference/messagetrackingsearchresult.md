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
description: L’élément MessageTrackingSearchResult contient un seul résultat de message pour un élément FindMessageTrackingReportResponse.
ms.openlocfilehash: 27e70cd9e11b480ab6bbb9b28275f142da7c76ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466681"
---
# <a name="messagetrackingsearchresult"></a><span data-ttu-id="38020-103">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="38020-103">MessageTrackingSearchResult</span></span>

<span data-ttu-id="38020-104">L’élément **MessageTrackingSearchResult** contient un seul résultat de message pour un élément [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="38020-104">The **MessageTrackingSearchResult** element contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span> 
  
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

 <span data-ttu-id="38020-105">**FindMessageTrackingSearchResultType**</span><span class="sxs-lookup"><span data-stu-id="38020-105">**FindMessageTrackingSearchResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="38020-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="38020-106">Attributes and elements</span></span>

<span data-ttu-id="38020-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="38020-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="38020-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="38020-108">Attributes</span></span>

<span data-ttu-id="38020-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="38020-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="38020-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="38020-110">Child elements</span></span>

|<span data-ttu-id="38020-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="38020-111">**Element**</span></span>|<span data-ttu-id="38020-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="38020-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="38020-113">Subject</span><span class="sxs-lookup"><span data-stu-id="38020-113">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="38020-114">Contient l’objet du message électronique.</span><span class="sxs-lookup"><span data-stu-id="38020-114">Contains the e-mail message subject.</span></span>  <br/> |
|[<span data-ttu-id="38020-115">Expéditeur (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="38020-115">Sender (EmailAddressType)</span></span>](sender-emailaddresstype.md) <br/> |<span data-ttu-id="38020-116">Contient l’adresse de l’expéditeur du message électronique.</span><span class="sxs-lookup"><span data-stu-id="38020-116">Contains the e-mail message sender's address.</span></span>  <br/> |
|[<span data-ttu-id="38020-117">PurportedSender</span><span class="sxs-lookup"><span data-stu-id="38020-117">PurportedSender</span></span>](purportedsender.md) <br/> |<span data-ttu-id="38020-118">Contient les informations de contact pour l’expéditeur allégué d’un message électronique.</span><span class="sxs-lookup"><span data-stu-id="38020-118">Contains contact information for the alleged sender of an e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="38020-119">Destinataires (ArrayOfRecipientsType)</span><span class="sxs-lookup"><span data-stu-id="38020-119">Recipients (ArrayOfRecipientsType)</span></span>](recipients-arrayofrecipientstype.md) <br/> |<span data-ttu-id="38020-120">Contient une liste des adresses de messagerie qui ont reçu ce message.</span><span class="sxs-lookup"><span data-stu-id="38020-120">Contains a list of e-mail addresses that received this message.</span></span>  <br/> |
|[<span data-ttu-id="38020-121">SubmittedTime</span><span class="sxs-lookup"><span data-stu-id="38020-121">SubmittedTime</span></span>](submittedtime.md) <br/> |<span data-ttu-id="38020-122">Contient l’heure à laquelle le message a été soumis.</span><span class="sxs-lookup"><span data-stu-id="38020-122">Contains the time that the message was submitted.</span></span>  <br/> |
|[<span data-ttu-id="38020-123">MessageTrackingReportId</span><span class="sxs-lookup"><span data-stu-id="38020-123">MessageTrackingReportId</span></span>](messagetrackingreportid.md) <br/> |<span data-ttu-id="38020-124">Contient un ID interne qui identifie le message dans la base de données de transport.</span><span class="sxs-lookup"><span data-stu-id="38020-124">Contains an internal ID that identifies the message in the transport database.</span></span>  <br/> |
|[<span data-ttu-id="38020-125">PreviousHopServer</span><span class="sxs-lookup"><span data-stu-id="38020-125">PreviousHopServer</span></span>](previoushopserver.md) <br/> |<span data-ttu-id="38020-126">Contient le nom du serveur dans la forêt qui a précédemment accepté le message.</span><span class="sxs-lookup"><span data-stu-id="38020-126">Contains the name of the server in the forest that previously accepted the message.</span></span>  <br/> |
|[<span data-ttu-id="38020-127">FirstHopServer</span><span class="sxs-lookup"><span data-stu-id="38020-127">FirstHopServer</span></span>](firsthopserver.md) <br/> |<span data-ttu-id="38020-128">Contient le nom du serveur dans la forêt qui a accepté le message en premier.</span><span class="sxs-lookup"><span data-stu-id="38020-128">Contains the name of the server in the forest that first accepted the message.</span></span>  <br/> |
|[<span data-ttu-id="38020-129">Propriétés (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="38020-129">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="38020-130">Contient une liste d’une ou plusieurs propriétés de suivi.</span><span class="sxs-lookup"><span data-stu-id="38020-130">Contains a list of one or more tracking properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="38020-131">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="38020-131">Parent elements</span></span>

|<span data-ttu-id="38020-132">**Élément**</span><span class="sxs-lookup"><span data-stu-id="38020-132">**Element**</span></span>|<span data-ttu-id="38020-133">**Description**</span><span class="sxs-lookup"><span data-stu-id="38020-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="38020-134">MessageTrackingSearchResults</span><span class="sxs-lookup"><span data-stu-id="38020-134">MessageTrackingSearchResults</span></span>](messagetrackingsearchresults.md) <br/> |<span data-ttu-id="38020-135">Contient une liste de messages qui correspondent aux critères de recherche.</span><span class="sxs-lookup"><span data-stu-id="38020-135">Contains a list of messages that match the search criteria.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="38020-136">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="38020-136">Text value</span></span>

<span data-ttu-id="38020-137">Aucun.</span><span class="sxs-lookup"><span data-stu-id="38020-137">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="38020-138">Remarques</span><span class="sxs-lookup"><span data-stu-id="38020-138">Remarks</span></span>

<span data-ttu-id="38020-139">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="38020-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="38020-140">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="38020-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="38020-141">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="38020-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="38020-142">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="38020-142">Schema Name</span></span>  <br/> |<span data-ttu-id="38020-143">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="38020-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="38020-144">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="38020-144">Validation File</span></span>  <br/> |<span data-ttu-id="38020-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="38020-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="38020-146">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="38020-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="38020-147">False</span><span class="sxs-lookup"><span data-stu-id="38020-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="38020-148">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="38020-148">See also</span></span>



[<span data-ttu-id="38020-149">Opération FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="38020-149">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)


- [<span data-ttu-id="38020-150">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="38020-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

