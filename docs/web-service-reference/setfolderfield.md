---
title: SetFolderField
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SetFolderField
api_type:
- schema
ms.assetid: 8c69db7b-54b5-4ae2-abca-4d6e0937a790
description: L’élément SetFolderField représente une mise à jour qui définit la valeur d’une propriété unique dans un dossier dans une opération UpdateFolder.
ms.openlocfilehash: 1919c335197c83999875a17397e9c9d4405d1e3f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829407"
---
# <a name="setfolderfield"></a><span data-ttu-id="0fc09-103">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="0fc09-103">SetFolderField</span></span>

<span data-ttu-id="0fc09-104">L’élément **SetFolderField** représente une mise à jour qui définit la valeur d’une propriété unique dans un dossier dans une opération UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="0fc09-104">The **SetFolderField** element represents an update that sets the value for a single property on a folder in an UpdateFolder operation.</span></span> 
  
```xml
<SetFolderField>
   <FieldURI/>
   <Folder/>
</SetFolderField>
```

 <span data-ttu-id="0fc09-105">**SetFolderFieldType**</span><span class="sxs-lookup"><span data-stu-id="0fc09-105">**SetFolderFieldType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0fc09-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0fc09-106">Attributes and elements</span></span>

<span data-ttu-id="0fc09-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0fc09-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0fc09-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="0fc09-108">Attributes</span></span>

<span data-ttu-id="0fc09-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0fc09-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0fc09-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0fc09-110">Child elements</span></span>

|<span data-ttu-id="0fc09-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0fc09-111">**Element**</span></span>|<span data-ttu-id="0fc09-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="0fc09-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0fc09-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="0fc09-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="0fc09-114">Identifie les propriétés fréquemment référencées par un URI.</span><span class="sxs-lookup"><span data-stu-id="0fc09-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="0fc09-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="0fc09-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="0fc09-116">Identifie les membres individuels d’un dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="0fc09-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="0fc09-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="0fc09-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="0fc09-118">Identifie les propriétés MAPI étendues.</span><span class="sxs-lookup"><span data-stu-id="0fc09-118">Identifies extended MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="0fc09-119">Folder</span><span class="sxs-lookup"><span data-stu-id="0fc09-119">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="0fc09-120">Identifie un dossier pour mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="0fc09-120">Identifies a folder to update.</span></span>  <br/> |
|[<span data-ttu-id="0fc09-121">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="0fc09-121">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="0fc09-122">Représente un dossier contenant principalement des éléments de calendrier.</span><span class="sxs-lookup"><span data-stu-id="0fc09-122">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="0fc09-123">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="0fc09-123">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="0fc09-124">Représente un dossier Contacts dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="0fc09-124">Represents a Contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="0fc09-125">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="0fc09-125">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="0fc09-126">Représente un dossier de recherche qui se trouve dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="0fc09-126">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="0fc09-127">Dossier tâches</span><span class="sxs-lookup"><span data-stu-id="0fc09-127">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="0fc09-128">Représente un dossier de tâches qui se trouve dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="0fc09-128">Represents a Tasks folder that is contained in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0fc09-129">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0fc09-129">Parent elements</span></span>

|<span data-ttu-id="0fc09-130">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0fc09-130">**Element**</span></span>|<span data-ttu-id="0fc09-131">**Description**</span><span class="sxs-lookup"><span data-stu-id="0fc09-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0fc09-132">Mises à jour (dossier)</span><span class="sxs-lookup"><span data-stu-id="0fc09-132">Updates (Folder)</span></span>](updates-folder.md) <br/> |<span data-ttu-id="0fc09-133">Contient un ensemble d’éléments qui définit append, définir et supprimer les modifications apportées aux propriétés d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="0fc09-133">Contains a set of elements that defines append, set, and delete changes to folder properties.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0fc09-134">Remarques</span><span class="sxs-lookup"><span data-stu-id="0fc09-134">Remarks</span></span>

<span data-ttu-id="0fc09-135">Si la propriété existe, la valeur de propriété est définie à la valeur spécifiée.</span><span class="sxs-lookup"><span data-stu-id="0fc09-135">If the property exists, the property value is set to the specified value.</span></span> <span data-ttu-id="0fc09-136">Si la propriété n’existe pas, la propriété est créée avec la valeur spécifiée.</span><span class="sxs-lookup"><span data-stu-id="0fc09-136">If the property does not exist, the property is created with the specified value.</span></span>
  
<span data-ttu-id="0fc09-137">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="0fc09-137">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0fc09-138">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0fc09-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0fc09-139">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0fc09-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0fc09-140">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0fc09-140">Schema Name</span></span>  <br/> |<span data-ttu-id="0fc09-141">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="0fc09-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="0fc09-142">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0fc09-142">Validation File</span></span>  <br/> |<span data-ttu-id="0fc09-143">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0fc09-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0fc09-144">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0fc09-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="0fc09-145">False</span><span class="sxs-lookup"><span data-stu-id="0fc09-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0fc09-146">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0fc09-146">See also</span></span>



[<span data-ttu-id="0fc09-147">Opération UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="0fc09-147">UpdateFolder operation</span></span>](updatefolder-operation.md)


- [<span data-ttu-id="0fc09-148">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0fc09-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

