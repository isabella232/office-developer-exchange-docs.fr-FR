---
title: ArchiveTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c4cb0718-37cd-41aa-86e7-b492c4bb86aa
description: L’élément ArchiveTag spécifie l’identificateur de rétention de la balise d’archivage définie sur un élément ou un dossier.
ms.openlocfilehash: 23167f3c96a6756fe4c6d915a4de91e815e620d9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464762"
---
# <a name="archivetag"></a><span data-ttu-id="be9a2-103">ArchiveTag</span><span class="sxs-lookup"><span data-stu-id="be9a2-103">ArchiveTag</span></span>

<span data-ttu-id="be9a2-104">L’élément **ArchiveTag** spécifie l’identificateur de rétention de la balise d’archivage définie sur un élément ou un dossier.</span><span class="sxs-lookup"><span data-stu-id="be9a2-104">The **ArchiveTag** element specifies the retention identifier of the archive tag set on an item or folder.</span></span> 
  
```XML
<ArchiveTag IsExplicit=""></ArchiveTag>
```

 <span data-ttu-id="be9a2-105">**RetentionTagType**</span><span class="sxs-lookup"><span data-stu-id="be9a2-105">**RetentionTagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="be9a2-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="be9a2-106">Attributes and elements</span></span>

<span data-ttu-id="be9a2-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="be9a2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="be9a2-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="be9a2-108">Attributes</span></span>

|<span data-ttu-id="be9a2-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="be9a2-109">**Attribute**</span></span>|<span data-ttu-id="be9a2-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="be9a2-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="be9a2-111">**IsExplicit**</span><span class="sxs-lookup"><span data-stu-id="be9a2-111">**IsExplicit**</span></span> <br/> |<span data-ttu-id="be9a2-112">Indique si la stratégie de rétention est définie de manière explicite sur un élément ou un dossier ou si elle est héritée d’un dossier parent.</span><span class="sxs-lookup"><span data-stu-id="be9a2-112">Specifies whether the retention policy is explicitly set on an item or folder or whether it is inherited from a parent folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="be9a2-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="be9a2-113">Child elements</span></span>

<span data-ttu-id="be9a2-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="be9a2-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="be9a2-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="be9a2-115">Parent elements</span></span>

|<span data-ttu-id="be9a2-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="be9a2-116">**Element**</span></span>|<span data-ttu-id="be9a2-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="be9a2-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="be9a2-118">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="be9a2-118">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="be9a2-119">Représente un dossier qui contient principalement des éléments de calendrier.</span><span class="sxs-lookup"><span data-stu-id="be9a2-119">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="be9a2-120">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="be9a2-120">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="be9a2-121">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="be9a2-121">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="be9a2-122">Contact</span><span class="sxs-lookup"><span data-stu-id="be9a2-122">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="be9a2-123">Représente un élément de contact dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="be9a2-123">Represents a contact item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="be9a2-124">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="be9a2-124">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="be9a2-125">Représente un dossier de contacts contenu dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="be9a2-125">Represents a contacts folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="be9a2-126">DistributionList</span><span class="sxs-lookup"><span data-stu-id="be9a2-126">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="be9a2-127">Représente une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="be9a2-127">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="be9a2-128">Folder</span><span class="sxs-lookup"><span data-stu-id="be9a2-128">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="be9a2-129">Définit un dossier à créer, obtenir, Rechercher, synchroniser ou mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="be9a2-129">Defines a folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="be9a2-130">Élément</span><span class="sxs-lookup"><span data-stu-id="be9a2-130">Item</span></span>](item.md) <br/> |<span data-ttu-id="be9a2-131">Représente un élément générique dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="be9a2-131">Represents a generic item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="be9a2-132">Message</span><span class="sxs-lookup"><span data-stu-id="be9a2-132">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="be9a2-133">Représente un message électronique Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="be9a2-133">Represents a Microsoft Exchange email message.</span></span>  <br/> |
|[<span data-ttu-id="be9a2-134">PostItem</span><span class="sxs-lookup"><span data-stu-id="be9a2-134">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="be9a2-135">Représente un élément post dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="be9a2-135">Represents a post item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="be9a2-136">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="be9a2-136">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="be9a2-137">Représente un dossier de recherche contenu dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="be9a2-137">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="be9a2-138">Tâche</span><span class="sxs-lookup"><span data-stu-id="be9a2-138">Task</span></span>](task.md) <br/> |<span data-ttu-id="be9a2-139">Représente une tâche dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="be9a2-139">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="be9a2-140">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="be9a2-140">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="be9a2-141">Représente un dossier tâches contenu dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="be9a2-141">Represents a tasks folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="be9a2-142">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="be9a2-142">Text value</span></span>

<span data-ttu-id="be9a2-143">La valeur de texte de l’élément **ArchiveTag** est un GUID qui identifie la stratégie de rétention.</span><span class="sxs-lookup"><span data-stu-id="be9a2-143">The text value of the **ArchiveTag** element is a GUID that identifies the retention policy.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="be9a2-144">Remarques</span><span class="sxs-lookup"><span data-stu-id="be9a2-144">Remarks</span></span>

<span data-ttu-id="be9a2-145">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="be9a2-145">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="be9a2-146">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="be9a2-146">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="be9a2-147">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="be9a2-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="be9a2-148">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="be9a2-148">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="be9a2-149">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="be9a2-149">Schema Name</span></span>  <br/> |<span data-ttu-id="be9a2-150">Schéma type</span><span class="sxs-lookup"><span data-stu-id="be9a2-150">Type schema</span></span>  <br/> |
|<span data-ttu-id="be9a2-151">Validation File</span><span class="sxs-lookup"><span data-stu-id="be9a2-151">Validation File</span></span>  <br/> |<span data-ttu-id="be9a2-152">types. xsd</span><span class="sxs-lookup"><span data-stu-id="be9a2-152">types.xsd</span></span>  <br/> |
|<span data-ttu-id="be9a2-153">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="be9a2-153">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="be9a2-154">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="be9a2-154">See also</span></span>

- [<span data-ttu-id="be9a2-155">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="be9a2-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

