---
title: ConnectionFailureCause
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConnectionFailureCause
api_type:
- schema
ms.assetid: d2160c8a-015c-4964-b7f7-93478764a173
description: L’élément ConnectionFailureCause spécifie la raison d’une déconnexion d’un appel téléphonique.
ms.openlocfilehash: 54b4f5b89efdb42ef82dbef8f1af14a39c0ccc6a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755542"
---
# <a name="connectionfailurecause"></a><span data-ttu-id="59416-103">ConnectionFailureCause</span><span class="sxs-lookup"><span data-stu-id="59416-103">ConnectionFailureCause</span></span>

<span data-ttu-id="59416-104">L’élément **ConnectionFailureCause** spécifie la raison d’une déconnexion d’un appel téléphonique.</span><span class="sxs-lookup"><span data-stu-id="59416-104">The **ConnectionFailureCause** element specifies the reason for a disconnection from a telephone call.</span></span> 
  
```xml
<ConnectionFailureCause>None or UserBusy or NoAnswer or Unavailable or Other</ConnectionFailureCause>
```

 <span data-ttu-id="59416-105">**ConnectionFailureCauseType**</span><span class="sxs-lookup"><span data-stu-id="59416-105">**ConnectionFailureCauseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="59416-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="59416-106">Attributes and elements</span></span>

<span data-ttu-id="59416-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="59416-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="59416-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="59416-108">Attributes</span></span>

<span data-ttu-id="59416-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="59416-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="59416-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="59416-110">Child elements</span></span>

<span data-ttu-id="59416-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="59416-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="59416-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="59416-112">Parent elements</span></span>

|<span data-ttu-id="59416-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="59416-113">**Element**</span></span>|<span data-ttu-id="59416-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="59416-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="59416-115">PhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="59416-115">PhoneCallInformation</span></span>](phonecallinformation.md) <br/> |<span data-ttu-id="59416-116">Spécifie les informations d’état pour un appel téléphonique.</span><span class="sxs-lookup"><span data-stu-id="59416-116">Specifies the state information for a telephone call.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="59416-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="59416-117">Text value</span></span>

<span data-ttu-id="59416-118">Le tableau suivant répertorie les valeurs possibles pour l’élément **ConnectionFailureCause** .</span><span class="sxs-lookup"><span data-stu-id="59416-118">The following table lists the possible values for the **ConnectionFailureCause** element.</span></span> 
  
<span data-ttu-id="59416-119">**Valeurs des éléments ConnectionFailureCause**</span><span class="sxs-lookup"><span data-stu-id="59416-119">**ConnectionFailureCause element values**</span></span>

|<span data-ttu-id="59416-120">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="59416-120">**Value**</span></span>|<span data-ttu-id="59416-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="59416-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="59416-122">None</span><span class="sxs-lookup"><span data-stu-id="59416-122">None</span></span>  <br/> |<span data-ttu-id="59416-123">État d’appel n’est pas déconnecté ou la raison de déconnexion n’est pas connue.</span><span class="sxs-lookup"><span data-stu-id="59416-123">Call state is not disconnected or the disconnect reason is not known.</span></span>  <br/> |
|<span data-ttu-id="59416-124">UserBusy</span><span class="sxs-lookup"><span data-stu-id="59416-124">UserBusy</span></span>  <br/> |<span data-ttu-id="59416-125">La ligne de la partie appelée était occupée.</span><span class="sxs-lookup"><span data-stu-id="59416-125">The called party line was busy.</span></span>  <br/> |
|<span data-ttu-id="59416-126">NoAnswer</span><span class="sxs-lookup"><span data-stu-id="59416-126">NoAnswer</span></span>  <br/> |<span data-ttu-id="59416-127">La personne appelée ne répond pas.</span><span class="sxs-lookup"><span data-stu-id="59416-127">The called party did not answer.</span></span>  <br/> |
|<span data-ttu-id="59416-128">Unavailable</span><span class="sxs-lookup"><span data-stu-id="59416-128">Unavailable</span></span>  <br/> |<span data-ttu-id="59416-129">Le numéro appelé n’était pas disponible.</span><span class="sxs-lookup"><span data-stu-id="59416-129">The called party number was not available.</span></span>  <br/> |
|<span data-ttu-id="59416-130">Other</span><span class="sxs-lookup"><span data-stu-id="59416-130">Other</span></span>  <br/> |<span data-ttu-id="59416-131">Fourre-tout pour d’autres raisons de déconnexion.</span><span class="sxs-lookup"><span data-stu-id="59416-131">Catch-all for other disconnect reasons.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="59416-132">Remarques</span><span class="sxs-lookup"><span data-stu-id="59416-132">Remarks</span></span>

<span data-ttu-id="59416-133">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="59416-133">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="59416-134">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="59416-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="59416-135">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="59416-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="59416-136">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="59416-136">Schema Name</span></span>  <br/> |<span data-ttu-id="59416-137">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="59416-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="59416-138">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="59416-138">Validation File</span></span>  <br/> |<span data-ttu-id="59416-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="59416-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="59416-140">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="59416-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="59416-141">False</span><span class="sxs-lookup"><span data-stu-id="59416-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="59416-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="59416-142">See also</span></span>



- [<span data-ttu-id="59416-143">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="59416-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
