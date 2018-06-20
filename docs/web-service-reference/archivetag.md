---
title: ArchiveTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c4cb0718-37cd-41aa-86e7-b492c4bb86aa
description: L’élément ArchiveTag Spécifie l’identificateur de rétention de la balise archive définie sur un élément ou un dossier.
ms.openlocfilehash: ae9c7d512981af3bf564bcb73a9a27c5c78217fc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755319"
---
# <a name="archivetag"></a><span data-ttu-id="c3b69-103">ArchiveTag</span><span class="sxs-lookup"><span data-stu-id="c3b69-103">ArchiveTag</span></span>

<span data-ttu-id="c3b69-104">L’élément **ArchiveTag** Spécifie l’identificateur de rétention de la balise archive définie sur un élément ou un dossier.</span><span class="sxs-lookup"><span data-stu-id="c3b69-104">The **ArchiveTag** element specifies the retention identifier of the archive tag set on an item or folder.</span></span> 
  
```XML
<ArchiveTag IsExplicit=""></ArchiveTag>
```

 <span data-ttu-id="c3b69-105">**RetentionTagType**</span><span class="sxs-lookup"><span data-stu-id="c3b69-105">**RetentionTagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c3b69-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c3b69-106">Attributes and elements</span></span>

<span data-ttu-id="c3b69-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c3b69-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c3b69-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c3b69-108">Attributes</span></span>

|<span data-ttu-id="c3b69-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="c3b69-109">**Attribute**</span></span>|<span data-ttu-id="c3b69-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="c3b69-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c3b69-111">**IsExplicit**</span><span class="sxs-lookup"><span data-stu-id="c3b69-111">**IsExplicit**</span></span> <br/> |<span data-ttu-id="c3b69-112">Spécifie si la stratégie de rétention est définie sur un élément ou d’un dossier ou si elle est héritée d’un dossier parent.</span><span class="sxs-lookup"><span data-stu-id="c3b69-112">Specifies whether the retention policy is explicitly set on an item or folder or whether it is inherited from a parent folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c3b69-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c3b69-113">Child elements</span></span>

<span data-ttu-id="c3b69-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c3b69-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c3b69-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c3b69-115">Parent elements</span></span>

|<span data-ttu-id="c3b69-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c3b69-116">**Element**</span></span>|<span data-ttu-id="c3b69-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="c3b69-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c3b69-118">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="c3b69-118">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="c3b69-119">Représente un dossier contenant principalement des éléments de calendrier.</span><span class="sxs-lookup"><span data-stu-id="c3b69-119">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="c3b69-120">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="c3b69-120">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="c3b69-121">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="c3b69-121">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="c3b69-122">Contact</span><span class="sxs-lookup"><span data-stu-id="c3b69-122">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="c3b69-123">Représente un élément de contact dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="c3b69-123">Represents a contact item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c3b69-124">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="c3b69-124">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="c3b69-125">Représente un dossier de contacts qui se trouve dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="c3b69-125">Represents a contacts folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c3b69-126">DistributionList</span><span class="sxs-lookup"><span data-stu-id="c3b69-126">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="c3b69-127">Représente une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="c3b69-127">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="c3b69-128">Folder</span><span class="sxs-lookup"><span data-stu-id="c3b69-128">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="c3b69-129">Définit un dossier pour créer, obtenir, recherchez, synchroniser ou mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="c3b69-129">Defines a folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="c3b69-130">Item</span><span class="sxs-lookup"><span data-stu-id="c3b69-130">Item</span></span>](item.md) <br/> |<span data-ttu-id="c3b69-131">Représente un élément générique dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="c3b69-131">Represents a generic item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c3b69-132">Message</span><span class="sxs-lookup"><span data-stu-id="c3b69-132">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="c3b69-133">Représente un message électronique de Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="c3b69-133">Represents a Microsoft Exchange email message.</span></span>  <br/> |
|[<span data-ttu-id="c3b69-134">Objet postItem</span><span class="sxs-lookup"><span data-stu-id="c3b69-134">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="c3b69-135">Représente un élément de publication dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="c3b69-135">Represents a post item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c3b69-136">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="c3b69-136">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="c3b69-137">Représente un dossier de recherche qui se trouve dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="c3b69-137">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="c3b69-138">Tâche</span><span class="sxs-lookup"><span data-stu-id="c3b69-138">Task</span></span>](task.md) <br/> |<span data-ttu-id="c3b69-139">Représente une tâche dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="c3b69-139">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="c3b69-140">Dossier tâches</span><span class="sxs-lookup"><span data-stu-id="c3b69-140">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="c3b69-141">Représente un dossier de tâches qui se trouve dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="c3b69-141">Represents a tasks folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c3b69-142">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="c3b69-142">Text value</span></span>

<span data-ttu-id="c3b69-143">La valeur de texte de l’élément **ArchiveTag** est un GUID qui identifie la stratégie de rétention.</span><span class="sxs-lookup"><span data-stu-id="c3b69-143">The text value of the **ArchiveTag** element is a GUID that identifies the retention policy.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c3b69-144">Remarques</span><span class="sxs-lookup"><span data-stu-id="c3b69-144">Remarks</span></span>

<span data-ttu-id="c3b69-145">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c3b69-145">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c3b69-146">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c3b69-146">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c3b69-147">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c3b69-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c3b69-148">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c3b69-148">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c3b69-149">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c3b69-149">Schema Name</span></span>  <br/> |<span data-ttu-id="c3b69-150">Schéma type</span><span class="sxs-lookup"><span data-stu-id="c3b69-150">Type schema</span></span>  <br/> |
|<span data-ttu-id="c3b69-151">Validation File</span><span class="sxs-lookup"><span data-stu-id="c3b69-151">Validation File</span></span>  <br/> |<span data-ttu-id="c3b69-152">types.xsd</span><span class="sxs-lookup"><span data-stu-id="c3b69-152">types.xsd</span></span>  <br/> |
|<span data-ttu-id="c3b69-153">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c3b69-153">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="c3b69-154">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c3b69-154">See also</span></span>

- [<span data-ttu-id="c3b69-155">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c3b69-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
