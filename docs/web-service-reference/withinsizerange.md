---
title: WithinSizeRange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WithinSizeRange
api_type:
- schema
ms.assetid: 6f98650e-3399-4f87-9b7f-40bf20cdb821
description: L’élément WithinSizeRange spécifie la taille minimale et maximale que les messages entrants doivent être dans l’ordre de l’exception ou la condition à appliquer.
ms.openlocfilehash: 7711db9ca68f972f080c98197e30c7710620119a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839057"
---
# <a name="withinsizerange"></a><span data-ttu-id="06acf-103">WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="06acf-103">WithinSizeRange</span></span>

<span data-ttu-id="06acf-104">L’élément **WithinSizeRange** spécifie la taille minimale et maximale que les messages entrants doivent être dans l’ordre de l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="06acf-104">The **WithinSizeRange** element specifies the minimum and maximum sizes that incoming messages must be in order for the condition or exception to apply.</span></span> 
  
```XML
<WithinSizeRange>
     <MinimumSize/>
     <MaximumSize/>
</WithinSizeRange>
```

 <span data-ttu-id="06acf-105">**RulePredicateSizeRangeType**</span><span class="sxs-lookup"><span data-stu-id="06acf-105">**RulePredicateSizeRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="06acf-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="06acf-106">Attributes and elements</span></span>

<span data-ttu-id="06acf-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="06acf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="06acf-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="06acf-108">Attributes</span></span>

<span data-ttu-id="06acf-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="06acf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="06acf-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="06acf-110">Child elements</span></span>

|<span data-ttu-id="06acf-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="06acf-111">**Element**</span></span>|<span data-ttu-id="06acf-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="06acf-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="06acf-113">MinimumSize</span><span class="sxs-lookup"><span data-stu-id="06acf-113">MinimumSize</span></span>](minimumsize.md) <br/> |<span data-ttu-id="06acf-114">Spécifie la taille minimale doit correspondre à un message afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="06acf-114">Specifies the minimum size that a message must be in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="06acf-115">MaximumSize</span><span class="sxs-lookup"><span data-stu-id="06acf-115">MaximumSize</span></span>](maximumsize.md) <br/> |<span data-ttu-id="06acf-116">Spécifie la taille maximale qui doit correspondre à un message afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="06acf-116">Specifies the maximum size that a message must be in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="06acf-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="06acf-117">Parent elements</span></span>

|<span data-ttu-id="06acf-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="06acf-118">**Element**</span></span>|<span data-ttu-id="06acf-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="06acf-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="06acf-120">Conditions</span><span class="sxs-lookup"><span data-stu-id="06acf-120">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="06acf-121">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="06acf-121">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="06acf-122">Exceptions</span><span class="sxs-lookup"><span data-stu-id="06acf-122">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="06acf-123">Représente toutes les conditions d’exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="06acf-123">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="06acf-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="06acf-124">Text value</span></span>

<span data-ttu-id="06acf-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="06acf-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="06acf-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="06acf-126">Remarks</span></span>

<span data-ttu-id="06acf-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="06acf-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="06acf-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="06acf-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="06acf-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="06acf-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="06acf-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="06acf-130">Schema Name</span></span>  <br/> |<span data-ttu-id="06acf-131">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="06acf-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="06acf-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="06acf-132">Validation File</span></span>  <br/> |<span data-ttu-id="06acf-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="06acf-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="06acf-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="06acf-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="06acf-135">True</span><span class="sxs-lookup"><span data-stu-id="06acf-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="06acf-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="06acf-136">See also</span></span>



- [<span data-ttu-id="06acf-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="06acf-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

