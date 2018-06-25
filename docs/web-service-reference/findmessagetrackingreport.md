---
title: FindMessageTrackingReport
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindMessageTrackingReport
api_type:
- schema
ms.assetid: 7ca6e2f7-aae1-4920-b839-73513ba8d4d8
description: L’élément FindMessageTrackingReport spécifie les critères pour les types de messages.
ms.openlocfilehash: 77545121aa056992248c045af3f3d36566678b94
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756410"
---
# <a name="findmessagetrackingreport"></a><span data-ttu-id="6727e-103">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="6727e-103">FindMessageTrackingReport</span></span>

<span data-ttu-id="6727e-104">L’élément **FindMessageTrackingReport** spécifie les critères pour les types de messages.</span><span class="sxs-lookup"><span data-stu-id="6727e-104">The **FindMessageTrackingReport** element specifies criteria for the types of messages to find.</span></span> 
  
```xml
<FindMessageTrackingReport>
   <Scope/>
   <Domain/>
   <Sender/>
   <PurportedSender/>
   <Recipient/>
   <Subject/>
   <StartDateTime/>
   <EndDateTime/>
   <MessageId/>
   <FederatedDeliveryMailbox/>
   <DiagnosticsLevel/>
   <ServerHint/>
   <Properties/>
</FindMessageTrackingReport>
```

 <span data-ttu-id="6727e-105">**FindMessageTrackingReportRequestType**</span><span class="sxs-lookup"><span data-stu-id="6727e-105">**FindMessageTrackingReportRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6727e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6727e-106">Attributes and elements</span></span>

<span data-ttu-id="6727e-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6727e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6727e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="6727e-108">Attributes</span></span>

<span data-ttu-id="6727e-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6727e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6727e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6727e-110">Child elements</span></span>

|<span data-ttu-id="6727e-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6727e-111">**Element**</span></span>|<span data-ttu-id="6727e-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="6727e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6727e-113">Étendue (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="6727e-113">Scope (NonEmptyStringType)</span></span>](scope-nonemptystringtype.md) <br/> |<span data-ttu-id="6727e-114">Représente le rapport de suivi des messages l’étendue doivent être.</span><span class="sxs-lookup"><span data-stu-id="6727e-114">Represents how extensive the message tracking report should be.</span></span>  <br/> |
|[<span data-ttu-id="6727e-115">Domaine (le suivi des messages)</span><span class="sxs-lookup"><span data-stu-id="6727e-115">Domain (Message Tracking)</span></span>](domain-message-tracking.md) <br/> |<span data-ttu-id="6727e-116">Contient le nom du domaine où le suivi des messages est exécutée.</span><span class="sxs-lookup"><span data-stu-id="6727e-116">Contains the name of the domain where the message tracking is executed.</span></span>  <br/> |
|[<span data-ttu-id="6727e-117">Expéditeur (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="6727e-117">Sender (EmailAddressType)</span></span>](sender-emailaddresstype.md) <br/> |<span data-ttu-id="6727e-118">Contient des informations de contact pour l’expéditeur du message électronique.</span><span class="sxs-lookup"><span data-stu-id="6727e-118">Contains contact information for the sender of the e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="6727e-119">PurportedSender</span><span class="sxs-lookup"><span data-stu-id="6727e-119">PurportedSender</span></span>](purportedsender.md) <br/> |<span data-ttu-id="6727e-120">Contient des informations de contact pour l’expéditeur présumé d’un message électronique.</span><span class="sxs-lookup"><span data-stu-id="6727e-120">Contains contact information for the alleged sender of an e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="6727e-121">Recipient</span><span class="sxs-lookup"><span data-stu-id="6727e-121">Recipient</span></span>](recipient.md) <br/> |<span data-ttu-id="6727e-122">Contient l’adresse de messagerie du destinataire du message.</span><span class="sxs-lookup"><span data-stu-id="6727e-122">Contains the e-mail address for the recipient of the message.</span></span>  <br/> |
|[<span data-ttu-id="6727e-123">Objet</span><span class="sxs-lookup"><span data-stu-id="6727e-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="6727e-124">Contient l’objet du message électronique.</span><span class="sxs-lookup"><span data-stu-id="6727e-124">Contains the subject of the e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="6727e-125">StartDateTime</span><span class="sxs-lookup"><span data-stu-id="6727e-125">StartDateTime</span></span>](startdatetime.md) <br/> |<span data-ttu-id="6727e-126">Contient la date et l’heure pour la recherche de départ.</span><span class="sxs-lookup"><span data-stu-id="6727e-126">Contains the starting date and time for the search.</span></span>  <br/> |
|[<span data-ttu-id="6727e-127">EndDateTime</span><span class="sxs-lookup"><span data-stu-id="6727e-127">EndDateTime</span></span>](enddatetime.md) <br/> |<span data-ttu-id="6727e-128">Contient la date et l’heure de la recherche.</span><span class="sxs-lookup"><span data-stu-id="6727e-128">Contains the ending date and time for the search.</span></span>  <br/> |
|[<span data-ttu-id="6727e-129">MessageId</span><span class="sxs-lookup"><span data-stu-id="6727e-129">MessageId</span></span>](messageid.md) <br/> |<span data-ttu-id="6727e-130">Contient l’identificateur de message pour la recherche.</span><span class="sxs-lookup"><span data-stu-id="6727e-130">Contains the message identifier for the search.</span></span>  <br/> |
|[<span data-ttu-id="6727e-131">FederatedDeliveryMailbox</span><span class="sxs-lookup"><span data-stu-id="6727e-131">FederatedDeliveryMailbox</span></span>](federateddeliverymailbox.md) <br/> |<span data-ttu-id="6727e-132">Contient le nom de la boîte aux lettres dans laquelle le message cross-site a été envoyé.</span><span class="sxs-lookup"><span data-stu-id="6727e-132">Contains the name of the mailbox where the cross-premise message was sent.</span></span>  <br/> |
|[<span data-ttu-id="6727e-133">DiagnosticsLevel</span><span class="sxs-lookup"><span data-stu-id="6727e-133">DiagnosticsLevel</span></span>](diagnosticslevel.md) <br/> |<span data-ttu-id="6727e-134">Représente le niveau de détail des rapports de diagnostic.</span><span class="sxs-lookup"><span data-stu-id="6727e-134">Represents the level of detail for diagnostic reports.</span></span>  <br/> |
|[<span data-ttu-id="6727e-135">ServerHint</span><span class="sxs-lookup"><span data-stu-id="6727e-135">ServerHint</span></span>](serverhint.md) <br/> |<span data-ttu-id="6727e-136">Représente le point de départ pour le suivi d’un message dans un site distant ou d’une forêt.</span><span class="sxs-lookup"><span data-stu-id="6727e-136">Represents the starting point for tracking a message in a remote site or forest.</span></span>  <br/> |
|[<span data-ttu-id="6727e-137">Propriétés (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="6727e-137">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="6727e-138">Contient une liste d’un ou plusieurs des propriétés de suivi.</span><span class="sxs-lookup"><span data-stu-id="6727e-138">Contains a list of one or more tracking properties.</span></span> <span data-ttu-id="6727e-139">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="6727e-139">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6727e-140">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6727e-140">Parent elements</span></span>

<span data-ttu-id="6727e-141">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6727e-141">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="6727e-142">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="6727e-142">Text value</span></span>

<span data-ttu-id="6727e-143">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6727e-143">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6727e-144">Remarques</span><span class="sxs-lookup"><span data-stu-id="6727e-144">Remarks</span></span>

<span data-ttu-id="6727e-145">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="6727e-145">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6727e-146">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6727e-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6727e-147">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6727e-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6727e-148">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6727e-148">Schema Name</span></span>  <br/> |<span data-ttu-id="6727e-149">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="6727e-149">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6727e-150">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6727e-150">Validation File</span></span>  <br/> |<span data-ttu-id="6727e-151">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6727e-151">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6727e-152">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6727e-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="6727e-153">False</span><span class="sxs-lookup"><span data-stu-id="6727e-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6727e-154">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6727e-154">See also</span></span>



[<span data-ttu-id="6727e-155">Opération FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="6727e-155">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)


- [<span data-ttu-id="6727e-156">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6727e-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

