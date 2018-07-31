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
ms.openlocfilehash: ed5c055c697865d5eb728d269c6f4c7ce60f4b5c
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353286"
---
# <a name="setfolderfield"></a><span data-ttu-id="48a28-103">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="48a28-103">SetFolderField</span></span>

<span data-ttu-id="48a28-104">L’élément **SetFolderField** représente une mise à jour qui définit la valeur d’une propriété unique dans un dossier dans une opération UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="48a28-104">The **SetFolderField** element represents an update that sets the value for a single property on a folder in an UpdateFolder operation.</span></span> 

```xml
<SetFolderField>
   <FieldURI/>
   <Folder/>
</SetFolderField>
```
  
```xml
<SetFolderField>
   <IndexedFieldURI/> 
   <SearchFolder/> 
</SetFolderField>
```

```xml
<SetFolderField>
   <FieldURI/> 
   <TasksFolder/>
</SetFolderField>
```

```xml
<SetFolderField>
   <ExtendedFieldURI/> 
   <CalendarFolder/> 
</SetFolderField>
```

```xml
<SetFolderField>
   <ExtendedFieldURI/> 
   <SearchFolder/>
</SetFolderField>
```

```xml
<SetFolderField>
   <ExtendedFieldURI/> 
   <Folder/> 
</SetFolderField>
```

```xml
<SetFolderField>
    <IndexedFieldURI/> 
    <TasksFolder/>
</SetFolderField>
```

```xml
<SetFolderField>
   <FieldURI/> 
   <SearchFolder/>
</SetFolderField>
```

```xml
<SetFolderField>
   <FieldURI/> 
   <CalendarFolder/> 
</SetFolderField>
```

```xml
<SetFolderField>
   <ExtendedFieldURI/> 
   <TasksFolder/> 
</SetFolderField>
```

```xml
<SetFolderField>
   <IndexedFieldURI/> 
   <CalendarFolder/> 
</SetFolderField>
```

```xml
<SetFolderField>
   <IndexedFieldURI/> 
   <Folder/>
</SetFolderField>
```

```xml
<SetFolderField>
    <FieldURI/> 
    <ContactsFolder/>
</SetFolderField>
```

```xml
<SetFolderField>
   <ExtendedFieldURI/> 
   <ContactsFolder/>
</SetFolderField>
```

```xml
<SetFolderField>
   <IndexedFieldURI/> 
   <ContactsFolder/> 
</SetFolderField>
```


<span data-ttu-id="48a28-105">**SetFolderFieldType**</span><span class="sxs-lookup"><span data-stu-id="48a28-105">**SetFolderFieldType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="48a28-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="48a28-106">Attributes and elements</span></span>

<span data-ttu-id="48a28-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="48a28-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="48a28-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="48a28-108">Attributes</span></span>

<span data-ttu-id="48a28-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="48a28-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="48a28-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="48a28-110">Child elements</span></span>

|<span data-ttu-id="48a28-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="48a28-111">**Element**</span></span>|<span data-ttu-id="48a28-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="48a28-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="48a28-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="48a28-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="48a28-114">Identifie les propriétés fréquemment référencées par un URI.</span><span class="sxs-lookup"><span data-stu-id="48a28-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="48a28-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="48a28-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="48a28-116">Identifie les membres individuels d’un dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="48a28-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="48a28-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="48a28-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="48a28-118">Identifie les propriétés MAPI étendues.</span><span class="sxs-lookup"><span data-stu-id="48a28-118">Identifies extended MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="48a28-119">Folder</span><span class="sxs-lookup"><span data-stu-id="48a28-119">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="48a28-120">Identifie un dossier pour mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="48a28-120">Identifies a folder to update.</span></span>  <br/> |
|[<span data-ttu-id="48a28-121">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="48a28-121">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="48a28-122">Représente un dossier contenant principalement des éléments de calendrier.</span><span class="sxs-lookup"><span data-stu-id="48a28-122">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="48a28-123">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="48a28-123">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="48a28-124">Représente un dossier Contacts dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="48a28-124">Represents a Contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="48a28-125">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="48a28-125">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="48a28-126">Représente un dossier de recherche qui se trouve dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="48a28-126">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="48a28-127">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="48a28-127">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="48a28-128">Représente un dossier de tâches qui se trouve dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="48a28-128">Represents a Tasks folder that is contained in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="48a28-129">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="48a28-129">Parent elements</span></span>

|<span data-ttu-id="48a28-130">**Élément**</span><span class="sxs-lookup"><span data-stu-id="48a28-130">**Element**</span></span>|<span data-ttu-id="48a28-131">**Description**</span><span class="sxs-lookup"><span data-stu-id="48a28-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="48a28-132">Updates (Folder)</span><span class="sxs-lookup"><span data-stu-id="48a28-132">Updates (Folder)</span></span>](updates-folder.md) <br/> |<span data-ttu-id="48a28-133">Contient un ensemble d’éléments qui définit append, définir et supprimer les modifications apportées aux propriétés d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="48a28-133">Contains a set of elements that defines append, set, and delete changes to folder properties.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="48a28-134">Remarques</span><span class="sxs-lookup"><span data-stu-id="48a28-134">Remarks</span></span>

<span data-ttu-id="48a28-135">Si la propriété existe, la valeur de propriété est définie à la valeur spécifiée.</span><span class="sxs-lookup"><span data-stu-id="48a28-135">If the property exists, the property value is set to the specified value.</span></span> <span data-ttu-id="48a28-136">Si la propriété n’existe pas, la propriété est créée avec la valeur spécifiée.</span><span class="sxs-lookup"><span data-stu-id="48a28-136">If the property does not exist, the property is created with the specified value.</span></span>
  
<span data-ttu-id="48a28-137">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="48a28-137">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="48a28-138">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="48a28-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="48a28-139">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="48a28-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="48a28-140">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="48a28-140">Schema Name</span></span>  <br/> |<span data-ttu-id="48a28-141">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="48a28-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="48a28-142">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="48a28-142">Validation File</span></span>  <br/> |<span data-ttu-id="48a28-143">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="48a28-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="48a28-144">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="48a28-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="48a28-145">False</span><span class="sxs-lookup"><span data-stu-id="48a28-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="48a28-146">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="48a28-146">See also</span></span>

- [<span data-ttu-id="48a28-147">Opération UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="48a28-147">UpdateFolder operation</span></span>](updatefolder-operation.md)
- [<span data-ttu-id="48a28-148">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="48a28-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

