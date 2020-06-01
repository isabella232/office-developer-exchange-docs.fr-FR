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
ms.openlocfilehash: e90c44dd4124d698ca5ef7655f6429a7167673e6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44465785"
---
# <a name="meetingrequesttype"></a><span data-ttu-id="25e2a-103">MeetingRequestType</span><span class="sxs-lookup"><span data-stu-id="25e2a-103">MeetingRequestType</span></span>

<span data-ttu-id="25e2a-104">L’élément **MeetingRequestType** décrit le type de la demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="25e2a-104">The **MeetingRequestType** element describes the type of the meeting request.</span></span> 
  
```xml
<MeetingRequestType/>
```

 <span data-ttu-id="25e2a-105">**MeetingRequestTypeType**</span><span class="sxs-lookup"><span data-stu-id="25e2a-105">**MeetingRequestTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="25e2a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="25e2a-106">Attributes and elements</span></span>

<span data-ttu-id="25e2a-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="25e2a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="25e2a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="25e2a-108">Attributes</span></span>

<span data-ttu-id="25e2a-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="25e2a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="25e2a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="25e2a-110">Child elements</span></span>

<span data-ttu-id="25e2a-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="25e2a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="25e2a-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="25e2a-112">Parent elements</span></span>

|<span data-ttu-id="25e2a-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="25e2a-113">**Element**</span></span>|<span data-ttu-id="25e2a-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="25e2a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="25e2a-115">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="25e2a-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="25e2a-116">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="25e2a-116">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="25e2a-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="25e2a-117">Text value</span></span>

<span data-ttu-id="25e2a-118">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="25e2a-118">A text value is required.</span></span> <span data-ttu-id="25e2a-119">Le tableau suivant répertorie les valeurs de texte possibles pour cet élément.</span><span class="sxs-lookup"><span data-stu-id="25e2a-119">The following table lists the possible text values for this element.</span></span>
  
|<span data-ttu-id="25e2a-120">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="25e2a-120">**Value**</span></span>|<span data-ttu-id="25e2a-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="25e2a-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="25e2a-122">FullUpdate</span><span class="sxs-lookup"><span data-stu-id="25e2a-122">FullUpdate</span></span>  <br/> |<span data-ttu-id="25e2a-123">Identifie la demande de réunion en tant que mise à jour complète d’une demande existante.</span><span class="sxs-lookup"><span data-stu-id="25e2a-123">Identifies the meeting request as a full update to an existing request.</span></span> <span data-ttu-id="25e2a-124">Une mise à jour complète a mis à jour le contenu horaire et informatif.</span><span class="sxs-lookup"><span data-stu-id="25e2a-124">A full update has updated time and informational content.</span></span>  <br/> |
|<span data-ttu-id="25e2a-125">InformationalUpdate</span><span class="sxs-lookup"><span data-stu-id="25e2a-125">InformationalUpdate</span></span>  <br/> |<span data-ttu-id="25e2a-126">Identifie la demande de réunion uniquement avec le contenu informatif mis à jour.</span><span class="sxs-lookup"><span data-stu-id="25e2a-126">Identifies the meeting request as only containing updated informational content.</span></span>  <br/> |
|<span data-ttu-id="25e2a-127">NewMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="25e2a-127">NewMeetingRequest</span></span>  <br/> |<span data-ttu-id="25e2a-128">Identifie la demande de réunion en tant que nouvelle demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="25e2a-128">Identifies the meeting request as a new meeting request.</span></span>  <br/> |
|<span data-ttu-id="25e2a-129">Aucun</span><span class="sxs-lookup"><span data-stu-id="25e2a-129">None</span></span>  <br/> |<span data-ttu-id="25e2a-130">Indique que le type de demande de réunion n’est pas défini.</span><span class="sxs-lookup"><span data-stu-id="25e2a-130">Indicates that the meeting request type is not defined.</span></span>  <br/> |
|<span data-ttu-id="25e2a-131">Obsolètes</span><span class="sxs-lookup"><span data-stu-id="25e2a-131">Outdated</span></span>  <br/> |<span data-ttu-id="25e2a-132">Identifie la demande de réunion comme étant obsolète.</span><span class="sxs-lookup"><span data-stu-id="25e2a-132">Identifies the meeting request as outdated.</span></span>  <br/> |
|<span data-ttu-id="25e2a-133">PrincipalWantsCopy</span><span class="sxs-lookup"><span data-stu-id="25e2a-133">PrincipalWantsCopy</span></span>  <br/> |<span data-ttu-id="25e2a-134">Indique que la demande de réunion appartient à un principal qui a transféré des messages de réunion à un délégué et que ses copies sont marquées comme informations.</span><span class="sxs-lookup"><span data-stu-id="25e2a-134">Indicates that the meeting request belongs to a principal who has forwarded meeting messages to a delegate and has his copies marked as informational.</span></span>  <br/> |
|<span data-ttu-id="25e2a-135">SilentUpdate</span><span class="sxs-lookup"><span data-stu-id="25e2a-135">SilentUpdate</span></span>  <br/> |<span data-ttu-id="25e2a-136">Identifie la demande de réunion en tant que mise à jour silencieuse d’une réunion existante.</span><span class="sxs-lookup"><span data-stu-id="25e2a-136">Identifies the meeting request as a silent update to an existing meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="25e2a-137">Remarques</span><span class="sxs-lookup"><span data-stu-id="25e2a-137">Remarks</span></span>

<span data-ttu-id="25e2a-138">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="25e2a-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="25e2a-139">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="25e2a-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="25e2a-140">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="25e2a-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="25e2a-141">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="25e2a-141">Schema Name</span></span>  <br/> |<span data-ttu-id="25e2a-142">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="25e2a-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="25e2a-143">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="25e2a-143">Validation File</span></span>  <br/> |<span data-ttu-id="25e2a-144">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="25e2a-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="25e2a-145">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="25e2a-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="25e2a-146">False</span><span class="sxs-lookup"><span data-stu-id="25e2a-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="25e2a-147">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="25e2a-147">See also</span></span>



- [<span data-ttu-id="25e2a-148">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="25e2a-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

