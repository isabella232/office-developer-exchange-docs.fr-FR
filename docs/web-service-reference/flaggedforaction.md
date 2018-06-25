---
title: FlaggedForAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FlaggedForAction
api_type:
- schema
ms.assetid: 6a08c48a-7b32-4754-8940-adbda55e8133
description: L’élément FlaggedForAction Spécifie l’indicateur pour la valeur d’action qui doit apparaître dans les messages entrants afin que l’exception ou la condition à appliquer.
ms.openlocfilehash: 5b6e714512edcf12ded2c04f414d047b8622d305
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756439"
---
# <a name="flaggedforaction"></a><span data-ttu-id="1e0f1-103">FlaggedForAction</span><span class="sxs-lookup"><span data-stu-id="1e0f1-103">FlaggedForAction</span></span>

<span data-ttu-id="1e0f1-104">L’élément **FlaggedForAction** Spécifie l’indicateur pour la valeur d’action qui doit apparaître dans les messages entrants afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="1e0f1-104">The **FlaggedForAction** element specifies the flag for action value that must appear on incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<FlaggedForAction/>
```

 <span data-ttu-id="1e0f1-105">**FlaggedForActionType**</span><span class="sxs-lookup"><span data-stu-id="1e0f1-105">**FlaggedForActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1e0f1-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1e0f1-106">Attributes and elements</span></span>

<span data-ttu-id="1e0f1-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1e0f1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1e0f1-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1e0f1-108">Attributes</span></span>

<span data-ttu-id="1e0f1-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1e0f1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1e0f1-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1e0f1-110">Child elements</span></span>

<span data-ttu-id="1e0f1-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1e0f1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1e0f1-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1e0f1-112">Parent elements</span></span>

|<span data-ttu-id="1e0f1-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1e0f1-113">**Element**</span></span>|<span data-ttu-id="1e0f1-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="1e0f1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1e0f1-115">Conditions</span><span class="sxs-lookup"><span data-stu-id="1e0f1-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="1e0f1-116">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="1e0f1-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="1e0f1-117">Exceptions</span><span class="sxs-lookup"><span data-stu-id="1e0f1-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="1e0f1-118">Représente les exceptions qui représentent toutes les conditions d'exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="1e0f1-118">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1e0f1-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="1e0f1-119">Text value</span></span>

<span data-ttu-id="1e0f1-120">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="1e0f1-120">A text value is required.</span></span> <span data-ttu-id="1e0f1-121">Les valeurs de texte possibles de cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="1e0f1-121">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="1e0f1-122">Tout</span><span class="sxs-lookup"><span data-stu-id="1e0f1-122">Any</span></span>
    
- <span data-ttu-id="1e0f1-123">Appel</span><span class="sxs-lookup"><span data-stu-id="1e0f1-123">Call</span></span>
    
- <span data-ttu-id="1e0f1-124">DoNotForward</span><span class="sxs-lookup"><span data-stu-id="1e0f1-124">DoNotForward</span></span>
    
- <span data-ttu-id="1e0f1-125">FollowUp</span><span class="sxs-lookup"><span data-stu-id="1e0f1-125">FollowUp</span></span>
    
- <span data-ttu-id="1e0f1-126">Pour info</span><span class="sxs-lookup"><span data-stu-id="1e0f1-126">FYI</span></span>
    
- <span data-ttu-id="1e0f1-127">Transférer</span><span class="sxs-lookup"><span data-stu-id="1e0f1-127">Forward</span></span>
    
- <span data-ttu-id="1e0f1-128">NoResponseNecessary</span><span class="sxs-lookup"><span data-stu-id="1e0f1-128">NoResponseNecessary</span></span>
    
- <span data-ttu-id="1e0f1-129">Lire</span><span class="sxs-lookup"><span data-stu-id="1e0f1-129">Read</span></span>
    
- <span data-ttu-id="1e0f1-130">Répondre</span><span class="sxs-lookup"><span data-stu-id="1e0f1-130">Reply</span></span>
    
- <span data-ttu-id="1e0f1-131">ReplyToAll</span><span class="sxs-lookup"><span data-stu-id="1e0f1-131">ReplyToAll</span></span>
    
- <span data-ttu-id="1e0f1-132">Passer en revue les</span><span class="sxs-lookup"><span data-stu-id="1e0f1-132">Review</span></span>
    
## <a name="remarks"></a><span data-ttu-id="1e0f1-133">Remarques</span><span class="sxs-lookup"><span data-stu-id="1e0f1-133">Remarks</span></span>

<span data-ttu-id="1e0f1-134">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="1e0f1-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1e0f1-135">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1e0f1-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1e0f1-136">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1e0f1-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1e0f1-137">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1e0f1-137">Schema Name</span></span>  <br/> |<span data-ttu-id="1e0f1-138">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="1e0f1-138">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1e0f1-139">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1e0f1-139">Validation File</span></span>  <br/> |<span data-ttu-id="1e0f1-140">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1e0f1-140">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1e0f1-141">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1e0f1-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="1e0f1-142">True</span><span class="sxs-lookup"><span data-stu-id="1e0f1-142">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1e0f1-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1e0f1-143">See also</span></span>



- [<span data-ttu-id="1e0f1-144">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1e0f1-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

