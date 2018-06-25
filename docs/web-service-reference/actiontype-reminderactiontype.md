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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755153"
---
# <a name="actiontype-reminderactiontype"></a><span data-ttu-id="f6cd7-103">ActionType (ReminderActionType)</span><span class="sxs-lookup"><span data-stu-id="f6cd7-103">ActionType (ReminderActionType)</span></span>

<span data-ttu-id="f6cd7-104">L’élément **ActionType** Spécifie l’action à effectuer sur le rappel.</span><span class="sxs-lookup"><span data-stu-id="f6cd7-104">The **ActionType** element specifies the action to take on the reminder.</span></span> 
  
```XML
<ActionType> Dismiss | Snooze </ActionType>
```

 <span data-ttu-id="f6cd7-105">**ReminderActionType**</span><span class="sxs-lookup"><span data-stu-id="f6cd7-105">**ReminderActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f6cd7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f6cd7-106">Attributes and elements</span></span>

<span data-ttu-id="f6cd7-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f6cd7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f6cd7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f6cd7-108">Attributes</span></span>

<span data-ttu-id="f6cd7-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f6cd7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f6cd7-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f6cd7-110">Child elements</span></span>

<span data-ttu-id="f6cd7-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f6cd7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f6cd7-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f6cd7-112">Parent elements</span></span>

[<span data-ttu-id="f6cd7-113">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="f6cd7-113">ReminderItemAction</span></span>](reminderitemaction.md)
  
## <a name="text-value"></a><span data-ttu-id="f6cd7-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="f6cd7-114">Text value</span></span>

<span data-ttu-id="f6cd7-115">La valeur de texte de l’élément **ActionType** Spécifie l’action à effectuer sur le rappel.</span><span class="sxs-lookup"><span data-stu-id="f6cd7-115">The text value of the **ActionType** element specifies the action to take on the reminder.</span></span> <span data-ttu-id="f6cd7-116">La valeur de texte de **faire disparaître** indique le rappel doit être fermé.</span><span class="sxs-lookup"><span data-stu-id="f6cd7-116">The text value of **Dismiss** indicates the reminder should be dismissed.</span></span> <span data-ttu-id="f6cd7-117">La valeur de texte de **Répéter** indique que le rappel doit être différé jusqu'à ce que le délai spécifié par l’élément [NewReminderTime](newremindertime.md) .</span><span class="sxs-lookup"><span data-stu-id="f6cd7-117">The text value of **Snooze** indicates that the reminder should be delayed until the time specified by the [NewReminderTime](newremindertime.md) element.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f6cd7-118">Remarques</span><span class="sxs-lookup"><span data-stu-id="f6cd7-118">Remarks</span></span>

<span data-ttu-id="f6cd7-119">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f6cd7-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f6cd7-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f6cd7-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f6cd7-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f6cd7-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f6cd7-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f6cd7-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f6cd7-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f6cd7-123">Schema Name</span></span>  <br/> |<span data-ttu-id="f6cd7-124">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="f6cd7-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="f6cd7-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f6cd7-125">Validation File</span></span>  <br/> |<span data-ttu-id="f6cd7-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f6cd7-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f6cd7-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f6cd7-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="f6cd7-128">False</span><span class="sxs-lookup"><span data-stu-id="f6cd7-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f6cd7-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f6cd7-129">See also</span></span>

- [<span data-ttu-id="f6cd7-130">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="f6cd7-130">ReminderItemAction</span></span>](reminderitemaction.md)
- [<span data-ttu-id="f6cd7-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f6cd7-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

