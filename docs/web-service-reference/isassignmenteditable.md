---
title: IsAssignmentEditable
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsAssignmentEditable
api_type:
- schema
ms.assetid: 0ddf9181-f65e-4ad6-ad69-7b074ea0f2e7
description: L’élément IsAssignmentEditable représente le type de tâche.
ms.openlocfilehash: 5eb091b24e2c97f7aa6072044fed998b6c9c1651
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468053"
---
# <a name="isassignmenteditable"></a><span data-ttu-id="939b2-103">IsAssignmentEditable</span><span class="sxs-lookup"><span data-stu-id="939b2-103">IsAssignmentEditable</span></span>

<span data-ttu-id="939b2-104">L’élément **IsAssignmentEditable** représente le type de tâche.</span><span class="sxs-lookup"><span data-stu-id="939b2-104">The **IsAssignmentEditable** element represents the task type.</span></span> 
  
```xml
<IsAssignmentEditable/>
```

 <span data-ttu-id="939b2-105">**entier**</span><span class="sxs-lookup"><span data-stu-id="939b2-105">**integer**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="939b2-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="939b2-106">Attributes and elements</span></span>

<span data-ttu-id="939b2-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="939b2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="939b2-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="939b2-108">Attributes</span></span>

<span data-ttu-id="939b2-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="939b2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="939b2-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="939b2-110">Child elements</span></span>

<span data-ttu-id="939b2-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="939b2-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="939b2-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="939b2-112">Parent elements</span></span>

|<span data-ttu-id="939b2-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="939b2-113">**Element**</span></span>|<span data-ttu-id="939b2-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="939b2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="939b2-115">Tâche</span><span class="sxs-lookup"><span data-stu-id="939b2-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="939b2-116">Représente une tâche dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="939b2-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="939b2-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="939b2-117">Text value</span></span>

<span data-ttu-id="939b2-118">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="939b2-118">This property is read-only.</span></span> <span data-ttu-id="939b2-119">Le tableau suivant répertorie les valeurs possibles.</span><span class="sxs-lookup"><span data-stu-id="939b2-119">The following table lists the possible values.</span></span>
  
|<span data-ttu-id="939b2-120">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="939b2-120">**Value**</span></span>|<span data-ttu-id="939b2-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="939b2-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="939b2-122">0</span><span class="sxs-lookup"><span data-stu-id="939b2-122">0</span></span>  <br/> |<span data-ttu-id="939b2-123">Valeur par défaut pour tous les éléments de tâche.</span><span class="sxs-lookup"><span data-stu-id="939b2-123">The default for all task items.</span></span>  <br/> |
|<span data-ttu-id="939b2-124">1 </span><span class="sxs-lookup"><span data-stu-id="939b2-124">1</span></span>  <br/> |<span data-ttu-id="939b2-125">Une demande de tâche.</span><span class="sxs-lookup"><span data-stu-id="939b2-125">A task request.</span></span>  <br/> |
|<span data-ttu-id="939b2-126">n°2</span><span class="sxs-lookup"><span data-stu-id="939b2-126">2</span></span>  <br/> |<span data-ttu-id="939b2-127">Acceptation d’une tâche d’un destinataire d’une demande de tâche.</span><span class="sxs-lookup"><span data-stu-id="939b2-127">A task acceptance from a recipient of a task request.</span></span>  <br/> |
|<span data-ttu-id="939b2-128">3</span><span class="sxs-lookup"><span data-stu-id="939b2-128">3</span></span>  <br/> |<span data-ttu-id="939b2-129">Une tâche de refus d’un destinataire d’une demande de tâche.</span><span class="sxs-lookup"><span data-stu-id="939b2-129">A task declination from a recipient of a task request.</span></span>  <br/> |
|<span data-ttu-id="939b2-130">4 </span><span class="sxs-lookup"><span data-stu-id="939b2-130">4</span></span>  <br/> |<span data-ttu-id="939b2-131">Mise à jour d’une demande de tâche précédente.</span><span class="sxs-lookup"><span data-stu-id="939b2-131">An update to a previous task request.</span></span>  <br/> |
|<span data-ttu-id="939b2-132">5 </span><span class="sxs-lookup"><span data-stu-id="939b2-132">5</span></span>  <br/> |<span data-ttu-id="939b2-133">Non utilisé.</span><span class="sxs-lookup"><span data-stu-id="939b2-133">Not used.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="939b2-134">Remarques</span><span class="sxs-lookup"><span data-stu-id="939b2-134">Remarks</span></span>

<span data-ttu-id="939b2-135">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="939b2-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="939b2-136">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="939b2-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="939b2-137">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="939b2-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="939b2-138">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="939b2-138">Schema Name</span></span>  <br/> |<span data-ttu-id="939b2-139">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="939b2-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="939b2-140">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="939b2-140">Validation File</span></span>  <br/> |<span data-ttu-id="939b2-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="939b2-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="939b2-142">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="939b2-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="939b2-143">False</span><span class="sxs-lookup"><span data-stu-id="939b2-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="939b2-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="939b2-144">See also</span></span>



- [<span data-ttu-id="939b2-145">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="939b2-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

