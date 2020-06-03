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
description: L’élément WithinSizeRange spécifie les tailles minimale et maximale que les messages entrants doivent être pour que la condition ou l’exception s’applique.
ms.openlocfilehash: 31da5815b70e20c47594da89b0b7ccab87eaf8f3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459741"
---
# <a name="withinsizerange"></a><span data-ttu-id="74d55-103">WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="74d55-103">WithinSizeRange</span></span>

<span data-ttu-id="74d55-104">L’élément **WithinSizeRange** spécifie les tailles minimale et maximale que les messages entrants doivent être pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="74d55-104">The **WithinSizeRange** element specifies the minimum and maximum sizes that incoming messages must be in order for the condition or exception to apply.</span></span> 
  
```XML
<WithinSizeRange>
     <MinimumSize/>
     <MaximumSize/>
</WithinSizeRange>
```

 <span data-ttu-id="74d55-105">**RulePredicateSizeRangeType**</span><span class="sxs-lookup"><span data-stu-id="74d55-105">**RulePredicateSizeRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="74d55-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="74d55-106">Attributes and elements</span></span>

<span data-ttu-id="74d55-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="74d55-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="74d55-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="74d55-108">Attributes</span></span>

<span data-ttu-id="74d55-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="74d55-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="74d55-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="74d55-110">Child elements</span></span>

|<span data-ttu-id="74d55-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="74d55-111">**Element**</span></span>|<span data-ttu-id="74d55-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="74d55-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74d55-113">MinimumSize</span><span class="sxs-lookup"><span data-stu-id="74d55-113">MinimumSize</span></span>](minimumsize.md) <br/> |<span data-ttu-id="74d55-114">Spécifie la taille minimale qu’un message doit être pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="74d55-114">Specifies the minimum size that a message must be in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="74d55-115">/M</span><span class="sxs-lookup"><span data-stu-id="74d55-115">MaximumSize</span></span>](maximumsize.md) <br/> |<span data-ttu-id="74d55-116">Spécifie la taille maximale qu’un message doit être pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="74d55-116">Specifies the maximum size that a message must be in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="74d55-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="74d55-117">Parent elements</span></span>

|<span data-ttu-id="74d55-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="74d55-118">**Element**</span></span>|<span data-ttu-id="74d55-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="74d55-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74d55-120">Conditions</span><span class="sxs-lookup"><span data-stu-id="74d55-120">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="74d55-121">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="74d55-121">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="74d55-122">Exceptions</span><span class="sxs-lookup"><span data-stu-id="74d55-122">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="74d55-123">Représente toutes les conditions d’exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="74d55-123">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="74d55-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="74d55-124">Text value</span></span>

<span data-ttu-id="74d55-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="74d55-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="74d55-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="74d55-126">Remarks</span></span>

<span data-ttu-id="74d55-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="74d55-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="74d55-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="74d55-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="74d55-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="74d55-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="74d55-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="74d55-130">Schema Name</span></span>  <br/> |<span data-ttu-id="74d55-131">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="74d55-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="74d55-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="74d55-132">Validation File</span></span>  <br/> |<span data-ttu-id="74d55-133">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="74d55-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="74d55-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="74d55-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="74d55-135">True</span><span class="sxs-lookup"><span data-stu-id="74d55-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="74d55-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="74d55-136">See also</span></span>



- [<span data-ttu-id="74d55-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="74d55-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

