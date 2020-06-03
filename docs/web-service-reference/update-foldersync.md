---
title: Mise à jour (FolderSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Update
api_type:
- schema
ms.assetid: 47ed8edb-2a94-471b-b965-93f91456252e
description: L’élément Update identifie un dossier unique à mettre à jour dans le magasin client local.
ms.openlocfilehash: 5c1b5b1fd87e4651125293eac431c56f732c6c02
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467136"
---
# <a name="update-foldersync"></a><span data-ttu-id="abf75-103">Mise à jour (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="abf75-103">Update (FolderSync)</span></span>

<span data-ttu-id="abf75-104">L’élément **Update** identifie un dossier unique à mettre à jour dans le magasin client local.</span><span class="sxs-lookup"><span data-stu-id="abf75-104">The **Update** element identifies a single folder to update in the local client store.</span></span> 
  
- [<span data-ttu-id="abf75-105">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="abf75-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md) 
- [<span data-ttu-id="abf75-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="abf75-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="abf75-107">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="abf75-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)  
- [<span data-ttu-id="abf75-108">Changes (hiérarchie)</span><span class="sxs-lookup"><span data-stu-id="abf75-108">Changes (Hierarchy)</span></span>](changes-hierarchy.md) 
- [<span data-ttu-id="abf75-109">Mise à jour (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="abf75-109">Update (FolderSync)</span></span>](update-foldersync.md)
  
```xml
<Update>
   <Folder/>
</Update>
```

```xml
<Update>
   <CalendarFolder/>
</Update>
```

```xml
<Update>
   <ContactsFolder/>
</Update>
```

```xml
<Update>
   <TasksFolder/>
</Update>
```

```xml
<Update>
   <SearchFolder/>
</Update>
```

<span data-ttu-id="abf75-110">**SyncFolderHierarchyCreateOrUpdateType**</span><span class="sxs-lookup"><span data-stu-id="abf75-110">**SyncFolderHierarchyCreateOrUpdateType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="abf75-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="abf75-111">Attributes and elements</span></span>

<span data-ttu-id="abf75-112">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="abf75-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="abf75-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="abf75-113">Attributes</span></span>

<span data-ttu-id="abf75-114">Aucune.</span><span class="sxs-lookup"><span data-stu-id="abf75-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="abf75-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="abf75-115">Child elements</span></span>

|<span data-ttu-id="abf75-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="abf75-116">**Element**</span></span>|<span data-ttu-id="abf75-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="abf75-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="abf75-118">Folder</span><span class="sxs-lookup"><span data-stu-id="abf75-118">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="abf75-119">Définit le dossier à créer, obtenir, Rechercher, synchroniser ou mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="abf75-119">Defines the folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="abf75-120">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="abf75-120">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="abf75-121">Représente un dossier qui contient principalement des éléments de calendrier.</span><span class="sxs-lookup"><span data-stu-id="abf75-121">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="abf75-122">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="abf75-122">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="abf75-123">Représente un dossier de contacts dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="abf75-123">Represents a contact folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="abf75-124">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="abf75-124">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="abf75-125">Représente un dossier de recherche contenu dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="abf75-125">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="abf75-126">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="abf75-126">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="abf75-127">Représente un dossier de tâches t est thcontained dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="abf75-127">Represents a task folder t is thcontained in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="abf75-128">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="abf75-128">Parent elements</span></span>

|<span data-ttu-id="abf75-129">**Élément**</span><span class="sxs-lookup"><span data-stu-id="abf75-129">**Element**</span></span>|<span data-ttu-id="abf75-130">**Description**</span><span class="sxs-lookup"><span data-stu-id="abf75-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="abf75-131">Changes (hiérarchie)</span><span class="sxs-lookup"><span data-stu-id="abf75-131">Changes (Hierarchy)</span></span>](changes-hierarchy.md) <br/> |<span data-ttu-id="abf75-132">Contient un tableau séquencé de types de modifications qui représentent le type de différences entre les dossiers sur le client et les dossiers sur le serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="abf75-132">Contains a sequenced array of change types that represent the type of differences between the folders on the client and the folders on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="abf75-133">Remarques</span><span class="sxs-lookup"><span data-stu-id="abf75-133">Remarks</span></span>

<span data-ttu-id="abf75-134">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="abf75-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="abf75-135">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="abf75-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="abf75-136">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="abf75-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="abf75-137">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="abf75-137">Schema name</span></span>  <br/> |<span data-ttu-id="abf75-138">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="abf75-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="abf75-139">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="abf75-139">Validation file</span></span>  <br/> |<span data-ttu-id="abf75-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="abf75-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="abf75-141">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="abf75-141">Can be empty</span></span>  <br/> |<span data-ttu-id="abf75-142">False</span><span class="sxs-lookup"><span data-stu-id="abf75-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="abf75-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="abf75-143">See also</span></span>

- [<span data-ttu-id="abf75-144">Opération SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="abf75-144">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
- [<span data-ttu-id="abf75-145">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="abf75-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

