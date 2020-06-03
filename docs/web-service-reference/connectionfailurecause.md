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
description: L’élément ConnectionFailureCause spécifie la raison pour laquelle une déconnexion à partir d’un appel téléphonique.
ms.openlocfilehash: 6385641eaee140a114906703232974d51d5ce344
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529447"
---
# <a name="connectionfailurecause"></a><span data-ttu-id="73d9a-103">ConnectionFailureCause</span><span class="sxs-lookup"><span data-stu-id="73d9a-103">ConnectionFailureCause</span></span>

<span data-ttu-id="73d9a-104">L’élément **ConnectionFailureCause** spécifie la raison pour laquelle une déconnexion à partir d’un appel téléphonique.</span><span class="sxs-lookup"><span data-stu-id="73d9a-104">The **ConnectionFailureCause** element specifies the reason for a disconnection from a telephone call.</span></span> 
  
```xml
<ConnectionFailureCause>None or UserBusy or NoAnswer or Unavailable or Other</ConnectionFailureCause>
```

 <span data-ttu-id="73d9a-105">**ConnectionFailureCauseType**</span><span class="sxs-lookup"><span data-stu-id="73d9a-105">**ConnectionFailureCauseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="73d9a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="73d9a-106">Attributes and elements</span></span>

<span data-ttu-id="73d9a-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="73d9a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="73d9a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="73d9a-108">Attributes</span></span>

<span data-ttu-id="73d9a-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="73d9a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="73d9a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="73d9a-110">Child elements</span></span>

<span data-ttu-id="73d9a-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="73d9a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="73d9a-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="73d9a-112">Parent elements</span></span>

|<span data-ttu-id="73d9a-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="73d9a-113">**Element**</span></span>|<span data-ttu-id="73d9a-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="73d9a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="73d9a-115">PhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="73d9a-115">PhoneCallInformation</span></span>](phonecallinformation.md) <br/> |<span data-ttu-id="73d9a-116">Spécifie les informations d’État pour un appel téléphonique.</span><span class="sxs-lookup"><span data-stu-id="73d9a-116">Specifies the state information for a telephone call.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="73d9a-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="73d9a-117">Text value</span></span>

<span data-ttu-id="73d9a-118">Le tableau suivant répertorie les valeurs possibles pour l’élément **ConnectionFailureCause** .</span><span class="sxs-lookup"><span data-stu-id="73d9a-118">The following table lists the possible values for the **ConnectionFailureCause** element.</span></span> 
  
<span data-ttu-id="73d9a-119">**Valeurs de l’élément ConnectionFailureCause**</span><span class="sxs-lookup"><span data-stu-id="73d9a-119">**ConnectionFailureCause element values**</span></span>

|<span data-ttu-id="73d9a-120">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="73d9a-120">**Value**</span></span>|<span data-ttu-id="73d9a-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="73d9a-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="73d9a-122">Aucun</span><span class="sxs-lookup"><span data-stu-id="73d9a-122">None</span></span>  <br/> |<span data-ttu-id="73d9a-123">L’état de l’appel n’est pas déconnecté ou le motif de déconnexion n’est pas connu.</span><span class="sxs-lookup"><span data-stu-id="73d9a-123">Call state is not disconnected or the disconnect reason is not known.</span></span>  <br/> |
|<span data-ttu-id="73d9a-124">UserBusy</span><span class="sxs-lookup"><span data-stu-id="73d9a-124">UserBusy</span></span>  <br/> |<span data-ttu-id="73d9a-125">La ligne de partie appelée était occupée.</span><span class="sxs-lookup"><span data-stu-id="73d9a-125">The called party line was busy.</span></span>  <br/> |
|<span data-ttu-id="73d9a-126">Noanswer</span><span class="sxs-lookup"><span data-stu-id="73d9a-126">NoAnswer</span></span>  <br/> |<span data-ttu-id="73d9a-127">La partie appelée n’a pas répondu.</span><span class="sxs-lookup"><span data-stu-id="73d9a-127">The called party did not answer.</span></span>  <br/> |
|<span data-ttu-id="73d9a-128">Indisponible</span><span class="sxs-lookup"><span data-stu-id="73d9a-128">Unavailable</span></span>  <br/> |<span data-ttu-id="73d9a-129">Le numéro de partie appelé n’était pas disponible.</span><span class="sxs-lookup"><span data-stu-id="73d9a-129">The called party number was not available.</span></span>  <br/> |
|<span data-ttu-id="73d9a-130">Autres</span><span class="sxs-lookup"><span data-stu-id="73d9a-130">Other</span></span>  <br/> |<span data-ttu-id="73d9a-131">Rattraper-tout pour d’autres raisons de déconnexion.</span><span class="sxs-lookup"><span data-stu-id="73d9a-131">Catch-all for other disconnect reasons.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="73d9a-132">Remarques</span><span class="sxs-lookup"><span data-stu-id="73d9a-132">Remarks</span></span>

<span data-ttu-id="73d9a-133">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="73d9a-133">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="73d9a-134">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="73d9a-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="73d9a-135">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="73d9a-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="73d9a-136">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="73d9a-136">Schema Name</span></span>  <br/> |<span data-ttu-id="73d9a-137">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="73d9a-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="73d9a-138">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="73d9a-138">Validation File</span></span>  <br/> |<span data-ttu-id="73d9a-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="73d9a-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="73d9a-140">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="73d9a-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="73d9a-141">False</span><span class="sxs-lookup"><span data-stu-id="73d9a-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="73d9a-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="73d9a-142">See also</span></span>



- [<span data-ttu-id="73d9a-143">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="73d9a-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

