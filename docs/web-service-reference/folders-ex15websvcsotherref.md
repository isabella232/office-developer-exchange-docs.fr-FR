---
title: Dossiers
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Folders
api_type:
- schema
ms.assetid: 8e71cb44-1df6-444a-add7-0c1363863f65
description: L’élément Folders contient un tableau de dossiers utilisés dans les opérations de dossier.
ms.openlocfilehash: b087be0501f04390b80458458e7e7ccc24bf27bd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530978"
---
# <a name="folders"></a><span data-ttu-id="0aa5b-103">Folders</span><span class="sxs-lookup"><span data-stu-id="0aa5b-103">Folders</span></span>

<span data-ttu-id="0aa5b-104">L’élément **Folders** contient un tableau de dossiers utilisés dans les opérations de dossier.</span><span class="sxs-lookup"><span data-stu-id="0aa5b-104">The **Folders** element contains an array of folders that are used in folder operations.</span></span> 
  
```xml
<Folders>
   <Folder/>
</Folders>
```

```xml
<Folders>
   <ContactsFolder/> 
</Folders>
```

```xml
<Folders>
   <TasksFolder/>
</Folders>
```

```xml
<Folders>
   <CalendarFolder/>
</Folders>
```

```xml
<Folders>
   <SearchFolder/> 
</Folders>
```

<span data-ttu-id="0aa5b-105">**ArrayOfFoldersType** ou **NonEmptyArrayOfFoldersType**</span><span class="sxs-lookup"><span data-stu-id="0aa5b-105">**ArrayOfFoldersType** or **NonEmptyArrayOfFoldersType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="0aa5b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0aa5b-106">Attributes and elements</span></span>

<span data-ttu-id="0aa5b-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0aa5b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0aa5b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="0aa5b-108">Attributes</span></span>

<span data-ttu-id="0aa5b-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="0aa5b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0aa5b-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0aa5b-110">Child elements</span></span>

|<span data-ttu-id="0aa5b-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0aa5b-111">**Element**</span></span>|<span data-ttu-id="0aa5b-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="0aa5b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0aa5b-113">Folder</span><span class="sxs-lookup"><span data-stu-id="0aa5b-113">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="0aa5b-114">Identifie un dossier à créer, obtenir, Rechercher, synchroniser ou mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="0aa5b-114">Identifies a folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="0aa5b-115">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="0aa5b-115">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="0aa5b-116">Représente un dossier qui contient principalement des éléments de calendrier.</span><span class="sxs-lookup"><span data-stu-id="0aa5b-116">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="0aa5b-117">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="0aa5b-117">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="0aa5b-118">Représente un dossier de contacts dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="0aa5b-118">Represents a Contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="0aa5b-119">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="0aa5b-119">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="0aa5b-120">Représente un dossier de recherche contenu dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="0aa5b-120">Represents a Search folder contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="0aa5b-121">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="0aa5b-121">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="0aa5b-122">Représente un dossier tâches dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="0aa5b-122">Represents a Tasks folder in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0aa5b-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0aa5b-123">Parent elements</span></span>

|<span data-ttu-id="0aa5b-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0aa5b-124">**Element**</span></span>|<span data-ttu-id="0aa5b-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="0aa5b-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0aa5b-126">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0aa5b-126">CopyFolderResponseMessage</span></span>](copyfolderresponsemessage.md) <br/> |<span data-ttu-id="0aa5b-127">Contient l’État et le résultat d’une seule demande d' [opération CopyFolder](copyfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="0aa5b-127">Contains the status and result of a single [CopyFolder operation](copyfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="0aa5b-128">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="0aa5b-128">CreateFolder</span></span>](createfolder.md) <br/> |<span data-ttu-id="0aa5b-129">Définit une demande de création d’un dossier dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="0aa5b-129">Defines a request to create a folder in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0aa5b-130">CreateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0aa5b-130">CreateFolderResponseMessage</span></span>](createfolderresponsemessage.md) <br/> |<span data-ttu-id="0aa5b-131">Contient l’État et le résultat d’une seule demande d' [opération CreateFolder](createfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="0aa5b-131">Contains the status and result of a single [CreateFolder operation](createfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="0aa5b-132">CreateManagedFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0aa5b-132">CreateManagedFolderResponseMessage</span></span>](createmanagedfolderresponsemessage.md) <br/> |<span data-ttu-id="0aa5b-133">Contient l’État et le résultat d’une seule demande d' [opération CreateManagedFolder](createmanagedfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="0aa5b-133">Contains the status and result of a single [CreateManagedFolder operation](createmanagedfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="0aa5b-134">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0aa5b-134">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md) <br/> |<span data-ttu-id="0aa5b-135">Contient l’État et le résultat d’une demande d' [opération GetFolder](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="0aa5b-135">Contains the status and result of a [GetFolder operation](getfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="0aa5b-136">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0aa5b-136">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md) <br/> |<span data-ttu-id="0aa5b-137">Contient l’État et le résultat d’une demande d' [opération MoveFolder](movefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="0aa5b-137">Contains the status and result of a [MoveFolder operation](movefolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="0aa5b-138">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="0aa5b-138">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> |<span data-ttu-id="0aa5b-139">Identifie le dossier dans lequel un nouveau dossier est créé.</span><span class="sxs-lookup"><span data-stu-id="0aa5b-139">Identifies the folder where a new folder is created.</span></span>  <br/> |
|[<span data-ttu-id="0aa5b-140">RootFolder (FindFolderResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="0aa5b-140">RootFolder (FindFolderResponseMessage)</span></span>](rootfolder-findfolderresponsemessage.md) <br/> |<span data-ttu-id="0aa5b-141">Contient les résultats de la recherche dans un dossier racine unique pendant une [opération FindFolder](findfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="0aa5b-141">Contains the results from searching a single root folder during a [FindFolder operation](findfolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="0aa5b-142">UpdateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0aa5b-142">UpdateFolderResponseMessage</span></span>](updatefolderresponsemessage.md) <br/> |<span data-ttu-id="0aa5b-143">Contient l’État et le résultat d’une seule demande d' [opération UpdateFolder](updatefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="0aa5b-143">Contains the status and result of a single [UpdateFolder operation](updatefolder-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0aa5b-144">Remarques</span><span class="sxs-lookup"><span data-stu-id="0aa5b-144">Remarks</span></span>

<span data-ttu-id="0aa5b-145">Cet élément est un élément enfant obligatoire de l’élément [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="0aa5b-145">This element is a required child element of the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span> 
  
<span data-ttu-id="0aa5b-146">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="0aa5b-146">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0aa5b-147">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0aa5b-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0aa5b-148">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0aa5b-148">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0aa5b-149">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0aa5b-149">Schema Name</span></span>  <br/> |<span data-ttu-id="0aa5b-150">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="0aa5b-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="0aa5b-151">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0aa5b-151">Validation File</span></span>  <br/> |<span data-ttu-id="0aa5b-152">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0aa5b-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0aa5b-153">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0aa5b-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="0aa5b-154">False</span><span class="sxs-lookup"><span data-stu-id="0aa5b-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0aa5b-155">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0aa5b-155">See also</span></span>

- [<span data-ttu-id="0aa5b-156">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="0aa5b-156">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md)

