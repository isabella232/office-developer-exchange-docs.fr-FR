---
title: Créer (FolderSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Create
api_type:
- schema
ms.assetid: 6b463d0a-70e9-40c5-ade4-c7d9a5f36bc1
description: L’élément Create identifie un dossier unique à créer dans le magasin client local.
ms.openlocfilehash: 43f6a6b3c084c8ecae767c512181bbdf50c7e786
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458375"
---
# <a name="create-foldersync"></a><span data-ttu-id="9c0b0-103">Créer (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="9c0b0-103">Create (FolderSync)</span></span>

<span data-ttu-id="9c0b0-104">L’élément **Create** identifie un dossier unique à créer dans le magasin client local.</span><span class="sxs-lookup"><span data-stu-id="9c0b0-104">The **Create** element identifies a single folder to create in the local client store.</span></span> 
  
[<span data-ttu-id="9c0b0-105">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="9c0b0-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
  
[<span data-ttu-id="9c0b0-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="9c0b0-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="9c0b0-107">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9c0b0-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
  
[<span data-ttu-id="9c0b0-108">Changes (hiérarchie)</span><span class="sxs-lookup"><span data-stu-id="9c0b0-108">Changes (Hierarchy)</span></span>](changes-hierarchy.md)
  
[<span data-ttu-id="9c0b0-109">Créer (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="9c0b0-109">Create (FolderSync)</span></span>](create-foldersync.md)
  
```xml
<Create>
   <Folder/>
   <CalendarFolder/>
   <ContactsFolder/>
   <SearchFolder/>
   <TasksFolder/>
</Create>
```

 <span data-ttu-id="9c0b0-110">**SyncFolderHierarchyCreateOrUpdateType**</span><span class="sxs-lookup"><span data-stu-id="9c0b0-110">**SyncFolderHierarchyCreateOrUpdateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9c0b0-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9c0b0-111">Attributes and elements</span></span>

<span data-ttu-id="9c0b0-112">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9c0b0-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9c0b0-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="9c0b0-113">Attributes</span></span>

<span data-ttu-id="9c0b0-114">Aucune.</span><span class="sxs-lookup"><span data-stu-id="9c0b0-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9c0b0-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9c0b0-115">Child elements</span></span>

|<span data-ttu-id="9c0b0-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9c0b0-116">**Element**</span></span>|<span data-ttu-id="9c0b0-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="9c0b0-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9c0b0-118">Folder</span><span class="sxs-lookup"><span data-stu-id="9c0b0-118">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="9c0b0-119">Définit le dossier à créer, obtenir, Rechercher, synchroniser ou mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="9c0b0-119">Defines the folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="9c0b0-120">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="9c0b0-120">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="9c0b0-121">Représente un dossier qui contient principalement des éléments de calendrier.</span><span class="sxs-lookup"><span data-stu-id="9c0b0-121">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="9c0b0-122">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="9c0b0-122">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="9c0b0-123">Représente un dossier de contacts dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="9c0b0-123">Represents a contact folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="9c0b0-124">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="9c0b0-124">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="9c0b0-125">Représente un dossier de recherche contenu dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="9c0b0-125">Represents a search folder contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="9c0b0-126">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="9c0b0-126">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="9c0b0-127">Représente un dossier de tâches contenu dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="9c0b0-127">Represents a task folder contained in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9c0b0-128">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9c0b0-128">Parent elements</span></span>

|<span data-ttu-id="9c0b0-129">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9c0b0-129">**Element**</span></span>|<span data-ttu-id="9c0b0-130">**Description**</span><span class="sxs-lookup"><span data-stu-id="9c0b0-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9c0b0-131">Changes (hiérarchie)</span><span class="sxs-lookup"><span data-stu-id="9c0b0-131">Changes (Hierarchy)</span></span>](changes-hierarchy.md) <br/> |<span data-ttu-id="9c0b0-132">Contient un tableau de séquence de types de modifications qui représentent le type de différences entre les éléments sur le client et les éléments sur le serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="9c0b0-132">Contains a sequence array of change types that represent the type of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9c0b0-133">Remarques</span><span class="sxs-lookup"><span data-stu-id="9c0b0-133">Remarks</span></span>

<span data-ttu-id="9c0b0-134">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="9c0b0-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9c0b0-135">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9c0b0-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9c0b0-136">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9c0b0-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9c0b0-137">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9c0b0-137">Schema name</span></span>  <br/> |<span data-ttu-id="9c0b0-138">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="9c0b0-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="9c0b0-139">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9c0b0-139">Validation file</span></span>  <br/> |<span data-ttu-id="9c0b0-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9c0b0-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9c0b0-141">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9c0b0-141">Can be empty</span></span>  <br/> |<span data-ttu-id="9c0b0-142">False</span><span class="sxs-lookup"><span data-stu-id="9c0b0-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9c0b0-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9c0b0-143">See also</span></span>



[<span data-ttu-id="9c0b0-144">Opération SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="9c0b0-144">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="9c0b0-145">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9c0b0-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

