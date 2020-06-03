---
title: ReminderGroup
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3e23c2a1-05d8-4fec-897c-f684a5b97e4c
description: L’élément ReminderGroup spécifie si le rappel est destiné à un élément de calendrier ou à une tâche.
ms.openlocfilehash: be6f4a7d7e9d495ed7b42ed40c60f016468e8c2c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529867"
---
# <a name="remindergroup"></a><span data-ttu-id="286c7-103">ReminderGroup</span><span class="sxs-lookup"><span data-stu-id="286c7-103">ReminderGroup</span></span>

<span data-ttu-id="286c7-104">L’élément **ReminderGroup** spécifie si le rappel est destiné à un élément de calendrier ou à une tâche.</span><span class="sxs-lookup"><span data-stu-id="286c7-104">The **ReminderGroup** element specifies whether the reminder is for a calendar item or a task.</span></span> 
  
```XML
<ReminderGroup> Calendar | Task </ReminderGroup>
```

 <span data-ttu-id="286c7-105">**ReminderGroupType**</span><span class="sxs-lookup"><span data-stu-id="286c7-105">**ReminderGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="286c7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="286c7-106">Attributes and elements</span></span>

<span data-ttu-id="286c7-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="286c7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="286c7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="286c7-108">Attributes</span></span>

<span data-ttu-id="286c7-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="286c7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="286c7-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="286c7-110">Child elements</span></span>

<span data-ttu-id="286c7-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="286c7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="286c7-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="286c7-112">Parent elements</span></span>

[<span data-ttu-id="286c7-113">Reminder</span><span class="sxs-lookup"><span data-stu-id="286c7-113">Reminder</span></span>](reminder.md)
  
## <a name="text-value"></a><span data-ttu-id="286c7-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="286c7-114">Text value</span></span>

<span data-ttu-id="286c7-115">La valeur de texte de l’élément **ReminderGroup** est le type de groupe du rappel.</span><span class="sxs-lookup"><span data-stu-id="286c7-115">The text value of the **ReminderGroup** element is the group type of the reminder.</span></span> <span data-ttu-id="286c7-116">La valeur texte de **Calendar** spécifie que le rappel est destiné à un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="286c7-116">The text value of **Calendar** specifies that the reminder is for a calendar item.</span></span> <span data-ttu-id="286c7-117">La valeur texte de **Task** spécifie que le rappel est destiné à un élément de tâche.</span><span class="sxs-lookup"><span data-stu-id="286c7-117">The text value of **Task** specifies that the reminder is for a task item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="286c7-118">Remarques</span><span class="sxs-lookup"><span data-stu-id="286c7-118">Remarks</span></span>

<span data-ttu-id="286c7-119">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="286c7-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="286c7-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="286c7-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="286c7-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="286c7-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="286c7-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="286c7-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="286c7-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="286c7-123">Schema Name</span></span>  <br/> |<span data-ttu-id="286c7-124">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="286c7-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="286c7-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="286c7-125">Validation File</span></span>  <br/> |<span data-ttu-id="286c7-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="286c7-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="286c7-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="286c7-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="286c7-128">False</span><span class="sxs-lookup"><span data-stu-id="286c7-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="286c7-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="286c7-129">See also</span></span>



[<span data-ttu-id="286c7-130">Reminder</span><span class="sxs-lookup"><span data-stu-id="286c7-130">Reminder</span></span>](reminder.md)


- [<span data-ttu-id="286c7-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="286c7-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

