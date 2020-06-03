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
description: L’élément SetFolderField représente une mise à jour qui définit la valeur d’une propriété unique sur un dossier dans une opération UpdateFolder.
ms.openlocfilehash: ab75a3862801b9a7b3369d9a4116c653b461781c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530316"
---
# <a name="setfolderfield"></a><span data-ttu-id="1e245-103">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="1e245-103">SetFolderField</span></span>

<span data-ttu-id="1e245-104">L’élément **SetFolderField** représente une mise à jour qui définit la valeur d’une propriété unique sur un dossier dans une opération UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="1e245-104">The **SetFolderField** element represents an update that sets the value for a single property on a folder in an UpdateFolder operation.</span></span> 

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


<span data-ttu-id="1e245-105">**SetFolderFieldType**</span><span class="sxs-lookup"><span data-stu-id="1e245-105">**SetFolderFieldType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="1e245-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1e245-106">Attributes and elements</span></span>

<span data-ttu-id="1e245-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1e245-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1e245-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1e245-108">Attributes</span></span>

<span data-ttu-id="1e245-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="1e245-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1e245-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1e245-110">Child elements</span></span>

|<span data-ttu-id="1e245-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1e245-111">**Element**</span></span>|<span data-ttu-id="1e245-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="1e245-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1e245-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="1e245-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="1e245-114">Identifie les propriétés référencées fréquemment par URI.</span><span class="sxs-lookup"><span data-stu-id="1e245-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="1e245-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="1e245-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="1e245-116">Identifie les membres individuels d’un dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="1e245-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="1e245-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="1e245-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="1e245-118">Identifie les propriétés MAPI étendues.</span><span class="sxs-lookup"><span data-stu-id="1e245-118">Identifies extended MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="1e245-119">Folder</span><span class="sxs-lookup"><span data-stu-id="1e245-119">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="1e245-120">Identifie un dossier à mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="1e245-120">Identifies a folder to update.</span></span>  <br/> |
|[<span data-ttu-id="1e245-121">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="1e245-121">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="1e245-122">Représente un dossier qui contient principalement des éléments de calendrier.</span><span class="sxs-lookup"><span data-stu-id="1e245-122">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="1e245-123">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="1e245-123">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="1e245-124">Représente un dossier de contacts dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="1e245-124">Represents a Contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="1e245-125">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="1e245-125">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="1e245-126">Représente un dossier de recherche contenu dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="1e245-126">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="1e245-127">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="1e245-127">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="1e245-128">Représente un dossier tâches contenu dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="1e245-128">Represents a Tasks folder that is contained in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1e245-129">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1e245-129">Parent elements</span></span>

|<span data-ttu-id="1e245-130">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1e245-130">**Element**</span></span>|<span data-ttu-id="1e245-131">**Description**</span><span class="sxs-lookup"><span data-stu-id="1e245-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1e245-132">Mises à jour (dossier)</span><span class="sxs-lookup"><span data-stu-id="1e245-132">Updates (Folder)</span></span>](updates-folder.md) <br/> |<span data-ttu-id="1e245-133">Contient un ensemble d’éléments qui définit les modifications apportées par l’ajout, la définition et la suppression aux propriétés du dossier.</span><span class="sxs-lookup"><span data-stu-id="1e245-133">Contains a set of elements that defines append, set, and delete changes to folder properties.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1e245-134">Remarques</span><span class="sxs-lookup"><span data-stu-id="1e245-134">Remarks</span></span>

<span data-ttu-id="1e245-135">Si la propriété existe, la valeur de la propriété est définie sur la valeur spécifiée.</span><span class="sxs-lookup"><span data-stu-id="1e245-135">If the property exists, the property value is set to the specified value.</span></span> <span data-ttu-id="1e245-136">Si la propriété n’existe pas, la propriété est créée avec la valeur spécifiée.</span><span class="sxs-lookup"><span data-stu-id="1e245-136">If the property does not exist, the property is created with the specified value.</span></span>
  
<span data-ttu-id="1e245-137">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="1e245-137">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1e245-138">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1e245-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1e245-139">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1e245-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1e245-140">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1e245-140">Schema Name</span></span>  <br/> |<span data-ttu-id="1e245-141">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="1e245-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="1e245-142">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1e245-142">Validation File</span></span>  <br/> |<span data-ttu-id="1e245-143">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1e245-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1e245-144">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1e245-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="1e245-145">False</span><span class="sxs-lookup"><span data-stu-id="1e245-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1e245-146">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1e245-146">See also</span></span>

- [<span data-ttu-id="1e245-147">Opération UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="1e245-147">UpdateFolder operation</span></span>](updatefolder-operation.md)
- [<span data-ttu-id="1e245-148">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1e245-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

