---
title: MeetingRequestType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingRequestType
api_type:
- schema
ms.assetid: bcd5c97c-19aa-4b1d-a8e8-e8c4bd473dd9
description: L’élément MeetingRequestType décrit le type de la demande de réunion.
ms.openlocfilehash: 7269587e2fa72aeb9070a7b53ee9215829729329
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828432"
---
# <a name="meetingrequesttype"></a><span data-ttu-id="df946-103">MeetingRequestType</span><span class="sxs-lookup"><span data-stu-id="df946-103">MeetingRequestType</span></span>

<span data-ttu-id="df946-104">L’élément **MeetingRequestType** décrit le type de la demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="df946-104">The **MeetingRequestType** element describes the type of the meeting request.</span></span> 
  
```xml
<MeetingRequestType/>
```

 <span data-ttu-id="df946-105">**MeetingRequestTypeType**</span><span class="sxs-lookup"><span data-stu-id="df946-105">**MeetingRequestTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="df946-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="df946-106">Attributes and elements</span></span>

<span data-ttu-id="df946-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="df946-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="df946-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="df946-108">Attributes</span></span>

<span data-ttu-id="df946-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="df946-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="df946-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="df946-110">Child elements</span></span>

<span data-ttu-id="df946-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="df946-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="df946-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="df946-112">Parent elements</span></span>

|<span data-ttu-id="df946-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="df946-113">**Element**</span></span>|<span data-ttu-id="df946-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="df946-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="df946-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="df946-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="df946-116">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="df946-116">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="df946-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="df946-117">Text value</span></span>

<span data-ttu-id="df946-118">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="df946-118">A text value is required.</span></span> <span data-ttu-id="df946-119">Le tableau suivant répertorie les valeurs de texte possibles pour cet élément.</span><span class="sxs-lookup"><span data-stu-id="df946-119">The following table lists the possible text values for this element.</span></span>
  
|<span data-ttu-id="df946-120">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="df946-120">**Value**</span></span>|<span data-ttu-id="df946-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="df946-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="df946-122">FullUpdate</span><span class="sxs-lookup"><span data-stu-id="df946-122">FullUpdate</span></span>  <br/> |<span data-ttu-id="df946-123">Identifie la demande de réunion en tant qu’une mise à jour complète pour une requête existante.</span><span class="sxs-lookup"><span data-stu-id="df946-123">Identifies the meeting request as a full update to an existing request.</span></span> <span data-ttu-id="df946-124">Une mise à jour intégrale a mis à jour le contenu d’information et du temps.</span><span class="sxs-lookup"><span data-stu-id="df946-124">A full update has updated time and informational content.</span></span>  <br/> |
|<span data-ttu-id="df946-125">InformationalUpdate</span><span class="sxs-lookup"><span data-stu-id="df946-125">InformationalUpdate</span></span>  <br/> |<span data-ttu-id="df946-126">Identifie la demande de réunion contenant uniquement de mise à jour le contenu d’information.</span><span class="sxs-lookup"><span data-stu-id="df946-126">Identifies the meeting request as only containing updated informational content.</span></span>  <br/> |
|<span data-ttu-id="df946-127">NewMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="df946-127">NewMeetingRequest</span></span>  <br/> |<span data-ttu-id="df946-128">Identifie la demande de réunion en tant qu’une nouvelle demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="df946-128">Identifies the meeting request as a new meeting request.</span></span>  <br/> |
|<span data-ttu-id="df946-129">Aucun</span><span class="sxs-lookup"><span data-stu-id="df946-129">None</span></span>  <br/> |<span data-ttu-id="df946-130">Indique que la demande de réunion type n’est pas défini.</span><span class="sxs-lookup"><span data-stu-id="df946-130">Indicates that the meeting request type is not defined.</span></span>  <br/> |
|<span data-ttu-id="df946-131">Obsolètes</span><span class="sxs-lookup"><span data-stu-id="df946-131">Outdated</span></span>  <br/> |<span data-ttu-id="df946-132">Identifie la demande de réunion est obsolète.</span><span class="sxs-lookup"><span data-stu-id="df946-132">Identifies the meeting request as outdated.</span></span>  <br/> |
|<span data-ttu-id="df946-133">PrincipalWantsCopy</span><span class="sxs-lookup"><span data-stu-id="df946-133">PrincipalWantsCopy</span></span>  <br/> |<span data-ttu-id="df946-134">Indique que la demande de réunion appartient à une entité qui a transféré des messages de réunion à un délégué et sa copie marqué comme d’information.</span><span class="sxs-lookup"><span data-stu-id="df946-134">Indicates that the meeting request belongs to a principal who has forwarded meeting messages to a delegate and has his copies marked as informational.</span></span>  <br/> |
|<span data-ttu-id="df946-135">SilentUpdate</span><span class="sxs-lookup"><span data-stu-id="df946-135">SilentUpdate</span></span>  <br/> |<span data-ttu-id="df946-136">Identifie la demande de réunion en tant qu’une mise à jour en mode silencieux à une réunion existante.</span><span class="sxs-lookup"><span data-stu-id="df946-136">Identifies the meeting request as a silent update to an existing meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="df946-137">Remarques</span><span class="sxs-lookup"><span data-stu-id="df946-137">Remarks</span></span>

<span data-ttu-id="df946-138">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="df946-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="df946-139">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="df946-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="df946-140">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="df946-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="df946-141">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="df946-141">Schema Name</span></span>  <br/> |<span data-ttu-id="df946-142">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="df946-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="df946-143">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="df946-143">Validation File</span></span>  <br/> |<span data-ttu-id="df946-144">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="df946-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="df946-145">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="df946-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="df946-146">False</span><span class="sxs-lookup"><span data-stu-id="df946-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="df946-147">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="df946-147">See also</span></span>



- [<span data-ttu-id="df946-148">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="df946-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

