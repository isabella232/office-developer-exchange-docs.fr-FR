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
description: L’élément PhoneCallState Spécifie l’état actuel d’un appel téléphonique.
ms.openlocfilehash: 184a7400810711442e565d1ef37094bd63b00914
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828761"
---
# <a name="phonecallstate"></a><span data-ttu-id="f1cbe-103">PhoneCallState</span><span class="sxs-lookup"><span data-stu-id="f1cbe-103">PhoneCallState</span></span>

<span data-ttu-id="f1cbe-104">L’élément **PhoneCallState** Spécifie l’état actuel d’un appel téléphonique.</span><span class="sxs-lookup"><span data-stu-id="f1cbe-104">The **PhoneCallState** element specifies the current state for a phone call.</span></span> 
  
```xml
<PhoneCallState>Idle or Connecting or Alerted or Connected or Disconnected or Incoming or Transferring or Forwarding</PhoneCallState>
```

 <span data-ttu-id="f1cbe-105">**PhoneCallStateType**</span><span class="sxs-lookup"><span data-stu-id="f1cbe-105">**PhoneCallStateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f1cbe-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f1cbe-106">Attributes and elements</span></span>

<span data-ttu-id="f1cbe-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f1cbe-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f1cbe-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f1cbe-108">Attributes</span></span>

<span data-ttu-id="f1cbe-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f1cbe-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f1cbe-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f1cbe-110">Child elements</span></span>

<span data-ttu-id="f1cbe-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f1cbe-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f1cbe-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f1cbe-112">Parent elements</span></span>

|<span data-ttu-id="f1cbe-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f1cbe-113">**Element**</span></span>|<span data-ttu-id="f1cbe-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="f1cbe-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f1cbe-115">PhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="f1cbe-115">PhoneCallInformation</span></span>](phonecallinformation.md) <br/> |<span data-ttu-id="f1cbe-116">Spécifie les informations d’état pour un appel téléphonique.</span><span class="sxs-lookup"><span data-stu-id="f1cbe-116">Specifies the state information for a phone call.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f1cbe-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="f1cbe-117">Text value</span></span>

<span data-ttu-id="f1cbe-118">Le tableau suivant répertorie les valeurs possibles pour l’élément **PhoneCallState** .</span><span class="sxs-lookup"><span data-stu-id="f1cbe-118">The following table lists the possible values for the **PhoneCallState** element.</span></span> 
  
<span data-ttu-id="f1cbe-119">**Valeurs des éléments PhoneCallState**</span><span class="sxs-lookup"><span data-stu-id="f1cbe-119">**PhoneCallState element values**</span></span>

|<span data-ttu-id="f1cbe-120">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="f1cbe-120">**Value**</span></span>|<span data-ttu-id="f1cbe-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="f1cbe-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f1cbe-122">Inactif</span><span class="sxs-lookup"><span data-stu-id="f1cbe-122">Idle</span></span>  <br/> |<span data-ttu-id="f1cbe-123">État de l’appel initial.</span><span class="sxs-lookup"><span data-stu-id="f1cbe-123">Initial call state.</span></span>  <br/> |
|<span data-ttu-id="f1cbe-124">Connexion</span><span class="sxs-lookup"><span data-stu-id="f1cbe-124">Connecting</span></span>  <br/> |<span data-ttu-id="f1cbe-125">Le système appelle cet appel.</span><span class="sxs-lookup"><span data-stu-id="f1cbe-125">The system is dialing this call.</span></span>  <br/> |
|<span data-ttu-id="f1cbe-126">Alerté</span><span class="sxs-lookup"><span data-stu-id="f1cbe-126">Alerted</span></span>  <br/> |<span data-ttu-id="f1cbe-127">L’appel se trouve dans l’alerte d’état (téléphone sonne).</span><span class="sxs-lookup"><span data-stu-id="f1cbe-127">The call is in alerting state (phone is ringing).</span></span>  <br/> |
|<span data-ttu-id="f1cbe-128">Connecté</span><span class="sxs-lookup"><span data-stu-id="f1cbe-128">Connected</span></span>  <br/> |<span data-ttu-id="f1cbe-129">L’appel est dans l’état connecté.</span><span class="sxs-lookup"><span data-stu-id="f1cbe-129">The call is in the connected state.</span></span>  <br/> |
|<span data-ttu-id="f1cbe-130">Déconnecté</span><span class="sxs-lookup"><span data-stu-id="f1cbe-130">Disconnected</span></span>  <br/> |<span data-ttu-id="f1cbe-131">L’appel est déconnecté.</span><span class="sxs-lookup"><span data-stu-id="f1cbe-131">The call is disconnected.</span></span>  <br/> |
|<span data-ttu-id="f1cbe-132">Entrant</span><span class="sxs-lookup"><span data-stu-id="f1cbe-132">Incoming</span></span>  <br/> |<span data-ttu-id="f1cbe-133">L’appel est entrant.</span><span class="sxs-lookup"><span data-stu-id="f1cbe-133">The call is inbound.</span></span>  <br/> |
|<span data-ttu-id="f1cbe-134">Transfert</span><span class="sxs-lookup"><span data-stu-id="f1cbe-134">Transferring</span></span>  <br/> |<span data-ttu-id="f1cbe-135">L’appel est transféré vers une autre destination.</span><span class="sxs-lookup"><span data-stu-id="f1cbe-135">The call is being transferred to another destination.</span></span>  <br/> |
|<span data-ttu-id="f1cbe-136">Transfert</span><span class="sxs-lookup"><span data-stu-id="f1cbe-136">Forwarding</span></span>  <br/> |<span data-ttu-id="f1cbe-137">L’appel est transféré vers une autre destination.</span><span class="sxs-lookup"><span data-stu-id="f1cbe-137">The call is being forwarded to another destination.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f1cbe-138">Remarques</span><span class="sxs-lookup"><span data-stu-id="f1cbe-138">Remarks</span></span>

<span data-ttu-id="f1cbe-139">Le schéma qui décrit cet élément se trouve dans le répertoire /ews/ de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="f1cbe-139">The schema that describes this element is located in the /ews/ directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f1cbe-140">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f1cbe-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f1cbe-141">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f1cbe-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f1cbe-142">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f1cbe-142">Schema Name</span></span>  <br/> |<span data-ttu-id="f1cbe-143">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="f1cbe-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="f1cbe-144">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f1cbe-144">Validation File</span></span>  <br/> |<span data-ttu-id="f1cbe-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f1cbe-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f1cbe-146">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f1cbe-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="f1cbe-147">False</span><span class="sxs-lookup"><span data-stu-id="f1cbe-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f1cbe-148">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f1cbe-148">See also</span></span>



- [<span data-ttu-id="f1cbe-149">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f1cbe-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

