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
description: L’élément FindMessageTrackingReport spécifie les critères pour les types de messages à rechercher.
ms.openlocfilehash: d30e5391bb4305cae0004a9788df971a57297cae
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462935"
---
# <a name="findmessagetrackingreport"></a><span data-ttu-id="a1a62-103">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="a1a62-103">FindMessageTrackingReport</span></span>

<span data-ttu-id="a1a62-104">L’élément **FindMessageTrackingReport** spécifie les critères pour les types de messages à rechercher.</span><span class="sxs-lookup"><span data-stu-id="a1a62-104">The **FindMessageTrackingReport** element specifies criteria for the types of messages to find.</span></span> 
  
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

 <span data-ttu-id="a1a62-105">**FindMessageTrackingReportRequestType**</span><span class="sxs-lookup"><span data-stu-id="a1a62-105">**FindMessageTrackingReportRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a1a62-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a1a62-106">Attributes and elements</span></span>

<span data-ttu-id="a1a62-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a1a62-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a1a62-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a1a62-108">Attributes</span></span>

<span data-ttu-id="a1a62-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="a1a62-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a1a62-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a1a62-110">Child elements</span></span>

|<span data-ttu-id="a1a62-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a1a62-111">**Element**</span></span>|<span data-ttu-id="a1a62-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="a1a62-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a1a62-113">Étendue (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="a1a62-113">Scope (NonEmptyStringType)</span></span>](scope-nonemptystringtype.md) <br/> |<span data-ttu-id="a1a62-114">Représente l’étendue du rapport de suivi des messages.</span><span class="sxs-lookup"><span data-stu-id="a1a62-114">Represents how extensive the message tracking report should be.</span></span>  <br/> |
|[<span data-ttu-id="a1a62-115">Domaine (suivi des messages)</span><span class="sxs-lookup"><span data-stu-id="a1a62-115">Domain (Message Tracking)</span></span>](domain-message-tracking.md) <br/> |<span data-ttu-id="a1a62-116">Contient le nom du domaine dans lequel le suivi des messages est exécuté.</span><span class="sxs-lookup"><span data-stu-id="a1a62-116">Contains the name of the domain where the message tracking is executed.</span></span>  <br/> |
|[<span data-ttu-id="a1a62-117">Expéditeur (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="a1a62-117">Sender (EmailAddressType)</span></span>](sender-emailaddresstype.md) <br/> |<span data-ttu-id="a1a62-118">Contient des informations de contact pour l’expéditeur du message électronique.</span><span class="sxs-lookup"><span data-stu-id="a1a62-118">Contains contact information for the sender of the e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="a1a62-119">PurportedSender</span><span class="sxs-lookup"><span data-stu-id="a1a62-119">PurportedSender</span></span>](purportedsender.md) <br/> |<span data-ttu-id="a1a62-120">Contient les informations de contact pour l’expéditeur allégué d’un message électronique.</span><span class="sxs-lookup"><span data-stu-id="a1a62-120">Contains contact information for the alleged sender of an e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="a1a62-121">Destinataire</span><span class="sxs-lookup"><span data-stu-id="a1a62-121">Recipient</span></span>](recipient.md) <br/> |<span data-ttu-id="a1a62-122">Contient l’adresse de messagerie du destinataire du message.</span><span class="sxs-lookup"><span data-stu-id="a1a62-122">Contains the e-mail address for the recipient of the message.</span></span>  <br/> |
|[<span data-ttu-id="a1a62-123">Subject</span><span class="sxs-lookup"><span data-stu-id="a1a62-123">Subject</span></span>](subject.md) <br/> |<span data-ttu-id="a1a62-124">Contient l’objet du message électronique.</span><span class="sxs-lookup"><span data-stu-id="a1a62-124">Contains the subject of the e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="a1a62-125">StartDateTime</span><span class="sxs-lookup"><span data-stu-id="a1a62-125">StartDateTime</span></span>](startdatetime.md) <br/> |<span data-ttu-id="a1a62-126">Contient la date et l’heure de début de la recherche.</span><span class="sxs-lookup"><span data-stu-id="a1a62-126">Contains the starting date and time for the search.</span></span>  <br/> |
|[<span data-ttu-id="a1a62-127">EndDateTime</span><span class="sxs-lookup"><span data-stu-id="a1a62-127">EndDateTime</span></span>](enddatetime.md) <br/> |<span data-ttu-id="a1a62-128">Contient la date et l’heure de fin de la recherche.</span><span class="sxs-lookup"><span data-stu-id="a1a62-128">Contains the ending date and time for the search.</span></span>  <br/> |
|[<span data-ttu-id="a1a62-129">MessageId</span><span class="sxs-lookup"><span data-stu-id="a1a62-129">MessageId</span></span>](messageid.md) <br/> |<span data-ttu-id="a1a62-130">Contient l’identificateur de message de la recherche.</span><span class="sxs-lookup"><span data-stu-id="a1a62-130">Contains the message identifier for the search.</span></span>  <br/> |
|[<span data-ttu-id="a1a62-131">FederatedDeliveryMailbox</span><span class="sxs-lookup"><span data-stu-id="a1a62-131">FederatedDeliveryMailbox</span></span>](federateddeliverymailbox.md) <br/> |<span data-ttu-id="a1a62-132">Contient le nom de la boîte aux lettres à laquelle le message intersites a été envoyé.</span><span class="sxs-lookup"><span data-stu-id="a1a62-132">Contains the name of the mailbox where the cross-premise message was sent.</span></span>  <br/> |
|[<span data-ttu-id="a1a62-133">DiagnosticsLevel</span><span class="sxs-lookup"><span data-stu-id="a1a62-133">DiagnosticsLevel</span></span>](diagnosticslevel.md) <br/> |<span data-ttu-id="a1a62-134">Représente le niveau de détail des rapports de diagnostic.</span><span class="sxs-lookup"><span data-stu-id="a1a62-134">Represents the level of detail for diagnostic reports.</span></span>  <br/> |
|[<span data-ttu-id="a1a62-135">ServerHint</span><span class="sxs-lookup"><span data-stu-id="a1a62-135">ServerHint</span></span>](serverhint.md) <br/> |<span data-ttu-id="a1a62-136">Représente le point de départ pour le suivi d’un message dans un site ou une forêt distante.</span><span class="sxs-lookup"><span data-stu-id="a1a62-136">Represents the starting point for tracking a message in a remote site or forest.</span></span>  <br/> |
|[<span data-ttu-id="a1a62-137">Propriétés (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="a1a62-137">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="a1a62-138">Contient une liste d’une ou plusieurs propriétés de suivi.</span><span class="sxs-lookup"><span data-stu-id="a1a62-138">Contains a list of one or more tracking properties.</span></span> <span data-ttu-id="a1a62-139">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="a1a62-139">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a1a62-140">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a1a62-140">Parent elements</span></span>

<span data-ttu-id="a1a62-141">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a1a62-141">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="a1a62-142">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="a1a62-142">Text value</span></span>

<span data-ttu-id="a1a62-143">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a1a62-143">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a1a62-144">Remarques</span><span class="sxs-lookup"><span data-stu-id="a1a62-144">Remarks</span></span>

<span data-ttu-id="a1a62-145">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a1a62-145">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a1a62-146">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a1a62-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a1a62-147">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a1a62-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a1a62-148">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a1a62-148">Schema Name</span></span>  <br/> |<span data-ttu-id="a1a62-149">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="a1a62-149">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a1a62-150">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a1a62-150">Validation File</span></span>  <br/> |<span data-ttu-id="a1a62-151">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="a1a62-151">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a1a62-152">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a1a62-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="a1a62-153">False</span><span class="sxs-lookup"><span data-stu-id="a1a62-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a1a62-154">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a1a62-154">See also</span></span>



[<span data-ttu-id="a1a62-155">Opération FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="a1a62-155">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)


- [<span data-ttu-id="a1a62-156">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a1a62-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

