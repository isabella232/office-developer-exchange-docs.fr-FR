---
title: PhoneCallState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PhoneCallState
api_type:
- schema
ms.assetid: ac009eb3-6334-49ce-82be-48fe83577f9c
description: L’élément PhoneCallState spécifie l’état actuel d’un appel téléphonique.
ms.openlocfilehash: d2088b9b2811befe80684188d49c8034c577cc55
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468529"
---
# <a name="phonecallstate"></a><span data-ttu-id="f82d3-103">PhoneCallState</span><span class="sxs-lookup"><span data-stu-id="f82d3-103">PhoneCallState</span></span>

<span data-ttu-id="f82d3-104">L’élément **PhoneCallState** spécifie l’état actuel d’un appel téléphonique.</span><span class="sxs-lookup"><span data-stu-id="f82d3-104">The **PhoneCallState** element specifies the current state for a phone call.</span></span> 
  
```xml
<PhoneCallState>Idle or Connecting or Alerted or Connected or Disconnected or Incoming or Transferring or Forwarding</PhoneCallState>
```

 <span data-ttu-id="f82d3-105">**PhoneCallStateType**</span><span class="sxs-lookup"><span data-stu-id="f82d3-105">**PhoneCallStateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f82d3-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f82d3-106">Attributes and elements</span></span>

<span data-ttu-id="f82d3-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f82d3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f82d3-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f82d3-108">Attributes</span></span>

<span data-ttu-id="f82d3-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f82d3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f82d3-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f82d3-110">Child elements</span></span>

<span data-ttu-id="f82d3-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f82d3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f82d3-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f82d3-112">Parent elements</span></span>

|<span data-ttu-id="f82d3-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f82d3-113">**Element**</span></span>|<span data-ttu-id="f82d3-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="f82d3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f82d3-115">PhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="f82d3-115">PhoneCallInformation</span></span>](phonecallinformation.md) <br/> |<span data-ttu-id="f82d3-116">Spécifie les informations d’État pour un appel téléphonique.</span><span class="sxs-lookup"><span data-stu-id="f82d3-116">Specifies the state information for a phone call.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f82d3-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="f82d3-117">Text value</span></span>

<span data-ttu-id="f82d3-118">Le tableau suivant répertorie les valeurs possibles pour l’élément **PhoneCallState** .</span><span class="sxs-lookup"><span data-stu-id="f82d3-118">The following table lists the possible values for the **PhoneCallState** element.</span></span> 
  
<span data-ttu-id="f82d3-119">**Valeurs de l’élément PhoneCallState**</span><span class="sxs-lookup"><span data-stu-id="f82d3-119">**PhoneCallState element values**</span></span>

|<span data-ttu-id="f82d3-120">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="f82d3-120">**Value**</span></span>|<span data-ttu-id="f82d3-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="f82d3-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f82d3-122">Engrenage</span><span class="sxs-lookup"><span data-stu-id="f82d3-122">Idle</span></span>  <br/> |<span data-ttu-id="f82d3-123">État initial de l’appel.</span><span class="sxs-lookup"><span data-stu-id="f82d3-123">Initial call state.</span></span>  <br/> |
|<span data-ttu-id="f82d3-124">Connexion</span><span class="sxs-lookup"><span data-stu-id="f82d3-124">Connecting</span></span>  <br/> |<span data-ttu-id="f82d3-125">Le système compose cet appel.</span><span class="sxs-lookup"><span data-stu-id="f82d3-125">The system is dialing this call.</span></span>  <br/> |
|<span data-ttu-id="f82d3-126">Averti</span><span class="sxs-lookup"><span data-stu-id="f82d3-126">Alerted</span></span>  <br/> |<span data-ttu-id="f82d3-127">L’appel est en état d’alerte (sonnerie du téléphone).</span><span class="sxs-lookup"><span data-stu-id="f82d3-127">The call is in alerting state (phone is ringing).</span></span>  <br/> |
|<span data-ttu-id="f82d3-128">Connecté</span><span class="sxs-lookup"><span data-stu-id="f82d3-128">Connected</span></span>  <br/> |<span data-ttu-id="f82d3-129">L’appel est à l’état connecté.</span><span class="sxs-lookup"><span data-stu-id="f82d3-129">The call is in the connected state.</span></span>  <br/> |
|<span data-ttu-id="f82d3-130">Déconnecté</span><span class="sxs-lookup"><span data-stu-id="f82d3-130">Disconnected</span></span>  <br/> |<span data-ttu-id="f82d3-131">L’appel est déconnecté.</span><span class="sxs-lookup"><span data-stu-id="f82d3-131">The call is disconnected.</span></span>  <br/> |
|<span data-ttu-id="f82d3-132">Entrant</span><span class="sxs-lookup"><span data-stu-id="f82d3-132">Incoming</span></span>  <br/> |<span data-ttu-id="f82d3-133">L’appel est entrant.</span><span class="sxs-lookup"><span data-stu-id="f82d3-133">The call is inbound.</span></span>  <br/> |
|<span data-ttu-id="f82d3-134">Transférés</span><span class="sxs-lookup"><span data-stu-id="f82d3-134">Transferring</span></span>  <br/> |<span data-ttu-id="f82d3-135">L’appel est transféré vers une autre destination.</span><span class="sxs-lookup"><span data-stu-id="f82d3-135">The call is being transferred to another destination.</span></span>  <br/> |
|<span data-ttu-id="f82d3-136">Transfert</span><span class="sxs-lookup"><span data-stu-id="f82d3-136">Forwarding</span></span>  <br/> |<span data-ttu-id="f82d3-137">L’appel est transféré vers une autre destination.</span><span class="sxs-lookup"><span data-stu-id="f82d3-137">The call is being forwarded to another destination.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f82d3-138">Remarques</span><span class="sxs-lookup"><span data-stu-id="f82d3-138">Remarks</span></span>

<span data-ttu-id="f82d3-139">Le schéma qui décrit cet élément se trouve dans le répertoire/EWS/de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="f82d3-139">The schema that describes this element is located in the /ews/ directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f82d3-140">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f82d3-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f82d3-141">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f82d3-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f82d3-142">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f82d3-142">Schema Name</span></span>  <br/> |<span data-ttu-id="f82d3-143">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="f82d3-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="f82d3-144">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f82d3-144">Validation File</span></span>  <br/> |<span data-ttu-id="f82d3-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f82d3-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f82d3-146">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f82d3-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="f82d3-147">False</span><span class="sxs-lookup"><span data-stu-id="f82d3-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f82d3-148">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f82d3-148">See also</span></span>



- [<span data-ttu-id="f82d3-149">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f82d3-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

