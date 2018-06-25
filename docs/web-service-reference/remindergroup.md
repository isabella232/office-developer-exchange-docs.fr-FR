---
title: ReminderGroup
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3e23c2a1-05d8-4fec-897c-f684a5b97e4c
description: L’élément ReminderGroup indique si le rappel est pour un élément de calendrier ou d’une tâche.
ms.openlocfilehash: d9d31cdab482d04149428021ad44cc742108053a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829060"
---
# <a name="remindergroup"></a><span data-ttu-id="b677c-103">ReminderGroup</span><span class="sxs-lookup"><span data-stu-id="b677c-103">ReminderGroup</span></span>

<span data-ttu-id="b677c-104">L’élément **ReminderGroup** indique si le rappel est pour un élément de calendrier ou d’une tâche.</span><span class="sxs-lookup"><span data-stu-id="b677c-104">The **ReminderGroup** element specifies whether the reminder is for a calendar item or a task.</span></span> 
  
```XML
<ReminderGroup> Calendar | Task </ReminderGroup>
```

 <span data-ttu-id="b677c-105">**ReminderGroupType**</span><span class="sxs-lookup"><span data-stu-id="b677c-105">**ReminderGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b677c-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b677c-106">Attributes and elements</span></span>

<span data-ttu-id="b677c-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b677c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b677c-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b677c-108">Attributes</span></span>

<span data-ttu-id="b677c-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b677c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b677c-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b677c-110">Child elements</span></span>

<span data-ttu-id="b677c-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b677c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b677c-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b677c-112">Parent elements</span></span>

[<span data-ttu-id="b677c-113">Rappel</span><span class="sxs-lookup"><span data-stu-id="b677c-113">Reminder</span></span>](reminder.md)
  
## <a name="text-value"></a><span data-ttu-id="b677c-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="b677c-114">Text value</span></span>

<span data-ttu-id="b677c-115">La valeur de texte de l’élément **ReminderGroup** est le type de groupe du rappel.</span><span class="sxs-lookup"><span data-stu-id="b677c-115">The text value of the **ReminderGroup** element is the group type of the reminder.</span></span> <span data-ttu-id="b677c-116">La valeur de texte du **calendrier** Spécifie que le rappel est destiné à un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="b677c-116">The text value of **Calendar** specifies that the reminder is for a calendar item.</span></span> <span data-ttu-id="b677c-117">La valeur de texte de la **tâche** Spécifie que le rappel est destiné à un élément de tâche.</span><span class="sxs-lookup"><span data-stu-id="b677c-117">The text value of **Task** specifies that the reminder is for a task item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b677c-118">Remarques</span><span class="sxs-lookup"><span data-stu-id="b677c-118">Remarks</span></span>

<span data-ttu-id="b677c-119">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b677c-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b677c-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b677c-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b677c-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b677c-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b677c-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b677c-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b677c-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b677c-123">Schema Name</span></span>  <br/> |<span data-ttu-id="b677c-124">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="b677c-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="b677c-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b677c-125">Validation File</span></span>  <br/> |<span data-ttu-id="b677c-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b677c-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b677c-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b677c-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="b677c-128">False</span><span class="sxs-lookup"><span data-stu-id="b677c-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b677c-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b677c-129">See also</span></span>



[<span data-ttu-id="b677c-130">Rappel</span><span class="sxs-lookup"><span data-stu-id="b677c-130">Reminder</span></span>](reminder.md)


- [<span data-ttu-id="b677c-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b677c-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

