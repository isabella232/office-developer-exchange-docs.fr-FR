---
title: ActionType (ReminderActionType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0ffcdcf4-8ea3-483c-bb7f-0cd84126120c
description: L’élément ActionType Spécifie l’action à effectuer sur le rappel.
ms.openlocfilehash: 361259f733756995fae2c2c2390013a728e475a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755153"
---
# <a name="actiontype-reminderactiontype"></a><span data-ttu-id="e362f-103">ActionType (ReminderActionType)</span><span class="sxs-lookup"><span data-stu-id="e362f-103">ActionType (ReminderActionType)</span></span>

<span data-ttu-id="e362f-104">L’élément **ActionType** Spécifie l’action à effectuer sur le rappel.</span><span class="sxs-lookup"><span data-stu-id="e362f-104">The **ActionType** element specifies the action to take on the reminder.</span></span> 
  
```XML
<ActionType> Dismiss | Snooze </ActionType>
```

 <span data-ttu-id="e362f-105">**ReminderActionType**</span><span class="sxs-lookup"><span data-stu-id="e362f-105">**ReminderActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e362f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e362f-106">Attributes and elements</span></span>

<span data-ttu-id="e362f-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e362f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e362f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e362f-108">Attributes</span></span>

<span data-ttu-id="e362f-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e362f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e362f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e362f-110">Child elements</span></span>

<span data-ttu-id="e362f-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e362f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e362f-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e362f-112">Parent elements</span></span>

[<span data-ttu-id="e362f-113">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="e362f-113">ReminderItemAction</span></span>](reminderitemaction.md)
  
## <a name="text-value"></a><span data-ttu-id="e362f-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="e362f-114">Text value</span></span>

<span data-ttu-id="e362f-115">La valeur de texte de l’élément **ActionType** Spécifie l’action à effectuer sur le rappel.</span><span class="sxs-lookup"><span data-stu-id="e362f-115">The text value of the **ActionType** element specifies the action to take on the reminder.</span></span> <span data-ttu-id="e362f-116">La valeur de texte de **faire disparaître** indique le rappel doit être fermé.</span><span class="sxs-lookup"><span data-stu-id="e362f-116">The text value of **Dismiss** indicates the reminder should be dismissed.</span></span> <span data-ttu-id="e362f-117">La valeur de texte de **Répéter** indique que le rappel doit être différé jusqu'à ce que le délai spécifié par l’élément [NewReminderTime](newremindertime.md) .</span><span class="sxs-lookup"><span data-stu-id="e362f-117">The text value of **Snooze** indicates that the reminder should be delayed until the time specified by the [NewReminderTime](newremindertime.md) element.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e362f-118">Remarques</span><span class="sxs-lookup"><span data-stu-id="e362f-118">Remarks</span></span>

<span data-ttu-id="e362f-119">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e362f-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e362f-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="e362f-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e362f-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e362f-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e362f-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e362f-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e362f-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e362f-123">Schema Name</span></span>  <br/> |<span data-ttu-id="e362f-124">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="e362f-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="e362f-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e362f-125">Validation File</span></span>  <br/> |<span data-ttu-id="e362f-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e362f-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e362f-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e362f-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="e362f-128">False</span><span class="sxs-lookup"><span data-stu-id="e362f-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e362f-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e362f-129">See also</span></span>

- [<span data-ttu-id="e362f-130">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="e362f-130">ReminderItemAction</span></span>](reminderitemaction.md)
- [<span data-ttu-id="e362f-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e362f-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

